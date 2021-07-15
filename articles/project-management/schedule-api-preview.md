---
title: Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτό το θέμα παρέχει πληροφορίες και δείγματα για τη χρήση των API χρονοδιαγράμματος έργου.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293227"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="249f0-103">Χρήση API χρονοδιαγράμματος έργου για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="249f0-103">Use Project schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="249f0-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="249f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="249f0-105">Ορισμένες ή όλες οι λειτουργίες που αναφέρονται σε αυτό το θέμα είναι διαθέσιμες ως μέρος μιας έκδοσης προεπισκόπησης.</span><span class="sxs-lookup"><span data-stu-id="249f0-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="249f0-106">Το περιεχόμενο και η λειτουργικότητα υπόκεινται σε αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="249f0-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="249f0-107">Οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="249f0-107">Scheduling entities</span></span>

<span data-ttu-id="249f0-108">Τα API χρονοδιαγράμματος έργου παρέχουν τη δυνατότητα εκτέλεσης λειτουργιών δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="249f0-108">Project schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="249f0-109">Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web.</span><span class="sxs-lookup"><span data-stu-id="249f0-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="249f0-110">Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="249f0-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="249f0-111">Ο παρακάτω πίνακας παρέχει μια πλήρη λίστα των οντοτήτων χρονοδιαγράμματος έργου.</span><span class="sxs-lookup"><span data-stu-id="249f0-111">The following table provides a full list of the Project schedule entities.</span></span>

| <span data-ttu-id="249f0-112">Όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="249f0-112">Entity name</span></span>  | <span data-ttu-id="249f0-113">Λογικό όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="249f0-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="249f0-114">Project</span><span class="sxs-lookup"><span data-stu-id="249f0-114">Project</span></span> | <span data-ttu-id="249f0-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="249f0-115">msdyn_project</span></span> |
| <span data-ttu-id="249f0-116">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-116">Project Task</span></span>  | <span data-ttu-id="249f0-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="249f0-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="249f0-118">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-118">Project Task Dependency</span></span>  | <span data-ttu-id="249f0-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="249f0-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="249f0-120">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="249f0-120">Resource Assignment</span></span> | <span data-ttu-id="249f0-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="249f0-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="249f0-122">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-122">Project Bucket</span></span>  | <span data-ttu-id="249f0-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="249f0-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="249f0-124">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-124">Project Team Member</span></span> | <span data-ttu-id="249f0-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="249f0-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="249f0-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="249f0-126">OperationSet</span></span>

<span data-ttu-id="249f0-127">Το OperationSet είναι ένα μοτίβο μονάδας εργασίας που μπορεί να χρησιμοποιηθεί όταν διάφορα αιτήματα που επηρεάζουν το χρονοδιάγραμμα πρέπει να υποβληθούν σε επεξεργασία εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="249f0-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="project-schedule-apis"></a><span data-ttu-id="249f0-128">API χρονοδιαγράμματος έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-128">Project schedule APIs</span></span>

<span data-ttu-id="249f0-129">Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος έργου.</span><span class="sxs-lookup"><span data-stu-id="249f0-129">The following is a list of current Project schedule APIs.</span></span>

- <span data-ttu-id="249f0-130">**msdyn_CreateProjectV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="249f0-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="249f0-131">Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="249f0-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="249f0-132">**msdyn_CreateTeamMemberV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός μέλους ομάδας έργου.</span><span class="sxs-lookup"><span data-stu-id="249f0-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="249f0-133">Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="249f0-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="249f0-134">**msdyn_CreateOperationSetV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="249f0-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="249f0-135">**msdyn_PSSCreateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="249f0-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="249f0-136">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία δημιουργίας.</span><span class="sxs-lookup"><span data-stu-id="249f0-136">The entity can be any of the Project scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="249f0-137">**msdyn_PSSUpdateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για την ενημέρωση μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="249f0-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="249f0-138">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία ενημέρωσης.</span><span class="sxs-lookup"><span data-stu-id="249f0-138">The entity can be any of the Project scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="249f0-139">**msdyn_PSSDeleteV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη διαγραφή μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="249f0-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="249f0-140">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού έργου που υποστηρίζουν τη λειτουργία διαγραφής.</span><span class="sxs-lookup"><span data-stu-id="249f0-140">The entity can be any of the Project scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="249f0-141">**msdyn_ExecuteOperationSetV1**: αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="249f0-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-project-schedule-apis-with-operationset"></a><span data-ttu-id="249f0-142">Χρήση API χρονοδιαγράμματος έργου με το OperationSet</span><span class="sxs-lookup"><span data-stu-id="249f0-142">Using Project schedule APIs with OperationSet</span></span>

<span data-ttu-id="249f0-143">Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="249f0-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="249f0-144">Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="249f0-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="249f0-145">Υποστηριζόμενες λειτουργίες</span><span class="sxs-lookup"><span data-stu-id="249f0-145">Supported operations</span></span>

| <span data-ttu-id="249f0-146">Οντότητα προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="249f0-146">Scheduling entity</span></span> | <span data-ttu-id="249f0-147">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="249f0-147">Create</span></span> | <span data-ttu-id="249f0-148">Ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="249f0-148">Update</span></span> | <span data-ttu-id="249f0-149">Delete</span><span class="sxs-lookup"><span data-stu-id="249f0-149">Delete</span></span> | <span data-ttu-id="249f0-150">Σημαντικές επισημάνσεις</span><span class="sxs-lookup"><span data-stu-id="249f0-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="249f0-151">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-151">Project task</span></span> | <span data-ttu-id="249f0-152">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-152">Yes</span></span> | <span data-ttu-id="249f0-153">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-153">Yes</span></span> | <span data-ttu-id="249f0-154">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-154">Yes</span></span> | <span data-ttu-id="249f0-155">Κανένας</span><span class="sxs-lookup"><span data-stu-id="249f0-155">None</span></span> |
| <span data-ttu-id="249f0-156">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-156">Project task dependency</span></span> | <span data-ttu-id="249f0-157">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-157">Yes</span></span> | <span data-ttu-id="249f0-158">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-158">Yes</span></span> | | <span data-ttu-id="249f0-159">Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="249f0-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="249f0-160">Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="249f0-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="249f0-161">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="249f0-161">Resource assignment</span></span> | <span data-ttu-id="249f0-162">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-162">Yes</span></span> | <span data-ttu-id="249f0-163">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-163">Yes</span></span> | | <span data-ttu-id="249f0-164">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="249f0-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="249f0-165">Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="249f0-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="249f0-166">Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="249f0-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="249f0-167">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-167">Project bucket</span></span> | <span data-ttu-id="249f0-168">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="249f0-168">N/A</span></span> | <span data-ttu-id="249f0-169">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="249f0-169">N/A</span></span> | <span data-ttu-id="249f0-170">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="249f0-170">N/A</span></span> | <span data-ttu-id="249f0-171">Ο προεπιλεγμένος κάδος δημιουργείται με χρήση του API **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="249f0-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="249f0-172">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-172">Project team member</span></span> | <span data-ttu-id="249f0-173">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-173">Yes</span></span> | <span data-ttu-id="249f0-174">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-174">Yes</span></span> | <span data-ttu-id="249f0-175">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-175">Yes</span></span> | <span data-ttu-id="249f0-176">Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="249f0-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="249f0-177">Project</span><span class="sxs-lookup"><span data-stu-id="249f0-177">Project</span></span> | <span data-ttu-id="249f0-178">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-178">Yes</span></span> | <span data-ttu-id="249f0-179">Ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-179">Yes</span></span> | <span data-ttu-id="249f0-180">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="249f0-180">N/A</span></span> | <span data-ttu-id="249f0-181">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**.</span><span class="sxs-lookup"><span data-stu-id="249f0-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="249f0-182">Αυτά τα API μπορούν να καλούνται με αντικείμενα οντότητας που περιλαμβάνουν προσαρμοσμένα πεδία.</span><span class="sxs-lookup"><span data-stu-id="249f0-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="249f0-183">Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="249f0-183">The ID property is optional.</span></span> <span data-ttu-id="249f0-184">Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="249f0-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="249f0-185">Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.</span><span class="sxs-lookup"><span data-stu-id="249f0-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="249f0-186">Περιορισμένα πεδία</span><span class="sxs-lookup"><span data-stu-id="249f0-186">Restricted fields</span></span>

<span data-ttu-id="249f0-187">Οι παρακάτω πίνακες ορίζουν τα πεδία που περιορίζονται από τα **Δημιουργία** και **Επεξεργασία.**</span><span class="sxs-lookup"><span data-stu-id="249f0-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="249f0-188">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-188">Project task</span></span>

| <span data-ttu-id="249f0-189">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="249f0-189">**Logical name**</span></span>                       | <span data-ttu-id="249f0-190">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-190">**Can create**</span></span> | <span data-ttu-id="249f0-191">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="249f0-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="249f0-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="249f0-193">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-193">no</span></span>             | <span data-ttu-id="249f0-194">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-194">no</span></span>               |
| <span data-ttu-id="249f0-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="249f0-196">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-196">no</span></span>             | <span data-ttu-id="249f0-197">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-197">no</span></span>               |
| <span data-ttu-id="249f0-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="249f0-198">msdyn_actualend</span></span>                        | <span data-ttu-id="249f0-199">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-199">no</span></span>             | <span data-ttu-id="249f0-200">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-200">no</span></span>               |
| <span data-ttu-id="249f0-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="249f0-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="249f0-202">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-202">no</span></span>             | <span data-ttu-id="249f0-203">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-203">no</span></span>               |
| <span data-ttu-id="249f0-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="249f0-205">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-205">no</span></span>             | <span data-ttu-id="249f0-206">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-206">no</span></span>               |
| <span data-ttu-id="249f0-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="249f0-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="249f0-208">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-208">no</span></span>             | <span data-ttu-id="249f0-209">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-209">no</span></span>               |
| <span data-ttu-id="249f0-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="249f0-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="249f0-211">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-211">no</span></span>             | <span data-ttu-id="249f0-212">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-212">no</span></span>               |
| <span data-ttu-id="249f0-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="249f0-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="249f0-214">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-214">no</span></span>             | <span data-ttu-id="249f0-215">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-215">no</span></span>               |
| <span data-ttu-id="249f0-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="249f0-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="249f0-217">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-217">no</span></span>             | <span data-ttu-id="249f0-218">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-218">no</span></span>               |
| <span data-ttu-id="249f0-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="249f0-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="249f0-220">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-220">no</span></span>             | <span data-ttu-id="249f0-221">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-221">no</span></span>               |
| <span data-ttu-id="249f0-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="249f0-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="249f0-223">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-223">no</span></span>             | <span data-ttu-id="249f0-224">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-224">no</span></span>               |
| <span data-ttu-id="249f0-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="249f0-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="249f0-226">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-226">no</span></span>             | <span data-ttu-id="249f0-227">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-227">no</span></span>               |
| <span data-ttu-id="249f0-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="249f0-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="249f0-229">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-229">no</span></span>             | <span data-ttu-id="249f0-230">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-230">no</span></span>               |
| <span data-ttu-id="249f0-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="249f0-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="249f0-232">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-232">no</span></span>             | <span data-ttu-id="249f0-233">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-233">no</span></span>               |
| <span data-ttu-id="249f0-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="249f0-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="249f0-235">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-235">no</span></span>             | <span data-ttu-id="249f0-236">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-236">no</span></span>               |
| <span data-ttu-id="249f0-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="249f0-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="249f0-238">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-238">no</span></span>             | <span data-ttu-id="249f0-239">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-239">no</span></span>               |
| <span data-ttu-id="249f0-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="249f0-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="249f0-241">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-241">no</span></span>             | <span data-ttu-id="249f0-242">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-242">no</span></span>               |
| <span data-ttu-id="249f0-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="249f0-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="249f0-244">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-244">no</span></span>             | <span data-ttu-id="249f0-245">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-245">no</span></span>               |
| <span data-ttu-id="249f0-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="249f0-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="249f0-247">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-247">no</span></span>             | <span data-ttu-id="249f0-248">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-248">no</span></span>               |
| <span data-ttu-id="249f0-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="249f0-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="249f0-250">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-250">no</span></span>             | <span data-ttu-id="249f0-251">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-251">no</span></span>               |
| <span data-ttu-id="249f0-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="249f0-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="249f0-253">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-253">no</span></span>             | <span data-ttu-id="249f0-254">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-254">no</span></span>               |
| <span data-ttu-id="249f0-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="249f0-256">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-256">no</span></span>             | <span data-ttu-id="249f0-257">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-257">no</span></span>               |
| <span data-ttu-id="249f0-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="249f0-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="249f0-259">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-259">no</span></span>             | <span data-ttu-id="249f0-260">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-260">no</span></span>               |
| <span data-ttu-id="249f0-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="249f0-262">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-262">no</span></span>             | <span data-ttu-id="249f0-263">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-263">no</span></span>               |
| <span data-ttu-id="249f0-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="249f0-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="249f0-265">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-265">no</span></span>             | <span data-ttu-id="249f0-266">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-266">no</span></span>               |
| <span data-ttu-id="249f0-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="249f0-267">msdyn_progress</span></span>                         | <span data-ttu-id="249f0-268">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-268">no</span></span>             | <span data-ttu-id="249f0-269">όχι (ναι για P4W)</span><span class="sxs-lookup"><span data-stu-id="249f0-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="249f0-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="249f0-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="249f0-271">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-271">no</span></span>             | <span data-ttu-id="249f0-272">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-272">no</span></span>               |
| <span data-ttu-id="249f0-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="249f0-274">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-274">no</span></span>             | <span data-ttu-id="249f0-275">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-275">no</span></span>               |
| <span data-ttu-id="249f0-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="249f0-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="249f0-277">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-277">no</span></span>             | <span data-ttu-id="249f0-278">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-278">no</span></span>               |
| <span data-ttu-id="249f0-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="249f0-280">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-280">no</span></span>             | <span data-ttu-id="249f0-281">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-281">no</span></span>               |
| <span data-ttu-id="249f0-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="249f0-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="249f0-283">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-283">no</span></span>             | <span data-ttu-id="249f0-284">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-284">no</span></span>               |
| <span data-ttu-id="249f0-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="249f0-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="249f0-286">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-286">no</span></span>             | <span data-ttu-id="249f0-287">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-287">no</span></span>               |
| <span data-ttu-id="249f0-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="249f0-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="249f0-289">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-289">no</span></span>             | <span data-ttu-id="249f0-290">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-290">no</span></span>               |
| <span data-ttu-id="249f0-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="249f0-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="249f0-292">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-292">no</span></span>             | <span data-ttu-id="249f0-293">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-293">no</span></span>               |
| <span data-ttu-id="249f0-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="249f0-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="249f0-295">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-295">no</span></span>             | <span data-ttu-id="249f0-296">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-296">no</span></span>               |
| <span data-ttu-id="249f0-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="249f0-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="249f0-298">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-298">no</span></span>             | <span data-ttu-id="249f0-299">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-299">no</span></span>               |
| <span data-ttu-id="249f0-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="249f0-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="249f0-301">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-301">no</span></span>             | <span data-ttu-id="249f0-302">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-302">no</span></span>               |
| <span data-ttu-id="249f0-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="249f0-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="249f0-304">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-304">no</span></span>             | <span data-ttu-id="249f0-305">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-305">no</span></span>               |
| <span data-ttu-id="249f0-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="249f0-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="249f0-307">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-307">no</span></span>             | <span data-ttu-id="249f0-308">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-308">no</span></span>               |
| <span data-ttu-id="249f0-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="249f0-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="249f0-310">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-310">no</span></span>             | <span data-ttu-id="249f0-311">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-311">no</span></span>               |
| <span data-ttu-id="249f0-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="249f0-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="249f0-313">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-313">no</span></span>             | <span data-ttu-id="249f0-314">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-314">no</span></span>               |
| <span data-ttu-id="249f0-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="249f0-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="249f0-316">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-316">no</span></span>             | <span data-ttu-id="249f0-317">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-317">no</span></span>               |
| <span data-ttu-id="249f0-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="249f0-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="249f0-319">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-319">no</span></span>             | <span data-ttu-id="249f0-320">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-320">no</span></span>               |
| <span data-ttu-id="249f0-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="249f0-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="249f0-322">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-322">no</span></span>             | <span data-ttu-id="249f0-323">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-323">no</span></span>               |
| <span data-ttu-id="249f0-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="249f0-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="249f0-325">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-325">no</span></span>             | <span data-ttu-id="249f0-326">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-326">no</span></span>               |
| <span data-ttu-id="249f0-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="249f0-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="249f0-328">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-328">no</span></span>             | <span data-ttu-id="249f0-329">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-329">no</span></span>               |
| <span data-ttu-id="249f0-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="249f0-330">msdyn_summary</span></span>                          | <span data-ttu-id="249f0-331">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-331">no</span></span>             | <span data-ttu-id="249f0-332">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-332">no</span></span>               |
| <span data-ttu-id="249f0-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="249f0-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="249f0-334">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-334">no</span></span>             | <span data-ttu-id="249f0-335">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-335">no</span></span>               |
| <span data-ttu-id="249f0-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="249f0-337">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-337">no</span></span>             | <span data-ttu-id="249f0-338">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="249f0-339">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-339">Project task dependency</span></span>

| <span data-ttu-id="249f0-340">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="249f0-340">**Logical name**</span></span>              | <span data-ttu-id="249f0-341">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-341">**Can create**</span></span> | <span data-ttu-id="249f0-342">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="249f0-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="249f0-343">msdyn_linktype</span></span>                | <span data-ttu-id="249f0-344">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-344">no</span></span>             | <span data-ttu-id="249f0-345">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-345">no</span></span>           |
| <span data-ttu-id="249f0-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="249f0-346">msdyn_linktypename</span></span>            | <span data-ttu-id="249f0-347">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-347">no</span></span>             | <span data-ttu-id="249f0-348">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-348">no</span></span>           |
| <span data-ttu-id="249f0-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="249f0-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="249f0-350">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-350">yes</span></span>            | <span data-ttu-id="249f0-351">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-351">no</span></span>           |
| <span data-ttu-id="249f0-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="249f0-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="249f0-353">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-353">yes</span></span>            | <span data-ttu-id="249f0-354">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-354">no</span></span>           |
| <span data-ttu-id="249f0-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="249f0-355">msdyn_project</span></span>                 | <span data-ttu-id="249f0-356">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-356">yes</span></span>            | <span data-ttu-id="249f0-357">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-357">no</span></span>           |
| <span data-ttu-id="249f0-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="249f0-358">msdyn_projectname</span></span>             | <span data-ttu-id="249f0-359">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-359">yes</span></span>            | <span data-ttu-id="249f0-360">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-360">no</span></span>           |
| <span data-ttu-id="249f0-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="249f0-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="249f0-362">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-362">yes</span></span>            | <span data-ttu-id="249f0-363">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-363">no</span></span>           |
| <span data-ttu-id="249f0-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="249f0-364">msdyn_successortask</span></span>           | <span data-ttu-id="249f0-365">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-365">yes</span></span>            | <span data-ttu-id="249f0-366">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-366">no</span></span>           |
| <span data-ttu-id="249f0-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="249f0-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="249f0-368">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-368">yes</span></span>            | <span data-ttu-id="249f0-369">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="249f0-370">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="249f0-370">Resource assignment</span></span>

| <span data-ttu-id="249f0-371">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="249f0-371">**Logical name**</span></span>             | <span data-ttu-id="249f0-372">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-372">**Can create**</span></span> | <span data-ttu-id="249f0-373">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="249f0-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="249f0-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="249f0-375">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-375">yes</span></span>            | <span data-ttu-id="249f0-376">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-376">no</span></span>           |
| <span data-ttu-id="249f0-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="249f0-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="249f0-378">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-378">yes</span></span>            | <span data-ttu-id="249f0-379">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-379">no</span></span>           |
| <span data-ttu-id="249f0-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="249f0-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="249f0-381">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-381">no</span></span>             | <span data-ttu-id="249f0-382">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-382">no</span></span>           |
| <span data-ttu-id="249f0-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="249f0-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="249f0-384">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-384">no</span></span>             | <span data-ttu-id="249f0-385">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-385">no</span></span>           |
| <span data-ttu-id="249f0-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="249f0-386">msdyn_committype</span></span>             | <span data-ttu-id="249f0-387">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-387">no</span></span>             | <span data-ttu-id="249f0-388">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-388">no</span></span>           |
| <span data-ttu-id="249f0-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="249f0-389">msdyn_committypename</span></span>         | <span data-ttu-id="249f0-390">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-390">no</span></span>             | <span data-ttu-id="249f0-391">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-391">no</span></span>           |
| <span data-ttu-id="249f0-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="249f0-392">msdyn_effort</span></span>                 | <span data-ttu-id="249f0-393">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-393">no</span></span>             | <span data-ttu-id="249f0-394">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-394">no</span></span>           |
| <span data-ttu-id="249f0-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="249f0-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="249f0-396">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-396">no</span></span>             | <span data-ttu-id="249f0-397">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-397">no</span></span>           |
| <span data-ttu-id="249f0-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="249f0-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="249f0-399">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-399">no</span></span>             | <span data-ttu-id="249f0-400">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-400">no</span></span>           |
| <span data-ttu-id="249f0-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="249f0-401">msdyn_finish</span></span>                 | <span data-ttu-id="249f0-402">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-402">no</span></span>             | <span data-ttu-id="249f0-403">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-403">no</span></span>           |
| <span data-ttu-id="249f0-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="249f0-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="249f0-405">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-405">no</span></span>             | <span data-ttu-id="249f0-406">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-406">no</span></span>           |
| <span data-ttu-id="249f0-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="249f0-408">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-408">no</span></span>             | <span data-ttu-id="249f0-409">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-409">no</span></span>           |
| <span data-ttu-id="249f0-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="249f0-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="249f0-411">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-411">no</span></span>             | <span data-ttu-id="249f0-412">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-412">no</span></span>           |
| <span data-ttu-id="249f0-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="249f0-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="249f0-414">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-414">no</span></span>             | <span data-ttu-id="249f0-415">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-415">no</span></span>           |
| <span data-ttu-id="249f0-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="249f0-417">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-417">no</span></span>             | <span data-ttu-id="249f0-418">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-418">no</span></span>           |
| <span data-ttu-id="249f0-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="249f0-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="249f0-420">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-420">no</span></span>             | <span data-ttu-id="249f0-421">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-421">no</span></span>           |
| <span data-ttu-id="249f0-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="249f0-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="249f0-423">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-423">no</span></span>             | <span data-ttu-id="249f0-424">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-424">no</span></span>           |
| <span data-ttu-id="249f0-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="249f0-425">msdyn_projectid</span></span>              | <span data-ttu-id="249f0-426">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-426">yes</span></span>            | <span data-ttu-id="249f0-427">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-427">no</span></span>           |
| <span data-ttu-id="249f0-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="249f0-428">msdyn_projectidname</span></span>          | <span data-ttu-id="249f0-429">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-429">no</span></span>             | <span data-ttu-id="249f0-430">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-430">no</span></span>           |
| <span data-ttu-id="249f0-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="249f0-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="249f0-432">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-432">no</span></span>             | <span data-ttu-id="249f0-433">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-433">no</span></span>           |
| <span data-ttu-id="249f0-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="249f0-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="249f0-435">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-435">no</span></span>             | <span data-ttu-id="249f0-436">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-436">no</span></span>           |
| <span data-ttu-id="249f0-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="249f0-437">msdyn_start</span></span>                  | <span data-ttu-id="249f0-438">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-438">no</span></span>             | <span data-ttu-id="249f0-439">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-439">no</span></span>           |
| <span data-ttu-id="249f0-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="249f0-440">msdyn_taskid</span></span>                 | <span data-ttu-id="249f0-441">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-441">no</span></span>             | <span data-ttu-id="249f0-442">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-442">no</span></span>           |
| <span data-ttu-id="249f0-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="249f0-443">msdyn_taskidname</span></span>             | <span data-ttu-id="249f0-444">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-444">no</span></span>             | <span data-ttu-id="249f0-445">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-445">no</span></span>           |
| <span data-ttu-id="249f0-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="249f0-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="249f0-447">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-447">no</span></span>             | <span data-ttu-id="249f0-448">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="249f0-449">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="249f0-449">Project team member</span></span>

| <span data-ttu-id="249f0-450">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="249f0-450">**Logical name**</span></span>                                 | <span data-ttu-id="249f0-451">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-451">**Can create**</span></span> | <span data-ttu-id="249f0-452">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="249f0-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="249f0-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="249f0-454">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-454">no</span></span>             | <span data-ttu-id="249f0-455">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-455">no</span></span>           |
| <span data-ttu-id="249f0-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="249f0-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="249f0-457">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-457">no</span></span>             | <span data-ttu-id="249f0-458">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-458">no</span></span>           |
| <span data-ttu-id="249f0-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="249f0-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="249f0-460">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-460">no</span></span>             | <span data-ttu-id="249f0-461">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-461">no</span></span>           |
| <span data-ttu-id="249f0-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="249f0-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="249f0-463">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-463">no</span></span>             | <span data-ttu-id="249f0-464">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-464">no</span></span>           |
| <span data-ttu-id="249f0-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="249f0-465">msdyn_effort</span></span>                                     | <span data-ttu-id="249f0-466">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-466">no</span></span>             | <span data-ttu-id="249f0-467">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-467">no</span></span>           |
| <span data-ttu-id="249f0-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="249f0-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="249f0-469">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-469">no</span></span>             | <span data-ttu-id="249f0-470">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-470">no</span></span>           |
| <span data-ttu-id="249f0-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="249f0-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="249f0-472">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-472">no</span></span>             | <span data-ttu-id="249f0-473">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-473">no</span></span>           |
| <span data-ttu-id="249f0-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="249f0-474">msdyn_finish</span></span>                                     | <span data-ttu-id="249f0-475">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-475">no</span></span>             | <span data-ttu-id="249f0-476">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-476">no</span></span>           |
| <span data-ttu-id="249f0-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="249f0-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="249f0-478">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-478">no</span></span>             | <span data-ttu-id="249f0-479">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-479">no</span></span>           |
| <span data-ttu-id="249f0-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="249f0-480">msdyn_hours</span></span>                                      | <span data-ttu-id="249f0-481">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-481">no</span></span>             | <span data-ttu-id="249f0-482">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-482">no</span></span>           |
| <span data-ttu-id="249f0-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="249f0-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="249f0-484">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-484">no</span></span>             | <span data-ttu-id="249f0-485">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-485">no</span></span>           |
| <span data-ttu-id="249f0-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="249f0-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="249f0-487">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-487">no</span></span>             | <span data-ttu-id="249f0-488">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-488">no</span></span>           |
| <span data-ttu-id="249f0-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="249f0-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="249f0-490">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-490">no</span></span>             | <span data-ttu-id="249f0-491">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-491">no</span></span>           |
| <span data-ttu-id="249f0-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="249f0-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="249f0-493">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-493">no</span></span>             | <span data-ttu-id="249f0-494">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-494">no</span></span>           |
| <span data-ttu-id="249f0-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="249f0-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="249f0-496">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-496">no</span></span>             | <span data-ttu-id="249f0-497">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-497">no</span></span>           |
| <span data-ttu-id="249f0-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="249f0-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="249f0-499">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-499">no</span></span>             | <span data-ttu-id="249f0-500">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-500">no</span></span>           |
| <span data-ttu-id="249f0-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="249f0-501">msdyn_start</span></span>                                      | <span data-ttu-id="249f0-502">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-502">no</span></span>             | <span data-ttu-id="249f0-503">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="249f0-504">Project</span><span class="sxs-lookup"><span data-stu-id="249f0-504">Project</span></span>

| <span data-ttu-id="249f0-505">**Λογικό όνομα**</span><span class="sxs-lookup"><span data-stu-id="249f0-505">**Logical name**</span></span>                       | <span data-ttu-id="249f0-506">**Δυνατότητα δημιουργίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-506">**Can create**</span></span> | <span data-ttu-id="249f0-507">**Δυνατότητα επεξεργασίας**</span><span class="sxs-lookup"><span data-stu-id="249f0-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="249f0-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="249f0-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="249f0-509">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-509">no</span></span>             | <span data-ttu-id="249f0-510">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-510">no</span></span>           |
| <span data-ttu-id="249f0-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="249f0-512">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-512">no</span></span>             | <span data-ttu-id="249f0-513">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-513">no</span></span>           |
| <span data-ttu-id="249f0-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="249f0-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="249f0-515">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-515">no</span></span>             | <span data-ttu-id="249f0-516">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-516">no</span></span>           |
| <span data-ttu-id="249f0-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="249f0-518">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-518">no</span></span>             | <span data-ttu-id="249f0-519">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-519">no</span></span>           |
| <span data-ttu-id="249f0-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="249f0-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="249f0-521">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-521">no</span></span>             | <span data-ttu-id="249f0-522">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-522">no</span></span>           |
| <span data-ttu-id="249f0-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="249f0-524">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-524">no</span></span>             | <span data-ttu-id="249f0-525">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-525">no</span></span>           |
| <span data-ttu-id="249f0-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="249f0-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="249f0-527">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-527">yes</span></span>            | <span data-ttu-id="249f0-528">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-528">no</span></span>           |
| <span data-ttu-id="249f0-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="249f0-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="249f0-530">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-530">yes</span></span>            | <span data-ttu-id="249f0-531">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-531">no</span></span>           |
| <span data-ttu-id="249f0-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="249f0-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="249f0-533">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-533">yes</span></span>            | <span data-ttu-id="249f0-534">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-534">no</span></span>           |
| <span data-ttu-id="249f0-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="249f0-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="249f0-536">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-536">no</span></span>             | <span data-ttu-id="249f0-537">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-537">no</span></span>           |
| <span data-ttu-id="249f0-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="249f0-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="249f0-539">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-539">no</span></span>             | <span data-ttu-id="249f0-540">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-540">no</span></span>           |
| <span data-ttu-id="249f0-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="249f0-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="249f0-542">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-542">no</span></span>             | <span data-ttu-id="249f0-543">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-543">no</span></span>           |
| <span data-ttu-id="249f0-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="249f0-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="249f0-545">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-545">no</span></span>             | <span data-ttu-id="249f0-546">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-546">no</span></span>           |
| <span data-ttu-id="249f0-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="249f0-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="249f0-548">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-548">no</span></span>             | <span data-ttu-id="249f0-549">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-549">no</span></span>           |
| <span data-ttu-id="249f0-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="249f0-550">msdyn_duration</span></span>                         | <span data-ttu-id="249f0-551">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-551">no</span></span>             | <span data-ttu-id="249f0-552">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-552">no</span></span>           |
| <span data-ttu-id="249f0-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="249f0-553">msdyn_effort</span></span>                           | <span data-ttu-id="249f0-554">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-554">no</span></span>             | <span data-ttu-id="249f0-555">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-555">no</span></span>           |
| <span data-ttu-id="249f0-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="249f0-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="249f0-557">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-557">no</span></span>             | <span data-ttu-id="249f0-558">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-558">no</span></span>           |
| <span data-ttu-id="249f0-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="249f0-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="249f0-560">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-560">no</span></span>             | <span data-ttu-id="249f0-561">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-561">no</span></span>           |
| <span data-ttu-id="249f0-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="249f0-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="249f0-563">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-563">no</span></span>             | <span data-ttu-id="249f0-564">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-564">no</span></span>           |
| <span data-ttu-id="249f0-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="249f0-565">msdyn_finish</span></span>                           | <span data-ttu-id="249f0-566">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-566">yes</span></span>            | <span data-ttu-id="249f0-567">ναι</span><span class="sxs-lookup"><span data-stu-id="249f0-567">yes</span></span>          |
| <span data-ttu-id="249f0-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="249f0-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="249f0-569">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-569">no</span></span>             | <span data-ttu-id="249f0-570">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-570">no</span></span>           |
| <span data-ttu-id="249f0-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="249f0-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="249f0-572">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-572">no</span></span>             | <span data-ttu-id="249f0-573">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-573">no</span></span>           |
| <span data-ttu-id="249f0-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="249f0-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="249f0-575">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-575">no</span></span>             | <span data-ttu-id="249f0-576">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-576">no</span></span>           |
| <span data-ttu-id="249f0-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="249f0-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="249f0-578">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-578">no</span></span>             | <span data-ttu-id="249f0-579">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-579">no</span></span>           |
| <span data-ttu-id="249f0-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="249f0-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="249f0-581">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-581">no</span></span>             | <span data-ttu-id="249f0-582">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-582">no</span></span>           |
| <span data-ttu-id="249f0-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="249f0-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="249f0-584">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-584">no</span></span>             | <span data-ttu-id="249f0-585">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-585">no</span></span>           |
| <span data-ttu-id="249f0-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="249f0-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="249f0-587">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-587">no</span></span>             | <span data-ttu-id="249f0-588">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-588">no</span></span>           |
| <span data-ttu-id="249f0-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="249f0-590">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-590">no</span></span>             | <span data-ttu-id="249f0-591">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-591">no</span></span>           |
| <span data-ttu-id="249f0-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="249f0-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="249f0-593">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-593">no</span></span>             | <span data-ttu-id="249f0-594">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-594">no</span></span>           |
| <span data-ttu-id="249f0-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="249f0-596">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-596">no</span></span>             | <span data-ttu-id="249f0-597">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-597">no</span></span>           |
| <span data-ttu-id="249f0-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="249f0-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="249f0-599">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-599">no</span></span>             | <span data-ttu-id="249f0-600">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-600">no</span></span>           |
| <span data-ttu-id="249f0-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="249f0-602">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-602">no</span></span>             | <span data-ttu-id="249f0-603">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-603">no</span></span>           |
| <span data-ttu-id="249f0-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="249f0-604">msdyn_progress</span></span>                         | <span data-ttu-id="249f0-605">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-605">no</span></span>             | <span data-ttu-id="249f0-606">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-606">no</span></span>           |
| <span data-ttu-id="249f0-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="249f0-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="249f0-608">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-608">no</span></span>             | <span data-ttu-id="249f0-609">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-609">no</span></span>           |
| <span data-ttu-id="249f0-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="249f0-611">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-611">no</span></span>             | <span data-ttu-id="249f0-612">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-612">no</span></span>           |
| <span data-ttu-id="249f0-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="249f0-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="249f0-614">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-614">no</span></span>             | <span data-ttu-id="249f0-615">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-615">no</span></span>           |
| <span data-ttu-id="249f0-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="249f0-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="249f0-617">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-617">no</span></span>             | <span data-ttu-id="249f0-618">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-618">no</span></span>           |
| <span data-ttu-id="249f0-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="249f0-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="249f0-620">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-620">no</span></span>             | <span data-ttu-id="249f0-621">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-621">no</span></span>           |
| <span data-ttu-id="249f0-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="249f0-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="249f0-623">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-623">no</span></span>             | <span data-ttu-id="249f0-624">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-624">no</span></span>           |
| <span data-ttu-id="249f0-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="249f0-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="249f0-626">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-626">no</span></span>             | <span data-ttu-id="249f0-627">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-627">no</span></span>           |
| <span data-ttu-id="249f0-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="249f0-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="249f0-629">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-629">no</span></span>             | <span data-ttu-id="249f0-630">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-630">no</span></span>           |
| <span data-ttu-id="249f0-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="249f0-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="249f0-632">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-632">no</span></span>             | <span data-ttu-id="249f0-633">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-633">no</span></span>           |
| <span data-ttu-id="249f0-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="249f0-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="249f0-635">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-635">no</span></span>             | <span data-ttu-id="249f0-636">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-636">no</span></span>           |
| <span data-ttu-id="249f0-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="249f0-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="249f0-638">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-638">no</span></span>             | <span data-ttu-id="249f0-639">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-639">no</span></span>           |
| <span data-ttu-id="249f0-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="249f0-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="249f0-641">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-641">no</span></span>             | <span data-ttu-id="249f0-642">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-642">no</span></span>           |
| <span data-ttu-id="249f0-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="249f0-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="249f0-644">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-644">no</span></span>             | <span data-ttu-id="249f0-645">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-645">no</span></span>           |
| <span data-ttu-id="249f0-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="249f0-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="249f0-647">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-647">no</span></span>             | <span data-ttu-id="249f0-648">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-648">no</span></span>           |
| <span data-ttu-id="249f0-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="249f0-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="249f0-650">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-650">no</span></span>             | <span data-ttu-id="249f0-651">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-651">no</span></span>           |
| <span data-ttu-id="249f0-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="249f0-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="249f0-653">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-653">no</span></span>             | <span data-ttu-id="249f0-654">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-654">no</span></span>           |
| <span data-ttu-id="249f0-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="249f0-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="249f0-656">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-656">no</span></span>             | <span data-ttu-id="249f0-657">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-657">no</span></span>           |
| <span data-ttu-id="249f0-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="249f0-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="249f0-659">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-659">no</span></span>             | <span data-ttu-id="249f0-660">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-660">no</span></span>           |
| <span data-ttu-id="249f0-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="249f0-662">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-662">no</span></span>             | <span data-ttu-id="249f0-663">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-663">no</span></span>           |
| <span data-ttu-id="249f0-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="249f0-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="249f0-665">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-665">no</span></span>             | <span data-ttu-id="249f0-666">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-666">no</span></span>           |
| <span data-ttu-id="249f0-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="249f0-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="249f0-668">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-668">no</span></span>             | <span data-ttu-id="249f0-669">όχι</span><span class="sxs-lookup"><span data-stu-id="249f0-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="249f0-670">Περιορισμοί και γνωστά προβλήματα</span><span class="sxs-lookup"><span data-stu-id="249f0-670">Limitations and known issues</span></span>
<span data-ttu-id="249f0-671">Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="249f0-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="249f0-672">Τα API χρονοδιαγράμματος έργου μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με Άδεια χρήσης του Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="249f0-672">Project Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="249f0-673">Δεν είναι δυνατό να χρησιμοποιηθούν από:</span><span class="sxs-lookup"><span data-stu-id="249f0-673">They can't be used by:</span></span>
    - <span data-ttu-id="249f0-674">Χρήστες εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="249f0-674">Application users</span></span>
    - <span data-ttu-id="249f0-675">Χρήστες συστήματος</span><span class="sxs-lookup"><span data-stu-id="249f0-675">System users</span></span>
    - <span data-ttu-id="249f0-676">Χρήστες ενοποίησης</span><span class="sxs-lookup"><span data-stu-id="249f0-676">Integration users</span></span>
    - <span data-ttu-id="249f0-677">Άλλοι χρήστες που δεν διαθέτουν την απαιτούμενη άδεια χρήσης</span><span class="sxs-lookup"><span data-stu-id="249f0-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="249f0-678">Κάθε **OperationSet** μπορεί να έχει μέγιστο αριθμό 100 λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="249f0-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="249f0-679">Κάθε χρήστης μπορεί να έχει μόνο μέγιστο αριθμό 10 ανοιχτών **OperationSets**.</span><span class="sxs-lookup"><span data-stu-id="249f0-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="249f0-680">Το Project Operations υποστηρίζει πλέον το πολύ έως 500 συνολικές εργασίες σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="249f0-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="249f0-681">Η κατάσταση αποτυχίας και τα αρχεία καταγραφής αποτυχίας του **OperationSet** δεν είναι αυτή τη στιγμή διαθέσιμα.</span><span class="sxs-lookup"><span data-stu-id="249f0-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="249f0-682">Όρια και περιορισμοί για έργα και εργασίες</span><span class="sxs-lookup"><span data-stu-id="249f0-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="249f0-683">Χειρισμός σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="249f0-683">Error handling</span></span>

   - <span data-ttu-id="249f0-684">Για να εξετάσετε τα σφάλματα που δημιουργούνται από τα σύνολα λειτουργιών, μεταβείτε στην επιλογή **Ρυθμίσεις** \> **Προγραμματισμός ενοποίησης** \> **Σύνολα λειτουργιών**.</span><span class="sxs-lookup"><span data-stu-id="249f0-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="249f0-685">Για να εξετάσετε τα σφάλματα που δημιουργούνται από την υπηρεσία χρονοδιαγράμματος έργου, μεταβείτε στις **Ρυθμίσεις** \> **Ενοποίηση προγραμματισμού** \> **Αρχεία καταγραφής σφαλμάτων PSS**.</span><span class="sxs-lookup"><span data-stu-id="249f0-685">To review errors generated from the Project schedule Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="249f0-686">Δείγμα σεναρίου</span><span class="sxs-lookup"><span data-stu-id="249f0-686">Sample scenario</span></span>

<span data-ttu-id="249f0-687">Σε αυτό το σενάριο, θα δημιουργήσετε ένα έργο, ένα μέλος ομάδας, τέσσερις εργασίες και δύο αναθέσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="249f0-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="249f0-688">Στη συνέχεια, θα ενημερώσετε μία εργασία, θα ενημερώσετε το έργο, θα διαγράψετε μια εργασία, θα διαγράψετε μία ανάθεση πόρου και θα δημιουργήσετε μια εξάρτηση εργασίας.</span><span class="sxs-lookup"><span data-stu-id="249f0-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="249f0-689">Πρόσθετα δείγματα</span><span class="sxs-lookup"><span data-stu-id="249f0-689">Additional samples</span></span>

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
