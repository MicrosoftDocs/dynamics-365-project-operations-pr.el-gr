---
title: Πρόταση πόρων έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο πρότασης πόρων έργου.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 02e47338e34a37e05455e2bc6e6a175210ed6bc7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997961"
---
# <a name="propose-project-resources"></a><span data-ttu-id="63924-103">Πρόταση πόρων έργου</span><span class="sxs-lookup"><span data-stu-id="63924-103">Propose project resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="63924-104">Οι διαχειριστές πόρων μπορούν να προτείνουν έναν πόρο στον διαχειριστή έργου χρησιμοποιώντας μια αίτηση πόρου.</span><span class="sxs-lookup"><span data-stu-id="63924-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="63924-105">Από το πλέγμα αίτησης ή την ίδια την αίτηση, επιλέξτε **Εύρεση πόρων**.</span><span class="sxs-lookup"><span data-stu-id="63924-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="63924-106">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, επιλέξτε τον πόρο και στη συνέχεια, στον παράθυρο **Δημιουργία κράτησης πόρου**, στο πεδίο **Κατάσταση κράτησης**, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="63924-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![Προτεινόμενοι πόροι που επιλέχθηκαν](media/Resource-Management-image62.png)

<span data-ttu-id="63924-108">Παρουσιάζονται οι ακόλουθες ενημερώσεις κατάστασης:</span><span class="sxs-lookup"><span data-stu-id="63924-108">The following status updates occur:</span></span>

- <span data-ttu-id="63924-109">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, οι δείκτες κατάστασης ενημερώνονται έτσι ώστε να δηλώνουν ότι προτείνεται η κράτηση και όχι η οριστική κράτηση.</span><span class="sxs-lookup"><span data-stu-id="63924-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![Δείκτες κατάστασης για την προτεινόμενη κράτηση στη σελίδα βοηθού χρονοδιαγράμματος](media/Resource-Management-image63.png)

- <span data-ttu-id="63924-111">Στην αίτηση πόρου, η κατάσταση αλλάζει σε **Απαιτείται εξέταση**.</span><span class="sxs-lookup"><span data-stu-id="63924-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![Η κατάσταση αίτησης πόρου αλλάζει σε Απαιτείται εξέταση](media/Resource-Management-image64.png)

- <span data-ttu-id="63924-113">Στην καρτέλα **Ομάδα** του έργου, η τιμή γενικού μέλους ομάδας **Κατάσταση αίτησης** αλλάζει σε **Απαιτείται εξέταση**.</span><span class="sxs-lookup"><span data-stu-id="63924-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![Η κατάσταση αίτησης του γενικού μέλους ομάδας αλλάζει σε Απαιτείται εξέταση στην καρτέλα ομάδας](media/Resource-Management-image48.png)

<span data-ttu-id="63924-115">Ο υπεύθυνος έργου μπορεί είτε να αποδεχτεί ή να απορρίψει την πρόταση.</span><span class="sxs-lookup"><span data-stu-id="63924-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="63924-116">Όταν οι διαχειριστές πόρων επεξεργάζονται αιτήσεις πόρων, μπορούν να χρησιμοποιήσουν οποιαδήποτε από τις παρακάτω προσεγγίσεις:</span><span class="sxs-lookup"><span data-stu-id="63924-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="63924-117">Προτείνετε πολλαπλούς πόρους για την ικανοποίηση της ζήτησης, σε περίπτωση που δεν υπάρχει διαθέσιμος μεμονωμένος πόρος για την πλήρωση των απαιτούμενων ωρών.</span><span class="sxs-lookup"><span data-stu-id="63924-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="63924-118">Στη συνέχεια, οι προτεινόμενες ώρες διαχωρίζονται μεταξύ πολλών πόρων που μπορούν να ικανοποιήσουν τις απαιτούμενες ώρες.</span><span class="sxs-lookup"><span data-stu-id="63924-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="63924-119">Σε αυτό το σενάριο, οι ώρες δεν είναι δυνατό να επικαλύπτονται.</span><span class="sxs-lookup"><span data-stu-id="63924-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="63924-120">Προτείνετε λιγότερους πόρους από αυτούς που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="63924-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="63924-121">Σε αυτό το σενάριο, η παραγωγική ικανότητα του προτεινόμενου πόρου είναι μικρότερη από τις απαιτούμενες ώρες που καθόρισε ο αιτών.</span><span class="sxs-lookup"><span data-stu-id="63924-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="63924-122">Επομένως, όταν ο αιτών αποδέχεται τους προτεινόμενους πόρους, δημιουργείται μια απαίτηση πόρου που δεν πληρούται για την καταγραφή της υπολειπόμενης ζήτησης.</span><span class="sxs-lookup"><span data-stu-id="63924-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="63924-123">Κάντε κράτηση πολλών πόρων για την ικανοποίηση της ζήτησης, σε περίπτωση που δεν υπάρχει διαθέσιμος μεμονωμένος πόρος για την ολοκλήρωση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="63924-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="63924-124">Κάντε κράτηση λιγότερων πόρων από αυτούς που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="63924-124">Book fewer resources than are required.</span></span> <span data-ttu-id="63924-125">Σε αυτό το σενάριο, οι ώρες που έχουν κρατηθεί είναι λιγότερες από τις απαιτούμενες ώρες.</span><span class="sxs-lookup"><span data-stu-id="63924-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="63924-126">Το σύστημα σάς καθοδηγεί να προτείνετε πόρους αντί για κρατήσεις, έτσι ώστε ο αιτών να μπορεί να επαληθεύει και να παρακολουθεί την εναπομένουσα ζήτηση.</span><span class="sxs-lookup"><span data-stu-id="63924-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="63924-127">Χρεώσιμη χρήση</span><span class="sxs-lookup"><span data-stu-id="63924-127">Billable utilization</span></span>

<span data-ttu-id="63924-128">Οι πόροι μπορούν να έχουν μια χρεώσιμη χρήση-στόχο.</span><span class="sxs-lookup"><span data-stu-id="63924-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="63924-129">Αυτή η χρήση-στόχος καθορίζεται είτε ως χαρακτηριστικό του προεπιλεγμένου ρόλου ενός πόρου ή ορίζεται στην καρτέλα του μεμονωμένου πόρου με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="63924-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="63924-130">Οι υπολογισμοί χρήσης βασίζονται στις πραγματικές ώρες που ανέφεραν οι πόροι χρησιμοποιώντας εγκεκριμένες καταχωρήσεις χρόνου.</span><span class="sxs-lookup"><span data-stu-id="63924-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="63924-131">Οι ακόλουθοι τύποι χρησιμοποιούνται για τον υπολογισμό της χρήσης:</span><span class="sxs-lookup"><span data-stu-id="63924-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="63924-132">Χρεώσιμη χρήση = χρεώσιμες πραγματικές ώρες ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="63924-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="63924-133">Μη χρεώσιμη χρήση = πραγματικός χρόνος με αναγνωριστικό τύπου χρέωσης = μη χρεώσιμο, συμπληρωματικό ή μη διαθέσιμο ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="63924-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="63924-134">Εσωτερικό = πραγματικός χρόνος χωρίς σύμβαση πωλήσεων ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="63924-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="63924-135">Παραγωγική ικανότητα πόρου = ώρες εργασίας πόρου – εκτός γραφείου – μη εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="63924-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="63924-136">Μπορείτε να βρείτε την προβολή **Χρήση πόρου** στο παράθυρο **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="63924-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![Προβολή χρήσης πόρου](media/Resource-Management-image65.png)

<span data-ttu-id="63924-138">Κάθε κελί στο πλέγμα αντιπροσωπεύει το ποσοστό χρέωσης χρήσης του πόρου σε μια περίοδο, όπως μια ημέρα, μια εβδομάδα ή ένα μήνα.</span><span class="sxs-lookup"><span data-stu-id="63924-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="63924-139">Οι ακόλουθοι τύποι χρησιμοποιούνται για τον χρωματισμό των κελιών:</span><span class="sxs-lookup"><span data-stu-id="63924-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="63924-140">**Πράσινο:** χρεώσιμη χρήση \>= Χρήση-στόχος πόρου</span><span class="sxs-lookup"><span data-stu-id="63924-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="63924-141">**Κίτρινο:** Χρήση-στόχος – 20 \<= Χρεώσιμη χρήση \< Χρήση-στόχος</span><span class="sxs-lookup"><span data-stu-id="63924-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="63924-142">**Κόκκινο:** Χρεώσιμη χρήση \< Χρήση-στόχος – 20</span><span class="sxs-lookup"><span data-stu-id="63924-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="63924-143">Επειδή η προβολή **Χρήση πόρου** βασίζεται στον πίνακα χρονοδιαγράμματος, μπορείτε να χρησιμοποιήσετε τις δυνατότητες φιλτραρίσματος του πίνακα χρονοδιαγράμματος για να φιλτράρετε τα αποτελέσματά σας.</span><span class="sxs-lookup"><span data-stu-id="63924-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="63924-144">Το πλέγμα απαιτεί να ορίσετε μια χρήση-στόχος στον ρόλο ή στον μεμονωμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="63924-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="63924-145">Για να κάνετε αυτή τη ρύθμιση, μεταβείτε στα στοιχεία **Πόροι** \> **Ρόλοι πόρων**.</span><span class="sxs-lookup"><span data-stu-id="63924-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="63924-146">Επιπλέον, ένας προεπιλεγμένος ρόλος πρέπει να ανατεθεί σε κάθε πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="63924-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="63924-147">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="63924-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="63924-148">Στην καρτέλα **Project Service** επαληθεύστε ότι καθορίζεται ένας ρόλος πόρου και ότι το πεδίο **Είναι προεπιλογή** έχει οριστεί σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="63924-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="63924-149">Μπορείτε να προσθέσετε επιπλέον ρόλους όπου το στοιχείο **Είναι προεπιλογή = όχι**.</span><span class="sxs-lookup"><span data-stu-id="63924-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="63924-150">Ο ρόλος όπου το στοιχείο **Είναι προεπιλογή = Ναι** χρησιμοποιείται για την αξιολόγηση της χρήσης του πόρου σε σχέση με τον προορισμό για αυτόν το ρόλο.</span><span class="sxs-lookup"><span data-stu-id="63924-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![Προεπιλεγμένος ρόλος](media/Resource-Management-image67.png)

<span data-ttu-id="63924-152">Στην καρτέλα **Project Service** μπορείτε επίσης να ορίσετε μια μεμονωμένη χρήση-στόχο για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="63924-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="63924-153">Στη συνέχεια, ο υπολογισμός χρήσης χρησιμοποιεί την εν λόγω χρήση-στόχο για την αξιολόγηση του στόχου πόρου αντί του στόχου του προεπιλεγμένου ρόλου του πόρου.</span><span class="sxs-lookup"><span data-stu-id="63924-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="63924-154">Η χρήση εμφανίζεται για έναν πόρο μόνο εάν αυτός ο πόρος έχει εγκρίνει τον χρεώσιμο χρόνο κατά τη διάρκεια της περιόδου που εμφανίζεται στο πλέγμα.</span><span class="sxs-lookup"><span data-stu-id="63924-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="63924-155">Τη διαθεσιμότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="63924-155">Resource availability</span></span>

<span data-ttu-id="63924-156">Είναι σημαντικό οι διαχειριστές πόρων να μπορούν να προβάλλουν τη διαθεσιμότητα των πόρων και να ενημερώνουν τις κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="63924-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="63924-157">Σε ορισμένες περιπτώσεις, δεν υπάρχει καμία τυπική ζήτηση (αίτηση πόρου), αλλά ένας διαχειριστής πόρων πρέπει να ανταποκριθεί σε μια μη προγραμματισμένη ζήτηση που προέρχεται από κανάλια όπως ένα μήνυμα ηλεκτρονικού ταχυδρομείου, μια τηλεφωνική κλήση ή ένα άμεσο μήνυμα.</span><span class="sxs-lookup"><span data-stu-id="63924-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="63924-158">Οι διαχειριστές πόρων χρησιμοποιούν τον πίνακα χρονοδιαγράμματος για την ενημέρωση των πόρων και των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="63924-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="63924-159">Οι ώρες εργασίας πόρων χρησιμοποιούνται ως βάση για τον υπολογισμό της διαθεσιμότητας ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="63924-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="63924-160">Με τις κρατήσεις πόρων καταναλώνεται η παραγωγική ικανότητα των πόρων.</span><span class="sxs-lookup"><span data-stu-id="63924-160">Resource bookings consume the capacity of the resources.</span></span>

![Πίνακας χρονοδιαγράμματος](media/Resource-Management-image68.png)

<span data-ttu-id="63924-162">Ο πίνακας χρονοδιαγράμματος χρησιμοποιεί χρώματα και σκίαση για την εμφάνιση κρατήσεων, τη διαθεσιμότητα και τις υπερκρατήσεις και επίσης την κατάσταση των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="63924-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="63924-163">Μια ρύθμιση στις ρυθμίσεις του πίνακα χρονοδιαγράμματος σάς δίνει τη δυνατότητα να εμφανίζετε μια λεζάντα.</span><span class="sxs-lookup"><span data-stu-id="63924-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="63924-164">Εάν εμφανίζεται ένα βέλος προς τα δεξιά δίπλα σε έναν μεμονωμένο πόρο με δυνατότητα κράτησης στον πίνακα χρονοδιαγράμματος, ο πόρος μπορεί να αναπτυχθεί ώστε να εμφανίζει λεπτομέρειες σχετικά με την εργασία στην οποία έχει γίνει κράτηση ο πόρος.</span><span class="sxs-lookup"><span data-stu-id="63924-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![Πόρος με δυνατότητα κράτησης ανεπτυγμένος στον πίνακα χρονοδιαγράμματος](media/Resource-Management-image69.png)

<span data-ttu-id="63924-166">Επειδή το Dynamics 365 Project Service Automation χρησιμοποιεί τη μηχανή Universal Resource Scheduling, εάν έχετε εγκατεστημένο το Dynamics 365 Field Service, μπορείτε να προβάλετε τις λεπτομέρειες των κρατήσεων πόρων για τα έργα, τις παραγγελίες εργασίας και οποιεσδήποτε άλλες οντότητες στις οποίες έχετε επεκτείνει τον προγραμματισμό.</span><span class="sxs-lookup"><span data-stu-id="63924-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![Λεπτομέρειες των κρατήσεων πόρων για τα έργα και τις παραγγελίες εργασίας](media/Resource-Management-image70.png)

<span data-ttu-id="63924-168">Για να προβάλετε περισσότερες λεπτομέρειες σχετικά με έναν μεμονωμένο πόρο, κάντε δεξί κλικ σε αυτόν για να ανοίξετε την καρτέλα πόρου.</span><span class="sxs-lookup"><span data-stu-id="63924-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![Κάρτα πόρου](media/Resource-Management-image71.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]