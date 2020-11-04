---
title: Προγραμματισμός έργου με μια δομή ανάλυσης εργασίας
description: Προγραμματισμός έργου με μια δομή ανάλυσης εργασίας στο Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: d77d9f8427f06015d4f4cb9438d7f59ac840b061
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077098"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="d1e9c-103">Προγραμματισμός έργου με μια δομή ανάλυσης εργασίας (Project Service)</span><span class="sxs-lookup"><span data-stu-id="d1e9c-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="d1e9c-104">Ένα χρονοδιάγραμμα έργου ενημερώνει για τις εργασίας που πρέπει να εκτελεστούν, τους πόρους που θα εκτελέσουν την εργασία, καθώς και το χρονικό πλαίσιο στο οποίο πρέπει να ολοκληρωθεί αυτή η εργασία.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="d1e9c-105">Το χρονοδιάγραμμα του έργου αντανακλά όλες τις εργασίες που σχετίζονται με την παράδοση του έργου εγκαίρως.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="d1e9c-106">Ένα από τα πρώτα βήματα για την αρχική φάση του έργου είναι να καταλήξετε στο χρονοδιάγραμμα του έργου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="d1e9c-107">Για να δημιουργήσετε ένα χρονοδιάγραμμα του έργου, πρέπει να δημιουργήσετε μια δομή ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="d1e9c-108">Δημιουργήσετε μια δομή έργου με μια δομή ανάλυσης εργασίας, η οποία σας βοηθά στα εξής:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="d1e9c-109">Ανάλυση έργου σε εργασίες διαχείρισης</span><span class="sxs-lookup"><span data-stu-id="d1e9c-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="d1e9c-110">Εκτίμηση του χρόνου που απαιτείται για την ολοκλήρωση μιας εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="d1e9c-111">Ορισμός των εξαρτήσεων των εργασιών και της διάρκειας των εργασιών</span><span class="sxs-lookup"><span data-stu-id="d1e9c-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="d1e9c-112">Προσδιορίστε τους ρόλους που απαιτούνται για την ολοκλήρωση κάθε εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="d1e9c-113">Το χρονοδιάγραμμα του έργου στη δομή ανάλυσης εργασίας προσφέρει μια γνώριμη εμπειρία εμφάνισης και χρήσης και περιλαμβάνει αλληλεπιδραστικό γράφημα Gantt.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="d1e9c-114">Δημιουργήσετε μια δομή ανάλυσης εργασίας για ένα έργο</span><span class="sxs-lookup"><span data-stu-id="d1e9c-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="d1e9c-115">Δημιουργήστε μια δομή ανάλυσης εργασίας για να αναπαραστήσετε τη σειρά των εργασιών σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="d1e9c-116">Η δομή ανάλυσης εργασίας περιλαμβάνει εργασίες, απαιτήσεις για την κάθε εργασία και πληροφορίες για τα έσοδα και το κόστος.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="d1e9c-117">Στη δομή ανάλυσης εργασίας, μπορείτε να προσθέσετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="d1e9c-118">Τη σειρά των εργασιών σε μια ιεραρχία</span><span class="sxs-lookup"><span data-stu-id="d1e9c-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="d1e9c-119">Άλλες εργασίες, εάν υπάρχουν, που πρέπει να ολοκληρωθούν πριν από την έναρξη μιας εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="d1e9c-120">Την ημερομηνία έναρξης, την ημερομηνία λήξης και τη διάρκεια μιας εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="d1e9c-121">Τον αριθμό των ωρών που απαιτούνται για μια εργασία</span><span class="sxs-lookup"><span data-stu-id="d1e9c-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="d1e9c-122">Τυχόν απαιτούμενες δεξιότητες και προαπαιτούμενα εκπαίδευσης των εργαζομένων</span><span class="sxs-lookup"><span data-stu-id="d1e9c-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="d1e9c-123">Τους εργαζόμενους στους οποίους έχει ανατεθεί μια εργασία</span><span class="sxs-lookup"><span data-stu-id="d1e9c-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="d1e9c-124">Εκτιμώμενα έσοδα και κόστη</span><span class="sxs-lookup"><span data-stu-id="d1e9c-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="d1e9c-125">Τύποι εργασιών</span><span class="sxs-lookup"><span data-stu-id="d1e9c-125">Task types</span></span>  
<span data-ttu-id="d1e9c-126">Θα χρησιμοποιήσετε τους παρακάτω τύπους εργασιών, κατά τη δημιουργία μιας δομής ανάλυσης εργασίας:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="d1e9c-127">**Κόμβος ρίζας έργου**</span><span class="sxs-lookup"><span data-stu-id="d1e9c-127">**Project root node**</span></span> | <span data-ttu-id="d1e9c-128">Την εργασία σύνοψης ανώτερου επιπέδου για το έργο.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-128">The top-level summary task for the project.</span></span> <span data-ttu-id="d1e9c-129">Όλες οι άλλες εργασίες του έργου δημιουργούνται σε αυτό.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-129">All other project tasks are created under it.</span></span> <span data-ttu-id="d1e9c-130">Το όνομα της εργασίας ρίζας είναι το όνομα του έργου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-130">The name of the root task is the project name.</span></span> <span data-ttu-id="d1e9c-131">Η προσπάθεια, οι ημερομηνίες και η διάρκεια του κόμβου ρίζας βασίζονται στις τιμές της ιεραρχίας που βρίσκονται κάτω από αυτό.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="d1e9c-132">Δεν μπορείτε να επεξεργαστείτε ιδιότητες του κόμβου ρίζας ή να διαγράψετε τον κόμβο ρίζας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="d1e9c-133">**Εργασίες σύνοψης ή κοντέινερ**</span><span class="sxs-lookup"><span data-stu-id="d1e9c-133">**Summary or container tasks**</span></span> | <span data-ttu-id="d1e9c-134">Μια εργασία σύνοψης είναι μια εργασία που έχει δευτερεύουσες εργασίες κάτω από αυτήν.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="d1e9c-135">Μια εργασία σύνοψης δεν έχει προσπάθεια εργασίας ή δικό της κόστος.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="d1e9c-136">Η προσπάθεια εργασίας και το κόστος είναι μια συνάθροιση των δευτερευουσών εργασιών της.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="d1e9c-137">Μπορείτε να αλλάξετε το όνομα μιας εργασίας σύνοψης, αλλά δεν μπορείτε να αλλάξετε την προσπάθεια, τις ημερομηνίες ή τη διάρκεια, επειδή αυτές υπολογίζονται αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="d1e9c-138">Με τη διαγραφή μιας εργασίας σύνοψης διαγράφεται η εργασία και όλες οι δευτερεύουσες εργασίες της.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="d1e9c-139">**Εργασίες κόμβου φύλλου**</span><span class="sxs-lookup"><span data-stu-id="d1e9c-139">**Leaf node tasks**</span></span> | <span data-ttu-id="d1e9c-140">Μια εργασία κόμβου φύλλου αντιπροσωπεύει τις πιο αναλυτικές εργασίες του έργου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="d1e9c-141">Περιλαμβάνει μια εκτιμώμενη προσπάθεια, έναν προγραμματισμένο αριθμό πόρων, τις προγραμματισμένες ημερομηνίες έναρξης και λήξης και τη διάρκεια.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="d1e9c-142">Ιεραρχία εργασιών</span><span class="sxs-lookup"><span data-stu-id="d1e9c-142">Task hierarchy</span></span>  
 <span data-ttu-id="d1e9c-143">Κατά τη δημιουργία μιας ιεραρχίας εργασιών, έχετε τις ακόλουθες επιλογές:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="d1e9c-144">**Προσθήκη εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-144">**Add task**.</span></span>   <span data-ttu-id="d1e9c-145">Μπορείτε να προσθέσετε μια εργασία σε μια θέση που επιλέγετε στην ιεραρχία εργασιών.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="d1e9c-146">Εάν δεν επιλέξετε θέση, η νέα εργασία σας εμφανίζεται στο τέλος.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="d1e9c-147">**Δημιουργία εσοχής εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-147">**Indent task**.</span></span>   <span data-ttu-id="d1e9c-148">Δημιουργήστε εσοχή σε μια εργασία, ώστε να είναι θυγατρική της εργασίας που βρίσκεται ακριβώς από επάνω της.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="d1e9c-149">**Προεξοχή εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-149">**Outdent task**.</span></span>   <span data-ttu-id="d1e9c-150">Δημιουργήστε μια προεξοχή εργασίας, ώστε να μην αποτελεί πλέον δευτερεύουσα εργασία της αρχικής γονικής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="d1e9c-151">**Μετακίνηση προς τα επάνω και μετακίνηση προς τα κάτω**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-151">**Move up and Move down**.</span></span>   <span data-ttu-id="d1e9c-152">Μετακινεί τις εργασίες προς τα επάνω και προς τα κάτω στην ιεραρχία της γονικής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="d1e9c-153">Η μετακίνηση μιας εργασίας προς τα επάνω ή προς τα κάτω δεν επηρεάζει την προσπάθεια, το κόστος, τις ημερομηνίες ή τη διάρκειά της.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="d1e9c-154">Χαρακτηριστικά εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-154">Task attributes</span></span>  
 <span data-ttu-id="d1e9c-155">Το όνομα μιας εργασίας περιγράφει την εργασία που πρέπει να ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="d1e9c-156">Μπορείτε να χρησιμοποιήσετε διάφορα χαρακτηριστικά εργασιών για να περιγράψετε το χρονοδιάγραμμα και τις απαιτήσεις προσωπικού για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="d1e9c-157">Χαρακτηριστικά χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="d1e9c-157">Schedule attributes</span></span>

 - <span data-ttu-id="d1e9c-158">Αντιστοιχίστε τιμές στα πεδία **Ώρες προσπάθειας** , **Αριθμός πόρων** , **Ημερομηνία έναρξης** , **Ημερομηνία λήξης** και **Διάρκεια** , για να προσδιορίσετε το χρονοδιάγραμμα για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-158">Assign values to **Effort hours** , **Number of resources** , **Start date** , **End date** , and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="d1e9c-159">Η **Προσπάθεια** είναι μια εκτίμηση των ωρών που απαιτούνται για την ολοκλήρωση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="d1e9c-160">Ο **Αριθμός πόρων** είναι μια εκτίμηση που εφαρμόζει ο διαχειριστής έργου στην εργασία, για να καταλήξετε στο βέλτιστο δυνατό χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="d1e9c-161">Η **Διάρκεια** (σε ημέρες) δηλώνει τον αριθμό των εργάσιμων ημερών που θα απαιτηθούν για την ολοκλήρωση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="d1e9c-162">Χαρακτηριστικά προσωπικού</span><span class="sxs-lookup"><span data-stu-id="d1e9c-162">Staffing attributes</span></span>

 - <span data-ttu-id="d1e9c-163">Ο **Ρόλος** , η **Οργανική μονάδα πόρου** , ο **Αριθμός πόρων** και οι **Πόροι** περιγράφουν τις απαιτήσεις προσωπικού για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-163">**Role** , **Resource organizational unit** , **Number of resources** , and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="d1e9c-164">Ο **Ρόλος** περιγράφει τον τύπο των πόρων που απαιτούνται για την εκτέλεση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="d1e9c-165">Η **Οργανική μονάδα πόρου** υποδεικνύει την οργανωτική μονάδα από την οποία θα πρέπει να στελεχωθούν οι πόροι για αυτήν την εργασία. Αυτό επηρεάζει, επίσης, το κόστος και την εκτίμηση πωλήσεων της εργασίας, δεδομένου ότι αυτοί οι παράγοντες λαμβάνονται υπόψη κατά τον προσδιορισμό της τιμής πώλησης για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="d1e9c-166">Οι **Πόροι** περιέχει έναν γενικό πόρο ή έναν καθορισμένο πόρο όταν εντοπίζεται.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="d1e9c-167">Εξαρτήσεις εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-167">Task dependencies</span></span>  
 <span data-ttu-id="d1e9c-168">Μπορείτε να δημιουργήσετε σχέσεις προκατόχου ανάμεσα σε μία ή περισσότερες εργασίες στη δομή ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="d1e9c-169">Μπορείτε να ορίσετε μία ή περισσότερες τιμές στο πεδίο προκατόχου σε εργασίες, για να υποδείξετε τις εργασίες από τις οποίες θα εξαρτάται.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="d1e9c-170">Όταν αντιστοιχίζετε μια τιμή προκατόχου σε μια εργασία, η εργασία μπορεί να ξεκινήσει μόνο όταν έχετε ολοκληρώσει όλες τις εργασίες του προκατόχου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="d1e9c-171">Η ρύθμιση αυτής της εξάρτησης σε μια εργασία θα έχει ως αποτέλεσμα τον επανυπολογισμό της προγραμματισμένης ημερομηνίας έναρξης της εργασίας σύμφωνα με τα τελευταία στοιχεία όλων των προκατόχων της.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="d1e9c-172">Οι επιπτώσεις που σχετίζονται με τον προκάτοχο σε ένα χρονοδιάγραμμα δεν περιορίζονται από τη λειτουργία της εργασίας που ορίζεται στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="d1e9c-173">Λειτουργία εργασιών</span><span class="sxs-lookup"><span data-stu-id="d1e9c-173">Task mode</span></span>  
 <span data-ttu-id="d1e9c-174">Η λειτουργία εργασιών είναι ένας από τους σημαντικούς παράγοντες που καθορίζουν τον προγραμματισμό εργασιών κόμβου φύλλου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="d1e9c-175">Υπάρχουν δύο λειτουργίες εργασιών για κάθε εργασία: λειτουργία αυτόματου προγραμματισμού και λειτουργία μη αυτόματη προγραμματισμού.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="d1e9c-176">**Αυτόματος προγραμματισμός**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-176">**Auto scheduling**.</span></span>   <span data-ttu-id="d1e9c-177">Όταν ορίζετε τη λειτουργία εργασιών στην επιλογή "Αυτόματα προγραμματισμένη", ο μηχανισμός προγραμματισμού της εργασίας χρησιμοποιεί τους κανόνες προγραμματισμού στα ακόλουθα χαρακτηριστικά εργασίας για τον προσδιορισμό του χρονοδιαγράμματος της εργασίας:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="d1e9c-178">Προκάτοχοι</span><span class="sxs-lookup"><span data-stu-id="d1e9c-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="d1e9c-179">Προσπάθεια</span><span class="sxs-lookup"><span data-stu-id="d1e9c-179">Effort</span></span>  
  
    -   <span data-ttu-id="d1e9c-180">Αριθμός πόρων</span><span class="sxs-lookup"><span data-stu-id="d1e9c-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="d1e9c-181">Τις ημερομηνίες έναρξης και λήξης</span><span class="sxs-lookup"><span data-stu-id="d1e9c-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="d1e9c-182">**Κανόνες προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-182">**Scheduling rules**.</span></span>   <span data-ttu-id="d1e9c-183">Η ημερομηνία έναρξης μιας εργασίας κόμβου φύλλου που δεν διαθέτει προκατόχους είναι από προεπιλογή η ημερομηνία έναρξης του χρονοδιαγράμματος του έργου.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="d1e9c-184">Η διάρκεια μιας εργασίας κόμβου φύλλου υπολογίζεται πάντα με βάση τον αριθμό των εργάσιμων ημερών μεταξύ των ημερομηνιών έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="d1e9c-185">Όταν μια εργασία προγραμματίζεται αυτόματα, ο μηχανισμός προγραμματισμού ακολουθεί τους παρακάτω κανόνες:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="d1e9c-186">Οι ημερομηνίες έναρξης και λήξης μιας εργασίας πρέπει να είναι πάντα εργάσιμες ημέρες, σύμφωνα με το ημερολόγιο προγραμματισμού του έργου</span><span class="sxs-lookup"><span data-stu-id="d1e9c-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="d1e9c-187">Η ημερομηνία έναρξης μιας εργασίας που έχει προκατόχους είναι από προεπιλογή η τελευταία ημερομηνία λήξης από τις προηγούμενές της</span><span class="sxs-lookup"><span data-stu-id="d1e9c-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="d1e9c-188">Προσπάθεια = Ο αριθμός ατόμων και η \* Διάρκεια \* σε ώρες σε μια τυπική εργάσιμη ημέρα του ημερολογίου έργου</span><span class="sxs-lookup"><span data-stu-id="d1e9c-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="d1e9c-189">**Μη αυτόματος προγραμματισμός**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-189">**Manual scheduling**.</span></span>   <span data-ttu-id="d1e9c-190">Σε ορισμένες υποθέσεις, μπορεί να θέλετε να αποκλίνετε από αυτούς τους κανόνες.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="d1e9c-191">Σε αυτές τις περιπτώσεις, μπορείτε να ορίσετε την λειτουργία εργασίας για την εργασία που πρέπει να προγραμματιστεί με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="d1e9c-192">Διακόπτει το μηχανισμό προγραμματισμού από τον υπολογισμό των τιμών για άλλα χαρακτηριστικά του χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="d1e9c-193">Η ρύθμιση προκατόχων σε εργασίες επηρεάζει πάντα την ημερομηνία έναρξης της εξαρτώμενης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="d1e9c-194">Δημιουργήστε μια δομή ανάλυσης εργασίας</span><span class="sxs-lookup"><span data-stu-id="d1e9c-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="d1e9c-195">Μεταβείτε στο μενού **Project Service > Έργα**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="d1e9c-196">Επιλέξτε το έργο στο οποίο θέλετε να εργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="d1e9c-197">Στη γραμμή στο επάνω μέρος της οθόνης, επιλέξτε το κάτω βέλος δίπλα από το όνομα του έργου και, στη συνέχεια, επιλέξτε "Δομή ανάλυσης εργασίας".</span><span class="sxs-lookup"><span data-stu-id="d1e9c-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="d1e9c-198">Για να προσθέσετε μια εργασία, κάντε κλικ στο κουμπί **Προσθήκη εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="d1e9c-199">Συμπληρώστε τα πεδία για την εργασία και έπειτα κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="d1e9c-200">Συνεχίστε να προσθέτετε εργασίες, μέχρι να ολοκληρωθεί η δομή ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="d1e9c-201">Κατά τη δημιουργία μιας δομής ανάλυσης εργασίας, μπορείτε να κάνετε τα εξής για να οργανώσετε τις εργασίες σας:</span><span class="sxs-lookup"><span data-stu-id="d1e9c-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="d1e9c-202">Επιλέξτε μια εργασία και κάντε κλικ στην επιλογή **Εσοχή** , για να τη μετακινήσετε κάτω από μια άλλη εργασία ή κάντε κλικ στο κουμπί "Προεξοχή", για να την μετακινήσετε από ένα επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="d1e9c-203">Επιλέξτε μια εργασία και κάντε κλικ στην επιλογή **Μετακίνηση επάνω** ή στην επιλογή **Μετακίνηση κάτω** , για να τη μετακινήσετε προς τα επάνω ή προς τα κάτω στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="d1e9c-204">Κάντε κλικ στην επιλογή **Απόκρυψη Gantt** για να αποκρύψετε το γράφημα Gantt, και κάντε κλικ στην επιλογή **Εμφάνιση Gantt** για να το εμφανίσετε ξανά.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="d1e9c-205">Επιλέξτε ένα διαφορετικό χρονικό διάστημα για το γράφημα Gantt στη **Χρονική κλίμακα**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="d1e9c-206">Για να προσθέσετε τους ρόλους που καθορίσατε στη δομή ανάλυσης εργασίας στα μέλη της ομάδας του έργου σας, κάντε κλικ στην επιλογή **Δημιουργία ομάδας έργου**.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="d1e9c-207">Κάντε κλικ στο κουμπί **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης, όταν ολοκληρώσετε τις αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="d1e9c-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="d1e9c-208">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="d1e9c-208">See Also</span></span>  
 [<span data-ttu-id="d1e9c-209">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="d1e9c-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
