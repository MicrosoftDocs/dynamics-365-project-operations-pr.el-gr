---
title: Συγχρονισμός κατηγοριών εξόδων έργου μεταξύ του Finance and Operations και του Project Service Automation
description: Αυτό το θέμα περιγράφει τα πρότυπα και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδων έργου μεταξύ του Microsoft Dynamics 365 Finance και του Dynamics 365 Project Service Automation.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: ed7ca3c85d3f99b7eefe10f4ddec822b9aeb1684
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077055"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>Συγχρονισμός κατηγοριών εξόδων έργου μεταξύ του Finance and Operations και του Project Service Automation

[!include[banner](../includes/banner.md)]

Αυτό το θέμα περιγράφει τα πρότυπα και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδων έργου μεταξύ του Dynamics 365 Finance και του Dynamics 365 Project Service Automation.

> [!NOTE]
> - Η ενοποίηση εργασιών έργου, οι κατηγορίες εξόδων, οι εκτιμήσεις ωρών, οι εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών είναι διαθέσιμα στην έκδοση 8.0.
> - Η ενοποίηση πραγματικών στοιχείων είναι διαθέσιμη στην έκδοση 8.0.1 ή μεταγενέστερη.
> - Αν χρησιμοποιείτε το Enterprise edition 7.3.0, μετά την εγκατάσταση των KB 4132657 και KB 4132660, θα μπορείτε να χρησιμοποιήσετε τα πρότυπα για να ενσωματώσετε εργασίες έργου, κατηγορίες εξόδων, εκτιμήσεις ωρών, εκτιμήσεις εξόδων και πραγματικές τιμές και για να ρυθμίσετε τις παραμέτρους του κλειδώματος λειτουργιών. Εάν πρέπει να επαναφέρετε τις λογιστικές κατανομές, συνιστάται επίσης η εγκατάσταση του KB 4131710.

## <a name="data-flow-for-project-service-automation-and-finance"></a>Ροή δεδομένων για το Project Service Automation και το Finance

Η λύση ενοποίησης Project Service Automation και Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Project Service Automation και Finance. Τα πρότυπα ενοποίησης που είναι διαθέσιμα με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιούν τη ροή των δεδομένων σχετικά με τις κατηγορίες συναλλαγών εξόδων έργου μεταξύ του Project Service Automation και του Finance.

Εάν οι κατηγορίες εξόδων έργου έχουν δημιουργηθεί στο Finance, η ροή ενοποίησης είναι από το Finance στο Project Service Automation. Στη συνέχεια, τα αναγνωριστικά ενοποίησης των κατηγοριών εξόδων έργου ενημερώνονται μέσω συγχρονισμού από το Project Service Automation στο Finance.

Εάν οι κατηγορίες εξόδων έργου έχουν δημιουργηθεί στο Project Service Automation, η ροή ενοποίησης είναι από το Project Service Automation στο Finance. Οι κατηγορίες έργου πρέπει να ρυθμιστούν ήδη στο Finance πριν από το συγχρονισμό από το Project Service Automation. Κατόπιν συγχρονίστε από το Finance στο Project Service Automation και μετά από το Project Service Automation στο Finance ξανά. Με αυτόν τον τρόπο, μπορείτε να εγγυηθείτε ότι οι κατηγορίες είναι συνδεδεμένες και ότι δεν δημιουργούνται διπλότυπα.

> [!NOTE]
> Συνήθως, οι κατηγορίες εξόδων έργου καταχωρούνται στο Finance. Ωστόσο, εάν δεν υπάρχουν ή εάν έχουν ήδη δημιουργηθεί κατηγορίες εξόδων στο Project Service Automation, πρέπει πρώτα να πραγματοποιήσετε συγχρονισμό χρησιμοποιώντας το πρότυπο κατηγοριών συναλλαγών εξόδων έργου (PSA σε Fin και Ops). Στη συνέχεια, πραγματοποιήστε συγχρονισμό χρησιμοποιώντας το πρότυπο κατηγοριών συναλλαγών εξόδων έργου (Fin and Ops σε PSA). Στη συνέχεια, θα πρέπει να εκτελέσετε τον συγχρονισμό από το Project Service Automation στο Finance μια ακόμα φορά.
>
> Εάν συγχρονίσετε πρώτα από το Project Service Automation, πρέπει να πληρούνται οι παρακάτω προϋποθέσεις στο Finance για την εκτέλεση του συγχρονισμού:
>
> - Η κοινόχρηστη κατηγορία που αντιστοιχεί στην κατηγορία έργου που έχει ρυθμιστεί στο Project Service Automation πρέπει να υπάρχει και πρέπει να είναι ενεργοποιημένη τόσο για το **Έργο** όσο και για το **Έξοδο**.
> - Για κάθε νομική οντότητα Finance με την οποία πρέπει να ενοποιηθεί, πρέπει να υπάρχουν οι ακόλουθες κατηγορίες έργου:
>
>     - Η **Κατηγορία έργου** υπάρχει. 
>     - Η **Χρήση σε έξοδο** έχει ενεργοποιηθεί.
>     - Το στοιχείο **Ενεργό στο ημερολόγιο** είναι ενεργοποιημένο.
>     - Ο **Τύπος συναλλαγής** ορίστηκε σε **Έξοδο**.

Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα μεταξύ Project Service Automation και Finance.

[![Ροή δεδομένων για την ενοποίηση του Project Service Automation με το Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>Συγχρονισμός κατηγορίας εξόδου έργου από το Finance στο Project Service Automation

### <a name="template-and-task"></a>Πρότυπο και εργασία

Για να αποκτήσετε πρόσβαση στο πρότυπο, στο κέντρο διαχείρισης του Microsoft Power Apps, επιλέξτε **Έργα** και, στη συνέχεια, στην επάνω δεξιά γωνία, επιλέξτε **Νέο έργο** για να επιλέξετε δημόσια πρότυπα.

Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδου έργου από το Finance στο Project Service Automation:

- **Όνομα του προτύπου στην ενοποίηση δεδομένων:** Κατηγορίες συναλλαγών εξόδου έργου (Fin και Ops σε PSA)
- **Όνομα της εργασίας του έργου:** Κατηγορίες συγχρονισμού στο PSA

### <a name="entity-set"></a>Σύνολο οντοτήτων

| Οικονομικά                           | Project Service Automation |
|-----------------------------------|----------------------------|
| Οντότητα ενοποίησης για κατηγορίες | Κατηγορίες συναλλαγών     |

### <a name="entity-flow"></a>Ροή οντότητας

Η διαχείριση των κατηγοριών εξόδων έργου γίνεται στο Finance και συγχρονίζονται με το Project Service Automation ως κατηγορίες συναλλαγών.

### <a name="power-query"></a>Power Query

Όταν εκτελείτε συγχρονισμό με το Project Service Automation, πρέπει να χρησιμοποιήσετε το Microsoft Power Query για Excel για να ορίσετε τον τύπο χρέωσης στην κατηγορία συναλλαγής. Το πρότυπο "κατηγορίες συναλλαγών εξόδων έργου" (FIN και OPS σε PSA) παρέχει μια προεπιλεγμένη στήλη και αντιστοίχιση. Εάν δημιουργήσετε το δικό σας πρότυπο, θα πρέπει να προσθέσετε μια στήλη υπό όρους στο Power Query. Ακολουθήστε αυτά τα βήματα.

1. Κάντε κλικ στο βέλος για να ανοίξετε την αντιστοίχιση των κατηγοριών εξόδων έργου στο πρότυπο κατηγοριών συναλλαγών εξόδων έργου (FIN και OPS σε PSA).
2. Κάντε κλικ στη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** για να ανοίξετε το Power Query.
2. Επιλέξτε **Προσθήκη στήλης υπό όρους**.
3. Καταγράψτε ένα όνομα για τη νέα στήλη, για παράδειγμα, **BillingType**.
4. Καταγράψτε την ακόλουθη συνθήκη: **Εάν το CATEGORYID δεν ισούται με null, τότε 19235001, διαφορετικά null**.
5. Επιλέξτε **OK** στη στήλη.
6. Βεβαιωθείτε ότι αντιστοιχίσατε αυτήν τη νέα στήλη στη σελίδα αντιστοίχισης.

Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων. Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Finance στο Project Service Automation.

[![Αντιστοίχιση προτύπων κατηγορίας εξόδου έργου στο Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>Συγχρονισμός κατηγορίας εξόδου έργου από το Project Service Automation στο Finance

### <a name="template-and-task"></a>Πρότυπο και εργασία

Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδου έργου από το Project Service Automation στο Finance:

- **Όνομα του προτύπου στην ενοποίηση δεδομένων:** Κατηγορίες συναλλαγών εξόδου έργου (PSA σε Fin και Ops)
- **Όνομα της εργασίας του έργου:** Κατηγορίες συγχρονισμού σε Fin Ops

### <a name="entity-set"></a>Σύνολο οντοτήτων

| Project Service Automation | Οικονομικά                           |
|----------------------------|-----------------------------------|
| Κατηγορίες συναλλαγών     | Οντότητα ενοποίησης για κατηγορίες |

### <a name="entity-flow"></a>Ροή οντότητας

Η διαχείριση των κατηγοριών εξόδων έργου γίνεται στο Finance και συγχρονίζονται με το Project Service Automation ως κατηγορίες συναλλαγών. Ο συγχρονισμός με ενημερώσεις του Finance ενημερώνει την κατηγορία έργου στο Finance με το αναγνωριστικό ενοποίησης από το Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων

Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.

> [!NOTE]
> Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.

[![Αντιστοίχιση προτύπων του Project Service Automation με το Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]