---
title: Δημιουργία κράτησης έργου από τον πίνακα χρονοδιαγράμματος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας μιας κράτησης έργου από τον πίνακα χρονοδιαγράμματος.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: 7032af78168c742ac64cb2a7174cabcbda579ff8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146528"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="ba7b6-103">Δημιουργία κράτησης έργου από τον πίνακα χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="ba7b6-103">Create a project booking from the Schedule board</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ba7b6-104">Μπορείτε να κράτηση ενός πόρου σε ένα έργο είτε απευθείας από την καρτέλα **Ομάδα** του έργου ή δημιουργώντας μια απαίτηση πόρου από μια ανάθεση μελών ομάδας γενικής χρήσης και, στη συνέχεια, τηρώντας τις απαιτήσεις που έχουν δημιουργηθεί με ένα μέλος της ομάδας έργου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="ba7b6-105">Μπορείτε επίσης να κάνετε κράτηση πόρων σε ένα έργο απευθείας από τον πίνακα χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="ba7b6-106">Υπάρχουν τρεις τρόποι για να το κάνετε αυτό:</span><span class="sxs-lookup"><span data-stu-id="ba7b6-106">There are three ways to do this:</span></span>

- <span data-ttu-id="ba7b6-107">**Κράτηση από μια απαίτηση πόρων που δημιουργήθηκε**: μπορείτε να δημιουργήσετε μια απαίτηση πόρου μετά τη δημιουργία ενός γενικού πόρου και την ανάθεση εργασιών σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="ba7b6-108">**Κράτηση από την κύρια απαίτηση** : οι κύριες απαιτήσεις εμφανίζονται στον πίνακα χρονοδιαγράμματος στην καρτέλα **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="ba7b6-109">**Κράτηση από μια νέα απαίτηση πόρων** : μπορείτε να δημιουργήσετε μια απαίτηση πόρου από την αρχή και να τη συσχετίσετε με ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="ba7b6-110">Στον πίνακα χρονοδιαγράμματος, οι απαιτήσεις πόρων εμφανίζονται στην καρτέλα **Ανοιχτές απαιτήσεις**.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="ba7b6-111">Κράτηση από μια απαίτηση πόρων που δημιουργήθηκε</span><span class="sxs-lookup"><span data-stu-id="ba7b6-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="ba7b6-112">Μπορείτε να δημιουργήσετε έναν γενικό πόρο και να αναθέσετε σε αυτόν μια εργασία ή πολλές εργασίες ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="ba7b6-113">Μπορείτε να δημιουργήσετε μια απαίτηση πόρου για το γενικό μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="ba7b6-114">Στον πίνακα χρονοδιαγράμματος, αυτός ο πόρος θα εμφανίζεται στην καρτέλα **Ανοιχτές απαιτήσεις**. Ίσως χρειαστεί να χρησιμοποιήσετε φίλτρα στήλης στο πλέγμα, εάν έχετε πολλές ανοιχτές απαιτήσεις.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="ba7b6-115">![Άνοιγμα καρτέλας απαιτήσεων στον πίνακα χροδοδιαγράμματος](media/FAQ-Project-Booking-Schedule-Board-1.png "Στιγμιότυπο οθόνης του πίνακα κρατήσεων και αναθέσεων")</span><span class="sxs-lookup"><span data-stu-id="ba7b6-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="ba7b6-116">Επιλέξτε την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-116">Select the requirement.</span></span> <span data-ttu-id="ba7b6-117">Η καρτέλα **Εύρεση διαθεσιμότητας** εμφανίζεται στο επάνω μέρος της επιλεγμένης γραμμής.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="ba7b6-118">Επιλέγοντας την καρτέλα ξεκινά η λειτουργία του Βοηθού χρονοδιαγράμματος του πίνακα χρονοδιαγράμματος και φιλτράρονται οι διαθέσιμοι πόροι που θα ικανοποιούν τις απαιτήσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="ba7b6-119">Από εκεί μπορείτε να κάνετε κράτηση ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="ba7b6-120">Μπορείτε επίσης να σύρετε και να αποθέστε την επιλεγμένη γραμμή από το κάτω μέρος του πίνακα χρονοδιαγράμματος σε ένα κελί πόρου στο πλέγμα παραπάνω.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="ba7b6-121">Αν την αφήσετε, ανοίγει ο πίνακας **Δημιουργία κράτησης πόρων** στα δεξιά.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="ba7b6-122">Αν επιλέξετε **Κράτηση** γίνεται κράτηση του πόρου στην ομάδα του έργου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-122">Selecting **Book** books the resource onto the project team.</span></span>

![Πίνακας δημιουργίας κράτησης πόρου](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="ba7b6-124">Κράτηση από την κύρια απαίτηση</span><span class="sxs-lookup"><span data-stu-id="ba7b6-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="ba7b6-125">Η δημιουργία ενός έργου στο Project Service δημιουργεί αυτόματα μια απαίτηση πόρων που ονομάζεται βασική απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="ba7b6-126">Αυτή είναι μια κενή απαίτηση που χρησιμοποιείται για τη γρήγορη κράτηση πόρων με τον πίνακα χρονοδιαγράμματος χωρίς δημιουργία απαίτησης ή δημιουργία από την αρχή.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="ba7b6-127">Επειδή η απαίτηση είναι κενή, πρέπει να καθορίσετε τις ημερομηνίες, καθώς και τη μέθοδο εκχώρησης και τις ώρες, εάν υπάρχουν.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="ba7b6-128">Για να κάνετε κράτηση ενός πόρου με τη βασική απαίτηση, στον πίνακα χρονοδιαγράμματος επιλέξτε την καρτέλα **Έργο**. Εάν έχετε πολλά έργα, ίσως είναι ευκολότερο να χρησιμοποιήσετε τα φίλτρα στήλης στη στήλη **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="ba7b6-129">![Φίλτρα στήλης στον πίνακα χρονοδιαγράμματος](media/FAQ-Project-Booking-Schedule-Board-2.png "Στιγμιότυπο οθόνης του πίνακα κρατήσεων και αναθέσεων")</span><span class="sxs-lookup"><span data-stu-id="ba7b6-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="ba7b6-130">Επιλέξτε την απαίτηση που έχει μόνο το όνομα του έργου ως όνομα και έχει διάρκεια μηδέν (0).</span><span class="sxs-lookup"><span data-stu-id="ba7b6-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="ba7b6-131">Επιλέξτε την καρτέλα **Εύρεση διαθεσιμότητας** που εμφανίζεται στη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="ba7b6-132">Αυτό φέρνει τον πίνακα χρονοδιαγράμματος στη λειτουργία βοηθού χρονοδιαγράμματος και δείχνει τους διαθέσιμους πόρους, που μπορούν να κρατηθούν στο έργο.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="ba7b6-133">Επειδή η **κύρια απαίτηση** είναι μια απαίτηση κενή με διάρκεια μηδέν (0), θα πρέπει να ορίσετε τη διάρκεια στον πίνακα **Δημιουργία κράτησης πόρων** όταν επιλέγετε και κάνετε κράτηση ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="ba7b6-134">Επίσης, μπορείτε να επιλέξετε τη **βασική απαίτηση έργου** στο κάτω μέρος του πίνακα χρονοδιαγράμματος και να τη σύρετε και να την αποθέστε σε έναν πόρο για να συνεχίσετε με την κράτηση του.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="ba7b6-135">Επειδή η **κύρια απαίτηση** είναι μια απαίτηση κενή με διάρκεια μηδέν (0), θα πρέπει να ορίσετε τη διάρκεια στον πίνακα **Δημιουργία κράτησης πόρων** όταν επιλέγετε και κάνετε κράτηση ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="ba7b6-136">Όταν κάνετε κράτηση ενός πόρου μέσω της **βασικής απαίτησης** στον πίνακα χρονοδιαγράμματος, μπορείτε να τον προσθέσετε στην ομάδα έργου χωρίς αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="ba7b6-137">Κράτηση από μια νέα απαίτηση πόρων</span><span class="sxs-lookup"><span data-stu-id="ba7b6-137">Book from a new resource requirement</span></span>
<span data-ttu-id="ba7b6-138">Ολοκληρώστε τα παρακάτω βήματα για να κάνετε κράτηση από μια νέα απαίτηση πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="ba7b6-139">Μεταβείτε στις **Απαιτήσεις πόρων** και επιλέξτε **Νέα** για τη δημιουργία μιας νέας απαίτησης πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="ba7b6-140">Στην καρτέλα **Έργο**, επιλέξτε ένα έργο για να συσχετίσετε την απαίτηση με το έργο.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="ba7b6-141">Στον πίνακα χρονοδιαγράμματος, αυτή η νέα απαίτηση εμφανίζεται ως **ανοιχτή απαίτηση** που μπορείτε να ικανοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="ba7b6-142">Η κράτηση ενός πόρου τον προσθέτει στην ομάδα του έργου.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="ba7b6-143">Τώρα που έχει γίνει κράτηση του πόρου, πρέπει να αναθέσετε τις εργασίες με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="ba7b6-143">Now that the resource is booked, you must assign tasks manually.</span></span>

