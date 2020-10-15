---
title: Ρύθμιση κατηγοριών εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης κατηγοριών εξόδων και κοινόχρηστων κατηγοριών για τις αναφορές εξόδων.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896686"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="258d6-103">Ρύθμιση κατηγοριών εξόδων</span><span class="sxs-lookup"><span data-stu-id="258d6-103">Set up expense categories</span></span>

<span data-ttu-id="258d6-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="258d6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="258d6-105">Όταν οι υπάλληλοι δημιουργούν αναφορές εξόδων, κάθε δαπάνη την οποία καταγράφουν πρέπει να συσχετίζεται με μια κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="258d6-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="258d6-106">Οι κατηγορίες δαπανών προέρχονται από κοινόχρηστες κατηγορίες, οι οποίες είναι δυνατό να χρησιμοποιηθούν από κοινού σε όλες τις νομικές οντότητες του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="258d6-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="258d6-107">Ανάλογα με τον τρόπο με τον οποίο καθορίζεται ο οργανισμός σας, αυτές οι κατηγορίες δαπανών μπορούν επίσης να χρησιμοποιηθούν από κοινού σε άλλες περιοχές.</span><span class="sxs-lookup"><span data-stu-id="258d6-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="258d6-108">Με βάση τον ορισμό του οργανισμού σας και την καθοδήγησή σας από την ομάδα υλοποίησης, πρέπει να καθορίσετε εάν οι κατηγορίες που χρησιμοποιούνται στη διαχείριση δαπανών θα χρησιμοποιηθούν μόνο στη διαχείριση εξόδων ή θα πρέπει να είναι κοινόχρηστες σε άλλες περιοχές.</span><span class="sxs-lookup"><span data-stu-id="258d6-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="258d6-109">Αυτές οι κατηγορίες είναι δυνατό να κατανεμηθούν μεταξύ της διαχείρισης έργου και της λογιστικής και της διαχείρισης εξόδων ή μεταξύ διαχείρισης έργου και λογιστικής και παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="258d6-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="258d6-110">Ωστόσο, δεν είναι δυνατή η κοινή χρήση τους μεταξύ διαχείρισης εξόδων και παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="258d6-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="258d6-111">Για να μπορέσετε να ξεκινήσετε τη διαδικασία εγκατάστασης, θα πρέπει να λάβετε τις παρακάτω αποφάσεις για κάθε κατηγορία εξόδων:</span><span class="sxs-lookup"><span data-stu-id="258d6-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="258d6-112">Ποια είναι η κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-112">What is the expense category?</span></span> <span data-ttu-id="258d6-113">Τα παραδείγματα περιλαμβάνουν κατηγορίες για πτήσεις, ξενοδοχεία ή χιλιόμετρα.</span><span class="sxs-lookup"><span data-stu-id="258d6-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="258d6-114">Μπορεί η κατηγορία εξόδων να χρησιμοποιηθεί και στη διαχείριση έργου και στη λογιστική;</span><span class="sxs-lookup"><span data-stu-id="258d6-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="258d6-115">Αν μπορεί, πρέπει να έχετε αποφασίσει για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="258d6-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="258d6-116">Ποιοι λογαριασμοί κόστους θα χρησιμοποιηθούν για τις ακόλουθες δαπάνες;</span><span class="sxs-lookup"><span data-stu-id="258d6-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="258d6-117">Κόστος</span><span class="sxs-lookup"><span data-stu-id="258d6-117">Cost</span></span>
        - <span data-ttu-id="258d6-118">Εκχώρηση μισθοδοσίας</span><span class="sxs-lookup"><span data-stu-id="258d6-118">Payroll allocation</span></span>
        - <span data-ttu-id="258d6-119">WIP-τιμή κόστους</span><span class="sxs-lookup"><span data-stu-id="258d6-119">WIP-cost value</span></span>
        - <span data-ttu-id="258d6-120">Κόστος-στοιχείο</span><span class="sxs-lookup"><span data-stu-id="258d6-120">Cost-item</span></span>
        - <span data-ttu-id="258d6-121">WIP-τιμή κόστους-στοιχείο</span><span class="sxs-lookup"><span data-stu-id="258d6-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="258d6-122">Συσσωρευμένη απώλεια</span><span class="sxs-lookup"><span data-stu-id="258d6-122">Accrued loss</span></span>
        - <span data-ttu-id="258d6-123">WIP-συσσωρευμένη απώλεια</span><span class="sxs-lookup"><span data-stu-id="258d6-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="258d6-124">Ποιοι λογαριασμοί εσόδων θα χρησιμοποιηθούν για τις ακόλουθες πηγές εσόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="258d6-125">Τιμολογημένα έσοδα</span><span class="sxs-lookup"><span data-stu-id="258d6-125">Invoiced revenue</span></span>
        - <span data-ttu-id="258d6-126">Συσσωρευμένα έσοδα - τιμή πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="258d6-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="258d6-127">WIP-τιμή πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="258d6-127">WIP-sales value</span></span>
        - <span data-ttu-id="258d6-128">Συσσωρευμένα έσοδα-παραγωγή</span><span class="sxs-lookup"><span data-stu-id="258d6-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="258d6-129">WIP-παραγωγή</span><span class="sxs-lookup"><span data-stu-id="258d6-129">WIP-production</span></span>
        - <span data-ttu-id="258d6-130">Συσσωρευμένα έσοδα-κέρδος</span><span class="sxs-lookup"><span data-stu-id="258d6-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="258d6-131">WIP-κέρδος</span><span class="sxs-lookup"><span data-stu-id="258d6-131">WIP-profit</span></span>
        - <span data-ttu-id="258d6-132">Συσσωρευμένα έσοδα-συνδρομή</span><span class="sxs-lookup"><span data-stu-id="258d6-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="258d6-133">WIP-συνδρομή</span><span class="sxs-lookup"><span data-stu-id="258d6-133">WIP-subscription</span></span>

- <span data-ttu-id="258d6-134">Ποιος είναι ο τύπος εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-134">What is the expense type?</span></span>
- <span data-ttu-id="258d6-135">Ποια είναι η προεπιλεγμένη μέθοδος πληρωμής για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="258d6-136">Οι δαπάνες στην κατηγορία εξόδων πρέπει να είναι αναλυτικές;</span><span class="sxs-lookup"><span data-stu-id="258d6-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="258d6-137">Ποιος είναι ο κύριος προεπιλεγμένος λογαριασμός για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="258d6-138">Ποια είναι η προεπιλεγμένη ομάδα φόρου πωλήσεων είδους για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="258d6-139">Επιτρέπονται επιπλέον μέθοδοι πληρωμής για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="258d6-140">Εάν ναι, ποιες είναι αυτές;</span><span class="sxs-lookup"><span data-stu-id="258d6-140">If so, what are they?</span></span>
- <span data-ttu-id="258d6-141">Υπάρχουν υποκατηγορίες σε αυτήν την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="258d6-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="258d6-142">Αν υπάρχουν υποκατηγορίες, πρέπει να έχετε αποφασίσει για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="258d6-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="258d6-143">Αποκλείεται καμία από τις υποκατηγορίες από την είσπραξη φόρων;</span><span class="sxs-lookup"><span data-stu-id="258d6-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="258d6-144">Ποια είναι η ομάδα φόρου πωλήσεων ειδών στις υποκατηγορίες;</span><span class="sxs-lookup"><span data-stu-id="258d6-144">What is the item sales tax group of the subcategories?</span></span>
