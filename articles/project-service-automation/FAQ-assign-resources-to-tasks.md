---
title: Ανάθεση πόρου σε εργασία
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ανάθεσης πόρων σε εργασίες.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.prod: Project Service
ms.technology: Dynamics 365 Project Service Automation 3.x
ms.assetid: 3ea9516c-0276-4e30-b308-f792f64d608b
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 509f7a4464b2e810900b31a78219ba696192a18b
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751697"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="d3b4f-103">Ανάθεση πόρου σε εργασία</span><span class="sxs-lookup"><span data-stu-id="d3b4f-103">Assign a resource to a task</span></span>

<span data-ttu-id="d3b4f-104">Υπάρχουν τρεις τρόποι με τους οποίους μπορείτε να αναθέσετε έναν πόρο σε μια εργασία στο Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="d3b4f-105">Κάντε κράτηση ενός πόρου ως μέλος της ομάδας και, στη συνέχεια, εκχωρήστε τον σε μια εργασία</span><span class="sxs-lookup"><span data-stu-id="d3b4f-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="d3b4f-106">Μπορείτε να προσθέσετε έναν πόρο στην ομάδα έργου και έπειτα να αναθέσετε τον πόρο σε εργασίες στο χρονοδιάγραμμα έργου.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="d3b4f-107">Στην καρτέλα **Μέλος ομάδας**, προσθέστε ένα νέο μέλος ομάδας επιλέγοντας **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="d3b4f-108">Ανοίγει ο πίνακας **Γρήγορη δημιουργία μέλους ομάδας** όπου μπορείτε να επιλέξετε το όνομα του πόρου με δυνατότητα κράτησης και να ορίσετε έναν ρόλο.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="d3b4f-109">Επιλέξτε μία από τις ακόλουθες μεθόδους ανάθεσης για την κράτηση του πόρου:</span><span class="sxs-lookup"><span data-stu-id="d3b4f-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="d3b4f-110">Η **Πλήρης παραγωγική ικανότητα** κάνει κράτηση της πλήρους παραγωγικής ικανότητας του πόρου για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="d3b4f-111">Η **Ποσοστιαία παραγωγική ικανότητα** κάνει κράτηση του πόρου για ένα ποσοστό της παραγωγικής του ικανότητας για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="d3b4f-112">Η **Κατά ώρες - Ομοιόμορφη κατανομή** κάνει κράτηση του πόρου για έναν συγκεκριμένο αριθμό ωρών, με ομοιόμορφη διανομή ανά ημέρα για τις καθορισμένες από και έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="d3b4f-113">Η **Κατά ώρες - Φόρτωση προσκηνίου** κάνει κράτηση του πόρου για έναν συγκεκριμένο αριθμό ωρών, με φόρτωση προσκηνίου ανά ώρες της ημέρας για τις καθορισμένες από/έως ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="d3b4f-114">Η επιλογή **Καμία** προσθέτει τον πόρο στην ομάδα, αλλά δεν δημιουργεί κρατήσεις που καλύπτουν την παραγωγική του ικανότητα.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="d3b4f-115">Στο πλέγμα **Χρονοδιάγραμμα** για την εργασία, επιλέξτε το εικονίδιο **Πόρος** στο κελί πόρων και μετά κάτω από τα **Μέλη ομάδας** επιλέξτε το μέλος της ομάδας που μόλις προσθέσατε.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="d3b4f-116">Σημειώστε ότι στην καρτέλα **Μέλος ομάδας** και στην καρτέλα **Εναρμόνιση** ο πόρος δείχνει τις ώρες που έχουν κρατηθεί και τις ώρες που έχουν ανατεθεί.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="d3b4f-117">Οι ώρες πρέπει να είναι ίδιες αλλά δεν χρειάζεται διότι οι κρατήσεις και οι αναθέσεις δεν συνδέονται στενά.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="d3b4f-118">Η καρτέλα **Εναρμόνιση** παρέχει λεπτομέρειες όταν διαφέρουν όπως όταν αναθέτετε έναν πόρο σε περισσότερες ώρες από αυτές που έχει κρατηθεί.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="d3b4f-119">Αν χρειάζεται, μπορείτε να διορθώσετε τις πληροφορίες επεκτείνοντας τις κρατήσεις του πόρου ή να αλλάξετε την ανάθεση.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="d3b4f-120">Δημιουργία γενικού μέλους ομάδας μέσω ανάθεσης εργασίας</span><span class="sxs-lookup"><span data-stu-id="d3b4f-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="d3b4f-121">Όταν δημιουργείτε ένα γενικό μέλος ομάδας μέσω ανάθεσης εργασίας, δημιουργήστε ένα σύμβολο κράτησης θέσης ή έναν γενικό πόρο που περιγράφει τα χαρακτηριστικά του πόρου με όνομα ο οποίος θέλετε τελικά να επεξεργαστεί τις εργασίες.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="d3b4f-122">Στη συνέχεια, δημιουργείτε μια απαίτηση (ή υποβάλετε μια αίτηση χρησιμοποιώντας την απαίτηση) που χρησιμοποιείται για την αναζήτηση και την κράτηση του πόρου με όνομα.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="d3b4f-123">Στο πλέγμα **Χρονοδιάγραμμα** για την εργασία, επιλέξτε το εικονίδιο **Πόρος** στο κελί πόρων.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="d3b4f-124">Πληκτρολογήστε ένα όνομα που θα χρησιμοποιηθεί ως το όνομα του πόρου συμβόλου κράτησης θέσης.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="d3b4f-125">Για παράδειγμα, "Διαχειριστής προγραμμάτων".</span><span class="sxs-lookup"><span data-stu-id="d3b4f-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="d3b4f-126">Στο πεδίο **Δημιουργία** και **Γρήγορη δημιουργία μέλους ομάδας έργου** ορίστε ρόλο για το γενικό πόρο.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="d3b4f-127">Μπορείτε να συνεχίσετε να αναθέτετε εργασίες σε αυτόν τον πόρο κράτησης θέσης, επιλέγοντας τον πόρο στον **Επιλογέα πόρου** για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="d3b4f-128">Εμφανίζονται κάτω από τα **μέλη της ομάδας**.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="d3b4f-129">Όταν ολοκληρώσετε την εργασία ανάθεσης πόρου γενικής χρήσης, επιλέξτε τον γενικό πόρο στην καρτέλα **Ομάδα** και επιλέξτε **Δημιουργία απαίτησης** για τη δημιουργία μιας απαίτησης πόρου για το γενικό πόρο.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="d3b4f-130">Επιλέξτε **Κράτηση** για το γενικό πόρο.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="d3b4f-131">Μπορείτε να χρησιμοποιήσετε τον πίνακα χρονοδιαγράμματος για τον εντοπισμό και την κράτηση ενός πόρου πραγματικού.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="d3b4f-132">Επίσης, μπορείτε να υποβάλετε την απαίτηση για πραγματοποίηση από έναν διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="d3b4f-133">Όταν διεκπεραιώνεται ένας γενικός πόρος με έναν πόρο με όνομα, ο γενικός πόρος καταργείται από την ομάδα και οι αναθέσεις εργασιών του γενικού πόρου εκχωρούνται στον πόρο με όνομα που ικανοποιούσε την απαίτηση πόρου του γενικού πόρου.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="d3b4f-134">Ανάθεση πόρου με όνομα από τη λίστα όλων των πόρων με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="d3b4f-135">Μπορείτε να χρησιμοποιήσετε το πλαίσιο αναζήτησης στον **επιλογέα πόρων** για την αναζήτηση σε όλους τους πόρους με δυνατότητα κράτησης και να τους αναθέσετε σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="d3b4f-136">Οι πόροι που έχουν ανατεθεί με αυτόν τον τρόπο προστίθενται στην ομάδα χωρίς καμία κράτηση.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="d3b4f-137">Αυτό είναι παρόμοιο με την προσθήκη ενός μέλους ομάδας και την επιλογή Καμία ως μέθοδο ανάθεσης.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="d3b4f-138">Ο πόρος εμφανίζεται στις καρτέλες **Ομάδα** και **Εναρμόνιση** ως πόροι με μόνο αναθέσεις και με έλλειμμα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="d3b4f-139">Κάντε κράτηση εάν θέλετε να χρησιμοποιήσετε τη διαθεσιμότητά τους.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="d3b4f-140">Στο πλέγμα **Χρονοδιάγραμμα** για την εργασία, επιλέξτε το εικονίδιο **Πόρος** στο κελί πόρων.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="d3b4f-141">Αρχίστε να πληκτρολογείτε ένα όνομα.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-141">Start typing a name.</span></span> <span data-ttu-id="d3b4f-142">Τα αποτελέσματα αναζήτησης για το όνομα εμφανίζονται στον **Επιλογέα πόρων** κάτω από το στοιχείο **Άλλοι πόροι**.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="d3b4f-143">Επιλέξτε τον πόρο που θέλετε να αναθέσετε στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="d3b4f-143">Select the resource that you want to assign to the task.</span></span>

