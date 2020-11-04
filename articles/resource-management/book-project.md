---
title: Κάντε κράτηση σε ένα έργο
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κράτηση ενός πόρου για ένα έργο.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 19128264ed3db7efeeba948155f0ddbdc806c2a0
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076768"
---
# <a name="book-to-a-project"></a><span data-ttu-id="c2a42-103">Κάντε κράτηση σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="c2a42-103">Book to a project</span></span>

<span data-ttu-id="c2a42-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="c2a42-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c2a42-105">Υπάρχουν φορές όπου ένας διαχειριστής έργου ή ένας διαχειριστής πόρου θα πρέπει να εκχωρήσει έναν πόρο στο έργο χωρίς μια συγκεκριμένη απαίτηση να καθορίζεται από ένα γενικό μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="c2a42-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="c2a42-106">Αυτό μπορεί να επιτευχθεί με έναν από τους εξής τρεις τρόπους.</span><span class="sxs-lookup"><span data-stu-id="c2a42-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="c2a42-107">Κράτηση από το πλέγμα μελών ομάδας</span><span class="sxs-lookup"><span data-stu-id="c2a42-107">Book from the team member grid</span></span>
- <span data-ttu-id="c2a42-108">Κράτηση από τον πίνακα χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="c2a42-108">Book from the schedule board</span></span>
- <span data-ttu-id="c2a42-109">Κάντε κράτηση από τη φόρμα **Έργο**</span><span class="sxs-lookup"><span data-stu-id="c2a42-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="c2a42-110">Κράτηση από το πλέγμα μελών ομάδας</span><span class="sxs-lookup"><span data-stu-id="c2a42-110">Book from the team member grid</span></span>

<span data-ttu-id="c2a42-111">Εάν ο οργανισμός σας λειτουργεί σε υβριδική λειτουργία εκχώρησης πόρων, ο υπεύθυνος έργου μπορεί να κάνει κράτηση ενός πόρου απευθείας στο έργο, ακολουθώντας τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="c2a42-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="c2a42-112">Από το έργο, μεταβείτε στο πλέγμα του μέλους ομάδας και επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="c2a42-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="c2a42-113">Καθορίστε το όνομα της θέσης και το ρόλο του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c2a42-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="c2a42-114">Επιλέξτε τον πόρο με δυνατότητα κράτησης από τη διαθέσιμη αναζήτηση.</span><span class="sxs-lookup"><span data-stu-id="c2a42-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="c2a42-115">Αφού επιλέξετε τον πόρο, καθορίστε τις παρακάτω πληροφορίες πεδίου για να κλείσετε τον πόρο:</span><span class="sxs-lookup"><span data-stu-id="c2a42-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="c2a42-116">Ημερομηνία έναρξης</span><span class="sxs-lookup"><span data-stu-id="c2a42-116">Start date</span></span>
    - <span data-ttu-id="c2a42-117">Ημερομηνία ολοκλήρωσης</span><span class="sxs-lookup"><span data-stu-id="c2a42-117">Finish date</span></span>
    - <span data-ttu-id="c2a42-118">Μέθοδος εκχώρησης</span><span class="sxs-lookup"><span data-stu-id="c2a42-118">Allocation method</span></span>
    - <span data-ttu-id="c2a42-119">Ώρες, ανάλογα με την περίπτωση</span><span class="sxs-lookup"><span data-stu-id="c2a42-119">Hours, if applicable</span></span>
    - <span data-ttu-id="c2a42-120">Υπεύθυνος έγκρισης έργου</span><span class="sxs-lookup"><span data-stu-id="c2a42-120">Project approver</span></span>

6. <span data-ttu-id="c2a42-121">Επιλέξτε **Αποθήκευση και κλείσιμο**</span><span class="sxs-lookup"><span data-stu-id="c2a42-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="c2a42-122">Κράτηση από τον πίνακα χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="c2a42-122">Book from the schedule board</span></span>

<span data-ttu-id="c2a42-123">Όταν ένας διαχειριστής πόρων χρειάζεται να κάνει κράτηση ενός πόρου απευθείας σε ένα έργο, μπορεί να χρησιμοποιήσει τον πίνακα χρονοδιαγράμματος και την απαίτηση έργου.</span><span class="sxs-lookup"><span data-stu-id="c2a42-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="c2a42-124">Η απαίτηση έργου είναι μια απαίτηση πόρου ο οποίος είναι πάντα διαθέσιμος για κράτηση.</span><span class="sxs-lookup"><span data-stu-id="c2a42-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="c2a42-125">Για απευθείας κράτηση σε έργο από τον πίνακα χρονοδιαγράμματος, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="c2a42-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="c2a42-126">Μεταβείτε στον πίνακα χρονοδιαγράμματος και στην αριστερή σελίδα, φιλτράρετε τους πόρους που λαμβάνετε υπόψη για την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="c2a42-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="c2a42-127">Στο κάτω παράθυρο, επιλέξτε την καρτέλα **Έργο** για να προβάλετε μια λίστα απαιτήσεων έργου.</span><span class="sxs-lookup"><span data-stu-id="c2a42-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="c2a42-128">Σύρετε την απαίτηση σε έναν πόρο και καθορίστε τις παρακάτω πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="c2a42-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="c2a42-129">Ημερομηνία έναρξης</span><span class="sxs-lookup"><span data-stu-id="c2a42-129">Start date</span></span>
    - <span data-ttu-id="c2a42-130">Ημερομηνία ολοκλήρωσης</span><span class="sxs-lookup"><span data-stu-id="c2a42-130">Finish date</span></span>
    - <span data-ttu-id="c2a42-131">Κατάσταση κράτησης</span><span class="sxs-lookup"><span data-stu-id="c2a42-131">Booking status</span></span>
    - <span data-ttu-id="c2a42-132">Μέθοδος κράτησης</span><span class="sxs-lookup"><span data-stu-id="c2a42-132">Booking method</span></span>
    - <span data-ttu-id="c2a42-133">Διάρκεια</span><span class="sxs-lookup"><span data-stu-id="c2a42-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="c2a42-134">Κάντε κράτηση από τη φόρμα Έργο</span><span class="sxs-lookup"><span data-stu-id="c2a42-134">Book from the Project form</span></span>

<span data-ttu-id="c2a42-135">Ως διαχειριστής έργου, μπορεί να χρειαστεί να κλείσετε έναν πόρο σε ένα έργο, αλλά να γνωρίζετε μόνο τα κριτήρια και όχι το όνομα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c2a42-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="c2a42-136">Ολοκληρώστε τα παρακάτω βήματα για να χρησιμοποιήσετε τον βοηθό χρονοδιαγράμματος για να βρείτε έναν πόρο με βάση τα διαθέσιμα χαρακτηριστικά του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c2a42-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="c2a42-137">Μεταβείτε στο έργο και επιλέξτε **Κράτηση** για να ανοίξετε τον βοηθό χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="c2a42-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="c2a42-138">Χρησιμοποιώντας τα φίλτρα που βρίσκονται στην αριστερή πλευρά του βοηθού χρονοδιαγράμματος, περιορίστε τα κριτήρια και επιλέξτε **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="c2a42-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="c2a42-139">Με βάση τους πόρους που επιστρέφονται στα αποτελέσματα, μπορείτε να κλείσετε έναν πόρο.</span><span class="sxs-lookup"><span data-stu-id="c2a42-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="c2a42-140">Αυτή η μέθοδος δεν δημιουργεί καμία κράτηση για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="c2a42-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="c2a42-141">Αντίθετα, προσθέτει τον πόρο στην ομάδα.</span><span class="sxs-lookup"><span data-stu-id="c2a42-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="c2a42-142">Μετά την προσθήκη του μέλους ομάδας στο έργο, ο υπεύθυνος έργου μπορεί να χρησιμοποιήσει τη διατήρηση κρατήσεων ή να επεκτείνει τις κρατήσεις για την προσθήκη των απαιτούμενων κρατήσεων στον πόρο.</span><span class="sxs-lookup"><span data-stu-id="c2a42-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>
