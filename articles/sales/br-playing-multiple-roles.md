---
title: Υπολογίστε τις πωλήσεις και το κόστος του έργου όταν ένας πόρος με δυνατότητα κράτησης εκτελεί πολλαπλούς ρόλους σε ένα έργο
description: Αυτό το θέμα εξηγεί τον τρόπο χρήσης των διαστάσεων τιμολόγησης για την υποστήριξη των εκτιμήσεων τιμολόγησης και κοστολόγησης για έναν πόρο που εκτελεί πολλαπλούς ρόλους σε ένα έργο.
author: rumant
manager: tfehr
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: da17f0f58623128d51fda0f5529182cd37ea41b9
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531439"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-on-a-project"></a><span data-ttu-id="f929d-103">Υπολογίστε τις πωλήσεις και το κόστος του έργου όταν ένας πόρος με δυνατότητα κράτησης εκτελεί πολλαπλούς ρόλους σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="f929d-103">Estimate project sales and costs when a bookable resource fills multiple roles on a project</span></span> 

<span data-ttu-id="f929d-104">_**Ισχύει για:** Project Operations για μη εφοδιασμένα σενάρια ή σενάρια βασισμένα σε πόρους, Lite ανάπτυξη - προσφορά σε προτιμολόγηση, Project Operations για μη εφοδιασμένα σενάρια ή σενάρια βασισμένα σε πόρους_</span><span class="sxs-lookup"><span data-stu-id="f929d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing, Project Operations for stocked/production-based scenarios_</span></span> 

<span data-ttu-id="f929d-105">Οι εταιρείες που βασίζονται σε έργα έχουν συχνά την ανάγκη ένας πόρος να εκτελεί πολλούς ρόλους σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f929d-105">Project-based companies often have the need for one resource to fill multiple roles on a project.</span></span> <span data-ttu-id="f929d-106">Κάθε ρόλος μπορεί να τιμολογηθεί και να κοστολογηθεί διαφορετικά.</span><span class="sxs-lookup"><span data-stu-id="f929d-106">Each role can be priced and costed differently.</span></span> <span data-ttu-id="f929d-107">Αυτό σημαίνει ότι ο χρόνος του ίδιου πόρου σε ένα έργο μπορεί να λάβει μια διαφορετική οικονομική εκτίμηση ανάλογα με τα ποσοστά χρέωσης και κόστους για κάθε ρόλο.</span><span class="sxs-lookup"><span data-stu-id="f929d-107">This means that the same resource's time on a project could get a different financial estimate depending on the bill and cost rates for each role.</span></span> <span data-ttu-id="f929d-108">Μπορείτε να ορίσετε τις τιμές στην καρτέλα μέλους ομάδας για τον κατονομαζόμενο πόρο με διαφορετικές παρακάμψεις σε καθεμία από τις εργασίες στις οποίες έχει ανατεθεί το μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="f929d-108">You can set up the values on the team member record for the named resource with different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="f929d-109">Το παρακάτω παράδειγμα σάς καθοδηγεί σχετικά με τον τρόπο με τον οποίο η απλή παράκαμψη μιας τιμής επιτρέπει σε έναν πόρο να έχει πολλούς ρόλους σε ένα έργο με διαφορετικά ποσοστά κόστους και χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="f929d-109">The following example walks you through how the simple override of a value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="f929d-110">Δημιουργία εργασιών</span><span class="sxs-lookup"><span data-stu-id="f929d-110">Create tasks</span></span>
<span data-ttu-id="f929d-111">Για να δημιουργήσετε εργασίες, θα πρέπει να προσθέσετε εργασίες, καθώς και εργασίες σύνοψης, και μετά θα πρέπει να αναθέσετε την εργασία πριν προσθέσετε τη διάρκεια της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="f929d-111">To create tasks, you need to add tasks, as well as summary tasks, after which you need to assign the task before you add task duration.</span></span> 

### <a name="add-tasks-and-summary-tasks"></a><span data-ttu-id="f929d-112">Προσθήκη εργασιών και εργασιών σύνοψης</span><span class="sxs-lookup"><span data-stu-id="f929d-112">Add tasks and summary tasks</span></span>
<span data-ttu-id="f929d-113">Για να προσθέσετε μια εργασία, ακολουθήστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="f929d-113">To add a task, complete the following steps.</span></span>

1. <span data-ttu-id="f929d-114">Μεταβείτε στην επιλογή **Έργα** και ανοίξτε το έργο στο οποίο θέλετε να προσθέσετε εργασίες.</span><span class="sxs-lookup"><span data-stu-id="f929d-114">Go to **Projects** and open the project to which you want to add tasks.</span></span>
2. <span data-ttu-id="f929d-115">Επιλέξτε **Προσθήκη νέας εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-115">Select **Add new task**.</span></span> <span data-ttu-id="f929d-116">Ονομάστε την εργασία και, στη συνέχεια, πατήστε το πλήκτρο **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f929d-116">Name the task, and then press **Enter**.</span></span>
3. <span data-ttu-id="f929d-117">Εισαγάγετε το όνομα μιας άλλης εργασίας και πατήστε **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f929d-117">Enter another task name and press **Enter**.</span></span> <span data-ttu-id="f929d-118">Επαναλάβετε αυτήν την ενέργεια, μέχρι να έχετε μια πλήρη λίστα εργασιών.</span><span class="sxs-lookup"><span data-stu-id="f929d-118">Repeat this until you have a full list of tasks.</span></span>
3. <span data-ttu-id="f929d-119">Για να δημιουργήσετε εσοχή εργασιών στην περιοχή εργασίες **Σύνοψης**, επιλέξτε τις τρεις κατακόρυφες κουκίδες με το όνομα της εργασίας και, στη συνέχεια, επιλέξτε **Δημιουργία δευτερεύουσας εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-119">To indent tasks under **Summary** tasks, select the three vertical dots by the task name, and then select **Make subtask**.</span></span> 

  > [!TIP]
  > <span data-ttu-id="f929d-120">Για να επιλέξετε περισσότερες από μία εργασίες, επιλέξτε μια εργασία, πατήστε και κρατήστε πατημένο το πλήκτρο **CTRL** και, στη συνέχεια, επιλέξτε μια άλλη εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-120">To select more than one task, select a task, press and hold **Ctrl**, and then select another task.</span></span>
  >
  > <span data-ttu-id="f929d-121">Μπορείτε, επίσης, να επιλέξετε **Προώθηση δευτερεύουσας εργασίας** για να μετακινήσετε τις εργασίες από την περιοχή εργασίες **Σύνοψης**.</span><span class="sxs-lookup"><span data-stu-id="f929d-121">You can also choose **Promote subtask** to move tasks out from under **Summary** tasks.</span></span>

### <a name="assign-tasks"></a><span data-ttu-id="f929d-122">Ανάθεση εργασιών</span><span class="sxs-lookup"><span data-stu-id="f929d-122">Assign tasks</span></span>

<span data-ttu-id="f929d-123">Ολοκληρώστε τα παρακάτω βήματα για να αναθέσετε εργασίες.</span><span class="sxs-lookup"><span data-stu-id="f929d-123">Complete the following steps to assign tasks.</span></span>

1. <span data-ttu-id="f929d-124">Στη στήλη **Ανάθεση σε** για μια εργασία, επιλέξτε το εικονίδιο του ατόμου.</span><span class="sxs-lookup"><span data-stu-id="f929d-124">In the  **Assigned to**  column for a task, select the person icon.</span></span>
2. <span data-ttu-id="f929d-125">Επιλέξτε ένα μέλος της ομάδας από τη λίστα ή εισαγάγετε κείμενο για να αναζητήσετε ένα όνομα.</span><span class="sxs-lookup"><span data-stu-id="f929d-125">Choose a team member from the list or enter text to search for a name.</span></span>

### <a name="add-task-duration-and-columns"></a><span data-ttu-id="f929d-126">Προσθήκη διάρκειας εργασίας και στηλών</span><span class="sxs-lookup"><span data-stu-id="f929d-126">Add task duration and columns</span></span>

<span data-ttu-id="f929d-127">Είναι συχνά πιο εύκολο να ξεκινήσετε την κατασκευή του έργου σας με τη διάρκεια.</span><span class="sxs-lookup"><span data-stu-id="f929d-127">It's often easiest to begin constructing your project with duration.</span></span> <span data-ttu-id="f929d-128">Ολοκληρώστε τα παρακάτω βήματα για να προσθέσετε μια διάρκεια εργασίας.</span><span class="sxs-lookup"><span data-stu-id="f929d-128">Complete the following steps to add a task duration.</span></span>

1. <span data-ttu-id="f929d-129">Στη στήλη **Διάρκεια** για μια εργασία, πληκτρολογήστε τον αριθμό των ημερών που θεωρείτε ότι θα χρειαστούν για την ολοκλήρωση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="f929d-129">In the **Duration** column for a task, type the number of days you think it will take to accomplish the task.</span></span> <span data-ttu-id="f929d-130">Εάν θέλετε να χρησιμοποιήσετε μια διαφορετική μονάδα χρόνου, εισαγάγετε έναν αριθμό συν τη λέξη **ώρες**, **εβδομάδες** ή **μήνες**.</span><span class="sxs-lookup"><span data-stu-id="f929d-130">If you want to use a different unit of time, enter a number plus the word **hours**, **weeks**, or **months**.</span></span>
2. <span data-ttu-id="f929d-131">Εάν θέλετε η εργασία σας να εμφανίζεται ως ορόσημο σε σχήμα διαμαντιού στην προβολή **Λωρίδας χρόνου**, στη στήλη **Διάρκεια**, εισαγάγετε **0 ημέρες**.</span><span class="sxs-lookup"><span data-stu-id="f929d-131">If you want your task to appear as a diamond-shaped milestone in the **Timeline** view, in the **Duration** column, enter **0 days** .</span></span>
3. <span data-ttu-id="f929d-132">Πατήστε το πλήκτρο **Enter** για να μεταβείτε στο πεδίο **Διάρκεια** της επόμενης εργασίας και να συνεχίσετε με την εισαγωγή διάρκειας.</span><span class="sxs-lookup"><span data-stu-id="f929d-132">Press **Enter**  to go to the next task's **Duration** field and continue entering durations.</span></span>

  > [!NOTE]
  > <span data-ttu-id="f929d-133">Δεν μπορείτε να ειαγάγετε μια διάρκεια για εργασίες σύνοψης.</span><span class="sxs-lookup"><span data-stu-id="f929d-133">You can't enter a duration for summary tasks.</span></span>

<span data-ttu-id="f929d-134">Μπορείτε να προσθέσετε στήλες στο έργο σας για να παρέχετε περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="f929d-134">You can add columns to your project to provide more details.</span></span> <span data-ttu-id="f929d-135">Για να το κάνετε αυτό, επιλέξτε **Προσθήκη στήλης**.</span><span class="sxs-lookup"><span data-stu-id="f929d-135">To do this, select **Add column**.</span></span> 

<span data-ttu-id="f929d-136">Για περισσότερες πληροφορίες, δείτε [Δημιουργία έργου](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span><span class="sxs-lookup"><span data-stu-id="f929d-136">For more information, see [Create a project](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span></span>

## <a name="set-up-the-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="f929d-137">Ρύθμιση του ρόλου και της μονάδας οργανισμού για ένα γενικό μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="f929d-137">Set up the role and organization unit for a generic project team member</span></span>
<span data-ttu-id="f929d-138">Ολοκληρώστε τα παρακάτω βήματα για να ρυθμίσετε έναν ρόλο και μια οργανική μονάδα για ένα γενικό μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="f929d-138">Complete the following steps to set up a role and organizational unit for a generic team member.</span></span>

1. <span data-ttu-id="f929d-139">Στη σελίδα **Εργασίες**, επιλέξτε τη γραμμή **Εργασία** για την **Εργασία Α**.</span><span class="sxs-lookup"><span data-stu-id="f929d-139">On the **Tasks** page, select the **Task** row for **Task A**.</span></span> 
2. <span data-ttu-id="f929d-140">Στο **Ανάθεση σε**, επιλέξτε **Προσθήκη γενικού πόρου**.</span><span class="sxs-lookup"><span data-stu-id="f929d-140">In **Assigned To**, select **Add generic resource**.</span></span> <span data-ttu-id="f929d-141">Με αυτήν την ενέργεια ανοίγει η σελίδα **Γρήγορη δημιουργία μέλους ομάδας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-141">This opens the **Team Member Quick Create** page.</span></span>
3. <span data-ttu-id="f929d-142">Στη σελίδα **Γρήγορη δημιουργία μέλους ομάδας**, καθορίστε τα χαρακτηριστικά του γενικού μέλους ομάδας που μπορεί να εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-142">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="f929d-143">Επιλέξτε τον κατάλληλο ρόλο και οργανωτική μονάδα και, στη συνέχεια, επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="f929d-143">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="f929d-144">Ένα γενικό μέλος ομάδας δημιουργείται και εκχωρείται σε αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-144">A generic team member is created and assigned to this task.</span></span> 
5. <span data-ttu-id="f929d-145">Επαναλάβετε τα βήματα 1-4 για την **Εργασία Β**. Ωστόσο, η **Εργασία Β** πρέπει να έχει διαφορετικό ρόλο και οργανωτική μονάδα που έχει ανατεθεί για το γενικό μέλος της ομάδας από την **Εργασία Α**.</span><span class="sxs-lookup"><span data-stu-id="f929d-145">Repeat steps 1-4 for **Task B**. However, **Task B** must have a different role and organizational unit assigned for the generic team member than **Task A**.</span></span> 

## <a name="set-up-the-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="f929d-146">Ρύθμιση του ρόλου και της μονάδας οργανισμού για μια εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="f929d-146">Set up the role and organization unit for a project task</span></span>
<span data-ttu-id="f929d-147">Ολοκληρώστε τα παρακάτω βήματα για να ρυθμίσετε έναν ρόλο και μια οργανική μονάδα για μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-147">Complete the following steps to set up a role and organizational unit for a task.</span></span>

1. <span data-ttu-id="f929d-148">Αφού δημιουργήσετε την **Εργασία Α**, επιλέξτε την εργασία και, στη συνέχεια, επιλέξτε το εικονόδιο **i** για να ανοίξετε το τμήμα παραθύρου **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-148">After you create **Task A**, select the task, and then select the **i** icon to open the **Task Details** pane.</span></span> 
2. <span data-ttu-id="f929d-149">Στο τμήμα παραθύρου **Λεπτομέρειες εργασίας**, κάντε κύλιση προς τα κάτω και επιλέξτε **Προβολή λεπτομερειών** για να ανοίξετε τη σελίδα **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-149">On the **Task Details** pane, scroll to the bottom and select **View Details** to open the **Task Details** page.</span></span>
3. <span data-ttu-id="f929d-150">Στη σελίδα **Λεπτομέρειες εργασίας**, στην ενότητα **Ρόλος** και **Οργανωτική μονάδα**, προσθέστε τις τιμές που απαιτούνται για την εκτέλεση αυτής της εργασίας για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="f929d-150">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required to perform this task for the resource.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="f929d-151">Εάν ολοκληρώσετε αυτό το σενάριο χρησιμοποιώντας τα δεδομένα επίδειξης του Project Operations, επιλέξτε **Συνεννόηση με υποψήφιο πελάτη** για τον ρόλο και **Fabrikam US** ως την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="f929d-151">If you complete this scenario using the Project Operations demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

4. <span data-ttu-id="f929d-152">Επιλέξτε **Εργασία Β**, και στη συνέχεια επιλέξτε την εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-152">Select **Task B**, and then select the task.</span></span>
5. <span data-ttu-id="f929d-153">Επιλέξτε το εικονίδιο **i** για να ανοίξετε το τμήμα παραθύρου **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-153">Select the **i** icon to open **Task Details** pane.</span></span> 
6. <span data-ttu-id="f929d-154">Στο τμήμα παραθύρου **Λεπτομέρειες εργασίας**, κάντε κύλιση προς τα κάτω και επιλέξτε **Προβολή λεπτομερειών** για να ανοίξετε τη σελίδα **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-154">On the **Task Details** pane, scroll to the bottom and select **View details** to open the **Task Details** page.</span></span>
7. <span data-ttu-id="f929d-155">Στη σελίδα **Λεπτομέρειες εργασίας**, στην ενότητα **Ρόλος** και **Οργανωτική μονάδα**, προσθέστε τις τιμές που απαιτούνται ενός πόρου που θα εκτελούσε αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="f929d-155">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="f929d-156">Οι τιμές στον **Ρόλο** και την **Οργανωτική μονάδα** για την **Εργασία Β** πρέπει να είναι διαφορετικές από αυτές για την **Εργασία Α**.</span><span class="sxs-lookup"><span data-stu-id="f929d-156">The values in **Role** and **Organizational Unit** for **Task B** must be different than those for **Task A**.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="f929d-157">Εάν ολοκληρώσετε αυτό το σενάριο χρησιμοποιώντας τα δεδομένα επίδειξης του Project Operations, επιλέξτε **Τεχνικός δικτύου** για τον ρόλο και **Fabrikam US** ως την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="f929d-157">If you complete this scenario using the Project Operations demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

8. <span data-ttu-id="f929d-158">Αποθηκεύστε και κλείστε τη σελίδα **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f929d-158">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="f929d-159">Συμπεριφορά μέλους ομάδας και εκτίμησης</span><span class="sxs-lookup"><span data-stu-id="f929d-159">Team member and estimates behavior</span></span> 
<span data-ttu-id="f929d-160">Για να κατανοήσετε τη συμπεριφορά στο πλέγμα **Μέλος ομάδας** και τις εκτιμήσεις, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="f929d-160">To understand the behavior on the **Team Member** grid and the estimates, complete the following steps.</span></span>

1. <span data-ttu-id="f929d-161">Στο πλέγμα **Μέλος ομάδας**, επιλέξτε τα δύο γενικά μέλη της ομάδας και, στη συνέχεια, επιλέξτε **Δημιουργία απαιτήσεων**.</span><span class="sxs-lookup"><span data-stu-id="f929d-161">On the **Team Member** grid, select the two generic team members, and then select **Generate Requirements**.</span></span> <span data-ttu-id="f929d-162">Με τον τρόπο αυτό θα δημιουργηθούν απαιτήσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="f929d-162">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="f929d-163">Επιλέξτε τη σειρά μελών ομάδας για τη **Συνεννόηση με υποψήφιο πελάτη** και, στη συνέχεια, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="f929d-163">Select the team member row for **Consulting Lead**, and then select **Book**.</span></span> <span data-ttu-id="f929d-164">Ο πίνακας χρονοδιαγράμματος ανοίγει με μια λίστα πόρων.</span><span class="sxs-lookup"><span data-stu-id="f929d-164">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="f929d-165">Επιλέξτε έναν πόρο και, στη συνέχεια, επιλέξτε **Κράτηση** για να δεσμεύεσετε τον πόρο σε αυτήν την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="f929d-165">Select a resource and then select **Book** to book the resource to that requirement.</span></span>
3. <span data-ttu-id="f929d-166">Επιλέξτε τη σειρά μελών ομάδας για τον **Τεχνικό δικτύου** και, στη συνέχεια, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="f929d-166">Select the team member row for **Network Technician**, and then select **Book**.</span></span> <span data-ttu-id="f929d-167">Ο πίνακας χρονοδιαγράμματος ανοίγει με μια λίστα πόρων.</span><span class="sxs-lookup"><span data-stu-id="f929d-167">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="f929d-168">Επιλέξτε τον ίδιο πόρο όπως παραπάνω και, στη συνέχεια, επιλέξτε **Κράτηση** για να δεσμεύεσετε τον πόρο σε αυτήν την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="f929d-168">Select the same resource as above and then select **Book** to book the resource to that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="f929d-169">Πλέγμα Μέλους ομάδας</span><span class="sxs-lookup"><span data-stu-id="f929d-169">Team Member grid</span></span> 

<span data-ttu-id="f929d-170">Στο πλέγμα **Μέλος ομάδας**, διαγράφονται και αντικαθίστανται οι δύο γενικές καρτέλες μελών ομάδας με μόνο έναν πόρο.</span><span class="sxs-lookup"><span data-stu-id="f929d-170">On the **Team Member** grid, the two generic team member records are deleted and replaced with only one resource.</span></span> <span data-ttu-id="f929d-171">Υπάρχει ένα σύνολο τιμών για αυτόν τον πόρο, οι οποίες είναι ένα προεπιλεγμένο σύνολο τιμών για τον **Ρόλο** και την **Οργανωτική μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="f929d-171">There is one set of values for that resource, which are a default set of values for **Role** and **Organizational Unit**.</span></span>

<span data-ttu-id="f929d-172">Όταν αναπτύξετε τη γραμμή για αυτήν την καρτέλα μέλους ομάδας, μπορείτε να δείτε διακριτές αναθέσεις στην καρτέλα μέλους ομάδας και για τις δύο εργασίες.</span><span class="sxs-lookup"><span data-stu-id="f929d-172">When you expand the row for that team member record, you can see distinct assignments on the team member record for both tasks.</span></span> <span data-ttu-id="f929d-173">Κάθε γραμμή ανάθεσης έχει συγκεκριμένες τιμές εργασιών για τον **Ρόλο** και την **Οργανωτική μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="f929d-173">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="f929d-174">Πλέγμα εκτιμήσεων</span><span class="sxs-lookup"><span data-stu-id="f929d-174">Estimates grid</span></span> 

<span data-ttu-id="f929d-175">Στο πλέγμα **Εκτιμήσεις**, και οι δύο αναθέσεις για τον ίδιο πόρο τιμολογούνται διαφορετικά.</span><span class="sxs-lookup"><span data-stu-id="f929d-175">On the **Estimates** grid, both assignments for the same resource are priced differently.</span></span> <span data-ttu-id="f929d-176">Η ανάθεση για τον πόρο στην **Εργασία Α** διατιμάται με χρήση της τιμής του χαρακτηριστικού **Ρόλος** της **Συνεννόησης με υποψήφιο πελάτη**.</span><span class="sxs-lookup"><span data-stu-id="f929d-176">The assignment for the resource on **Task A** is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="f929d-177">Η ανάθεση για τον ίδιο πόρο στην **Εργασία Β** διατιμάται με χρήση της τιμής του χαρακτηριστικού **Ρόλος** του **Τεχνικού δικτύου**.</span><span class="sxs-lookup"><span data-stu-id="f929d-177">The assignment for the same resource on **Task B** is priced using the **Role** attribute value of **Network Technician**.</span></span>