---
title: Αλλαγές διαχείρισης πόρων (Project Service Automation 3.x)
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις αλλαγές στην περιοχή διαχείρισης πόρων.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e888d55b93c40e08e51bd4480853fec37f2b6333
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007816"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="397cb-103">Αλλαγές διαχείρισης πόρων (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="397cb-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="397cb-104">Οι ενότητες αυτού του θέματος παρέχουν πληροφορίες σχετικά με τις αλλαγές που έχουν γίνει στην περιοχή διαχείρισης πόρων του Dynamics 365 Project Service Automation έκδοση 3.x.</span><span class="sxs-lookup"><span data-stu-id="397cb-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="397cb-105">Εκτιμήσεις έργων</span><span class="sxs-lookup"><span data-stu-id="397cb-105">Project estimates</span></span>

<span data-ttu-id="397cb-106">Αντί να βασιστούν στην οντότητα **msdyn\_projecttask** (**Εργασία έργου**), οι εκτιμήσεις έργου βασίζονται στην οντότητα **msdyn\_resourceassignment** (**Ανάθεση πόρου**).</span><span class="sxs-lookup"><span data-stu-id="397cb-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="397cb-107">Οι αναθέσεις πόρων έχουν γίνει η "προέλευση της αλήθειας" για τον προγραμματισμό και την τιμολόγηση των εργασιών.</span><span class="sxs-lookup"><span data-stu-id="397cb-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="397cb-108">Εργασίες γραμμής</span><span class="sxs-lookup"><span data-stu-id="397cb-108">Line tasks</span></span>

<span data-ttu-id="397cb-109">Στο PSA 3.x, οι εργασίες γραμμής είναι παλιές (δεν χρησιμοποιούνται).</span><span class="sxs-lookup"><span data-stu-id="397cb-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="397cb-110">Οι αναθέσεις τώρα παραπέμπουν σε ολόκληρη την εργασία αντί για τις εργασίες γραμμής.</span><span class="sxs-lookup"><span data-stu-id="397cb-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="397cb-111">Το παρακάτω παράδειγμα δείχνει τον τρόπο με τον οποίο η εργασία που ονομάζεται "δοκιμαστική εργασία" ανατίθεται στα μέλη της ομάδας Α και Β σε προγενέστερες εκδόσεις του PSA και στο PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="397cb-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="397cb-112">**Πριν από το PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="397cb-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="397cb-113">Δοκιμαστική εργασία</span><span class="sxs-lookup"><span data-stu-id="397cb-113">Test task</span></span>

        - <span data-ttu-id="397cb-114">Δοκιμαστική εργασία – Εργασία γραμμής 1</span><span class="sxs-lookup"><span data-stu-id="397cb-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="397cb-115">Ανάθεση σε Α</span><span class="sxs-lookup"><span data-stu-id="397cb-115">Assignment to A</span></span>

        - <span data-ttu-id="397cb-116">Δοκιμαστική εργασία – Εργασία γραμμής 2</span><span class="sxs-lookup"><span data-stu-id="397cb-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="397cb-117">Ανάθεση σε Β</span><span class="sxs-lookup"><span data-stu-id="397cb-117">Assignment to B</span></span>

- <span data-ttu-id="397cb-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="397cb-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="397cb-119">Δοκιμαστική εργασία</span><span class="sxs-lookup"><span data-stu-id="397cb-119">Test task</span></span>

        - <span data-ttu-id="397cb-120">Ανάθεση σε Α</span><span class="sxs-lookup"><span data-stu-id="397cb-120">Assignment to A</span></span>
        - <span data-ttu-id="397cb-121">Ανάθεση σε Β</span><span class="sxs-lookup"><span data-stu-id="397cb-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="397cb-122">Μη εκχωρημένη ανάθεση</span><span class="sxs-lookup"><span data-stu-id="397cb-122">Unassigned assignment</span></span>

<span data-ttu-id="397cb-123">Στο PSA 3.x, μια ανάθεση που δεν έχει ανατεθεί είναι μια ανάθεση που έχει ανατεθεί σε μέλος της ομάδας **NULL** και σε έναν πόρο **NULL**.</span><span class="sxs-lookup"><span data-stu-id="397cb-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="397cb-124">Οι εκχωρήσεις που δεν έχουν ανατεθεί μπορεί να προκύψουν σε μερικά σενάρια:</span><span class="sxs-lookup"><span data-stu-id="397cb-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="397cb-125">Εάν μια εργασία έχει δημιουργηθεί, αλλά δεν έχει ανατεθεί ακόμα σε κάποιο μέλος της ομάδας, δημιουργείται πάντα μια ανάθεση που δεν έχει εκχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="397cb-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="397cb-126">Εάν καταργηθούν όλοι όσοι έχουν ανατεθεί σε μια εργασία, δημιουργείται εκ νέου μια ανάθεση που δεν έχει ανατεθεί για αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="397cb-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="397cb-127">Πεδία χρονοδιαγράμματος στην οντότητα εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="397cb-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="397cb-128">Τα πεδία στην οντότητα **msdyn\_projecttask** δεν χρησιμοποιούνται πλέον ή έχουν μετακινηθεί στην οντότητα **msdyn\_resourceassignment** ή πλέον αναφέρονται από την οντότητα **msdyn\_projectteam** (**Μέλος ομάδας έργου**).</span><span class="sxs-lookup"><span data-stu-id="397cb-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="397cb-129">Πεδίο που δεν χρησιμοποιείται πλέον στο msdyn\_projecttask (Εργασία έργου)</span><span class="sxs-lookup"><span data-stu-id="397cb-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="397cb-130">Νέο πεδίο στο msdyn\_resourceassignment (Ανάθεση πόρου)</span><span class="sxs-lookup"><span data-stu-id="397cb-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="397cb-131">Σχόλιο</span><span class="sxs-lookup"><span data-stu-id="397cb-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="397cb-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="397cb-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="397cb-133">Καμία</span><span class="sxs-lookup"><span data-stu-id="397cb-133">None</span></span> | |
| <span data-ttu-id="397cb-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="397cb-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="397cb-135">Καμία</span><span class="sxs-lookup"><span data-stu-id="397cb-135">None</span></span> | |
| <span data-ttu-id="397cb-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="397cb-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="397cb-137">Καμία</span><span class="sxs-lookup"><span data-stu-id="397cb-137">None</span></span> | |
| <span data-ttu-id="397cb-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="397cb-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="397cb-139">Καμία</span><span class="sxs-lookup"><span data-stu-id="397cb-139">None</span></span> | |
| <span data-ttu-id="397cb-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="397cb-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="397cb-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="397cb-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="397cb-142">Η μορφή της δομής δεδομένων JavaScript Object Notation (JSON) η οποία είναι αποθηκευμένη στο πεδίο έχει αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="397cb-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="397cb-143">Καμπύλη χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="397cb-143">Schedule contour</span></span>

<span data-ttu-id="397cb-144">Η καμπύλη χρονοδιαγράμματος αποθηκεύεται στο πεδίο **Προγραμματισμένη εργασία** (**\_msdyn** plannedwork) κάθε οντότητας **Ανάθεση πόρου** (**msdyn\_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="397cb-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="397cb-145">Δομή</span><span class="sxs-lookup"><span data-stu-id="397cb-145">Structure</span></span>

<span data-ttu-id="397cb-146">Η νέα δομή της καμπύλης χρονοδιαγράμματος αποτελείται από ευέλικτα τμήματα χρόνου που καθορίζονται για κάθε ημέρα του χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="397cb-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="397cb-147">Κάθε τμήμα χρόνου έχει τις ακόλουθες ιδιότητες:</span><span class="sxs-lookup"><span data-stu-id="397cb-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="397cb-148">**Έναρξη** – η έναρξη των ωρών εργασίας της ημέρας, σύμφωνα με το ημερολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="397cb-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="397cb-149">**Τέλος** – το τέλος των ωρών εργασίας της ημέρας, σύμφωνα με το ημερολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="397cb-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="397cb-150">**Ώρες** – ο αριθμός των ωρών που ανατίθενται την ημέρα.</span><span class="sxs-lookup"><span data-stu-id="397cb-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="397cb-151">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="397cb-151">**Example**</span></span>

<span data-ttu-id="397cb-152">Αυτό το παράδειγμα χρησιμοποιεί ένα ημερολόγιο έργου όπου η εργάσιμη ημέρα είναι από τις 9 πμ έως τις 5 μμ στη ζώνη ώρας UTC-8.</span><span class="sxs-lookup"><span data-stu-id="397cb-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="397cb-153">Αυτόματος προγραμματισμός και μη αυτόματος προγραμματισμός</span><span class="sxs-lookup"><span data-stu-id="397cb-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="397cb-154">Εάν μια εργασία έχει προγραμματιστεί αυτόματα, οι ώρες έχουν τοποθετηθεί μπροστά και η διάρκεια της εργασίας μπορεί να μειωθεί.</span><span class="sxs-lookup"><span data-stu-id="397cb-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="397cb-155">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="397cb-155">**Example**</span></span>

<span data-ttu-id="397cb-156">Η παρακάτω εργασία προγραμματίζεται αυτόματα για 18 ώρες σε τρεις ημέρες (3 Δεκεμβρίου 2018 έως 5 Δεκεμβρίου 2018).</span><span class="sxs-lookup"><span data-stu-id="397cb-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="397cb-157">Εάν μια εργασία προγραμματιστεί με μη αυτόματο τρόπο, οι ώρες κατανέμονται ομοιόμορφα σε όλες τις ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="397cb-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="397cb-158">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="397cb-158">**Example**</span></span>

<span data-ttu-id="397cb-159">Η παρακάτω εργασία προγραμματίζεται μη αυτόματα για 18 ώρες σε τρεις ημέρες (3 Δεκεμβρίου 2018 έως 5 Δεκεμβρίου 2018).</span><span class="sxs-lookup"><span data-stu-id="397cb-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="397cb-160">Μονάδα ανάθεσης</span><span class="sxs-lookup"><span data-stu-id="397cb-160">Assignment unit</span></span>

<span data-ttu-id="397cb-161">Η μονάδα ανάθεσης έχει καταργηθεί στο PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="397cb-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="397cb-162">Οι ώρες προσπάθειας εργασίας είναι πλέον ισότιμες, ανά ημέρα, μεταξύ όλων των πόρων που έχουν ανατεθεί.</span><span class="sxs-lookup"><span data-stu-id="397cb-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="397cb-163">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="397cb-163">**Example**</span></span>

<span data-ttu-id="397cb-164">Σε αυτό το παράδειγμα, η εργασία έχει ανατεθεί σε δύο πόρους και έχει προγραμματιστεί αυτόματα για 36 ώρες σε τρεις ημέρες (3 Δεκεμβρίου 2018 έως 5 Δεκεμβρίου 2018).</span><span class="sxs-lookup"><span data-stu-id="397cb-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="397cb-165">Ανάθεση 1:</span><span class="sxs-lookup"><span data-stu-id="397cb-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="397cb-166">Ανάθεση 2:</span><span class="sxs-lookup"><span data-stu-id="397cb-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="397cb-167">Διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="397cb-167">Pricing dimensions</span></span>

<span data-ttu-id="397cb-168">Στο PSA 3.x, τα πεδία διάστασης τιμολόγησης που αφορούν πόρους (όπως **Ρόλος** και **Οργανική μονάδα**) έχουν καταργηθεί από την οντότητα **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="397cb-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="397cb-169">Είναι δυνατή η ανάκτηση αυτών των πεδίων από το αντίστοιχο μέλος της ομάδας έργου (**msdyn\_projectteam**) της ανάθεσης πόρου (**msdyn\_resourceassignment**) όταν δημιουργούνται εκτιμήσεις του έργου.</span><span class="sxs-lookup"><span data-stu-id="397cb-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="397cb-170">Ένα νέο πεδίο **msdyn\_organizationalunit**, έχει προστεθεί στην οντότητα **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="397cb-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="397cb-171">Πεδίο που δεν χρησιμοποιείται πλέον στο msdyn\_projecttask (Εργασία έργου)</span><span class="sxs-lookup"><span data-stu-id="397cb-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="397cb-172">Πεδίο από το msdyn\_projectteam (Μέλος ομάδας έργου) το οποίο χρησιμοποιείται.</span><span class="sxs-lookup"><span data-stu-id="397cb-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="397cb-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="397cb-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="397cb-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="397cb-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="397cb-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="397cb-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="397cb-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="397cb-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="397cb-177">Καμπύλες</span><span class="sxs-lookup"><span data-stu-id="397cb-177">Contours</span></span>

<span data-ttu-id="397cb-178">Τα πεδία καμπύλης τιμολόγησης και εκτίμησης δεν χρησιμοποιούνται στην οντότητα **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="397cb-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="397cb-179">Έχουν μετακινηθεί στην οντότητα **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="397cb-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="397cb-180">Πεδίο που δεν χρησιμοποιείται πλέον στο msdyn\_projecttask (Εργασία έργου)</span><span class="sxs-lookup"><span data-stu-id="397cb-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="397cb-181">Νέο πεδίο στο msdyn\_resourceassignment (Ανάθεση πόρου)</span><span class="sxs-lookup"><span data-stu-id="397cb-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="397cb-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="397cb-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="397cb-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="397cb-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="397cb-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="397cb-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="397cb-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="397cb-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="397cb-186">Τα παρακάτω πεδία έχουν προστεθεί στην οντότητα **msdyn\_resourceassignment**:</span><span class="sxs-lookup"><span data-stu-id="397cb-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="397cb-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="397cb-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="397cb-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="397cb-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="397cb-189">Τα παρακάτω πεδία για προγραμματισμένο, πραγματικό και υπολειπόμενο κόστος και πωλήσεις παραμένουν αμετάβλητα στην οντότητα **msdyn\_projecttask**:</span><span class="sxs-lookup"><span data-stu-id="397cb-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="397cb-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="397cb-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="397cb-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="397cb-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="397cb-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="397cb-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="397cb-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="397cb-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="397cb-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="397cb-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="397cb-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="397cb-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]