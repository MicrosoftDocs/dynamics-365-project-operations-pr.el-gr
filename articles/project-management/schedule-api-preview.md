---
title: Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού
description: Αυτή θέμα παρέχει πληροφορίες και δείγματα για τη χρήση API χρονοδιαγράμματος.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868129"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="d4182-103">Χρήση API χρονοδιαγράμματος για την εκτέλεση λειτουργιών με οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="d4182-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="d4182-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="d4182-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="d4182-105">Ορισμένες ή όλες οι λειτουργίες που αναφέρονται σε αυτό το θέμα είναι διαθέσιμες ως μέρος μιας έκδοσης προεπισκόπησης.</span><span class="sxs-lookup"><span data-stu-id="d4182-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="d4182-106">Το περιεχόμενο και η λειτουργικότητα υπόκεινται σε αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="d4182-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="d4182-107">Οντότητες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="d4182-107">Scheduling entities</span></span>

<span data-ttu-id="d4182-108">Τα API χρονοδιαγράμματος παρέχουν τη δυνατότητα εκτέλεσης δημιουργίας, ενημέρωσης και διαγραφής λειτουργιών με **Οντότητες προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="d4182-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="d4182-109">Η διαχείριση αυτών των οντοτήτων γίνεται μέσω της μηχανής προγραμματισμού στο Έργο για το web.</span><span class="sxs-lookup"><span data-stu-id="d4182-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="d4182-110">Οι λειτουργίες δημιουργίας, ενημέρωσης και διαγραφής με **Οντότητες προγραμματισμού** περιορίστηκαν σε προηγούμενες εκδόσεις του Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="d4182-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="d4182-111">Ο παρακάτω πίνακας περιλαμβάνει μια πλήρη λίστα των **Οντοτήτων προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="d4182-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="d4182-112">Όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="d4182-112">Entity name</span></span>  | <span data-ttu-id="d4182-113">Λογικό όνομα οντότητας</span><span class="sxs-lookup"><span data-stu-id="d4182-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="d4182-114">Project</span><span class="sxs-lookup"><span data-stu-id="d4182-114">Project</span></span> | <span data-ttu-id="d4182-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="d4182-115">msdyn_project</span></span> |
| <span data-ttu-id="d4182-116">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-116">Project Task</span></span>  | <span data-ttu-id="d4182-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="d4182-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="d4182-118">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-118">Project Task Dependency</span></span>  | <span data-ttu-id="d4182-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="d4182-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="d4182-120">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="d4182-120">Resource Assignment</span></span> | <span data-ttu-id="d4182-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="d4182-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="d4182-122">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-122">Project Bucket</span></span>  | <span data-ttu-id="d4182-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="d4182-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="d4182-124">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-124">Project Team Member</span></span> | <span data-ttu-id="d4182-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="d4182-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="d4182-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="d4182-126">OperationSet</span></span>

<span data-ttu-id="d4182-127">Το OperationSet είναι ένα μοτίβο μονάδας εργασίας που μπορεί να χρησιμοποιηθεί όταν διάφορα αιτήματα που επηρεάζουν το χρονοδιάγραμμα πρέπει να υποβληθούν σε επεξεργασία εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d4182-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="d4182-128">Προγραμματισμός API</span><span class="sxs-lookup"><span data-stu-id="d4182-128">Schedule APIs</span></span>

<span data-ttu-id="d4182-129">Ακολουθεί μια λίστα με τα τρέχοντα API χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="d4182-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="d4182-130">**msdyn_CreateProjectV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="d4182-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="d4182-131">Το έργο και ο προεπιλεγμένος κάδος έργου δημιουργούνται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="d4182-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="d4182-132">**msdyn_CreateTeamMemberV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός μέλους ομάδας έργου.</span><span class="sxs-lookup"><span data-stu-id="d4182-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="d4182-133">Η καρτέλα μέλους ομάδας δημιουργείται αμέσως.</span><span class="sxs-lookup"><span data-stu-id="d4182-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="d4182-134">**msdyn_CreateOperationSetV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τον προγραμματισμό διαφόρων αιτήσεων που πρέπει να εκτελεστούν εντός μιας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d4182-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="d4182-135">**msdyn_PSSCreateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη δημιουργία μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="d4182-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="d4182-136">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία δημιουργίας.</span><span class="sxs-lookup"><span data-stu-id="d4182-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="d4182-137">**msdyn_PSSUpdateV1**: αυτό το API μπορεί να χρησιμοποιηθεί για την ενημέρωση μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="d4182-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="d4182-138">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία ενημέρωσης.</span><span class="sxs-lookup"><span data-stu-id="d4182-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="d4182-139">**msdyn_PSSDeleteV1**: αυτό το API μπορεί να χρησιμοποιηθεί για τη διαγραφή μιας οντότητας.</span><span class="sxs-lookup"><span data-stu-id="d4182-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="d4182-140">Η οντότητα μπορεί να είναι οποιαδήποτε από τις οντότητες προγραμματισμού που υποστηρίζουν τη λειτουργία διαγραφής.</span><span class="sxs-lookup"><span data-stu-id="d4182-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="d4182-141">**msdyn_ExecuteOperationSetV1**: αυτό το API χρησιμοποιείται για την εκτέλεση όλων των λειτουργιών εντός του δεδομένου συνόλου λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="d4182-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="d4182-142">Χρήση API χρονοδιαγράμματος με το OperationSet</span><span class="sxs-lookup"><span data-stu-id="d4182-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="d4182-143">Επειδή οι καρτέλες και με το **CreateProjectV1** και το **CreateTeamMemberV1** δημιουργούνται αμέσως, αυτά τα API δεν μπορούν να χρησιμοποιηθούν απευθείας στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="d4182-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="d4182-144">Ωστόσο, μπορείτε να χρησιμοποιήσετε το API για να δημιουργήσετε απαραίτητες καρτέλες, να δημιουργήσετε ένα **OperationSet** και, στη συνέχεια, να χρησιμοποιήσετε αυτές τις προ-δημιουργημένες καρτέλες στο **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="d4182-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="d4182-145">Υποστηριζόμενες λειτουργίες</span><span class="sxs-lookup"><span data-stu-id="d4182-145">Supported operations</span></span>

| <span data-ttu-id="d4182-146">Οντότητα προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="d4182-146">Scheduling entity</span></span> | <span data-ttu-id="d4182-147">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="d4182-147">Create</span></span> | <span data-ttu-id="d4182-148">Ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="d4182-148">Update</span></span> | <span data-ttu-id="d4182-149">Delete</span><span class="sxs-lookup"><span data-stu-id="d4182-149">Delete</span></span> | <span data-ttu-id="d4182-150">Σημαντικές επισημάνσεις</span><span class="sxs-lookup"><span data-stu-id="d4182-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="d4182-151">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-151">Project task</span></span> | <span data-ttu-id="d4182-152">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-152">Yes</span></span> | <span data-ttu-id="d4182-153">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-153">Yes</span></span> | <span data-ttu-id="d4182-154">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-154">Yes</span></span> | <span data-ttu-id="d4182-155">Κανένας</span><span class="sxs-lookup"><span data-stu-id="d4182-155">None</span></span> |
| <span data-ttu-id="d4182-156">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-156">Project task dependency</span></span> | <span data-ttu-id="d4182-157">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-157">Yes</span></span> | <span data-ttu-id="d4182-158">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-158">Yes</span></span> | | <span data-ttu-id="d4182-159">Οι καρτέλες εξάρτησης εργασιών έργου δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="d4182-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="d4182-160">Αντίθετα, είναι δυνατό να διαγραφεί μια παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="d4182-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="d4182-161">Ανάθεση πόρου</span><span class="sxs-lookup"><span data-stu-id="d4182-161">Resource assignment</span></span> | <span data-ttu-id="d4182-162">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-162">Yes</span></span> | <span data-ttu-id="d4182-163">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-163">Yes</span></span> | | <span data-ttu-id="d4182-164">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** και **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="d4182-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="d4182-165">Οι καρτέλες ανάθεσης πόρων δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="d4182-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="d4182-166">Αντίθετα, είναι δυνατό να διαγραφεί η παλιά καρτέλα και να δημιουργηθεί μια νέα καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="d4182-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="d4182-167">Κάδος έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-167">Project bucket</span></span> | <span data-ttu-id="d4182-168">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="d4182-168">N/A</span></span> | <span data-ttu-id="d4182-169">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="d4182-169">N/A</span></span> | <span data-ttu-id="d4182-170">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="d4182-170">N/A</span></span> | <span data-ttu-id="d4182-171">Ο προεπιλεγμένος κάδος δημιουργείται με χρήση του API **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="d4182-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="d4182-172">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="d4182-172">Project team member</span></span> | <span data-ttu-id="d4182-173">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-173">Yes</span></span> | <span data-ttu-id="d4182-174">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-174">Yes</span></span> | <span data-ttu-id="d4182-175">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-175">Yes</span></span> | <span data-ttu-id="d4182-176">Για τη λειτουργία δημιουργίας, χρησιμοποιήστε το API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="d4182-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="d4182-177">Project</span><span class="sxs-lookup"><span data-stu-id="d4182-177">Project</span></span> | <span data-ttu-id="d4182-178">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-178">Yes</span></span> | <span data-ttu-id="d4182-179">Ναι</span><span class="sxs-lookup"><span data-stu-id="d4182-179">Yes</span></span> | <span data-ttu-id="d4182-180">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="d4182-180">N/A</span></span> | <span data-ttu-id="d4182-181">Οι λειτουργίες με τα ακόλουθα πεδία δεν υποστηρίζονται: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** και **Duration**.</span><span class="sxs-lookup"><span data-stu-id="d4182-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="d4182-182">Αυτά τα API μπορούν να καλούνται με αντικείμενα οντότητας που περιλαμβάνουν προσαρμοσμένα πεδία.</span><span class="sxs-lookup"><span data-stu-id="d4182-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="d4182-183">Η ιδιότητα αναγνωριστικού είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="d4182-183">The ID property is optional.</span></span> <span data-ttu-id="d4182-184">Εάν παρέχεται, το σύστημα επιχειρεί να τη χρησιμοποιήσει και προσφέρει εξαίρεση, εάν δεν μπορεί να χρησιμοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="d4182-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="d4182-185">Εάν δεν παρέχεται, το σύστημα θα το δημιουργήσει.</span><span class="sxs-lookup"><span data-stu-id="d4182-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="d4182-186">Περιορισμοί και γνωστά προβλήματα</span><span class="sxs-lookup"><span data-stu-id="d4182-186">Limitations and known issues</span></span>
<span data-ttu-id="d4182-187">Ακολουθεί μια λίστα με περιορισμούς και γνωστά ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="d4182-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="d4182-188">Τα API προγραμματισμού μπορούν να χρησιμοποιηθούν μόνο από **Χρήστες με άδεια χρήσης του Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="d4182-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="d4182-189">Δεν είναι δυνατό να χρησιμοποιηθούν από:</span><span class="sxs-lookup"><span data-stu-id="d4182-189">They can't be used by:</span></span>
    - <span data-ttu-id="d4182-190">Χρήστες εφαρμογής</span><span class="sxs-lookup"><span data-stu-id="d4182-190">Application users</span></span>
    - <span data-ttu-id="d4182-191">Χρήστες συστήματος</span><span class="sxs-lookup"><span data-stu-id="d4182-191">System users</span></span>
    - <span data-ttu-id="d4182-192">Χρήστες ενοποίησης</span><span class="sxs-lookup"><span data-stu-id="d4182-192">Integration users</span></span>
    - <span data-ttu-id="d4182-193">Άλλοι χρήστες που δεν διαθέτουν την απαιτούμενη άδεια χρήσης</span><span class="sxs-lookup"><span data-stu-id="d4182-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="d4182-194">Κάθε **OperationSet** μπορεί να έχει μέγιστο αριθμό 100 λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="d4182-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="d4182-195">Κάθε χρήστης μπορεί να έχει μόνο μέγιστο αριθμό 10 ανοιχτών **OperationSets**.</span><span class="sxs-lookup"><span data-stu-id="d4182-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="d4182-196">Το Project Operations υποστηρίζει πλέον το πολύ έως 500 συνολικές εργασίες σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="d4182-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="d4182-197">Η κατάσταση αποτυχίας και τα αρχεία καταγραφής αποτυχίας του **OperationSet** δεν είναι αυτή τη στιγμή διαθέσιμα.</span><span class="sxs-lookup"><span data-stu-id="d4182-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="d4182-198">Τα API προγραμματισμού είναι σε δημόσια προεπισκόπηση.</span><span class="sxs-lookup"><span data-stu-id="d4182-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="d4182-199">Η χρήση αυτών των API σε περιβάλλον παραγωγής δεν υποστηρίζεται από τη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4182-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="d4182-200">Δείγμα σεναρίου</span><span class="sxs-lookup"><span data-stu-id="d4182-200">Sample scenario</span></span>

<span data-ttu-id="d4182-201">Σε αυτό το σενάριο, θα δημιουργήσετε ένα έργο, ένα μέλος ομάδας, τέσσερις εργασίες και δύο αναθέσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="d4182-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="d4182-202">Στη συνέχεια, θα ενημερώσετε μία εργασία, θα ενημερώσετε το έργο, θα διαγράψετε μια εργασία, θα διαγράψετε μία ανάθεση πόρου και θα δημιουργήσετε μια εξάρτηση εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d4182-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="d4182-203">Πρόσθετα δείγματα</span><span class="sxs-lookup"><span data-stu-id="d4182-203">Additional samples</span></span>

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
