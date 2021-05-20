---
title: Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτή θέμα παρέχει πληροφορίες και δείγματα για τη χρήση API χρονοδιαγράμματος.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950804"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="36928-103">Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="36928-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="36928-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="36928-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="36928-105">Ορισμένες ή όλες οι λειτουργίες που αναφέρονται σε αυτό το θέμα είναι διαθέσιμες ως μέρος μιας έκδοσης προεπισκόπησης.</span><span class="sxs-lookup"><span data-stu-id="36928-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="36928-106">Το περιεχόμενο και η λειτουργικότητα υπόκεινται σε αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="36928-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="36928-107">Οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="36928-107">Scheduling entities</span></span>

<span data-ttu-id="36928-108">Τα API χρονοδιαγράμματος παρέχουν τη δυνατότητα εκτέλεσης δημιουργίας, ενημέρωσης και διαγραφής λειτουργιών με **Οντότητες προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="36928-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="36928-109">Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web.</span><span class="sxs-lookup"><span data-stu-id="36928-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="36928-110">Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="36928-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="36928-111">Ο παρακάτω πίνακας περιλαμβάνει μια πλήρη λίστα των **Οντοτήτων προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="36928-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="36928-112">Όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="36928-112">Entity name</span></span>  | <span data-ttu-id="36928-113">Λογικό όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="36928-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="36928-114">Project</span><span class="sxs-lookup"><span data-stu-id="36928-114">Project</span></span> | <span data-ttu-id="36928-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="36928-115">msdyn_project</span></span> |
| <span data-ttu-id="36928-116">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="36928-116">Project Task</span></span>  | <span data-ttu-id="36928-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="36928-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="36928-118">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-118">Project Task Dependency</span></span>  | <span data-ttu-id="36928-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="36928-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="36928-120">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="36928-120">Resource Assignment</span></span> | <span data-ttu-id="36928-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="36928-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="36928-122">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="36928-122">Project Bucket</span></span>  | <span data-ttu-id="36928-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="36928-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="36928-124">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-124">Project Team Member</span></span> | <span data-ttu-id="36928-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="36928-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="36928-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="36928-126">OperationSet</span></span>

<span data-ttu-id="36928-127">Το OperationSet είναι ένα μοτίβο μονάδας εργασίας που μπορεί να χρησιμοποιηθεί όταν διάφορα αιτήματα που επηρεάζουν το χρονοδιάγραμμα πρέπει να υποβληθούν σε επεξεργασία εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="36928-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="36928-128">Προγραμματισμός API</span><span class="sxs-lookup"><span data-stu-id="36928-128">Schedule APIs</span></span>

<span data-ttu-id="36928-129">Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="36928-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="36928-130">**msdyn_CreateProjectV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="36928-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="36928-131">Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="36928-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="36928-132">**msdyn_CreateTeamMemberV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός μέλους ομάδας έργου.</span><span class="sxs-lookup"><span data-stu-id="36928-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="36928-133">Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="36928-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="36928-134">**msdyn_CreateOperationSetV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="36928-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="36928-135">**msdyn_PSSCreateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="36928-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="36928-136">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία δημιουργίας.</span><span class="sxs-lookup"><span data-stu-id="36928-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="36928-137">**msdyn_PSSUpdateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για την ενημέρωση μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="36928-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="36928-138">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία ενημέρωσης.</span><span class="sxs-lookup"><span data-stu-id="36928-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="36928-139">**msdyn_PSSDeleteV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη διαγραφή μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="36928-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="36928-140">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία διαγραφής.</span><span class="sxs-lookup"><span data-stu-id="36928-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="36928-141">**msdyn_ExecuteOperationSetV1**: αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="36928-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="36928-142">Χρήση API χρονοδιαγράμματος με το OperationSet</span><span class="sxs-lookup"><span data-stu-id="36928-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="36928-143">Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="36928-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="36928-144">Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="36928-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="36928-145">Υποστηριζόμενες λειτουργίες</span><span class="sxs-lookup"><span data-stu-id="36928-145">Supported operations</span></span>

| <span data-ttu-id="36928-146">Οντότητα προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="36928-146">Scheduling entity</span></span> | <span data-ttu-id="36928-147">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="36928-147">Create</span></span> | <span data-ttu-id="36928-148">Ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="36928-148">Update</span></span> | <span data-ttu-id="36928-149">Delete</span><span class="sxs-lookup"><span data-stu-id="36928-149">Delete</span></span> | <span data-ttu-id="36928-150">Σημαντικές επισημάνσεις</span><span class="sxs-lookup"><span data-stu-id="36928-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="36928-151">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="36928-151">Project task</span></span> | <span data-ttu-id="36928-152">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-152">Yes</span></span> | <span data-ttu-id="36928-153">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-153">Yes</span></span> | <span data-ttu-id="36928-154">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-154">Yes</span></span> | <span data-ttu-id="36928-155">Κανένας</span><span class="sxs-lookup"><span data-stu-id="36928-155">None</span></span> |
| <span data-ttu-id="36928-156">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-156">Project task dependency</span></span> | <span data-ttu-id="36928-157">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-157">Yes</span></span> | <span data-ttu-id="36928-158">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-158">Yes</span></span> | | <span data-ttu-id="36928-159">Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="36928-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="36928-160">Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="36928-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="36928-161">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="36928-161">Resource assignment</span></span> | <span data-ttu-id="36928-162">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-162">Yes</span></span> | <span data-ttu-id="36928-163">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-163">Yes</span></span> | | <span data-ttu-id="36928-164">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="36928-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="36928-165">Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="36928-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="36928-166">Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="36928-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="36928-167">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="36928-167">Project bucket</span></span> | <span data-ttu-id="36928-168">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="36928-168">N/A</span></span> | <span data-ttu-id="36928-169">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="36928-169">N/A</span></span> | <span data-ttu-id="36928-170">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="36928-170">N/A</span></span> | <span data-ttu-id="36928-171">Ο προεπιλεγμένος κάδος δημιουργείται με χρήση του API **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="36928-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="36928-172">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-172">Project team member</span></span> | <span data-ttu-id="36928-173">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-173">Yes</span></span> | <span data-ttu-id="36928-174">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-174">Yes</span></span> | <span data-ttu-id="36928-175">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-175">Yes</span></span> | <span data-ttu-id="36928-176">Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="36928-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="36928-177">Project</span><span class="sxs-lookup"><span data-stu-id="36928-177">Project</span></span> | <span data-ttu-id="36928-178">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-178">Yes</span></span> | <span data-ttu-id="36928-179">Ναι</span><span class="sxs-lookup"><span data-stu-id="36928-179">Yes</span></span> | <span data-ttu-id="36928-180">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="36928-180">N/A</span></span> | <span data-ttu-id="36928-181">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**.</span><span class="sxs-lookup"><span data-stu-id="36928-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="36928-182">Αυτά τα API μπορούν να καλούνται με αντικείμενα οντότητας που περιλαμβάνουν προσαρμοσμένα πεδία.</span><span class="sxs-lookup"><span data-stu-id="36928-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="36928-183">Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="36928-183">The ID property is optional.</span></span> <span data-ttu-id="36928-184">Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="36928-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="36928-185">Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.</span><span class="sxs-lookup"><span data-stu-id="36928-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="36928-186">Περιορισμένα πεδία</span><span class="sxs-lookup"><span data-stu-id="36928-186">Restricted fields</span></span>

<span data-ttu-id="36928-187">Οι παρακάτω πίνακες ορίζουν τα πεδία που περιορίζονται από τα **Δημιουργία** και **Επεξεργασία.**</span><span class="sxs-lookup"><span data-stu-id="36928-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="36928-188">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="36928-188">Project task</span></span>

| <span data-ttu-id="36928-189">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="36928-189">**Logical name**</span></span>                       | <span data-ttu-id="36928-190">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="36928-190">**Can create**</span></span> | <span data-ttu-id="36928-191">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="36928-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="36928-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="36928-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="36928-193">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-193">no</span></span>             | <span data-ttu-id="36928-194">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-194">no</span></span>               |
| <span data-ttu-id="36928-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="36928-196">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-196">no</span></span>             | <span data-ttu-id="36928-197">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-197">no</span></span>               |
| <span data-ttu-id="36928-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="36928-198">msdyn_actualend</span></span>                        | <span data-ttu-id="36928-199">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-199">no</span></span>             | <span data-ttu-id="36928-200">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-200">no</span></span>               |
| <span data-ttu-id="36928-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="36928-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="36928-202">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-202">no</span></span>             | <span data-ttu-id="36928-203">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-203">no</span></span>               |
| <span data-ttu-id="36928-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="36928-205">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-205">no</span></span>             | <span data-ttu-id="36928-206">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-206">no</span></span>               |
| <span data-ttu-id="36928-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="36928-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="36928-208">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-208">no</span></span>             | <span data-ttu-id="36928-209">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-209">no</span></span>               |
| <span data-ttu-id="36928-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="36928-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="36928-211">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-211">no</span></span>             | <span data-ttu-id="36928-212">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-212">no</span></span>               |
| <span data-ttu-id="36928-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="36928-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="36928-214">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-214">no</span></span>             | <span data-ttu-id="36928-215">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-215">no</span></span>               |
| <span data-ttu-id="36928-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="36928-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="36928-217">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-217">no</span></span>             | <span data-ttu-id="36928-218">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-218">no</span></span>               |
| <span data-ttu-id="36928-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="36928-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="36928-220">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-220">no</span></span>             | <span data-ttu-id="36928-221">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-221">no</span></span>               |
| <span data-ttu-id="36928-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="36928-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="36928-223">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-223">no</span></span>             | <span data-ttu-id="36928-224">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-224">no</span></span>               |
| <span data-ttu-id="36928-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="36928-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="36928-226">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-226">no</span></span>             | <span data-ttu-id="36928-227">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-227">no</span></span>               |
| <span data-ttu-id="36928-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="36928-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="36928-229">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-229">no</span></span>             | <span data-ttu-id="36928-230">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-230">no</span></span>               |
| <span data-ttu-id="36928-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="36928-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="36928-232">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-232">no</span></span>             | <span data-ttu-id="36928-233">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-233">no</span></span>               |
| <span data-ttu-id="36928-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="36928-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="36928-235">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-235">no</span></span>             | <span data-ttu-id="36928-236">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-236">no</span></span>               |
| <span data-ttu-id="36928-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="36928-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="36928-238">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-238">no</span></span>             | <span data-ttu-id="36928-239">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-239">no</span></span>               |
| <span data-ttu-id="36928-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="36928-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="36928-241">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-241">no</span></span>             | <span data-ttu-id="36928-242">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-242">no</span></span>               |
| <span data-ttu-id="36928-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="36928-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="36928-244">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-244">no</span></span>             | <span data-ttu-id="36928-245">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-245">no</span></span>               |
| <span data-ttu-id="36928-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="36928-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="36928-247">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-247">no</span></span>             | <span data-ttu-id="36928-248">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-248">no</span></span>               |
| <span data-ttu-id="36928-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="36928-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="36928-250">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-250">no</span></span>             | <span data-ttu-id="36928-251">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-251">no</span></span>               |
| <span data-ttu-id="36928-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="36928-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="36928-253">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-253">no</span></span>             | <span data-ttu-id="36928-254">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-254">no</span></span>               |
| <span data-ttu-id="36928-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="36928-256">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-256">no</span></span>             | <span data-ttu-id="36928-257">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-257">no</span></span>               |
| <span data-ttu-id="36928-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="36928-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="36928-259">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-259">no</span></span>             | <span data-ttu-id="36928-260">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-260">no</span></span>               |
| <span data-ttu-id="36928-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="36928-262">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-262">no</span></span>             | <span data-ttu-id="36928-263">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-263">no</span></span>               |
| <span data-ttu-id="36928-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="36928-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="36928-265">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-265">no</span></span>             | <span data-ttu-id="36928-266">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-266">no</span></span>               |
| <span data-ttu-id="36928-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="36928-267">msdyn_progress</span></span>                         | <span data-ttu-id="36928-268">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-268">no</span></span>             | <span data-ttu-id="36928-269">όχι (ναι για P4W)</span><span class="sxs-lookup"><span data-stu-id="36928-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="36928-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="36928-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="36928-271">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-271">no</span></span>             | <span data-ttu-id="36928-272">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-272">no</span></span>               |
| <span data-ttu-id="36928-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="36928-274">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-274">no</span></span>             | <span data-ttu-id="36928-275">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-275">no</span></span>               |
| <span data-ttu-id="36928-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="36928-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="36928-277">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-277">no</span></span>             | <span data-ttu-id="36928-278">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-278">no</span></span>               |
| <span data-ttu-id="36928-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="36928-280">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-280">no</span></span>             | <span data-ttu-id="36928-281">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-281">no</span></span>               |
| <span data-ttu-id="36928-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="36928-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="36928-283">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-283">no</span></span>             | <span data-ttu-id="36928-284">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-284">no</span></span>               |
| <span data-ttu-id="36928-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="36928-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="36928-286">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-286">no</span></span>             | <span data-ttu-id="36928-287">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-287">no</span></span>               |
| <span data-ttu-id="36928-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="36928-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="36928-289">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-289">no</span></span>             | <span data-ttu-id="36928-290">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-290">no</span></span>               |
| <span data-ttu-id="36928-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="36928-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="36928-292">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-292">no</span></span>             | <span data-ttu-id="36928-293">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-293">no</span></span>               |
| <span data-ttu-id="36928-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="36928-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="36928-295">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-295">no</span></span>             | <span data-ttu-id="36928-296">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-296">no</span></span>               |
| <span data-ttu-id="36928-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="36928-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="36928-298">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-298">no</span></span>             | <span data-ttu-id="36928-299">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-299">no</span></span>               |
| <span data-ttu-id="36928-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="36928-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="36928-301">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-301">no</span></span>             | <span data-ttu-id="36928-302">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-302">no</span></span>               |
| <span data-ttu-id="36928-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="36928-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="36928-304">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-304">no</span></span>             | <span data-ttu-id="36928-305">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-305">no</span></span>               |
| <span data-ttu-id="36928-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="36928-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="36928-307">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-307">no</span></span>             | <span data-ttu-id="36928-308">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-308">no</span></span>               |
| <span data-ttu-id="36928-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="36928-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="36928-310">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-310">no</span></span>             | <span data-ttu-id="36928-311">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-311">no</span></span>               |
| <span data-ttu-id="36928-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="36928-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="36928-313">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-313">no</span></span>             | <span data-ttu-id="36928-314">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-314">no</span></span>               |
| <span data-ttu-id="36928-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="36928-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="36928-316">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-316">no</span></span>             | <span data-ttu-id="36928-317">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-317">no</span></span>               |
| <span data-ttu-id="36928-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="36928-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="36928-319">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-319">no</span></span>             | <span data-ttu-id="36928-320">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-320">no</span></span>               |
| <span data-ttu-id="36928-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="36928-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="36928-322">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-322">no</span></span>             | <span data-ttu-id="36928-323">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-323">no</span></span>               |
| <span data-ttu-id="36928-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="36928-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="36928-325">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-325">no</span></span>             | <span data-ttu-id="36928-326">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-326">no</span></span>               |
| <span data-ttu-id="36928-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="36928-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="36928-328">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-328">no</span></span>             | <span data-ttu-id="36928-329">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-329">no</span></span>               |
| <span data-ttu-id="36928-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="36928-330">msdyn_summary</span></span>                          | <span data-ttu-id="36928-331">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-331">no</span></span>             | <span data-ttu-id="36928-332">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-332">no</span></span>               |
| <span data-ttu-id="36928-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="36928-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="36928-334">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-334">no</span></span>             | <span data-ttu-id="36928-335">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-335">no</span></span>               |
| <span data-ttu-id="36928-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="36928-337">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-337">no</span></span>             | <span data-ttu-id="36928-338">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="36928-339">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-339">Project task dependency</span></span>

| <span data-ttu-id="36928-340">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="36928-340">**Logical name**</span></span>              | <span data-ttu-id="36928-341">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="36928-341">**Can create**</span></span> | <span data-ttu-id="36928-342">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="36928-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="36928-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="36928-343">msdyn_linktype</span></span>                | <span data-ttu-id="36928-344">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-344">no</span></span>             | <span data-ttu-id="36928-345">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-345">no</span></span>           |
| <span data-ttu-id="36928-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="36928-346">msdyn_linktypename</span></span>            | <span data-ttu-id="36928-347">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-347">no</span></span>             | <span data-ttu-id="36928-348">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-348">no</span></span>           |
| <span data-ttu-id="36928-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="36928-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="36928-350">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-350">yes</span></span>            | <span data-ttu-id="36928-351">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-351">no</span></span>           |
| <span data-ttu-id="36928-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="36928-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="36928-353">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-353">yes</span></span>            | <span data-ttu-id="36928-354">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-354">no</span></span>           |
| <span data-ttu-id="36928-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="36928-355">msdyn_project</span></span>                 | <span data-ttu-id="36928-356">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-356">yes</span></span>            | <span data-ttu-id="36928-357">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-357">no</span></span>           |
| <span data-ttu-id="36928-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="36928-358">msdyn_projectname</span></span>             | <span data-ttu-id="36928-359">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-359">yes</span></span>            | <span data-ttu-id="36928-360">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-360">no</span></span>           |
| <span data-ttu-id="36928-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="36928-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="36928-362">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-362">yes</span></span>            | <span data-ttu-id="36928-363">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-363">no</span></span>           |
| <span data-ttu-id="36928-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="36928-364">msdyn_successortask</span></span>           | <span data-ttu-id="36928-365">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-365">yes</span></span>            | <span data-ttu-id="36928-366">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-366">no</span></span>           |
| <span data-ttu-id="36928-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="36928-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="36928-368">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-368">yes</span></span>            | <span data-ttu-id="36928-369">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="36928-370">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="36928-370">Resource assignment</span></span>

| <span data-ttu-id="36928-371">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="36928-371">**Logical name**</span></span>             | <span data-ttu-id="36928-372">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="36928-372">**Can create**</span></span> | <span data-ttu-id="36928-373">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="36928-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="36928-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="36928-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="36928-375">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-375">yes</span></span>            | <span data-ttu-id="36928-376">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-376">no</span></span>           |
| <span data-ttu-id="36928-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="36928-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="36928-378">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-378">yes</span></span>            | <span data-ttu-id="36928-379">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-379">no</span></span>           |
| <span data-ttu-id="36928-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="36928-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="36928-381">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-381">no</span></span>             | <span data-ttu-id="36928-382">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-382">no</span></span>           |
| <span data-ttu-id="36928-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="36928-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="36928-384">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-384">no</span></span>             | <span data-ttu-id="36928-385">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-385">no</span></span>           |
| <span data-ttu-id="36928-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="36928-386">msdyn_committype</span></span>             | <span data-ttu-id="36928-387">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-387">no</span></span>             | <span data-ttu-id="36928-388">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-388">no</span></span>           |
| <span data-ttu-id="36928-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="36928-389">msdyn_committypename</span></span>         | <span data-ttu-id="36928-390">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-390">no</span></span>             | <span data-ttu-id="36928-391">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-391">no</span></span>           |
| <span data-ttu-id="36928-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="36928-392">msdyn_effort</span></span>                 | <span data-ttu-id="36928-393">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-393">no</span></span>             | <span data-ttu-id="36928-394">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-394">no</span></span>           |
| <span data-ttu-id="36928-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="36928-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="36928-396">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-396">no</span></span>             | <span data-ttu-id="36928-397">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-397">no</span></span>           |
| <span data-ttu-id="36928-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="36928-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="36928-399">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-399">no</span></span>             | <span data-ttu-id="36928-400">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-400">no</span></span>           |
| <span data-ttu-id="36928-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="36928-401">msdyn_finish</span></span>                 | <span data-ttu-id="36928-402">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-402">no</span></span>             | <span data-ttu-id="36928-403">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-403">no</span></span>           |
| <span data-ttu-id="36928-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="36928-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="36928-405">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-405">no</span></span>             | <span data-ttu-id="36928-406">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-406">no</span></span>           |
| <span data-ttu-id="36928-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="36928-408">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-408">no</span></span>             | <span data-ttu-id="36928-409">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-409">no</span></span>           |
| <span data-ttu-id="36928-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="36928-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="36928-411">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-411">no</span></span>             | <span data-ttu-id="36928-412">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-412">no</span></span>           |
| <span data-ttu-id="36928-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="36928-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="36928-414">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-414">no</span></span>             | <span data-ttu-id="36928-415">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-415">no</span></span>           |
| <span data-ttu-id="36928-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="36928-417">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-417">no</span></span>             | <span data-ttu-id="36928-418">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-418">no</span></span>           |
| <span data-ttu-id="36928-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="36928-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="36928-420">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-420">no</span></span>             | <span data-ttu-id="36928-421">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-421">no</span></span>           |
| <span data-ttu-id="36928-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="36928-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="36928-423">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-423">no</span></span>             | <span data-ttu-id="36928-424">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-424">no</span></span>           |
| <span data-ttu-id="36928-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="36928-425">msdyn_projectid</span></span>              | <span data-ttu-id="36928-426">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-426">yes</span></span>            | <span data-ttu-id="36928-427">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-427">no</span></span>           |
| <span data-ttu-id="36928-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="36928-428">msdyn_projectidname</span></span>          | <span data-ttu-id="36928-429">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-429">no</span></span>             | <span data-ttu-id="36928-430">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-430">no</span></span>           |
| <span data-ttu-id="36928-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="36928-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="36928-432">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-432">no</span></span>             | <span data-ttu-id="36928-433">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-433">no</span></span>           |
| <span data-ttu-id="36928-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="36928-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="36928-435">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-435">no</span></span>             | <span data-ttu-id="36928-436">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-436">no</span></span>           |
| <span data-ttu-id="36928-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="36928-437">msdyn_start</span></span>                  | <span data-ttu-id="36928-438">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-438">no</span></span>             | <span data-ttu-id="36928-439">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-439">no</span></span>           |
| <span data-ttu-id="36928-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="36928-440">msdyn_taskid</span></span>                 | <span data-ttu-id="36928-441">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-441">no</span></span>             | <span data-ttu-id="36928-442">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-442">no</span></span>           |
| <span data-ttu-id="36928-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="36928-443">msdyn_taskidname</span></span>             | <span data-ttu-id="36928-444">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-444">no</span></span>             | <span data-ttu-id="36928-445">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-445">no</span></span>           |
| <span data-ttu-id="36928-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="36928-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="36928-447">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-447">no</span></span>             | <span data-ttu-id="36928-448">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="36928-449">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="36928-449">Project team member</span></span>

| <span data-ttu-id="36928-450">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="36928-450">**Logical name**</span></span>                                 | <span data-ttu-id="36928-451">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="36928-451">**Can create**</span></span> | <span data-ttu-id="36928-452">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="36928-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="36928-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="36928-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="36928-454">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-454">no</span></span>             | <span data-ttu-id="36928-455">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-455">no</span></span>           |
| <span data-ttu-id="36928-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="36928-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="36928-457">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-457">no</span></span>             | <span data-ttu-id="36928-458">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-458">no</span></span>           |
| <span data-ttu-id="36928-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="36928-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="36928-460">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-460">no</span></span>             | <span data-ttu-id="36928-461">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-461">no</span></span>           |
| <span data-ttu-id="36928-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="36928-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="36928-463">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-463">no</span></span>             | <span data-ttu-id="36928-464">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-464">no</span></span>           |
| <span data-ttu-id="36928-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="36928-465">msdyn_effort</span></span>                                     | <span data-ttu-id="36928-466">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-466">no</span></span>             | <span data-ttu-id="36928-467">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-467">no</span></span>           |
| <span data-ttu-id="36928-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="36928-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="36928-469">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-469">no</span></span>             | <span data-ttu-id="36928-470">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-470">no</span></span>           |
| <span data-ttu-id="36928-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="36928-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="36928-472">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-472">no</span></span>             | <span data-ttu-id="36928-473">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-473">no</span></span>           |
| <span data-ttu-id="36928-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="36928-474">msdyn_finish</span></span>                                     | <span data-ttu-id="36928-475">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-475">no</span></span>             | <span data-ttu-id="36928-476">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-476">no</span></span>           |
| <span data-ttu-id="36928-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="36928-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="36928-478">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-478">no</span></span>             | <span data-ttu-id="36928-479">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-479">no</span></span>           |
| <span data-ttu-id="36928-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="36928-480">msdyn_hours</span></span>                                      | <span data-ttu-id="36928-481">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-481">no</span></span>             | <span data-ttu-id="36928-482">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-482">no</span></span>           |
| <span data-ttu-id="36928-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="36928-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="36928-484">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-484">no</span></span>             | <span data-ttu-id="36928-485">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-485">no</span></span>           |
| <span data-ttu-id="36928-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="36928-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="36928-487">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-487">no</span></span>             | <span data-ttu-id="36928-488">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-488">no</span></span>           |
| <span data-ttu-id="36928-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="36928-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="36928-490">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-490">no</span></span>             | <span data-ttu-id="36928-491">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-491">no</span></span>           |
| <span data-ttu-id="36928-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="36928-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="36928-493">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-493">no</span></span>             | <span data-ttu-id="36928-494">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-494">no</span></span>           |
| <span data-ttu-id="36928-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="36928-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="36928-496">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-496">no</span></span>             | <span data-ttu-id="36928-497">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-497">no</span></span>           |
| <span data-ttu-id="36928-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="36928-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="36928-499">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-499">no</span></span>             | <span data-ttu-id="36928-500">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-500">no</span></span>           |
| <span data-ttu-id="36928-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="36928-501">msdyn_start</span></span>                                      | <span data-ttu-id="36928-502">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-502">no</span></span>             | <span data-ttu-id="36928-503">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="36928-504">Project</span><span class="sxs-lookup"><span data-stu-id="36928-504">Project</span></span>

| <span data-ttu-id="36928-505">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="36928-505">**Logical name**</span></span>                       | <span data-ttu-id="36928-506">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="36928-506">**Can create**</span></span> | <span data-ttu-id="36928-507">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="36928-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="36928-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="36928-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="36928-509">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-509">no</span></span>             | <span data-ttu-id="36928-510">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-510">no</span></span>           |
| <span data-ttu-id="36928-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="36928-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="36928-512">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-512">no</span></span>             | <span data-ttu-id="36928-513">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-513">no</span></span>           |
| <span data-ttu-id="36928-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="36928-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="36928-515">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-515">no</span></span>             | <span data-ttu-id="36928-516">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-516">no</span></span>           |
| <span data-ttu-id="36928-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="36928-518">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-518">no</span></span>             | <span data-ttu-id="36928-519">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-519">no</span></span>           |
| <span data-ttu-id="36928-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="36928-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="36928-521">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-521">no</span></span>             | <span data-ttu-id="36928-522">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-522">no</span></span>           |
| <span data-ttu-id="36928-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="36928-524">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-524">no</span></span>             | <span data-ttu-id="36928-525">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-525">no</span></span>           |
| <span data-ttu-id="36928-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="36928-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="36928-527">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-527">yes</span></span>            | <span data-ttu-id="36928-528">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-528">no</span></span>           |
| <span data-ttu-id="36928-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="36928-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="36928-530">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-530">yes</span></span>            | <span data-ttu-id="36928-531">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-531">no</span></span>           |
| <span data-ttu-id="36928-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="36928-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="36928-533">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-533">yes</span></span>            | <span data-ttu-id="36928-534">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-534">no</span></span>           |
| <span data-ttu-id="36928-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="36928-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="36928-536">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-536">no</span></span>             | <span data-ttu-id="36928-537">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-537">no</span></span>           |
| <span data-ttu-id="36928-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="36928-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="36928-539">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-539">no</span></span>             | <span data-ttu-id="36928-540">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-540">no</span></span>           |
| <span data-ttu-id="36928-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="36928-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="36928-542">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-542">no</span></span>             | <span data-ttu-id="36928-543">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-543">no</span></span>           |
| <span data-ttu-id="36928-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="36928-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="36928-545">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-545">no</span></span>             | <span data-ttu-id="36928-546">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-546">no</span></span>           |
| <span data-ttu-id="36928-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="36928-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="36928-548">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-548">no</span></span>             | <span data-ttu-id="36928-549">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-549">no</span></span>           |
| <span data-ttu-id="36928-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="36928-550">msdyn_duration</span></span>                         | <span data-ttu-id="36928-551">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-551">no</span></span>             | <span data-ttu-id="36928-552">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-552">no</span></span>           |
| <span data-ttu-id="36928-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="36928-553">msdyn_effort</span></span>                           | <span data-ttu-id="36928-554">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-554">no</span></span>             | <span data-ttu-id="36928-555">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-555">no</span></span>           |
| <span data-ttu-id="36928-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="36928-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="36928-557">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-557">no</span></span>             | <span data-ttu-id="36928-558">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-558">no</span></span>           |
| <span data-ttu-id="36928-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="36928-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="36928-560">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-560">no</span></span>             | <span data-ttu-id="36928-561">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-561">no</span></span>           |
| <span data-ttu-id="36928-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="36928-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="36928-563">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-563">no</span></span>             | <span data-ttu-id="36928-564">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-564">no</span></span>           |
| <span data-ttu-id="36928-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="36928-565">msdyn_finish</span></span>                           | <span data-ttu-id="36928-566">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-566">yes</span></span>            | <span data-ttu-id="36928-567">ναι</span><span class="sxs-lookup"><span data-stu-id="36928-567">yes</span></span>          |
| <span data-ttu-id="36928-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="36928-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="36928-569">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-569">no</span></span>             | <span data-ttu-id="36928-570">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-570">no</span></span>           |
| <span data-ttu-id="36928-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="36928-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="36928-572">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-572">no</span></span>             | <span data-ttu-id="36928-573">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-573">no</span></span>           |
| <span data-ttu-id="36928-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="36928-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="36928-575">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-575">no</span></span>             | <span data-ttu-id="36928-576">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-576">no</span></span>           |
| <span data-ttu-id="36928-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="36928-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="36928-578">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-578">no</span></span>             | <span data-ttu-id="36928-579">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-579">no</span></span>           |
| <span data-ttu-id="36928-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="36928-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="36928-581">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-581">no</span></span>             | <span data-ttu-id="36928-582">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-582">no</span></span>           |
| <span data-ttu-id="36928-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="36928-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="36928-584">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-584">no</span></span>             | <span data-ttu-id="36928-585">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-585">no</span></span>           |
| <span data-ttu-id="36928-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="36928-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="36928-587">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-587">no</span></span>             | <span data-ttu-id="36928-588">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-588">no</span></span>           |
| <span data-ttu-id="36928-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="36928-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="36928-590">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-590">no</span></span>             | <span data-ttu-id="36928-591">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-591">no</span></span>           |
| <span data-ttu-id="36928-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="36928-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="36928-593">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-593">no</span></span>             | <span data-ttu-id="36928-594">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-594">no</span></span>           |
| <span data-ttu-id="36928-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="36928-596">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-596">no</span></span>             | <span data-ttu-id="36928-597">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-597">no</span></span>           |
| <span data-ttu-id="36928-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="36928-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="36928-599">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-599">no</span></span>             | <span data-ttu-id="36928-600">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-600">no</span></span>           |
| <span data-ttu-id="36928-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="36928-602">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-602">no</span></span>             | <span data-ttu-id="36928-603">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-603">no</span></span>           |
| <span data-ttu-id="36928-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="36928-604">msdyn_progress</span></span>                         | <span data-ttu-id="36928-605">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-605">no</span></span>             | <span data-ttu-id="36928-606">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-606">no</span></span>           |
| <span data-ttu-id="36928-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="36928-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="36928-608">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-608">no</span></span>             | <span data-ttu-id="36928-609">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-609">no</span></span>           |
| <span data-ttu-id="36928-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="36928-611">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-611">no</span></span>             | <span data-ttu-id="36928-612">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-612">no</span></span>           |
| <span data-ttu-id="36928-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="36928-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="36928-614">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-614">no</span></span>             | <span data-ttu-id="36928-615">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-615">no</span></span>           |
| <span data-ttu-id="36928-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="36928-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="36928-617">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-617">no</span></span>             | <span data-ttu-id="36928-618">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-618">no</span></span>           |
| <span data-ttu-id="36928-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="36928-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="36928-620">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-620">no</span></span>             | <span data-ttu-id="36928-621">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-621">no</span></span>           |
| <span data-ttu-id="36928-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="36928-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="36928-623">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-623">no</span></span>             | <span data-ttu-id="36928-624">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-624">no</span></span>           |
| <span data-ttu-id="36928-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="36928-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="36928-626">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-626">no</span></span>             | <span data-ttu-id="36928-627">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-627">no</span></span>           |
| <span data-ttu-id="36928-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="36928-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="36928-629">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-629">no</span></span>             | <span data-ttu-id="36928-630">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-630">no</span></span>           |
| <span data-ttu-id="36928-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="36928-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="36928-632">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-632">no</span></span>             | <span data-ttu-id="36928-633">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-633">no</span></span>           |
| <span data-ttu-id="36928-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="36928-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="36928-635">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-635">no</span></span>             | <span data-ttu-id="36928-636">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-636">no</span></span>           |
| <span data-ttu-id="36928-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="36928-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="36928-638">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-638">no</span></span>             | <span data-ttu-id="36928-639">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-639">no</span></span>           |
| <span data-ttu-id="36928-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="36928-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="36928-641">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-641">no</span></span>             | <span data-ttu-id="36928-642">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-642">no</span></span>           |
| <span data-ttu-id="36928-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="36928-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="36928-644">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-644">no</span></span>             | <span data-ttu-id="36928-645">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-645">no</span></span>           |
| <span data-ttu-id="36928-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="36928-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="36928-647">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-647">no</span></span>             | <span data-ttu-id="36928-648">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-648">no</span></span>           |
| <span data-ttu-id="36928-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="36928-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="36928-650">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-650">no</span></span>             | <span data-ttu-id="36928-651">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-651">no</span></span>           |
| <span data-ttu-id="36928-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="36928-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="36928-653">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-653">no</span></span>             | <span data-ttu-id="36928-654">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-654">no</span></span>           |
| <span data-ttu-id="36928-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="36928-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="36928-656">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-656">no</span></span>             | <span data-ttu-id="36928-657">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-657">no</span></span>           |
| <span data-ttu-id="36928-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="36928-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="36928-659">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-659">no</span></span>             | <span data-ttu-id="36928-660">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-660">no</span></span>           |
| <span data-ttu-id="36928-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="36928-662">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-662">no</span></span>             | <span data-ttu-id="36928-663">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-663">no</span></span>           |
| <span data-ttu-id="36928-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="36928-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="36928-665">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-665">no</span></span>             | <span data-ttu-id="36928-666">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-666">no</span></span>           |
| <span data-ttu-id="36928-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="36928-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="36928-668">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-668">no</span></span>             | <span data-ttu-id="36928-669">όχι</span><span class="sxs-lookup"><span data-stu-id="36928-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="36928-670">Περιορισμοί και γνωστά προβλήματα</span><span class="sxs-lookup"><span data-stu-id="36928-670">Limitations and known issues</span></span>
<span data-ttu-id="36928-671">Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="36928-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="36928-672">Τα API προγραμματισμού μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με άδεια χρήσης του Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="36928-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="36928-673">Δεν είναι δυνατό να χρησιμοποιηθούν από:</span><span class="sxs-lookup"><span data-stu-id="36928-673">They can't be used by:</span></span>
    - <span data-ttu-id="36928-674">Χρήστες εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="36928-674">Application users</span></span>
    - <span data-ttu-id="36928-675">Χρήστες συστήματος</span><span class="sxs-lookup"><span data-stu-id="36928-675">System users</span></span>
    - <span data-ttu-id="36928-676">Χρήστες ενοποίησης</span><span class="sxs-lookup"><span data-stu-id="36928-676">Integration users</span></span>
    - <span data-ttu-id="36928-677">Άλλοι χρήστες που δεν διαθέτουν την απαιτούμενη άδεια χρήσης</span><span class="sxs-lookup"><span data-stu-id="36928-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="36928-678">Κάθε **OperationSet** μπορεί να έχει μέγιστο αριθμό 100 λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="36928-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="36928-679">Κάθε χρήστης μπορεί να έχει μόνο μέγιστο αριθμό 10 ανοιχτών **OperationSets**.</span><span class="sxs-lookup"><span data-stu-id="36928-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="36928-680">Το Project Operations υποστηρίζει πλέον το πολύ έως 500 συνολικές εργασίες σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="36928-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="36928-681">Η κατάσταση αποτυχίας και τα αρχεία καταγραφής αποτυχίας του **OperationSet** δεν είναι αυτή τη στιγμή διαθέσιμα.</span><span class="sxs-lookup"><span data-stu-id="36928-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="36928-682">Τα API προγραμματισμού είναι σε δημόσια προεπισκόπηση.</span><span class="sxs-lookup"><span data-stu-id="36928-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="36928-683">Η χρήση αυτών των API σε περιβάλλον παραγωγής δεν υποστηρίζεται από τη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="36928-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="36928-684">Όρια και περιορισμοί για έργα και εργασίες</span><span class="sxs-lookup"><span data-stu-id="36928-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="36928-685">Χειρισμός σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="36928-685">Error handling</span></span>

   - <span data-ttu-id="36928-686">Για να εξετάσετε τα σφάλματα που δημιουργούνται από τα σύνολα λειτουργιών, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Σύνολα λειτουργιών**.</span><span class="sxs-lookup"><span data-stu-id="36928-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="36928-687">Για να εξετάσετε τα σφάλματα που δημιουργούνται από την υπηρεσία προγραμματισμού έργου, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Αρχεία σφαλμάτων PSS**.</span><span class="sxs-lookup"><span data-stu-id="36928-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="36928-688">Δείγμα σεναρίου</span><span class="sxs-lookup"><span data-stu-id="36928-688">Sample scenario</span></span>

<span data-ttu-id="36928-689">Σε αυτό το σενάριο, θα δημιουργήσετε ένα έργο, ένα μέλος ομάδας, τέσσερις εργασίες και δύο αναθέσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="36928-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="36928-690">Στη συνέχεια, θα ενημερώσετε μία εργασία, θα ενημερώσετε το έργο, θα διαγράψετε μια εργασία, θα διαγράψετε μία ανάθεση πόρου και θα δημιουργήσετε μια εξάρτηση εργασίας.</span><span class="sxs-lookup"><span data-stu-id="36928-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="36928-691">Πρόσθετα δείγματα</span><span class="sxs-lookup"><span data-stu-id="36928-691">Additional samples</span></span>

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
