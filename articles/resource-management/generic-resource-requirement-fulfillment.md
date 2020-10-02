---
title: Εκπλήρωση γενικών απαιτήσεων πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κράτηση καθορισμένων πόρων για μια απαίτηση γενικού πόρου.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 76dd47fa2451b5cb61298ff332d77bae646a288a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897586"
---
# <a name="generic-resource-requirement-fulfillment"></a><span data-ttu-id="1de9c-103">Εκπλήρωση γενικών απαιτήσεων πόρων</span><span class="sxs-lookup"><span data-stu-id="1de9c-103">Generic resource requirement fulfillment</span></span>

<span data-ttu-id="1de9c-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1de9c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1de9c-105">Μπορείτε να κάνετε κράτηση ενός καθορισμένου πόρου για να αντικαταστήσετε έναν γενικό πόρο που διαθέτει μια απαίτηση πόρου.</span><span class="sxs-lookup"><span data-stu-id="1de9c-105">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="1de9c-106">Στη σελίδα **Έργα**, επιλέξτε την καρτέλα **Ομάδα**.</span><span class="sxs-lookup"><span data-stu-id="1de9c-106">On the **Projects** page, select the **Team** tab.</span></span>
2. <span data-ttu-id="1de9c-107">Επιλέξτε τον γενικό πόρο που διαθέτει μια απαίτηση πόρου από τη λίστα και, μετά επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="1de9c-107">Select the generic resource that has a resource requirement from the list, and then select **Book**.</span></span> <span data-ttu-id="1de9c-108">Εναλλακτικά, ανοίξτε την απαίτηση πόρου και, στη συνέχεια επιλέξτε την **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="1de9c-108">Or, open the resource requirement and then select **Book**.</span></span>
3. <span data-ttu-id="1de9c-109">Στη σελίδα **Βοηθός χρονοδιαγράμματος**, επιλέξτε έναν καθορισμένο πόρο για να κάνετε κράτηση στην ομάδα έργου σας και επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="1de9c-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then select **Book**.</span></span>

<span data-ttu-id="1de9c-110">Όταν η κράτηση ολοκληρωθεί και πληρούται από έναν καθορισμένο πόρο, ο γενικός πόρος αντικαθίσταται με τον καθορισμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="1de9c-110">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

<span data-ttu-id="1de9c-111">Οι αναθέσεις στο χρονοδιάγραμμα ενημερώνονται και με τον καθορισμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="1de9c-111">The assignments on the schedule are updated with the named resource as well.</span></span>

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="1de9c-112">Κάλυψη γενικού πόρου με πολλούς καθορισμένους πόρους</span><span class="sxs-lookup"><span data-stu-id="1de9c-112">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="1de9c-113">Η ικανοποίηση μιας απαίτησης για έναν γενικό πόρο με πολλούς καθορισμένους πόρους είναι παρόμοια με την ανάθεση ενός μεμονωμένου καθορισμένου πόρου.</span><span class="sxs-lookup"><span data-stu-id="1de9c-113">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="1de9c-114">Για παράδειγμα, υπάρχει μια εργασία διάρκειας πέντε ημερών και 120 ωρών προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="1de9c-114">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="1de9c-115">Αυτή η εργασία δεν μπορεί να ολοκληρωθεί από έναν πόρο που λειτουργεί μια τυπική ημέρα οκτώ ωρών κατά τη διάρκεια μιας εβδομάδας πέντε ημερών.</span><span class="sxs-lookup"><span data-stu-id="1de9c-115">This task can't be completed by one resource that works a typical eight-hour day over a five-day week.</span></span> 

<span data-ttu-id="1de9c-116">Η απαίτηση είναι για 120 ώρες ρομποτικής μηχανικής πάνω από πέντε ημέρες, η οποία είναι 24 ώρες την ημέρα.</span><span class="sxs-lookup"><span data-stu-id="1de9c-116">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

<span data-ttu-id="1de9c-117">Αυτό είναι ένα παράδειγμα όταν απαιτούνται πολλαπλοί καθορισμένοι πόροι για την ικανοποίηση μιας αίτησης γενικού πόρου.</span><span class="sxs-lookup"><span data-stu-id="1de9c-117">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="1de9c-118">Θα χρειαστεί να κάνετε κράτηση πολλών πόρων για να εκπληρώσετε την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="1de9c-118">You will need to book multiple resources to fulfill the requirement.</span></span>

<span data-ttu-id="1de9c-119">Η κύρια διαφορά σε αυτό το σενάριο είναι ότι ο γενικός πόρος παραμένει στην ομάδα που έχει ανατεθεί στην εργασία και ότι τα καθορισμένα μέλη της ομάδας πόρων για τα οποία έχει γίνει κράτηση δεν αντιστοιχίζονται ως μέρος της θέσης.</span><span class="sxs-lookup"><span data-stu-id="1de9c-119">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="1de9c-120">Ο υπεύθυνος έργου μπορεί να αναθέσει την εργασία όπως απαιτείται στους καθορισμένους πόρους.</span><span class="sxs-lookup"><span data-stu-id="1de9c-120">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="1de9c-121">Η προβολή **Εναρμόνιση** παρέχει στον υπεύθυνο έργου μια ανάλυση των κρατήσεων σε πολλούς πόρους σε πολλές αναθέσεις εργασιών.</span><span class="sxs-lookup"><span data-stu-id="1de9c-121">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="1de9c-122">Αυτό δεν γίνεται αυτόματα, επειδή σε πιο περίπλοκα σενάρια, όπως ένα όπου έχετε μια δέσμη των εργασιών που αποτελούν την απαίτηση ή την πρόθεση του υπεύθυνου έργου για το πώς θέλει να αναθέσει, πρέπει να ληφθεί υπόψη από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="1de9c-122">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement or the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="1de9c-123">Επειδή το σύστημα δεν μπορεί να κατανοήσει την πρόθεση, είναι πιθανό οι υποθέσεις πιθανώς να είναι διαφορετικές από αυτές που προορίζονται και ένα λανθασμένο ή μη προβλέψιμο αποτέλεσμα θα προκύψει.</span><span class="sxs-lookup"><span data-stu-id="1de9c-123">Because the system can't understand intent, it's likely that the assumptions will be different than intended and an incorrect or unpredictable result will occur.</span></span> <span data-ttu-id="1de9c-124">Το προβλέψιμο αποτέλεσμα είναι ότι ο γενικός πόρος παραμένει εκχωρημένος έως ότου ο υπεύθυνος έργου δημιουργεί σκόπιμα αναθέσεις χρησιμοποιώντας την προβολή **Εναρμόνιση**.</span><span class="sxs-lookup"><span data-stu-id="1de9c-124">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


