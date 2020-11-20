---
title: Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κράτηση καθορισμένων πόρων για μια απαίτηση γενικού πόρου.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: d7ff58ec08661adc702867c6c26805a74a3637c9
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125898"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="20944-103">Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="20944-103">Book named resources from resource requirements</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="20944-104">Μπορείτε να κάνετε κράτηση ενός καθορισμένου πόρου για να αντικαταστήσετε έναν γενικό πόρο που διαθέτει μια απαίτηση πόρου.</span><span class="sxs-lookup"><span data-stu-id="20944-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="20944-105">Στο Project Service Automation (PSA), στη σελίδα **Έργα**, επιλέξτε την καρτέλα **Ομάδα**.</span><span class="sxs-lookup"><span data-stu-id="20944-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="20944-106">Επιλέξτε τον γενικό πόρο που διαθέτει μια απαίτηση πόρου από τη λίστα και, μετά επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="20944-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="20944-107">Εναλλακτικά, ανοίξτε την απαίτηση πόρου και, στη συνέχεια κάντε κλικ στην **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="20944-107">Or, open the resource requirement and then click **Book**.</span></span>


![Κράτηση γενικού μέλους ομάδας](media/RM-how-to-14.png)


3. <span data-ttu-id="20944-109">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, επιλέξτε έναν καθορισμένο πόρο για να κάνετε κράτηση στην ομάδα έργου σας και πατήστε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="20944-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![Κράτηση γενικού μέλους ομάδας με χρήση του βοηθού χρονοδιαγράμματος](media/RM-how-to-15.png)

<span data-ttu-id="20944-111">Όταν η κράτηση ολοκληρωθεί και πληρούται από έναν καθορισμένο πόρο, ο γενικός πόρος αντικαθίσταται με τον καθορισμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="20944-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![Καθορισμένο μέλος ομάδας που αντικαθιστά ένα γενικό μέλος ομάδας](media/RM-how-to-16.png)

<span data-ttu-id="20944-113">Οι αναθέσεις στο χρονοδιάγραμμα ενημερώνονται και με τον καθορισμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="20944-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![Καθορισμένο μέλος ομάδας με ανάθεση σε εργασίες έργου](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="20944-115">Κάλυψη γενικού πόρου με πολλούς καθορισμένους πόρους</span><span class="sxs-lookup"><span data-stu-id="20944-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="20944-116">Η ικανοποίηση μιας απαίτησης για έναν γενικό πόρο με πολλούς καθορισμένους πόρους είναι παρόμοια με την ανάθεση ενός μεμονωμένου καθορισμένου πόρου.</span><span class="sxs-lookup"><span data-stu-id="20944-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="20944-117">Για παράδειγμα, υπάρχει μια εργασία διάρκειας πέντε ημερών και 120 ωρών προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="20944-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="20944-118">Αυτή η εργασία δεν μπορεί να ολοκληρωθεί από έναν πόρο που λειτουργεί μια τυπική ημέρα οκτώ ωρών κατά τη διάρκεια μιας εβδομάδας πέντε ημερών.</span><span class="sxs-lookup"><span data-stu-id="20944-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![Μια εργασία που απαιτεί 120 ώρες προσπάθειας για πέντε ημέρες](media/RM-how-to-21.png)

<span data-ttu-id="20944-120">Η απαίτηση είναι για 120 ώρες ρομποτικής μηχανικής πάνω από πέντε ημέρες, η οποία είναι 24 ώρες την ημέρα.</span><span class="sxs-lookup"><span data-stu-id="20944-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![Απαίτηση ανά ημέρα](media/RM-how-to-22.png)

<span data-ttu-id="20944-122">Αυτό είναι ένα παράδειγμα όταν απαιτούνται πολλαπλοί καθορισμένοι πόροι για την ικανοποίηση μιας αίτησης γενικού πόρου.</span><span class="sxs-lookup"><span data-stu-id="20944-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="20944-123">Θα χρειαστεί να κάνετε κράτηση πολλών πόρων για να εκπληρώσετε την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="20944-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![Θα χρειαστεί να κάνετε κράτηση πολλών πόρων για να εκπληρώσετε την απαίτηση](media/RM-how-to-23.png)

<span data-ttu-id="20944-125">Η κύρια διαφορά σε αυτό το σενάριο είναι ότι ο γενικός πόρος παραμένει στην ομάδα που έχει ανατεθεί στην εργασία και ότι τα καθορισμένα μέλη της ομάδας πόρων για τα οποία έχει γίνει κράτηση δεν αντιστοιχίζονται ως μέρος της θέσης.</span><span class="sxs-lookup"><span data-stu-id="20944-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="20944-126">Ο υπεύθυνος έργου μπορεί να αναθέσει την εργασία όπως απαιτείται στους καθορισμένους πόρους.</span><span class="sxs-lookup"><span data-stu-id="20944-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="20944-127">Η προβολή **Εναρμόνιση** παρέχει στον υπεύθυνο έργου μια ανάλυση των κρατήσεων σε πολλούς πόρους σε πολλές αναθέσεις εργασιών.</span><span class="sxs-lookup"><span data-stu-id="20944-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="20944-128">Αυτό δεν γίνεται αυτόματα, επειδή σε πιο περίπλοκα σενάρια, όπως ένα όπου έχετε μια δέσμη των εργασιών που αποτελούν την απαίτηση, η πρόθεση του υπεύθυνου έργου για το πώς θέλει να αναθέσει, πρέπει να ληφθεί υπόψη από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="20944-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="20944-129">Επειδή το σύστημα δεν μπορεί να κατανοήσει την πρόθεση, οι υποθέσεις να είναι διαφορετικές από αυτές που προορίζονται και ένα λανθασμένο ή μη προβλέψιμο αποτέλεσμα θα προκύψει.</span><span class="sxs-lookup"><span data-stu-id="20944-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="20944-130">Το προβλέψιμο αποτέλεσμα είναι ότι ο γενικός πόρος παραμένει εκχωρημένος έως ότου ο υπεύθυνος έργου δημιουργεί σκόπιμα αναθέσεις χρησιμοποιώντας την προβολή **Εναρμόνιση**.</span><span class="sxs-lookup"><span data-stu-id="20944-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


