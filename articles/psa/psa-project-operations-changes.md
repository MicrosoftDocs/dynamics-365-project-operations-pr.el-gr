---
title: Αλλαγές δυνατοτήτων από το Project Service Automation στο Project Operations
description: Αυτό το άρθρο παρέχει μια επισκόπηση των αλλαγών των δυνατοτήτων από το Project Service Automation στο Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: a9c69fc4296d30763f3994a4955e64ab258ceb4f
ms.sourcegitcommit: 675e9f3615e701c5f998de3a5ea3e25df11ae107
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/09/2022
ms.locfileid: "9459926"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Αλλαγές δυνατοτήτων από το Project Service Automation στο Project Operations

Η αναβάθμιση από το Dynamics 365 Project Service Automation στο Dynamics 365 Project Operations Lite θα παραδοθεί σε τρεις φάσεις. Αυτό άρθρο παρέχει πληροφορίες σχετικά με τις μεγάλες αλλαγές που μπορείτε να περιμένετε να δείτε όταν ολοκληρωθεί η αναβάθμιση.

| Παράδοση αναβάθμισης | Φάση 1 <br>(Ιανουάριος 2022) | Φάση 2 <br>(Νοέμβριος 2022) | Φάση 3  |
|------------------|------------------------|---------------------------|---------------------------|
| Καμία εξάρτηση στη δομή ανάλυσης εργασίας (WBS) για έργα. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Το WBS περιλαμβάνεται στα όρια του Project Operations που υποστηρίζονται αυτή τη στιγμή. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| Το WBS εκτός των ορίων του Project Operations που υποστηρίζονται αυτή τη στιγμή, συμπεριλαμβανομένης της υποστήριξης για το Project desktop client. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Διαχείριση έργων

Οι πιο σημαντικές αλλαγές στην εμπειρία χρήστη θα είναι στον τομέα σχεδιασμού έργων. Το Project Operations υιοθετεί μια νέα σύγχρονη εμπειρία για τη διαχείριση μιας δομής ανάλυσης εργασίας (WBS) αξιοποιώντας τις δυνατότητες προγραμματισμού που παρέχονται από το [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Διαφορές στην εμπειρία προγραμματισμού

Ο παρακάτω πίνακας συνοψίζει τις διαφορές προγραμματισμού μεταξύ των Project Service Automation και Project Operations.

|  Χρονοδιάγραμμα     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Πρότυπα έργου - Δυνατότητα καθορισμού και εφαρμογής προτύπων έργων κατά τη δημιουργία ενός έργου  |  &nbsp;    | :heavy_check_mark: |
| Ενοποίηση δομής ανάλυσης εργασίας (WBS) έργου με υπολογιστή-πελάτη υπολογιστή   |    &nbsp;  | :heavy_check_mark: |
| Περιορισμοί - Ξεκινήστε όχι νωρίτερα από, ολοκληρώστε το όχι αργότερα από  | :heavy_check_mark: |   &nbsp;  |
| Ορόσημα - Εργασίες με μηδενική διάρκεια   | :heavy_check_mark:  |  &nbsp;  |
| Οι εργασίες που καθορίζονται από πόρους θα τηρούν τη διαθεσιμότητα των πόρων που έχουν ανατεθεί   | :heavy_check_mark: |  &nbsp;    |
| Επεξεργασία σε χρονικά στάδια - Επεξεργασία σχεδίων και εργασία καθημερινά   |   &nbsp;  | :heavy_check_mark: |
| Αυτόματος/μη αυτόματος προγραμματισμός - Χρησιμοποιήστε τη μηχανή προγραμματισμού έργων για αυτόματο ή μη αυτόματο προγραμματισμό εργασιών |  &nbsp; | :heavy_check_mark:  |
| Επεξεργασία μεγάλων έργων απευθείας στο περιβάλλον εργασίας χρήστη: Δεν υπάρχει όριο στο μέγεθος των σχεδίων με δυνατότητα επεξεργασίας  | Όριο 500 εργασιών  | :heavy_check_mark:       |
| Ποσοστό ολοκλήρωσης - Σήμανση προόδου εργασίας   | :heavy_check_mark:  |  &nbsp;  |
| [Λειτουργίες προγραμματισμού έργων](../project-management/scheduling-modes.md) - Καθορισμός του έργου ως σταθερών μονάδων, σταθερής προσπάθειας ή σταθερής διάρκειας | :heavy_check_mark: | &nbsp; |
| Χρονοδιάγραμμα - Δημιουργήστε και προσαρμόστε την προβολή χρονοδιαγράμματος για να απεικονίσετε τις λεπτομέρειες του χρονοδιαγράμματος και να επικοινωνήσετε με ενδιαφερόμενους. | :heavy_check_mark:  | &nbsp; |
| Εργασίες που καθοδηγούνται από την προσπάθεια - Υποστήριξη μηχανής προγραμματισμού για τον προγραμματισμό μιας εργασίας ως καθοδηγούμενη προσπάθεια  | :heavy_check_mark:  | &nbsp; |
| Παράθυρο διαλόγου **Πληροφορίες εργασίας** - Αποθήκευση λεπτομερειών εργασίας χρησιμοποιώντας ένα παράθυρο διαλόγου | :heavy_check_mark:  |  &nbsp;  |
| Μεταφορά και απόθεση - Εργασίες πολλαπλής επιλογής και τροποποίηση της θέσης τους στο WBS | :heavy_check_mark: | &nbsp;  |
| Ευέλικτες μόνιμες προβολές - Καθορίστε πιο λεπτομερείς προβολές των χαρακτηριστικών εργασιών   | :heavy_check_mark:  | &nbsp; |
| Ταξινόμηση και φιλτράρισμα WBS  | :heavy_check_mark:  | &nbsp; |
| Προβολή πινάκων για παράδοση έργων μη καταρράκτη  | :heavy_check_mark:   | &nbsp; |
| Προβολή χρονοδιαγράμματος - Αλληλεπιδραστικό γράφημα Gantt που χρησιμοποιείται για την απεικόνιση και επεξεργασία του WBS   | :heavy_check_mark:  | &nbsp; |
| Συντομεύσεις πληκτρολογίου - Χρήση συντομεύσεων πληκτρολογίου για κοινές λειτουργίες, όπως είναι η εσοχή ή η εισαγωγή  | :heavy_check_mark:  |  &nbsp; |
| Αναίρεση πολλών επιπέδων - Εκτέλεση ανάλυσης what-if για την πλήρη κατανόηση του αντίκτυπου των αλλαγών με την αντιστροφή και την εκ νέου εφαρμογή ενός ολόκληρου συνόλου λειτουργιών | :heavy_check_mark: | &nbsp; |
| Αποκοπή/αντιγραφή/επικόλληση - Συνεργαστείτε κατά την ανάπτυξη χρονοδιαγράμματος αντιγράφοντας και επικολλώντας λεπτομέρειες χρονοδιαγράμματος μεταξύ εφαρμογών  | :heavy_check_mark: | &nbsp; |
| Λίστες ελέγχου εργασιών - Προσθήκη έως και 20 στοιχείων λίστας ελέγχου σε μια εργασία   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Σχεδιασμός έργου

Η σελίδα **έργου** στο Project Operations έχει ένα σημαντικό αριθμό διαφορών σε σύγκριση με τη σελίδα **έργου** στο Project Service Automation.

Οι παρακάτω ενέργειες έχουν καταργηθεί από τη σελίδα **Έργα** ως μέρος της αναβάθμισης φάσης 1:

  - **Άνοιγμα στο MS Project**
  - **Δημιουργία προτύπου**
  - **Κατάργηση σύνδεσης από το MS Project**

Η σελίδα **Έργο** στο Project Operations περιλαμβάνει τις ακόλουθες νέες καρτέλες.

- **Εκτιμήσεις υλικών**
- **Ρύθμιση χρέωσης εργασίας**

Η καρτέλα **Κατάσταση** έχει καταργηθεί και το πεδίο **Κατάσταση** βρίσκεται πλέον στην καρτέλα **Σύνοψη** με τη λειτουργία προγραμματισμού του έργου.

   ![Ενημερώσεις στη σελίδα έργου.](media/projectform.png)

Η καρτέλα **Χρονοδιάγραμμα** μετονομάστηκε σε καρτέλα **Εργασία** και διαθέτει τη νέα εμπειρία σχεδιασμού έργου με το Project for the Web.

   ![Καρτέλα Νέες εργασίες έργου.](media/tasktab.png)

## <a name="scheduling-modes"></a>Λειτουργίες προγραμματισμού

Το Project Operations έχει εισαγάγει μια νέα δυνατότητα, τις [λειτουργίες προγραμματισμού](../project-management/scheduling-modes.md). Όλα τα υπάρχοντα έργα Project Service Automation θα τεθούν από προεπιλογή σε **Σταθερή διάρκεια** στο Project Operations. Ωστόσο, η διαχείριση της προεπιλογής για τα νέα έργα μπορεί να γίνει με μετάβαση στις **Ρυθμίσεις** > **Παράμετροι** > **Παράμετρος** > **Λειτουργία προγραμματισμού**.

   ![Ρυθμίσεις παραμέτρων έργου για τη λειτουργία προγραμαμτισμού.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Όρια σχεδιασμού έργου

Το Project Operations βασίζεται στο Project for the Web για όλες τις λειτουργίες προγραμματισμού έργου. Το Project for the Web διαχειρίζεται τη δομή ανάλυσης εργασίας χρησιμοποιώντας τα όρια που περιλαμβάνει ο παρακάτω πίνακας.

| **Πεδίο**                                          | **Όριο**             |
|----------------------------------------------------|-----------------------|
| Μέγιστος συνολικός αριθμός εργασιών για ένα έργο                  | 500                   |
| Μέγιστη συνολική διάρκεια για ένα έργο               | 3650 ημέρες (10 έτη)  |
| Μέγιστοι συνολικοί πόροι για ένα έργο              | 300                   |
| Μέγιστες συνολικές συνδέσεις (μόνο διάδοχος) για ένα έργο | 600                   |
| Μέγιστα συνολικά προσαρμοσμένα πεδία για ένα έργο          | 10                    |
| Μέγιστο επίπεδο ιεραρχίας                            | 10 επίπεδα             |
| Μέγιστες συνδέσεις (διάδοχός + προκάτοχος)            | 20                    |
| Μέγιστη διάρκεια τερματικής εργασίας                      | 1250 ημέρες             |
| Μέγιστη διάρκεια μιας συνοπτικής εργασίας                 | 3650 ημέρες (10 έτη)  |
| Μέγιστοι πόροι που ανατέθηκαν σε μια εργασία               | 20 πόροι          |
| Υποστηριζόμενο εύρος ημερομηνιών για μια εργασία                    | 1/1/2000 - 12/31/2149 |
| Στοιχεία λίστας ελέγχου                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Επεκτασιμότητα και ανάπτυξη σχεδιασμού έργου

Μετά την αναβάθμιση στο Project Operations, πρέπει να χρησιμοποιήσετε τα API προγραμματισμού έργου για να εκτελέσετε λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής στις ακόλουθες οντότητες:

|   Όνομα οντότητας           |   Λογικό όνομα οντότητας       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Εργασία έργου            | msdyn_projecttask           |
| Εξάρτηση εργασίας έργου | msdyn_projecttaskdependency |
| Ανάθεση πόρου     | msdyn_resourceassignment    |
| Κάδος έργου          | msdyn_projectbucket         |
| Μέλος ομάδας έργου     | msdyn_projectteam           |

Εάν προς το παρόν έχετε προσαρμογές που αφορούν αυτές τις οντότητες, ανατρέξτε στο θέμα [Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες](../project-management/schedule-api-preview.md) για καθοδήγηση υλοποίησης.

## <a name="data-model-changes"></a>Αλλαγές μοντέλου δεδομένων

Ως μέρος της φάσης αναβάθμισης 1, υπάρχουν αλλαγές στο μοντέλο δεδομένων. Αυτές οι αλλαγές είναι κυρίως αλλαγές πεδίων σε υπάρχουσες οντότητες. Στη Φάση 1, οι οντότητες, **msydn_project** και **msdyn_projectteam** αποτελούν επανασχεδιασμό προσαρμογών. 

> [!IMPORTANT]
> Αυτή η ενότητα θα ενημερωθεί με πρόσθετες οντότητες, καθώς θα ολοκληρωθούν οι μελλοντικές φάσεις αναβάθμισης.

Τα ακόλουθα πεδία έχουν αντικατασταθεί με νέα πεδία.

|   Entity          |   Παλαιό λογικό όνομα   |   Νέο λογικό όνομα    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Έχουν προστεθεί τα ακόλουθα πεδία.

|   Entity          |   Λογικό όνομα                               |   Description |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Εμφανίζει τη συγκεντρωτική τιμή των πραγματικών πωλήσεων χρέωσης στο έργο. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_actualmaterialcost                     | Εμφανίζει τη συγκεντρωτική τιμή του πραγματικού κόστους υλικών στο έργο. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_actualmaterialsales                    | Εμφανίζει τη συγκεντρωτική τιμή των πραγματικών πωλήσεων υλικών στο έργο. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Η γραμμή σύμβασης που σχετίζεται με αυτό το έργο. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Αυτό είναι ένα πεδίο εσωτερικού συστήματος που χρησιμοποιείται για **Αντιγραφή έργου** που σχετίζεται με το αναγνωριστικό συσχέτισης. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Αυτό είναι ένα πεδίο εσωτερικού συστήματος που χρησιμοποιείται για **Αντιγραφή έργου** που σχετίζεται με το αναγνωριστικό περιόδου λειτουργίας. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Διακριτικό καθολικής αναθεώρησης xRM τελευταίου συγχρονισμού από την υπηρεσία προγραμματισμού έργου. |
| msdyn_project     | msdyn_msprojectdocument                      | Το έγγραφο Microsoft Project που ανήκει στο έργο. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Η συγκεντρωτική τιμή του σχεδιασμένου κόστους υλικών στο έργο. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Η συγκεντρωτική τιμή των σχεδιασμένων πωλήσεων υλικών στο έργο. Για χρήση στο Project Service Automation μόνο. |
| msdyn_project     | msdyn_program                                | Το πρόγραμμα με το οποίο σχετίζεται αυτό το έργο. |
| msdyn_project     | msdyn_quotelineproject                       | Η γραμμή προσφοράς που σχετίζεται με αυτό το έργο. |
| msdyn_project     | msdyn_replaylogheader                        | Η κεφαλίδα για τα αρχεία καταγραφής επανάληψης. |
| msdyn_project     | msdyn_schedulemode                           | Η προεπιλεγμένη λειτουργία προγραμματισμού που χρησιμοποιείται για όλες τις εργασίες στο έργο.  |
| msdyn_project     | msdyn_taskearlieststart                      | Η πιο πρώιμη ημερομηνία έναρξης οποιασδήποτε εργασίας στο έργο.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Το μέλος της ομάδας έργου από το οποίο αντιγράφηκε αυτό το μέλος της ομάδας έργου. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Υποδιεκνύει αν θα δημιουργηθεί η απαίτηση πόρου για ένα νέο μέλος ομάδας γενικής χρήσης.  |
| msdyn_projectteam | msdyn_deletestatus                           | Η κατάσταση διαγραφής του μέλους ομάδας για να παρακολουθήσετε εάν υπάρχει αίτημα διαγραφής που εστάλη στην υπηρεσία προγραμματισμού έργων και αν αποστέλλει επιτυχώς μια απάντηση εντός του αναμενόμενου χρονικού παραθύρου. |
| msdyn_projectteam | msdyn_effortcompleted                        | Παρακολουθεί την προσπάθεια που επιτεύχθηκε από το μέλος της ομάδας στις αναθέσεις του. |
| msdyn_projectteam | msdyn_effortremaining                        | Παρακολουθεί την προσπάθεια που μένει να ολοκληρωθεί από το μέλος της ομάδας στις αναθέσεις του. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Η περίοδος αναμονής από την οποία το μέλος της ομάδας στέλνει μια αίτηση διαγραφής στην υπηρεσία προγραμματισμού έργου έως ότου το μέλος της ομάδας διαγραφεί πραγματικά στο Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Η χρονική σήμανση για εγγραφή όταν το αίτημα διαγραφής του μέλους της ομάδας αποστέλλεται στην υπηρεσία προγραμματισμού έργου. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Εμφανίζει το μέλος της ομάδας έργου από το οποίο αντιγράφηκε αυτό το μέλος της ομάδας έργου.  |

## <a name="project-templates"></a>Πρότυπα έργων

Το Project Operations δεν παρέχει υποστήριξη για πρότυπα έργων. Ωστόσο, μπορείτε να αναπαραγάγετε μεγάλο μέρος της βασικής λειτουργικότητας με τη χρήση του [API αντιγραφής έργου](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Υποστήριξη προσθετών για επιτραπέζιο υπολογιστή

Η υποστήριξη για το πρόσθετο Microsoft Project Desktop δεν θα είναι διαθέσιμη στις 2 πρώτες φάσεις της αναβάθμισης. Στη Φάση 3, οι πελάτες που διαθέτουν έργα μεγαλύτερα από τα όρια του Project for the Web που υποστηρίζονται τη δεδομένη στιγμή θα μπορούν να χρησιμοποιήσουν το πρόσθετο για επιτραπέζιο υπολογιστή.

## <a name="editing-resource-assignment-contours"></a>Επεξεργασία καμπύλων εκχώρησης πόρων

Η δυνατότητα επεξεργασίας καμπυλών εκχώρησης πόρων θα είναι διαθέσιμη όταν θα είναι διαθέσιμη η Φάση 2 της αναβάθμισης.

## <a name="billing-and-pricing"></a>Χρέωση και τιμολόγηση

Οι ακόλουθες νέες δυνατότητες έχουν προστεθεί στο Project Operations. Αυτές οι δυνατότητες είναι αθροιστικής φύσης και δεν επηρεάζουν το μοντέλο δεδομένων Project Service Automation.

- [Καταγραφή χρήσης υλικού σε έργα και εργασίες έργων](../material/material-usage-log.md)
- [Διαχείριση υπεργολαβίας](../pro/subcontracting/managing-subcontracts-overview.md)
- [Συμβάσεις βάσει προπληρωμών και προκαταβολών](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Η σύμβαση να μην υπερβαίνει την κατάσταση και τις επικυρώσεις](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Χρέωση βάσει εργασίας](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Στοιχεία υπό απόσυρση

Οι παρακάτω πίνακες εγγράφουν όλα τα αποσυρμένα πεδία που έχουν μετακινηθεί στη λύση αποσυρμένων στοιχείων μετά την αναβάθμιση. Για περισσότερες πληροφορίες και μια σύνδεση στη λύση, δείτε [Dynamics 365 Project Service Automation 3x στο Project Operations 4x αποσυρμένα στοιχεία](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salesorderdetail

| Πεδία                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

