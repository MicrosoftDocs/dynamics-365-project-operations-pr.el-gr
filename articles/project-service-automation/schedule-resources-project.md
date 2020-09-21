---
title: Προγραμματισμός πόρων για ένα έργο
description: Πώς γίνεται ο προγραμματισμός πόρων για ένα έργο στο Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 4935567d-9318-4f7c-9c02-c584a78b7841
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: d9767e324b3caec4b5f9723347537dbe97ea34fb
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751669"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="57269-103">Προγραμματισμός πόρων για ένα έργο (Project Service)</span><span class="sxs-lookup"><span data-stu-id="57269-103">Schedule resources for a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="57269-104">Μπορείτε να ελέγξετε τη διαθεσιμότητα των πόρων, για να έχετε μια συνολική εικόνα του κατά πόσο κατειλημμένοι είναι οι πόροι σας, ή μπορείτε να φιλτράρετε την προβολή ανάλογα με τις δεξιότητες, την ομάδα, τη θέση και άλλες επιλογές.</span><span class="sxs-lookup"><span data-stu-id="57269-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="57269-105">Ο πίνακας χρονοδιαγράμματος εμφανίζει λίστα με τους πόρους και τη διαθεσιμότητά τους.</span><span class="sxs-lookup"><span data-stu-id="57269-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="57269-106">Επιλέξτε έναν τρόπο λειτουργίας προβολής για να εμφανίσετε τη διαθεσιμότητα ανά **Ώρες**, **Ημέρα**, **Εβδομάδα** ή **Μήνα**.</span><span class="sxs-lookup"><span data-stu-id="57269-106">Select a view mode to show availability by **Hours**, **Day**, **Week**, or **Month**.</span></span>  
  
<span data-ttu-id="57269-107">Για να χρησιμοποιήσετε τον πίνακα χρονοδιαγράμματος, είναι σημαντικό να ρυθμίσετε τις παραμέτρους του.</span><span class="sxs-lookup"><span data-stu-id="57269-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="57269-108">Για περισσότερες πληροφορίες, δείτε [Ρύθμιση παραμέτρων του πίνακα χρονοδιαγράμματος (Field Service ή Project Service Automation)](../field-service/configure-schedule-board.md).</span><span class="sxs-lookup"><span data-stu-id="57269-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](../field-service/configure-schedule-board.md).</span></span>
  
<span data-ttu-id="57269-109">Εάν χρησιμοποιείτε μια παλαιότερη έκδοση, για διαθεσιμότητα πόρου, ανατρέξτε στο θέμα [Προβολή διαθεσιμότητας πόρου](../project-service/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="57269-109">If you are using an older version, for resource availability, see [View resource availability](../project-service/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="57269-110">Για να χρησιμοποιήσετε τη λειτουργία κράτησης πίνακα χρονοδιαγράμματος, γεωγραφικής κωδικοποίησης και υπηρεσιών τοποθεσίας, πρέπει να ενεργοποιήσετε τους χάρτες.</span><span class="sxs-lookup"><span data-stu-id="57269-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="57269-111">Σο κύριο μενού, επιλέξτε **Προγραμματισμός πόρων** > **Διαχείριση**.</span><span class="sxs-lookup"><span data-stu-id="57269-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="57269-112">Επιλέξτε **Παράμετροι προγραμματισμού**.</span><span class="sxs-lookup"><span data-stu-id="57269-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="57269-113">Ανοίξτε την καρτέλα και κάντε κύλιση προς τα κάτω στην ενότητα **Resource Scheduling Optimization**.</span><span class="sxs-lookup"><span data-stu-id="57269-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="57269-114">Στο πεδίο **Σύνδεση με χάρτες**, επιλέξτε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="57269-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="57269-115">Αποδεχτείτε τους όρους και αποθηκεύστε την καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="57269-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="57269-116">Στο κύριο μενού, επιλέξτε **Project Service** > **Πίνακας χρονοδιαγράμματος**.</span><span class="sxs-lookup"><span data-stu-id="57269-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="57269-117">Εδώ, υπάρχουν διάφοροι τρόποι για να προγραμματίσετε μη αυτόματα μια απαίτηση κράτησης.</span><span class="sxs-lookup"><span data-stu-id="57269-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="57269-118">Επιλέξτε τη μέθοδο που σας εξυπηρετεί.</span><span class="sxs-lookup"><span data-stu-id="57269-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="57269-119">Βρείτε διαθέσιμους πόρους</span><span class="sxs-lookup"><span data-stu-id="57269-119">Find available resources</span></span>

1.  <span data-ttu-id="57269-120">Από τη λίστα **Απαίτηση κράτησης**, κάντε δεξί κλικ σε μια μη προγραμματισμένη κράτηση και επιλέξτε ένα από τα εξής:</span><span class="sxs-lookup"><span data-stu-id="57269-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="57269-121">Επιλέξτε **Εύρεση διαθεσιμότητας - Τρέχοντες πόροι**για την εύρεση διαθέσιμου πόρου από τη λίστα στον πίνακα χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="57269-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="57269-122">Επιλέξτε **Εύρεση διαθεσιμότητας - Όλοι οι πόροι**για την εύρεση ενός διαθέσιμου πόρου από τους πόρους στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="57269-122">Choose **Find availability - All Resources**, to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="57269-123">Όταν το κάνετε αυτό, τα φίλτρα θα εμφανίσουν επιλογές για την απαίτηση της επιλεγμένης κράτησης.</span><span class="sxs-lookup"><span data-stu-id="57269-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="57269-124">Όταν δείτε μια διαθέσιμη υποδιαίρεση, κάντε δεξί κλικ στη χρονική υποδιαίρεση στον πίνακα χρονοδιαγράμματος και επιλέξτε **Κράτηση εδώ**.</span><span class="sxs-lookup"><span data-stu-id="57269-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="57269-125">Εναλλακτικά, σύρετε και αποθέστε την απαίτηση κράτησης στη διαθέσιμη χρονική υποδιαίρεση.</span><span class="sxs-lookup"><span data-stu-id="57269-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="57269-126">Κάντε κράτηση ενός πόρου χρησιμοποιώντας την ημερήσια προβολή και δείτε για ποιον πόρο δεν έχουν γίνει πολλές κρατήσεις</span><span class="sxs-lookup"><span data-stu-id="57269-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="57269-127">Στον πίνακα χρονοδιαγράμματος, επιλέξτε **Λειτουργία προβολής** και επιλέξτε **Ημέρες**.</span><span class="sxs-lookup"><span data-stu-id="57269-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="57269-128">Αυτό εμφανίζει μια προβολή πλέγματος των ωρών για τις οποίες έχει γίνει κράτηση ενός πόρου ανά ημέρα και των ημερών που είναι ελεύθερες.</span><span class="sxs-lookup"><span data-stu-id="57269-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="57269-129">Κάντε κλικ στο όνομα του πόρου για τον οποίο θέλετε να κάνετε κράτηση και, στη συνέχεια, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="57269-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="57269-130">Στο παράθυρο διαλόγου **Κράτηση πόρου (δημιουργία)**, επιλέξτε το έργο για το οποίο θέλετε να κάνετε κράτηση του πόρου μαζί με τη μέθοδο κράτησης και τις ώρες έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="57269-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="57269-131">Όταν είστε έτοιμοι, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="57269-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="57269-132">Προβολή στον πίνακα χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="57269-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="57269-133">Επιλέξτε μια απαίτηση μη προγραμματισμένης κράτησης για τη λίστα στο κάτω μέρος.</span><span class="sxs-lookup"><span data-stu-id="57269-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="57269-134">Σύρετε την απαίτηση κράτησης σε έναν διαθέσιμο πόρο ή σε μια διαθέσιμη χρονική περίοδο στον πίνακα χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="57269-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="57269-135">Όταν είστε έτοιμοι, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="57269-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="57269-136">Πρόσθετοι πόροι</span><span class="sxs-lookup"><span data-stu-id="57269-136">Additional resources</span></span>  
 [<span data-ttu-id="57269-137">Οδηγός υπεύθυνου πόρων</span><span class="sxs-lookup"><span data-stu-id="57269-137">Resource manager guide</span></span>](../project-service/resource-manager-guide.md)
