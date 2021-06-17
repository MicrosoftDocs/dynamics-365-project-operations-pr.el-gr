---
title: Πώς μπορώ να αναθέσω έναν πόρο με δυνατότητα κράτησης σε μια εργασία από την εφαρμογή web
description: Μια επισκόπηση των τρόπων με τους οποίους μπορείτε να αναθέσετε πόρους με δυνατότητα κράτησης.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32a04ddef901515cd77262b5ae6be2458cb6b00c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993294"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="67d38-103">Πώς μπορώ να αναθέσω έναν πόρο με δυνατότητα κράτησης σε μια εργασία από την εφαρμογή web (εφαρμογή Project Service v2.x);</span><span class="sxs-lookup"><span data-stu-id="67d38-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="67d38-104">Υπάρχουν δύο τρόποι με τους οποίους μπορείτε να αναθέσετε έναν πόρο σε μια εργασία στο Project Service.</span><span class="sxs-lookup"><span data-stu-id="67d38-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="67d38-105">Μπορείτε να κάνετε κράτηση ενός πόρου ως μέλος της ομάδας και, στη συνέχεια, να του αναθέσετε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="67d38-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="67d38-106">Εναλλακτικά, μπορείτε να δημιουργήσετε ένα γενικό μέλος ομάδας μέσω εκχώρησης ρόλου σε εργασίες, να δημιουργήσετε μια ομάδα, και, στη συνέχεια, να ικανοποιήσετε τις απαιτήσεις υποστήριξης με έναν πόρο με όνομα.</span><span class="sxs-lookup"><span data-stu-id="67d38-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="67d38-107">Σημειώστε ότι, εάν θέλετε να αναθέσετε σε έναν πόρο με δυνατότητα κράτησης μια εργασία, το μέλος της ομάδας του πόρου με δυνατότητα κράτησης πρέπει να διαθέτει αρκετές κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="67d38-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="67d38-108">Η κατάσταση της κράτησης πρέπει να είναι Τύπος δέσμευσης οριστική κράτηση και η κατάσταση Δεσμευμένος.</span><span class="sxs-lookup"><span data-stu-id="67d38-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="67d38-109">Εάν δεν υπάρχουν αρκετές κρατήσεις για τον πόρο, το Project Service καταργεί την ανάθεση και εμφανίζει το ακόλουθο μήνυμα σφάλματος:</span><span class="sxs-lookup"><span data-stu-id="67d38-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="67d38-110">*Δεν είναι δυνατή η ανάθεση πόρου σε εργασία - Οι παρακάτω πόροι δεν έχουν αρκετές ώρες κράτησης σε σχέση με ένα έργο*</span><span class="sxs-lookup"><span data-stu-id="67d38-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="67d38-111">Κάντε κράτηση ενός πόρου ως μέλος της ομάδας και, στη συνέχεια, εκχωρήστε τον σε μια εργασία</span><span class="sxs-lookup"><span data-stu-id="67d38-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="67d38-112">Έτσι μπορείτε να προσθέσετε έναν πόρο στην ομάδα έργου και έπειτα να αναθέσετε στον πόρο εργασίες στο χρονοδιάγραμμα έργου.</span><span class="sxs-lookup"><span data-stu-id="67d38-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="67d38-113">Πώς να το κάνετε:</span><span class="sxs-lookup"><span data-stu-id="67d38-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="67d38-114">Στο πλέγμα μελών ομάδας, προσθέστε ένα νέο μέλος ομάδας επιλέγοντας **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="67d38-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="67d38-115">Στην οθόνη γρήγορης δημιουργίας μέλους ομάδας, επιλέξτε το όνομα του πόρου με δυνατότητα κράτησης και να ορίσετε έναν ρόλο.</span><span class="sxs-lookup"><span data-stu-id="67d38-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="67d38-116">Επιλέξτε ημερομηνίες **Από** και **Έως**.</span><span class="sxs-lookup"><span data-stu-id="67d38-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="67d38-117">![Στιγμιότυπο οθόνης προσθήκης μέλους ομάδας](media/FAQ-Resources-to-Tasks2-1.png "Στιγμιότυπο οθόνης προσθήκης μέλους ομάδας")</span><span class="sxs-lookup"><span data-stu-id="67d38-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="67d38-118">Επιλέξτε μία από τις ακόλουθες μεθόδους ανάθεσης για την κράτηση του πόρου:</span><span class="sxs-lookup"><span data-stu-id="67d38-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="67d38-119">Η **Πλήρης παραγωγική ικανότητα** κάνει κράτηση της πλήρους παραγωγικής ικανότητας του πόρου για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="67d38-120">Η **Ποσοστιαία παραγωγική ικανότητα** κάνει κράτηση του πόρου για ένα ποσοστό της παραγωγικής του ικανότητας για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="67d38-121">Η **Κατά ώρες - Ομοιόμορφη κατανομή** κάνει κράτηση του πόρου για έναν συγκεκριμένο αριθμό ωρών, με ομοιόμορφη διανομή ανά ημέρα για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="67d38-122">Η **Κατά ώρες - Φόρτωση προσκηνίου** κάνει κράτηση του πόρου για έναν συγκεκριμένο αριθμό ωρών, με φόρτωση προσκηνίου ανά ώρες της ημέρας για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="67d38-123">Μην επιλέξετε **Καμία** διότι αυτή η μέθοδος προσθέτει τον πόρο ως ένα μέλος της ομάδας αλλά δεν δημιουργεί κρατήσεις που καλύπτουν την παραγωγική ικανότητα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="67d38-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="67d38-124">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="67d38-124">Select **Save**.</span></span>

    <span data-ttu-id="67d38-125">Σημειώστε ότι οι ώρες κράτησης πρέπει να είναι αρκετές ώστε να καλύπτουν τις ώρες προσπάθειας και το εύρος ημερομηνιών των εργασιών τις οποίες αναθέτετε σε αυτόν τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="67d38-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="67d38-126">Εάν δεν είναι ευθυγραμμισμένες, δεν μπορείτε να αντιστοιχίσετε τον πόρο στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="67d38-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="67d38-127">Στη δομή ανάλυσης εργασίας (WBS) για την εργασία, κάντε κλικ στο αναπτυσσόμενο κελί πόρων.</span><span class="sxs-lookup"><span data-stu-id="67d38-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="67d38-128">Τότε:</span><span class="sxs-lookup"><span data-stu-id="67d38-128">Then:</span></span> 

    1. <span data-ttu-id="67d38-129">Επιλέξτε **Προσθήκη**.</span><span class="sxs-lookup"><span data-stu-id="67d38-129">Select **Add**.</span></span>
    2. <span data-ttu-id="67d38-130">Επιλέξτε την αναπτυσσόμενη λίστα στην περιοχή **Πόροι** και επιλέξτε το μέλος της ομάδας που προσθέσατε παραπάνω.</span><span class="sxs-lookup"><span data-stu-id="67d38-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="67d38-131">Επιλέξτε **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="67d38-131">Select **OK**.</span></span> <span data-ttu-id="67d38-132">Η εργασία έχει πλέον ανατεθεί στο μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="67d38-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="67d38-133">![Στιγμιότυπο οθόνης προσθήκης πόρων με WBS](media/FAQ-Resources-to-Tasks2-2.png "Στιγμιότυπο οθόνης προσθήκης πόρων με WBS")</span><span class="sxs-lookup"><span data-stu-id="67d38-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="67d38-134">Στο πλέγμα μελών ομάδας, θα δείτε τον συνολικό αριθμό των ωρών του πόρου κάτω από τις Αντιστοιχισμένες ώρες.</span><span class="sxs-lookup"><span data-stu-id="67d38-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="67d38-135">Ισούνται ή είναι λιγότερες από τις ώρες κράτησης για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="67d38-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="67d38-136">![Στιγμιότυπο οθόνης ανατεθειμένων ωρών για έναν πόρο](media/FAQ-Resources-to-Tasks2-3.png "Στιγμιότυπο οθόνης ανατεθειμένων ωρών για έναν πόρο")</span><span class="sxs-lookup"><span data-stu-id="67d38-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="67d38-137">Εάν η εργασία που επιχειρείτε να αναθέσετε στον πόρο ξεκινά μετά από την ημερομηνία λήξης των κρατήσεων πόρων, ο πόρος δεν θα εμφανιστεί στην αναπτυσσόμενη λίστα.</span><span class="sxs-lookup"><span data-stu-id="67d38-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="67d38-138">Σημειώστε ότι μπορείτε να αναθέσετε έναν πόρο σε περισσότερες ώρες από αυτές για τις οποίες έχει γίνει κράτηση αν ο πόρος διαθέτει κάποια υπολειπόμενη μη εκχωρημένη παραγωγική ικανότητα.</span><span class="sxs-lookup"><span data-stu-id="67d38-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="67d38-139">Σε αυτή την περίπτωση ο πόρος θα αντιστοιχεί εν μέρει στις κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="67d38-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="67d38-140">Μπορείτε να δείτε αυτές τις υπόλοιπες ώρες μη εκχωρημένης εργασίας με την προσθήκη της στήλης Ώρες χωρίς στελέχωση στη δομή ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="67d38-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="67d38-141">Εάν οι πόροι ανατίθενται στις ώρες κράτησης (οι ώρες κράτησης ισούνται με τις ώρες που έχουν ανατεθεί), θα δείτε το ακόλουθο μήνυμα σφάλματος όταν προσπαθείτε να αντιστοιχίσετε περισσότερες εργασίες:</span><span class="sxs-lookup"><span data-stu-id="67d38-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="67d38-142">*Δεν είναι δυνατή η ανάθεση πόρου σε εργασία - Οι παρακάτω πόροι δεν έχουν αρκετές ώρες κράτησης σε σχέση με ένα έργο.*</span><span class="sxs-lookup"><span data-stu-id="67d38-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="67d38-143">Επιπλέον, το προεπιλεγμένο μέλος ομάδας διαχειριστή έργου που έχει προστεθεί στην ομάδα κατά τη δημιουργία του έργου προστίθεται χωρίς κρατήσεις και δεν μπορεί να αντιστοιχιστεί σε κάθε εργασία.</span><span class="sxs-lookup"><span data-stu-id="67d38-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="67d38-144">Δεν θα εμφανιστούν στην αναπτυσσόμενη λίστα πόρων για εργασίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="67d38-145">Εάν θέλετε να αναθέσετε αυτόν τον πόρο, πρέπει να τον καταργήσετε από την ομάδα και, στη συνέχεια, να τον προσθέσετε ξανά με μέθοδο εκχώρησης εκτός της Καμία.</span><span class="sxs-lookup"><span data-stu-id="67d38-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="67d38-146">Ο λόγος που προστίθενται στην ομάδα όταν το έργο δημιουργείται είναι για να έχει ένα έργο τουλάχιστον έναν υπεύθυνον έγκρισης από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="67d38-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="67d38-147">Δημιουργία γενικού μέλους ομάδας μέσω αναθέσεων ρόλων σε εργασίες</span><span class="sxs-lookup"><span data-stu-id="67d38-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="67d38-148">Αυτή η μέθοδος εξασφαλίζει ότι οι πόροι έχουν αρκετές κρατήσεις για εργασίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="67d38-149">Πρώτα δημιουργήστε ένα σύμβολο κράτησης θέσης ή έναν γενικό πόρο που περιγράφει τα χαρακτηριστικά του πόρου με όνομα ο οποίος θέλετε τελικά να επεξεργαστεί τις εργασίες δημιουργώντας μια ομάδα μετά την ανάθεση ρόλων σε εργασίες.</span><span class="sxs-lookup"><span data-stu-id="67d38-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="67d38-150">Πώς να το κάνετε:</span><span class="sxs-lookup"><span data-stu-id="67d38-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="67d38-151">Στη δομή ανάλυσης εργασίας, επιλέξτε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="67d38-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="67d38-152">Επιλέξτε το αναπτυσσόμενο εικονίδιο **Έχει ανατεθεί ρόλος** στο κελί πόρων.</span><span class="sxs-lookup"><span data-stu-id="67d38-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="67d38-153">Επιλέξτε **Ρόλος** και επιλέξτε τον ρόλο για το γενικό πόρο.</span><span class="sxs-lookup"><span data-stu-id="67d38-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="67d38-154">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="67d38-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="67d38-155">![Στιγμιότυπο οθόνης χρήσης WBS για προσθήκη πόρου](media/FAQ-Resources-to-Tasks2-4.png "Στιγμιότυπο οθόνης χρήσης WBS για προσθήκη πόρου")</span><span class="sxs-lookup"><span data-stu-id="67d38-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="67d38-156">Όταν ολοκληρώσετε την αντιστοίχιση ρόλων σε εργασίες στο WBS, επιλέξτε **Δημιουργία ομάδας έργου**.</span><span class="sxs-lookup"><span data-stu-id="67d38-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="67d38-157">Το Project Service δημιουργεί τον ελάχιστο αριθμό γενικών μελών ομάδας βάσει ρόλων, στελεχώνοντας μονάδες του οργανισμού και δημιουργώντας το ημερολόγιο έργου με τη συγκέντρωση των αναθέσεων εργασιών.</span><span class="sxs-lookup"><span data-stu-id="67d38-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="67d38-158">![Στιγμιότυπο οθόνης δημιουργίας ομάδας έργου](media/FAQ-Resources-to-Tasks2-5.png "Στιγμιότυπο οθόνης δημιουργίας ομάδας έργου")</span><span class="sxs-lookup"><span data-stu-id="67d38-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="67d38-159">Στο πλέγμα μελών ομάδας, θα δείτε πόρους γενικού τύπου με το όνομα ρόλου και της θέσης.</span><span class="sxs-lookup"><span data-stu-id="67d38-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="67d38-160">Εάν δύο πόρους απαιτούνται για ένα ρόλο για να ολοκληρώσει τις εργασίες, η δυνατότητα "Δημιουργία ομάδας" δημιουργεί δύο μέλη της ομάδας και χρησιμοποιεί το όνομα της θέσης για να τα διαχωρίσετε.</span><span class="sxs-lookup"><span data-stu-id="67d38-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="67d38-161">![Στιγμιότυπο οθόνης προσθήκης δύο γενικών πόρων](media/FAQ-Resources-to-Tasks2-6.png "Στιγμιότυπο οθόνης προσθήκης δύο γενικών πόρων")</span><span class="sxs-lookup"><span data-stu-id="67d38-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="67d38-162">Μπορείτε να ανοίξετε την απαίτηση πόρων για το γενικό μέλος της ομάδας επιλέγοντας τη σύνδεση στην περιοχή απαίτησης πόρου.</span><span class="sxs-lookup"><span data-stu-id="67d38-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="67d38-163">![Στιγμιότυπο οθόνης ανοίγματος της εφεδρικής απαίτησης πόρων](media/FAQ-Resources-to-Tasks2-7.png "Στιγμιότυπο οθόνης ανοίγματος της εφεδρικής απαίτησης πόρων")</span><span class="sxs-lookup"><span data-stu-id="67d38-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="67d38-164">Επιλέξτε **Κράτηση** για τον γενικό πόρο και, στη συνέχεια, μπορείτε να χρησιμοποιήσετε τον πίνακα χρονοδιαγράμματος για τον εντοπισμό και την κράτηση ενός πραγματικού πόρου.</span><span class="sxs-lookup"><span data-stu-id="67d38-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="67d38-165">Επίσης, μπορείτε να υποβάλετε την απαίτηση για πραγματοποίηση από έναν διαχειριστή πόρων επιλέγοντας **Υποβολή αιτήματος**.</span><span class="sxs-lookup"><span data-stu-id="67d38-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="67d38-166">Όταν διεκπεραιώνεται ένας γενικός πόρος με έναν πόρο με όνομα, ο γενικός πόρος καταργείται από την ομάδα και οι αναθέσεις εργασιών του γενικού πόρου εκχωρούνται στον πόρο με όνομα που ικανοποιούσε την απαίτηση πόρου του γενικού πόρου.</span><span class="sxs-lookup"><span data-stu-id="67d38-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]