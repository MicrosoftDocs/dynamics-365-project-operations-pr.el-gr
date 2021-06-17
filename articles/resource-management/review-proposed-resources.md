---
title: Έλεγχος προτεινόμενων πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο πρότασης πόρων έργου.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 987ea08c77c1824182856c0d52ee0cd15e7029b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000751"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="ba103-103">Έλεγχος προτεινόμενων πόρων</span><span class="sxs-lookup"><span data-stu-id="ba103-103">Review proposed resources</span></span>

<span data-ttu-id="ba103-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="ba103-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ba103-105">Οι διαχειριστές πόρων μπορούν να προτείνουν έναν πόρο στον διαχειριστή έργου χρησιμοποιώντας μια αίτηση πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba103-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="ba103-106">Από το πλέγμα αίτησης ή την ίδια την αίτηση, επιλέξτε **Εύρεση πόρων**.</span><span class="sxs-lookup"><span data-stu-id="ba103-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="ba103-107">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, επιλέξτε τον πόρο και στη συνέχεια, στον παράθυρο **Δημιουργία κράτησης πόρου**, στο πεδίο **Κατάσταση κράτησης**, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="ba103-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="ba103-108">Παρουσιάζονται οι ακόλουθες ενημερώσεις κατάστασης:</span><span class="sxs-lookup"><span data-stu-id="ba103-108">The following status updates occur:</span></span>

- <span data-ttu-id="ba103-109">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, οι δείκτες κατάστασης ενημερώνονται έτσι ώστε να δηλώνουν ότι προτείνεται η κράτηση και όχι η οριστική κράτηση.</span><span class="sxs-lookup"><span data-stu-id="ba103-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="ba103-110">Στην αίτηση πόρου, η κατάσταση αλλάζει σε **Απαιτείται εξέταση**.</span><span class="sxs-lookup"><span data-stu-id="ba103-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="ba103-111">Στην καρτέλα **Ομάδα** του έργου, η τιμή γενικού μέλους ομάδας **Κατάσταση αίτησης** αλλάζει σε **Απαιτείται εξέταση**.</span><span class="sxs-lookup"><span data-stu-id="ba103-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="ba103-112">Ο υπεύθυνος έργου μπορεί είτε να αποδεχτεί ή να απορρίψει την πρόταση.</span><span class="sxs-lookup"><span data-stu-id="ba103-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="ba103-113">Όταν οι διαχειριστές πόρων επεξεργάζονται αιτήσεις πόρων, μπορούν να χρησιμοποιήσουν οποιαδήποτε από τις παρακάτω προσεγγίσεις:</span><span class="sxs-lookup"><span data-stu-id="ba103-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="ba103-114">Προτείνετε πολλαπλούς πόρους για την ικανοποίηση της ζήτησης, σε περίπτωση που δεν υπάρχει διαθέσιμος μεμονωμένος πόρος για την πλήρωση των απαιτούμενων ωρών.</span><span class="sxs-lookup"><span data-stu-id="ba103-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="ba103-115">Στη συνέχεια, οι προτεινόμενες ώρες διαχωρίζονται μεταξύ πολλών πόρων που μπορούν να ικανοποιήσουν τις απαιτούμενες ώρες.</span><span class="sxs-lookup"><span data-stu-id="ba103-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="ba103-116">Σε αυτό το σενάριο, οι ώρες δεν είναι δυνατό να επικαλύπτονται.</span><span class="sxs-lookup"><span data-stu-id="ba103-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="ba103-117">Προτείνετε λιγότερους πόρους από αυτούς που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="ba103-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="ba103-118">Σε αυτό το σενάριο, η παραγωγική ικανότητα του προτεινόμενου πόρου είναι μικρότερη από τις απαιτούμενες ώρες που καθόρισε ο αιτών.</span><span class="sxs-lookup"><span data-stu-id="ba103-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="ba103-119">Επομένως, όταν ο αιτών αποδέχεται τους προτεινόμενους πόρους, δημιουργείται μια απαίτηση πόρου που δεν πληρούται για την καταγραφή της υπολειπόμενης ζήτησης.</span><span class="sxs-lookup"><span data-stu-id="ba103-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="ba103-120">Κάντε κράτηση πολλών πόρων για την ικανοποίηση της ζήτησης, σε περίπτωση που δεν υπάρχει διαθέσιμος μεμονωμένος πόρος για την ολοκλήρωση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="ba103-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="ba103-121">Κάντε κράτηση λιγότερων πόρων από αυτούς που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="ba103-121">Book fewer resources than are required.</span></span> <span data-ttu-id="ba103-122">Σε αυτό το σενάριο, οι ώρες που έχουν κρατηθεί είναι λιγότερες από τις απαιτούμενες ώρες.</span><span class="sxs-lookup"><span data-stu-id="ba103-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="ba103-123">Το σύστημα σάς καθοδηγεί να προτείνετε πόρους αντί για κρατήσεις, έτσι ώστε ο αιτών να μπορεί να επαληθεύει και να παρακολουθεί την εναπομένουσα ζήτηση.</span><span class="sxs-lookup"><span data-stu-id="ba103-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="ba103-124">Τη διαθεσιμότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="ba103-124">Resource availability</span></span>

<span data-ttu-id="ba103-125">Είναι σημαντικό οι διαχειριστές πόρων να μπορούν να προβάλλουν τη διαθεσιμότητα των πόρων και να ενημερώνουν τις κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="ba103-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="ba103-126">Σε ορισμένες περιπτώσεις, δεν υπάρχει καμία τυπική ζήτηση (αίτηση πόρου), αλλά ένας διαχειριστής πόρων πρέπει να ανταποκριθεί σε μια μη προγραμματισμένη ζήτηση που προέρχεται από κανάλια όπως ένα μήνυμα ηλεκτρονικού ταχυδρομείου, μια τηλεφωνική κλήση ή ένα άμεσο μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="ba103-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="ba103-127">Οι διαχειριστές πόρων χρησιμοποιούν τον πίνακα χρονοδιαγράμματος για την ενημέρωση των πόρων και των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="ba103-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="ba103-128">Οι ώρες εργασίας πόρων χρησιμοποιούνται ως βάση για τον υπολογισμό της διαθεσιμότητας ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba103-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="ba103-129">Με τις κρατήσεις πόρων καταναλώνεται η παραγωγική ικανότητα των πόρων.</span><span class="sxs-lookup"><span data-stu-id="ba103-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="ba103-130">Ο πίνακας χρονοδιαγράμματος χρησιμοποιεί χρώματα και σκίαση για την εμφάνιση κρατήσεων, τη διαθεσιμότητα και τις υπερκρατήσεις και επίσης την κατάσταση των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="ba103-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="ba103-131">Μια ρύθμιση στις ρυθμίσεις του πίνακα χρονοδιαγράμματος σάς δίνει τη δυνατότητα να εμφανίζετε μια λεζάντα.</span><span class="sxs-lookup"><span data-stu-id="ba103-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="ba103-132">Εάν εμφανίζεται ένα βέλος προς τα δεξιά δίπλα σε έναν μεμονωμένο πόρο με δυνατότητα κράτησης στον πίνακα χρονοδιαγράμματος, ο πόρος μπορεί να αναπτυχθεί ώστε να εμφανίζει λεπτομέρειες σχετικά με την εργασία στην οποία έχει γίνει κράτηση ο πόρος.</span><span class="sxs-lookup"><span data-stu-id="ba103-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="ba103-133">Επειδή το Dynamics 365 Project Operations χρησιμοποιεί τη μηχανή Universal Resource Scheduling, εάν έχετε εγκατεστημένο το Dynamics 365 Field Service, μπορείτε να προβάλετε τις λεπτομέρειες των κρατήσεων πόρων για τα έργα, τις παραγγελίες εργασίας και οποιεσδήποτε άλλες οντότητες στις οποίες έχετε επεκτείνει τον προγραμματισμό.</span><span class="sxs-lookup"><span data-stu-id="ba103-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="ba103-134">Για να προβάλετε περισσότερες λεπτομέρειες σχετικά με έναν μεμονωμένο πόρο, κάντε δεξί κλικ σε αυτόν για να ανοίξετε την καρτέλα πόρου.</span><span class="sxs-lookup"><span data-stu-id="ba103-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]