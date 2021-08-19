---
title: Συγχρονισμός εργασιών έργου απευθείας από το Project Service Automation στο Finance and Operations
description: Αυτό το θέμα περιγράφει το πρότυπο και την υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Microsoft Dynamics 365 Project Service Automation στο Dynamics 365 Finance.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 45846d7a6dd7b84fe28f0a78ccc103679236917ea506180c5b383fd2828624eb
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/06/2021
ms.locfileid: "6992791"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Συγχρονισμός εργασιών έργου απευθείας από το Project Service Automation στο Finance and Operations

[!include[banner](../includes/banner.md)]

Αυτό το θέμα περιγράφει το πρότυπο και την υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Dynamics 365 Project Service Automation στο Dynamics 365 Finance.

> [!NOTE]
> - Η ενοποίηση εργασιών έργου, οι κατηγορίες εξόδων, οι εκτιμήσεις ωρών, οι εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών είναι διαθέσιμα στην έκδοση 8.0.
> - Αν χρησιμοποιείτε το Enterprise edition 7.3.0, μετά την εγκατάσταση των KB 4132657 και KB 4132660, θα μπορείτε να χρησιμοποιήσετε τα πρότυπα για να ενσωματώσετε εργασίες έργου, κατηγορίες εξόδων, εκτιμήσεις ωρών, εκτιμήσεις εξόδων και πραγματικές τιμές και για να ρυθμίσετε τις παραμέτρους του κλειδώματος λειτουργιών. Εάν πρέπει να επαναφέρετε τις λογιστικές κατανομές, συνιστάται επίσης η εγκατάσταση του KB 4131710.
> - Η ενοποίηση πραγματικών στοιχείων είναι διαθέσιμη στην έκδοση 8.0.1 ή μεταγενέστερη.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Ροή δεδομένων για το Project Service Automation στο Finance

Η λύση ενοποίησης Project Service Automation σε Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Project Service Automation και Finance. Το πρότυπο ενοποίησης που είναι διαθέσιμο με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιεί τη ροή των δεδομένων σχετικά με τις εργασίες του έργου από το Project Service Automation στο Finance.

Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα μεταξύ Project Service Automation και Finance.

[![Ροή δεδομένων για την ενοποίηση του Project Service Automation με το Finance.](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>Πρότυπο και εργασία

Για να αποκτήσετε πρόσβαση στο πρότυπο, στο κέντρο διαχείρισης του Microsoft Power Apps, επιλέξτε **Έργα** και, στη συνέχεια, στην επάνω δεξιά γωνία, επιλέξτε **Νέο έργο** για να επιλέξετε δημόσια πρότυπα.

Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Project Service Automation στο Finance:

- **Όνομα του προτύπου στην ενοποίηση δεδομένων:** Εργασίες έργου (PSA σε Fin και Ops)
- **Όνομα της εργασίας στο έργο:** Εργασίες έργου

Για να είναι δυνατός ο συγχρονισμός των εργασιών έργου, πρέπει να συγχρονίσετε τις συμβάσεις και τα έργα του έργου.

## <a name="entity-set"></a>Σύνολο οντοτήτων

| Project Service Automation | Οικονομικά                             |
|----------------------------|-------------------------------------|
| Εργασίες έργου              | Οντότητα ενοποίησης για εργασία έργου |

## <a name="entity-flow"></a>Ροή οντότητας

Η διαχείριση των εργασιών έργου γίνεται στο Project Service Automation και συγχρονίζονται με το Finance ως δραστηριότητες έργου.

## <a name="prerequisites-and-mapping-setup"></a>Προϋποθέσεις και ρύθμιση αντιστοίχισης

Για να είναι δυνατός ο συγχρονισμός των εργασιών έργου, πρέπει να συγχρονίσετε τις συμβάσεις και τα έργα του έργου.

## <a name="power-query"></a>Power Query

Πρέπει να χρησιμοποιήσετε το Microsoft Power Query για Excel για να φιλτράρετε τα δεδομένα, εάν πληρούνται αυτές οι προϋποθέσεις:

- Διαθέτετε καρτέλες συγκεκριμένων πόρων σε μια εργασία έργου.

Εάν πρέπει να χρησιμοποιήσετε το Power Query, ακολουθήστε την παρακάτω οδηγία:

- Το πρότυπο Εργασίες έργου (PSA σε Fin και Ops) έχει ένα προεπιλεγμένο φίλτρο που αποκλείει καρτέλες που αφορούν πόρους από μια εργασία έργου, ορίζοντας το φίλτρο στο **IsLineTask** σε **Ψευδές**. Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτό το φίλτρο.

## <a name="template-mapping-in-data-integration"></a>Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων

Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων. Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.

[![Αντιστοίχιση προτύπου.](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]