---
title: Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτό το άρθρο παρέχει πληροφορίες και δείγματα για τη χρήση API χρονοδιαγράμματος έργου.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541124"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_


**Οντότητες προγραμματισμού**

Τα API χρονοδιαγράμματος έργου παρέχουν τη δυνατότητα εκτέλεσης λειτουργιών δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού**. Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web. Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.

Ο παρακάτω πίνακας παρέχει μια πλήρη λίστα των οντοτήτων χρονοδιαγράμματος έργου.

| **Όνομα οντότητας**         | **Λογικό όνομα οντότητας**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Εργασία έργου            | msdyn_projecttask           |
| Εξάρτηση εργασίας έργου | msdyn_projecttaskdependency |
| Ανάθεση πόρου     | msdyn_resourceassignment    |
| Κάδος έργου          | msdyn_projectbucket         |
| Μέλος ομάδας έργου     | msdyn_projectteam           |
| Λίστες ελέγχου έργου      | msdyn_projectchecklist      |
| Ετικέτα έργου           | msdyn_projectlabel          |
| Εργασία έργου για την ετικέτα   | msdyn_projecttasktolabel    |
| Κύκλος επανάληψης έργου          | msdyn_projectsprint         |

**OperationSet**

Το OperationSet είναι ένα μοτίβο μονάδας εργασίας που μπορεί να χρησιμοποιηθεί όταν διάφορα αιτήματα που επηρεάζουν το χρονοδιάγραμμα πρέπει να υποβληθούν σε επεξεργασία εντός μιας συναλλαγής.

**API χρονοδιαγράμματος έργου**

Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος έργου.

| **API**                                 | Description                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | Αυτό το API χρησιμοποιείται για τη δημιουργία ενός έργου. Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.                         |
| **msdyn_CreateTeamMemberV1**            | Αυτό το API χρησιμοποιείται για τη δημιουργία ενός μέλους ομάδας έργου. Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.                                  |
| **msdyn_CreateOperationSetV1**          | Αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.                                        |
| **msdyn_PssCreateV1**                   | Αυτό το API χρησιμοποιείται για τη δημιουργία μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία δημιουργίας. |
| **msdyn_PssUpdateV1**                   | Αυτό το API χρησιμοποιείται για την ενημέρωση μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία ενημέρωσης  |
| **msdyn_PssDeleteV1**                   | Αυτό το API χρησιμοποιείται για τη διαγραφή μιας οντότητας. Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία διαγραφής. |
| **msdyn_ExecuteOperationSetV1**         | Αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | Αυτό το API χρησιμοποιείται για την ενημέρωση μιας προγραμματισμένης εργασίας ανάθεσης πόρων.                                                        |



**Χρήση API χρονοδιαγράμματος έργου με το OperationSet**

Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**. Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.

**Υποστηριζόμενες λειτουργίες**

| **Οντότητα προγραμματισμού**   | **Δημιουργία** | **Ενημέρωση** | **Delete** | **Σημαντικές επισημάνσεις**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Εργασία έργου            | Ναι        | Ναι        | Ναι        | Μπορείτε να επεξεργαστείτε τα πεδία **Πρόοδος**, **EffortCompleted** και **EffortRemaining** στο Project for the Web, αλλά δεν είναι δυνατή η επεξεργασία τους στο Project Operations.                                                                                                                                                                                             |
| Εξάρτηση εργασίας έργου | Όχι        | όχι         | Όχι        | Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.                                                                                                                                                                                                                                 |
| Ανάθεση πόρου     | Όχι        | Ναι\*      | Όχι        | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**. Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται. Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα. Έχει παρασχεθεί ένα ξεχωριστό API για την ενημέρωση των αδειών εκχώρησης πόρων. |
| Κάδος έργου          | Όχι        | Όχι        | Όχι        | Ο προεπιλεγμένος κάδος δημιουργείται με τη χρήση του API **CreateProjectV1**. Η υποστήριξη για τη δημιουργία και διαγραφή κάδων έργων προστέθηκε στην έκδοση ενημέρωσης 16.                                                                                                                                                                                                   |
| Μέλος ομάδας έργου     | Ναι        | Ναι        | Ναι        | Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**.                                                                                                                                                                                                                                                                                           |
| Project                 | Ναι        | Ναι        |            | Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**.                                                                                       |
| Λίστες ελέγχου έργου      | Όχι        | Όχι        | Όχι        |                                                                                                                                                                                                                                                                                                                                                         |
| Ετικέτα έργου           | όχι         | Όχι        | όχι         | Τα ονόματα ετικετών μπορούν να αλλάξουν. Αυτή η δυνατότητα είναι διαθέσιμη μόνο στο Project for the Web                                                                                                                                                                                                                                                                      |
| Εργασία έργου για την ετικέτα   | Όχι        | όχι         | Όχι        | Αυτή η δυνατότητα είναι διαθέσιμη μόνο στο Project for the Web                                                                                                                                                                                                                                                                                                  |
| Κύκλος επανάληψης έργου          | Όχι        | Όχι        | Όχι        | Το πεδίο **Έναρξη** πρέπει να έχει μια ημερομηνία προγενέστερη από το πεδίο **Τέλος**. Οι κύκλοι επανάληψης για το ίδιο έργο δεν επικαλύπτονται μεταξύ τους. Αυτή η δυνατότητα είναι διαθέσιμη μόνο στο Project for the Web                                                                                                                                                                    |




Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση. Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί. Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.

**Περιορισμοί και γνωστά προβλήματα**

Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:

-   Τα API χρονοδιαγράμματος έργου μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με Άδεια χρήσης του Microsoft Project**. Δεν είναι δυνατό να χρησιμοποιηθούν από:
    -   Χρήστες εφαρμογής
    -   Χρήστες συστήματος
    -   Χρήστες ενοποίησης
    -   Άλλοι χρήστες που δεν διαθέτουν την απαιτούμενη άδεια χρήσης
-   Κάθε **OperationSet** μπορεί να έχει μέγιστο αριθμό 100 λειτουργιών.
-   Κάθε χρήστης μπορεί να έχει μόνο μέγιστο αριθμό 10 ανοιχτών **OperationSets**.
-   Το Project Operations υποστηρίζει πλέον το πολύ έως 500 συνολικές εργασίες σε ένα έργο.
-   Κάθε λειτουργία ενημέρωσης ενημέρωσης καμπύλης εκχώρησης πόρων μετράει ως μία λειτουργία.
-   Κάθε λίστα ενημερωμένων καμπυλών μπορεί να περιέχει το πολύ έως 100 τμήματα χρόνου.
-   Η κατάσταση αποτυχίας και τα αρχεία καταγραφής αποτυχίας του **OperationSet** δεν είναι αυτή τη στιγμή διαθέσιμα.
-   Υπάρχει μέγιστο όριο 400 κύκλοι επανάληψης ανά έργο.
-   [Όρια και περιορισμοί για έργα και εργασίες](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   Οι ετικέτες είναι αυτήν τη στιγμή διαθέσιμες μόνο για το Project for the Web.

**Χειρισμός σφαλμάτων**

-   Για να εξετάσετε τα σφάλματα που δημιουργούνται από τα σύνολα λειτουργιών, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Σύνολα λειτουργιών**.
-   Για να εξετάσετε τα σφάλματα που δημιουργούνται από την υπηρεσία χρονοδιαγράμματος έργου, μεταβείτε στις **Ρυθμίσεις** \> **Ενοποίηση προγραμματισμού** \> **Αρχεία καταγραφής σφαλμάτων PSS**.

**Επεξεργασία καμπύλων εκχώρησης πόρων**

Σε αντίθεση με όλα τα άλλα API προγραμματισμού έργου που ενημερώνουν μια οντότητα, το API καμπύλης ανάθεσης πόρων είναι αποκλειστικά υπεύθυνο για τις ενημερώσεις σε ένα μόνο πεδίο, msdyn_plannedwork, σε μία μόνο οντότητα msydn_resourceassignment.

Η δεδομένη λειτουργία χρονοδιαγράμματος είναι:

-   **σταθερές μονάδες**
-   το ημερολόγιο έργου είναι 9-5p είναι 9-5ps, Δευτ., Τρίτ., Πέμπ., Παρασκ. (ΚΑΜΙΑ ΕΡΓΑΣΙΑ ΤΗΝ ΤΕΤΑΡΤΗ)
-   και το ημερολόγιο πόρων είναι 9-1p PST Δευτέρα έως Παρασκευή

Αυτή η εκχώρηση είναι για μία εβδομάδα, τέσσερις ώρες την ημέρα. Αυτό συμβαίνει επειδή το ημερολόγιο πόρου προέρχεται από 9-1 PST ή τέσσερις ώρες την ημέρα.

| &nbsp;     | Κλείσιμο εργασίας | Ημερομηνία έναρξης | Ημερομηνία λήξης  | Ποσότητα | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 υπάλληλος |  T1  | 6/13/2022  | 6/17/2022 | 20       | 4         | 4         | 4         | 4         | 4         |

Για παράδειγμα, εάν θέλετε ο εργαζόμενος να εργάζεται μόνο τρεις ώρες κάθε ημέρα αυτήν την εβδομάδα και να έχει μια ώρα για άλλες εργασίες.

#### <a name="updatedcontours-sample-payload"></a>Δείγμα ωφέλιμου φορτίου UpdatedContours:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

Αυτή είναι η εκχώρηση μετά την εκτέλεση του API χρονοδιαγράμματος ενημέρωσης καμπύλης.

| &nbsp;     | Κλείσιμο εργασίας | Ημερομηνία έναρξης | Ημερομηνία λήξης  | Ποσότητα | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 υπάλληλος | T1   | 6/13/2022  | 6/17/2022 | 15       | 3         | 3         | 3         | 3         | 3         |


**Δείγμα σεναρίου**

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

** Πρόσθετα δείγματα

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
