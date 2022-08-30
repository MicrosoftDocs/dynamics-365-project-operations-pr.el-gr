---
title: Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτό το άρθρο παρέχει πληροφορίες και δείγματα για τη χρήση API χρονοδιαγράμματος έργου.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3248a057b831d81fdc2bc198b4ed4da5e46462f2
ms.sourcegitcommit: 8edd24201cded2672cec16cd5dc84c6a3516b6c2
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/06/2022
ms.locfileid: "9230315"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_



## <a name="scheduling-entities"></a>Οντότητες προγραμματισμού

Τα API χρονοδιαγράμματος έργου παρέχουν τη δυνατότητα εκτέλεσης λειτουργιών δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού**. Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web. Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.

Ο παρακάτω πίνακας παρέχει μια πλήρη λίστα των οντοτήτων χρονοδιαγράμματος έργου.

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

## <a name="project-schedule-apis"></a>API χρονοδιαγράμματος έργου

Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος έργου.

- **msdyn_CreateProjectV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός έργου. Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.
- **msdyn_CreateTeamMemberV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός μέλους ομάδας έργου. Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.
- **msdyn_CreateOperationSetV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.
- **msdyn_PssCreateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία δημιουργίας.
- **msdyn_PssUpdateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για την ενημέρωση μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία ενημέρωσης.
- **msdyn_PssDeleteV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη διαγραφή μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία διαγραφής.
- **msdyn_ExecuteOperationSetV1**: αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.

## <a name="using-project-schedule-apis-with-operationset"></a>Χρήση API χρονοδιαγράμματος έργου με το OperationSet

Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**. Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.

## <a name="supported-operations"></a>Υποστηριζόμενες λειτουργίες

| Οντότητα προγραμματισμού | Δημιουργία | Update | Delete | Σημαντικές επισημάνσεις |
| --- | --- | --- | --- | --- |
Εργασία έργου | Ναι | Ναι | Ναι | Μπορείτε να επεξεργαστείτε τα πεδία **Πρόοδος**, **EffortCompleted** και **EffortRemaining** στο Project for the Web, αλλά δεν είναι δυνατή η επεξεργασία τους στο Project Operations.  |
| Εξάρτηση εργασίας έργου | Ναι |  | Ναι | Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα. |
| Ανάθεση πόρου | Ναι | Ναι | | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**. Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα. |
| Κάδος έργου | Ναι | Ναι | Ναι | Ο προεπιλεγμένος κάδος δημιουργείται με τη χρήση του API **CreateProjectV1**. Η υποστήριξη για τη δημιουργία και διαγραφή κάδων έργων προστέθηκε στην έκδοση ενημέρωσης 16. |
| Μέλος ομάδας έργου | Ναι | Ναι | Ναι | Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**. |
| Project | Ναι | Ναι |  | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**. |

Αυτά τα API μπορούν να καλούνται με αντικείμενα οντότητας που περιλαμβάνουν προσαρμοσμένα πεδία.

Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση. Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί. Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.

## <a name="restricted-fields"></a>Περιορισμένα πεδία

Οι παρακάτω πίνακες ορίζουν τα πεδία που περιορίζονται από τα **Δημιουργία** και **Επεξεργασία**.

### <a name="project-task"></a>Εργασία έργου

| Λογικό όνομα                           | Δυνατότητα δημιουργίας     | Δυνατότητα επεξεργασίας         |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | No             | No               |
| msdyn_actualcost_base                  | No             | No               |
| msdyn_actualend                        | No             | No               |
| msdyn_actualsales                      | No             | No               |
| msdyn_actualsales_base                 | No             | No               |
| msdyn_actualstart                      | No             | No               |
| msdyn_costatcompleteestimate           | No             | No               |
| msdyn_costatcompleteestimate_base      | No             | No               |
| msdyn_costconsumptionpercentage        | No             | No               |
| msdyn_effortcompleted                  | Όχι (ναι για το Project)             | Όχι (ναι για το Project)               |
| msdyn_effortremaining                  | Όχι (ναι για το Project)              | Όχι (ναι για το Project)                |
| msdyn_effortestimateatcomplete         | No             | No               |
| msdyn_iscritical                       | No             | No               |
| msdyn_iscriticalname                   | No             | No               |
| msdyn_ismanual                         | No             | No               |
| msdyn_ismanualname                     | No             | No               |
| msdyn_ismilestone                      | No             | No               |
| msdyn_ismilestonename                  | No             | No               |
| msdyn_LinkStatus                       | No             | No               |
| msdyn_linkstatusname                   | No             | No               |
| msdyn_msprojectclientid                | No             | No               |
| msdyn_plannedcost                      | No             | No               |
| msdyn_plannedcost_base                 | No             | No               |
| msdyn_plannedsales                     | No             | No               |
| msdyn_plannedsales_base                | No             | No               |
| msdyn_pluginprocessingdata             | No             | No               |
| msdyn_progress                         | Όχι (ναι για το Project)             | Όχι (ναι για το Project) |
| msdyn_remainingcost                    | No             | No               |
| msdyn_remainingcost_base               | No             | No               |
| msdyn_remainingsales                   | No             | No               |
| msdyn_remainingsales_base              | No             | No               |
| msdyn_requestedhours                   | No             | No               |
| msdyn_resourcecategory                 | No             | No               |
| msdyn_resourcecategoryname             | No             | No               |
| msdyn_resourceorganizationalunitid     | No             | No               |
| msdyn_resourceorganizationalunitidname | No             | No               |
| msdyn_salesconsumptionpercentage       | No             | No               |
| msdyn_salesestimateatcomplete          | No             | No               |
| msdyn_salesestimateatcomplete_base     | No             | No               |
| msdyn_salesvariance                    | No             | No               |
| msdyn_salesvariance_base               | No             | No               |
| msdyn_scheduleddurationminutes         | No             | No               |
| msdyn_scheduledend                     | No             | No               |
| msdyn_scheduledstart                   | No             | No               |
| msdyn_schedulevariance                 | No             | No               |
| msdyn_skipupdateestimateline           | No             | No               |
| msdyn_skipupdateestimatelinename       | No             | No               |
| msdyn_summary                          | No             | No               |
| msdyn_varianceofcost                   | No             | No               |
| msdyn_varianceofcost_base              | No             | No               |

### <a name="project-task-dependency"></a>Εξάρτηση εργασίας έργου

| Λογικό όνομα                  | Δυνατότητα δημιουργίας     | Δυνατότητα επεξεργασίας     |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | No             | No           |
| msdyn_linktypename            | No             | No           |
| msdyn_predecessortask         | Ναι            | No           |
| msdyn_predecessortaskname     | Ναι            | No           |
| msdyn_project                 | Ναι            | No           |
| msdyn_projectname             | Ναι            | No           |
| msdyn_projecttaskdependencyid | Ναι            | No           |
| msdyn_successortask           | Ναι            | No           |
| msdyn_successortaskname       | Ναι            | No           |

### <a name="resource-assignment"></a>Ανάθεση πόρου

| Λογικό όνομα                 | Δυνατότητα δημιουργίας     | Δυνατότητα επεξεργασίας     |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | Ναι            | No           |
| msdyn_bookableresourceidname | Ναι            | No           |
| msdyn_bookingstatusid        | No             | No           |
| msdyn_bookingstatusidname    | No             | No           |
| msdyn_committype             | No             | No           |
| msdyn_committypename         | No             | No           |
| msdyn_effort                 | No             | No           |
| msdyn_effortcompleted        | No             | No           |
| msdyn_effortremaining        | No             | No           |
| msdyn_finish                 | No             | No           |
| msdyn_plannedcost            | No             | No           |
| msdyn_plannedcost_base       | No             | No           |
| msdyn_plannedcostcontour     | No             | No           |
| msdyn_plannedsales           | No             | No           |
| msdyn_plannedsales_base      | No             | No           |
| msdyn_plannedsalescontour    | No             | No           |
| msdyn_plannedwork            | No             | No           |
| msdyn_projectid              | Ναι            | No           |
| msdyn_projectidname          | No             | No           |
| msdyn_projectteamid          | No             | No           |
| msdyn_projectteamidname      | No             | No           |
| msdyn_start                  | No             | No           |
| msdyn_taskid                 | No             | No           |
| msdyn_taskidname             | No             | No           |
| msdyn_userresourceid         | No             | No           |

### <a name="project-team-member"></a>Μέλος ομάδας έργου

| Λογικό όνομα                                     | Δυνατότητα δημιουργίας     | Δυνατότητα επεξεργασίας     |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | No             | No           |
| msdyn_creategenericteammemberwithrequirementname | No             | No           |
| msdyn_deletestatus                               | No             | No           |
| msdyn_deletestatusname                           | No             | No           |
| msdyn_effort                                     | No             | No           |
| msdyn_effortcompleted                            | No             | No           |
| msdyn_effortremaining                            | No             | No           |
| msdyn_finish                                     | No             | No           |
| msdyn_hardbookedhours                            | No             | No           |
| msdyn_hours                                      | No             | No           |
| msdyn_markedfordeletiontimer                     | No             | No           |
| msdyn_markedfordeletiontimestamp                 | No             | No           |
| msdyn_msprojectclientid                          | No             | No           |
| msdyn_percentage                                 | No             | No           |
| msdyn_requiredhours                              | No             | No           |
| msdyn_softbookedhours                            | No             | No           |
| msdyn_start                                      | No             | No           |

### <a name="project"></a>Project

| Λογικό όνομα                           | Δυνατότητα δημιουργίας     | Δυνατότητα επεξεργασίας     |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | No             | No           |
| msdyn_actualexpensecost_base           | No             | No           |
| msdyn_actuallaborcost                  | No             | No           |
| msdyn_actuallaborcost_base             | No             | No           |
| msdyn_actualsales                      | No             | No           |
| msdyn_actualsales_base                 | No             | No           |
| msdyn_contractlineproject              | Ναι            | No           |
| msdyn_contractorganizationalunitid     | Ναι            | No           |
| msdyn_contractorganizationalunitidname | Ναι            | No           |
| msdyn_costconsumption                  | No             | No           |
| msdyn_costestimateatcomplete           | No             | No           |
| msdyn_costestimateatcomplete_base      | No             | No           |
| msdyn_costvariance                     | No             | No           |
| msdyn_costvariance_base                | No             | No           |
| msdyn_duration                         | No             | No           |
| msdyn_effort                           | No             | No           |
| msdyn_effortcompleted                  | No             | No           |
| msdyn_effortestimateatcompleteeac      | No             | No           |
| msdyn_effortremaining                  | No             | No           |
| msdyn_finish                           | Ναι            | Ναι          |
| msdyn_globalrevisiontoken              | No             | No           |
| msdyn_islinkedtomsprojectclient        | No             | No           |
| msdyn_islinkedtomsprojectclientname    | No             | No           |
| msdyn_linkeddocumenturl                | No             | No           |
| msdyn_msprojectdocument                | No             | No           |
| msdyn_msprojectdocumentname            | No             | No           |
| msdyn_plannedexpensecost               | No             | No           |
| msdyn_plannedexpensecost_base          | No             | No           |
| msdyn_plannedlaborcost                 | No             | No           |
| msdyn_plannedlaborcost_base            | No             | No           |
| msdyn_plannedsales                     | No             | No           |
| msdyn_plannedsales_base                | No             | No           |
| msdyn_progress                         | No             | No           |
| msdyn_remainingcost                    | No             | No           |
| msdyn_remainingcost_base               | No             | No           |
| msdyn_remainingsales                   | No             | No           |
| msdyn_remainingsales_base              | No             | No           |
| msdyn_replaylogheader                  | No             | No           |
| msdyn_salesconsumption                 | No             | No           |
| msdyn_salesestimateatcompleteeac       | No             | No           |
| msdyn_salesestimateatcompleteeac_base  | No             | No           |
| msdyn_salesvariance                    | No             | No           |
| msdyn_salesvariance_base               | No             | No           |
| msdyn_scheduleperformance              | No             | No           |
| msdyn_scheduleperformancename          | No             | No           |
| msdyn_schedulevariance                 | No             | No           |
| msdyn_taskearlieststart                | No             | No           |
| msdyn_teamsize                         | No             | No           |
| msdyn_teamsize_date                    | No             | No           |
| msdyn_teamsize_state                   | No             | No           |
| msdyn_totalactualcost                  | No             | No           |
| msdyn_totalactualcost_base             | No             | No           |
| msdyn_totalplannedcost                 | No             | No           |
| msdyn_totalplannedcost_base            | No             | No           |

### <a name="project-bucket"></a>Κάδος έργου

| Λογικό όνομα          | Δυνατότητα δημιουργίας      | Δυνατότητα επεξεργασίας     |
|-----------------------|-----------------|--------------|
| msdyn_displayorder    | Ναι             | No           |
| msdyn_name            | Ναι             | Ναι          |
| msdyn_project         | Ναι             | No           |
| msdyn_projectbucketid | Ναι             | No           |

## <a name="limitations-and-known-issues"></a>Περιορισμοί και γνωστά προβλήματα
Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:

- Τα API χρονοδιαγράμματος έργου μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με Άδεια χρήσης του Microsoft Project**. Δεν είναι δυνατό να χρησιμοποιηθούν από:

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
- Για να εξετάσετε τα σφάλματα που δημιουργούνται από την υπηρεσία χρονοδιαγράμματος έργου, μεταβείτε στις **Ρυθμίσεις** \> **Ενοποίηση προγραμματισμού** \> **Αρχεία καταγραφής σφαλμάτων PSS**.

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
