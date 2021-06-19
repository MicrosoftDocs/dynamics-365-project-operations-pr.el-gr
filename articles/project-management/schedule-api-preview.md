---
title: Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτή θέμα παρέχει πληροφορίες και δείγματα για τη χρήση API χρονοδιαγράμματος.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116797"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

> [!IMPORTANT] 
> Ορισμένες ή όλες οι λειτουργίες που αναφέρονται σε αυτό το θέμα είναι διαθέσιμες ως μέρος μιας έκδοσης προεπισκόπησης. Το περιεχόμενο και η λειτουργικότητα υπόκεινται σε αλλαγές. 

## <a name="scheduling-entities"></a>Οντότητες προγραμματισμού

Τα API χρονοδιαγράμματος παρέχουν τη δυνατότητα εκτέλεσης δημιουργίας, ενημέρωσης και διαγραφής λειτουργιών με **Οντότητες προγραμματισμού**. Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web. Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.

Ο παρακάτω πίνακας περιλαμβάνει μια πλήρη λίστα των **Οντοτήτων προγραμματισμού**.

| Όνομα οντότητας  | Λογικό όνομα οντότητας |
| --- | --- |
| Project | msdyn_project |
| Εργασία έργου  | msdyn_projecttask  |
| Εξάρτηση εργασίας έργου  | msdyn_projecttaskdependency  |
| Ανάθεση πόρου | msdyn_resourceassignment |
| Κάδος έργου  | msdyn_projectbucket |
| Μέλος ομάδας έργου | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

Το OperationSet είναι ένα μοτίβο μονάδας εργασίας που μπορεί να χρησιμοποιηθεί όταν διάφορα αιτήματα που επηρεάζουν το χρονοδιάγραμμα πρέπει να υποβληθούν σε επεξεργασία εντός μιας συναλλαγής.

## <a name="schedule-apis"></a>Προγραμματισμός API

Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος.

- **msdyn_CreateProjectV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός έργου. Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.
- **msdyn_CreateTeamMemberV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός μέλους ομάδας έργου. Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.
- **msdyn_CreateOperationSetV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.
- **msdyn_PSSCreateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία δημιουργίας.
- **msdyn_PSSUpdateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για την ενημέρωση μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία ενημέρωσης.
- **msdyn_PSSDeleteV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη διαγραφή μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία διαγραφής.
- **msdyn_ExecuteOperationSetV1**: αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.

## <a name="using-schedule-apis-with-operationset"></a>Χρήση API χρονοδιαγράμματος με το OperationSet

Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**. Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.

## <a name="supported-operations"></a>Υποστηριζόμενες λειτουργίες

| Οντότητα προγραμματισμού | Δημιουργία | Ενημέρωση | Delete | Σημαντικές επισημάνσεις |
| --- | --- | --- | --- | --- |
Εργασία έργου | Ναι | Ναι | Ναι | Κανένας |
| Εξάρτηση εργασίας έργου | Ναι | Ναι | | Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα. |
| Ανάθεση πόρου | Ναι | Ναι | | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**. Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα. |
| Κάδος έργου | Μη διαθέσιμο | Μη διαθέσιμο | Μη διαθέσιμο | Ο προεπιλεγμένος κάδος δημιουργείται με χρήση του API **CreateProjectV1**. |
| Μέλος ομάδας έργου | Ναι | Ναι | Ναι | Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**. |
| Project | Ναι | Ναι | Μη διαθέσιμο | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**. |

Αυτά τα API μπορούν να καλούνται με αντικείμενα οντότητας που περιλαμβάνουν προσαρμοσμένα πεδία.

Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση. Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί. Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.

## <a name="restricted-fields"></a>Περιορισμένα πεδία

Οι παρακάτω πίνακες ορίζουν τα πεδία που περιορίζονται από τα **Δημιουργία** και **Επεξεργασία.**

### <a name="project-task"></a>Εργασία έργου

| **Λογικό όνομα**                       | **Δυνατότητα δημιουργίας** | **Δυνατότητα επεξεργασίας**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | όχι             | όχι               |
| msdyn_actualcost_base                  | όχι             | όχι               |
| msdyn_actualend                        | όχι             | όχι               |
| msdyn_actualsales                      | όχι             | όχι               |
| msdyn_actualsales_base                 | όχι             | όχι               |
| msdyn_actualstart                      | όχι             | όχι               |
| msdyn_costatcompleteestimate           | όχι             | όχι               |
| msdyn_costatcompleteestimate_base      | όχι             | όχι               |
| msdyn_costconsumptionpercentage        | όχι             | όχι               |
| msdyn_effortcompleted                  | όχι             | όχι               |
| msdyn_effortestimateatcomplete         | όχι             | όχι               |
| msdyn_iscritical                       | όχι             | όχι               |
| msdyn_iscriticalname                   | όχι             | όχι               |
| msdyn_ismanual                         | όχι             | όχι               |
| msdyn_ismanualname                     | όχι             | όχι               |
| msdyn_ismilestone                      | όχι             | όχι               |
| msdyn_ismilestonename                  | όχι             | όχι               |
| msdyn_LinkStatus                       | όχι             | όχι               |
| msdyn_linkstatusname                   | όχι             | όχι               |
| msdyn_msprojectclientid                | όχι             | όχι               |
| msdyn_plannedcost                      | όχι             | όχι               |
| msdyn_plannedcost_base                 | όχι             | όχι               |
| msdyn_plannedsales                     | όχι             | όχι               |
| msdyn_plannedsales_base                | όχι             | όχι               |
| msdyn_pluginprocessingdata             | όχι             | όχι               |
| msdyn_progress                         | όχι             | όχι (ναι για P4W) |
| msdyn_remainingcost                    | όχι             | όχι               |
| msdyn_remainingcost_base               | όχι             | όχι               |
| msdyn_remainingsales                   | όχι             | όχι               |
| msdyn_remainingsales_base              | όχι             | όχι               |
| msdyn_requestedhours                   | όχι             | όχι               |
| msdyn_resourcecategory                 | όχι             | όχι               |
| msdyn_resourcecategoryname             | όχι             | όχι               |
| msdyn_resourceorganizationalunitid     | όχι             | όχι               |
| msdyn_resourceorganizationalunitidname | όχι             | όχι               |
| msdyn_salesconsumptionpercentage       | όχι             | όχι               |
| msdyn_salesestimateatcomplete          | όχι             | όχι               |
| msdyn_salesestimateatcomplete_base     | όχι             | όχι               |
| msdyn_salesvariance                    | όχι             | όχι               |
| msdyn_salesvariance_base               | όχι             | όχι               |
| msdyn_scheduleddurationminutes         | όχι             | όχι               |
| msdyn_scheduledend                     | όχι             | όχι               |
| msdyn_scheduledstart                   | όχι             | όχι               |
| msdyn_schedulevariance                 | όχι             | όχι               |
| msdyn_skipupdateestimateline           | όχι             | όχι               |
| msdyn_skipupdateestimatelinename       | όχι             | όχι               |
| msdyn_summary                          | όχι             | όχι               |
| msdyn_varianceofcost                   | όχι             | όχι               |
| msdyn_varianceofcost_base              | όχι             | όχι               |

### <a name="project-task-dependency"></a>Εξάρτηση εργασίας έργου

| **Λογικό όνομα**              | **Δυνατότητα δημιουργίας** | **Δυνατότητα επεξεργασίας** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | όχι             | όχι           |
| msdyn_linktypename            | όχι             | όχι           |
| msdyn_predecessortask         | ναι            | όχι           |
| msdyn_predecessortaskname     | ναι            | όχι           |
| msdyn_project                 | ναι            | όχι           |
| msdyn_projectname             | ναι            | όχι           |
| msdyn_projecttaskdependencyid | ναι            | όχι           |
| msdyn_successortask           | ναι            | όχι           |
| msdyn_successortaskname       | ναι            | όχι           |

### <a name="resource-assignment"></a>Ανάθεση πόρου

| **Λογικό όνομα**             | **Δυνατότητα δημιουργίας** | **Δυνατότητα επεξεργασίας** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | ναι            | όχι           |
| msdyn_bookableresourceidname | ναι            | όχι           |
| msdyn_bookingstatusid        | όχι             | όχι           |
| msdyn_bookingstatusidname    | όχι             | όχι           |
| msdyn_committype             | όχι             | όχι           |
| msdyn_committypename         | όχι             | όχι           |
| msdyn_effort                 | όχι             | όχι           |
| msdyn_effortcompleted        | όχι             | όχι           |
| msdyn_effortremaining        | όχι             | όχι           |
| msdyn_finish                 | όχι             | όχι           |
| msdyn_plannedcost            | όχι             | όχι           |
| msdyn_plannedcost_base       | όχι             | όχι           |
| msdyn_plannedcostcontour     | όχι             | όχι           |
| msdyn_plannedsales           | όχι             | όχι           |
| msdyn_plannedsales_base      | όχι             | όχι           |
| msdyn_plannedsalescontour    | όχι             | όχι           |
| msdyn_plannedwork            | όχι             | όχι           |
| msdyn_projectid              | ναι            | όχι           |
| msdyn_projectidname          | όχι             | όχι           |
| msdyn_projectteamid          | όχι             | όχι           |
| msdyn_projectteamidname      | όχι             | όχι           |
| msdyn_start                  | όχι             | όχι           |
| msdyn_taskid                 | όχι             | όχι           |
| msdyn_taskidname             | όχι             | όχι           |
| msdyn_userresourceid         | όχι             | όχι           |

### <a name="project-team-member"></a>Μέλος ομάδας έργου

| **Λογικό όνομα**                                 | **Δυνατότητα δημιουργίας** | **Δυνατότητα επεξεργασίας** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | όχι             | όχι           |
| msdyn_creategenericteammemberwithrequirementname | όχι             | όχι           |
| msdyn_deletestatus                               | όχι             | όχι           |
| msdyn_deletestatusname                           | όχι             | όχι           |
| msdyn_effort                                     | όχι             | όχι           |
| msdyn_effortcompleted                            | όχι             | όχι           |
| msdyn_effortremaining                            | όχι             | όχι           |
| msdyn_finish                                     | όχι             | όχι           |
| msdyn_hardbookedhours                            | όχι             | όχι           |
| msdyn_hours                                      | όχι             | όχι           |
| msdyn_markedfordeletiontimer                     | όχι             | όχι           |
| msdyn_markedfordeletiontimestamp                 | όχι             | όχι           |
| msdyn_msprojectclientid                          | όχι             | όχι           |
| msdyn_percentage                                 | όχι             | όχι           |
| msdyn_requiredhours                              | όχι             | όχι           |
| msdyn_softbookedhours                            | όχι             | όχι           |
| msdyn_start                                      | όχι             | όχι           |

### <a name="project"></a>Project

| **Λογικό όνομα**                       | **Δυνατότητα δημιουργίας** | **Δυνατότητα επεξεργασίας** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | όχι             | όχι           |
| msdyn_actualexpensecost_base           | όχι             | όχι           |
| msdyn_actuallaborcost                  | όχι             | όχι           |
| msdyn_actuallaborcost_base             | όχι             | όχι           |
| msdyn_actualsales                      | όχι             | όχι           |
| msdyn_actualsales_base                 | όχι             | όχι           |
| msdyn_contractlineproject              | ναι            | όχι           |
| msdyn_contractorganizationalunitid     | ναι            | όχι           |
| msdyn_contractorganizationalunitidname | ναι            | όχι           |
| msdyn_costconsumption                  | όχι             | όχι           |
| msdyn_costestimateatcomplete           | όχι             | όχι           |
| msdyn_costestimateatcomplete_base      | όχι             | όχι           |
| msdyn_costvariance                     | όχι             | όχι           |
| msdyn_costvariance_base                | όχι             | όχι           |
| msdyn_duration                         | όχι             | όχι           |
| msdyn_effort                           | όχι             | όχι           |
| msdyn_effortcompleted                  | όχι             | όχι           |
| msdyn_effortestimateatcompleteeac      | όχι             | όχι           |
| msdyn_effortremaining                  | όχι             | όχι           |
| msdyn_finish                           | ναι            | ναι          |
| msdyn_globalrevisiontoken              | όχι             | όχι           |
| msdyn_islinkedtomsprojectclient        | όχι             | όχι           |
| msdyn_islinkedtomsprojectclientname    | όχι             | όχι           |
| msdyn_linkeddocumenturl                | όχι             | όχι           |
| msdyn_msprojectdocument                | όχι             | όχι           |
| msdyn_msprojectdocumentname            | όχι             | όχι           |
| msdyn_plannedexpensecost               | όχι             | όχι           |
| msdyn_plannedexpensecost_base          | όχι             | όχι           |
| msdyn_plannedlaborcost                 | όχι             | όχι           |
| msdyn_plannedlaborcost_base            | όχι             | όχι           |
| msdyn_plannedsales                     | όχι             | όχι           |
| msdyn_plannedsales_base                | όχι             | όχι           |
| msdyn_progress                         | όχι             | όχι           |
| msdyn_remainingcost                    | όχι             | όχι           |
| msdyn_remainingcost_base               | όχι             | όχι           |
| msdyn_remainingsales                   | όχι             | όχι           |
| msdyn_remainingsales_base              | όχι             | όχι           |
| msdyn_replaylogheader                  | όχι             | όχι           |
| msdyn_salesconsumption                 | όχι             | όχι           |
| msdyn_salesestimateatcompleteeac       | όχι             | όχι           |
| msdyn_salesestimateatcompleteeac_base  | όχι             | όχι           |
| msdyn_salesvariance                    | όχι             | όχι           |
| msdyn_salesvariance_base               | όχι             | όχι           |
| msdyn_scheduleperformance              | όχι             | όχι           |
| msdyn_scheduleperformancename          | όχι             | όχι           |
| msdyn_schedulevariance                 | όχι             | όχι           |
| msdyn_taskearlieststart                | όχι             | όχι           |
| msdyn_teamsize                         | όχι             | όχι           |
| msdyn_teamsize_date                    | όχι             | όχι           |
| msdyn_teamsize_state                   | όχι             | όχι           |
| msdyn_totalactualcost                  | όχι             | όχι           |
| msdyn_totalactualcost_base             | όχι             | όχι           |
| msdyn_totalplannedcost                 | όχι             | όχι           |
| msdyn_totalplannedcost_base            | όχι             | όχι           |


## <a name="limitations-and-known-issues"></a>Περιορισμοί και γνωστά προβλήματα
Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:

- Τα API προγραμματισμού μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με άδεια χρήσης του Microsoft Project.** Δεν είναι δυνατό να χρησιμοποιηθούν από:
    - Χρήστες εφαρμογής
    - Χρήστες συστήματος
    - Χρήστες ενοποίησης
    - Άλλοι χρήστες που δεν διαθέτουν την απαιτούμενη άδεια χρήσης
- Κάθε **OperationSet** μπορεί να έχει μέγιστο αριθμό 100 λειτουργιών.
- Κάθε χρήστης μπορεί να έχει μόνο μέγιστο αριθμό 10 ανοιχτών **OperationSets**.
- Το Project Operations υποστηρίζει πλέον το πολύ έως 500 συνολικές εργασίες σε ένα έργο.
- Η κατάσταση αποτυχίας και τα αρχεία καταγραφής αποτυχίας του **OperationSet** δεν είναι αυτή τη στιγμή διαθέσιμα.
- [Όρια και περιορισμοί για έργα και εργασίες](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>Χειρισμός σφαλμάτων

   - Για να εξετάσετε τα σφάλματα που δημιουργούνται από τα σύνολα λειτουργιών, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Σύνολα λειτουργιών**.
   - Για να εξετάσετε τα σφάλματα που δημιουργούνται από την υπηρεσία προγραμματισμού έργου, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Αρχεία σφαλμάτων PSS**.

## <a name="sample-scenario"></a>Δείγμα σεναρίου

Σε αυτό το σενάριο, θα δημιουργήσετε ένα έργο, ένα μέλος ομάδας, τέσσερις εργασίες και δύο αναθέσεις πόρων. Στη συνέχεια, θα ενημερώσετε μία εργασία, θα ενημερώσετε το έργο, θα διαγράψετε μια εργασία, θα διαγράψετε μία ανάθεση πόρου και θα δημιουργήσετε μια εξάρτηση εργασίας.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Πρόσθετα δείγματα

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
