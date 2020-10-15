---
title: Διαχείριση ζωνών ώρας
description: Όταν δημιουργείται ένα έργο, η ζώνη ώρας του βασίζεται στη ζώνη ώρας που καθορίζεται στο πρότυπο ωρών εργασίας που εφαρμόζεται.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961870"
---
# <a name="manage-time-zones"></a><span data-ttu-id="df582-103">Διαχείριση ζωνών ώρας</span><span class="sxs-lookup"><span data-stu-id="df582-103">Manage time zones</span></span>

<span data-ttu-id="df582-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="df582-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="df582-105">Έργα</span><span class="sxs-lookup"><span data-stu-id="df582-105">Projects</span></span>

<span data-ttu-id="df582-106">Όταν δημιουργείται ένα έργο, η ζώνη ώρας του βασίζεται στη ζώνη ώρας που καθορίζεται στο πρότυπο ωρών εργασίας που εφαρμόζεται.</span><span class="sxs-lookup"><span data-stu-id="df582-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="df582-107">Στο **Έργο**, οι ημερομηνίες είναι πάντα σχετικές με τη ζώνη ώρας του χρήστη που είναι συνδεδεμένος σε κάθε καρτέλα, εκτός από την καρτέλα **Εργασία**. Όταν προβάλετε τη δομή ανάλυσης εργασίας, οι ημερομηνίες θα εμφανίζονται πάντα στη ζώνη ώρας του έργου.</span><span class="sxs-lookup"><span data-stu-id="df582-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="df582-108">Εργασίες</span><span class="sxs-lookup"><span data-stu-id="df582-108">Tasks</span></span>

<span data-ttu-id="df582-109">Όταν δημιουργείται μια εργασία, ο χρόνος έναρξης, η ώρα λήξης και οι ώρες/ημέρα ελέγχονται από τις ώρες εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="df582-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="df582-110">Για παράδειγμα, εάν μια εργασία δημιουργηθεί με ένα έργο του οποίου η ζώνη ώρας είναι-8 PST και έχει τις ακόλουθες ώρες εργασίας: 9:00 Π.Μ. έως 5:00 ΜΜ Δευτέρα έως Παρασκευή, οποιαδήποτε εργασία που έχει δημιουργηθεί χωρίς ανάθεση θα σέβεται την ώρα έναρξης και την ώρα λήξης του ημερολογίου έργου.</span><span class="sxs-lookup"><span data-stu-id="df582-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="df582-111">Διαχείριση πόρων με ζώνες ώρας</span><span class="sxs-lookup"><span data-stu-id="df582-111">Manage resources with time zones</span></span>

<span data-ttu-id="df582-112">Για ακριβή και προβλέψιμα αποτελέσματα κατά τη χρήση της **επέκτασης κράτησης**, υπάρχουν δύο βασικές προϋποθέσεις που πρέπει να πληρούνται:</span><span class="sxs-lookup"><span data-stu-id="df582-112">For accurate and predictable results when using **Extend Booking**, there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="df582-113">Ο χρήστης πρέπει να ρυθμίσει τη ζώνη ώρας της συσκευής του ώστε να συμφωνεί με τη ζώνη ώρας που ορίζεται στις **Ρυθμίσεις εξατομίκευσης** του συστήματος.</span><span class="sxs-lookup"><span data-stu-id="df582-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Ρυθμίσεις ζώνης ώρας στα Windows 10](media/reconcile-assignments-03.png)

  ![Ρυθμίσεις ζώνης ώρας στις ρυθμίσεις εξατομίκευσης](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="df582-116">Ο πόρος με δυνατότητα κράτησης πρέπει να έχει τουλάχιστον ένα λεπτό χρόνου εργασίας που να επικαλύπτεται με τις καμπύλες που χρησιμοποιούνται για τον καθορισμό της επέκτασης που ζητήθηκε.</span><span class="sxs-lookup"><span data-stu-id="df582-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="df582-117">Για παράδειγμα, οι παρακάτω πόροι με ώρες εργασίας βρίσκονται μεταξύ 9:00 πμ και 7:00 μμ.</span><span class="sxs-lookup"><span data-stu-id="df582-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![Σύγκριση των καμπυλών πόρων](media/reconcile-assignments-05.png)

<span data-ttu-id="df582-119">Ο παρακάτω πίνακας δείχνει:</span><span class="sxs-lookup"><span data-stu-id="df582-119">The following table shows:</span></span>

- <span data-ttu-id="df582-120">Ένα πρότυπο ημερολογίου έργου</span><span class="sxs-lookup"><span data-stu-id="df582-120">A project calendar template</span></span>
- <span data-ttu-id="df582-121">Πόρος Α: Αυτός ο πόρος έχει το ίδιο ημερολόγιο και είναι στην ίδια ζώνη ώρας με το έργο.</span><span class="sxs-lookup"><span data-stu-id="df582-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="df582-122">Η ώρα έναρξης των κρατήσεων θα είναι 9:00 πμ.</span><span class="sxs-lookup"><span data-stu-id="df582-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="df582-123">Πόρος Β: αυτός ο πόρος βρίσκεται σε διαφορετική ζώνη ώρας από το έργο και ξεκινά στις 7:00 Π.Μ. στη ζώνη ώρας του.</span><span class="sxs-lookup"><span data-stu-id="df582-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="df582-124">Ωστόσο, οι κρατήσεις θα ξεκινήσουν στις 9:00 πμ, καθώς αυτή είναι η πρώτη ώρα έναρξης της καμπύλης ανάθεσης.</span><span class="sxs-lookup"><span data-stu-id="df582-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="df582-125">Πόροι Γ και Δ: οι πόροι βρίσκονται σε διαφορετικές ζώνες ώρας, και οι δύο διαφορετικές μεταξύ τους και το έργο και η κράτησή τους ξεκινά όχι νωρίτερα από τους αντίστοιχους διαθέσιμους χρόνους έναρξής τους.</span><span class="sxs-lookup"><span data-stu-id="df582-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="df582-126">Οντότητα</span><span class="sxs-lookup"><span data-stu-id="df582-126">Entity</span></span>  |<span data-ttu-id="df582-127">Ημερολόγιο</span><span class="sxs-lookup"><span data-stu-id="df582-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="df582-128">Πρότυπο ημερολογίου έργου</span><span class="sxs-lookup"><span data-stu-id="df582-128">Project calendar template</span></span>   | ![ημερολόγιο έργου](media/reconcile-assignments-06.png) |
|<span data-ttu-id="df582-130">Πόρος Α</span><span class="sxs-lookup"><span data-stu-id="df582-130">Resource A</span></span>  | ![Ημερολόγιο πόρου Α](media/reconcile-assignments-06.png) |
|<span data-ttu-id="df582-132">Πόρος Β</span><span class="sxs-lookup"><span data-stu-id="df582-132">Resource B</span></span>  |  ![Ημερολόγιο πόρου Β](media/reconcile-assignments-07.png) |
|<span data-ttu-id="df582-134">Πόρος Γ</span><span class="sxs-lookup"><span data-stu-id="df582-134">Resource C</span></span>  |  ![Ημερολόγιο πόρου Γ](media/reconcile-assignments-08.png) |
|<span data-ttu-id="df582-136">Πόρος Δ</span><span class="sxs-lookup"><span data-stu-id="df582-136">Resource D</span></span>  | ![Ημερολόγιο πόρου Δ](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="df582-138">Όταν μεταβαίνετε στην προβολή **Συμφωνία**, εμφανίζονται οι αναθέσεις πόρων και οι σχετικές ελλείψεις κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="df582-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![Προβολή εναρμόνισης πριν από την επέκταση](media/reconcile-assignments-10.png)

<span data-ttu-id="df582-140">Αφού χρησιμοποιηθεί η λειτουργικότητα επέκτασης κράτησης για κάθε πόρο, οι κρατήσεις έχουν επεκταθεί με επιτυχία για κάθε πόρο, επειδή οι ώρες εργασίας κάθε πόρου επικαλύπτονται με το περίγραμμα της έλλειψης.</span><span class="sxs-lookup"><span data-stu-id="df582-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![Προβολή εναρμόνισης μετά την επέκταση κράτησης](media/reconcile-assignments-11.png) 

<span data-ttu-id="df582-142">Προσέξτε ότι μια πιο προσεκτική ματιά στις λεπτομέρειες των κρατήσεων παρουσιάζει διαφορές στην ώρα έναρξης των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="df582-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="df582-143">Οι κρατήσεις ξεκινούν όχι νωρίτερα από την ώρα έναρξης της καμπύλης ανάθεσης και όχι νωρίτερα από τη διαθέσιμη ώρα έναρξης του πόρου.</span><span class="sxs-lookup"><span data-stu-id="df582-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![Νέες κρατήσεις πόρων στον πίνακα χρονοδιαγράμματος](media/reconcile-assignments-12.png)
