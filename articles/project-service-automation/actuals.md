---
title: 'Πραγματικές τιμές '
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις πραγματικές τιμές έργου.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751658"
---
# <a name="actuals"></a><span data-ttu-id="f5f4a-103">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="f5f4a-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f5f4a-104">Οι πραγματικές τιμές είναι ο όγκος εργασίας που έχει ολοκληρωθεί σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="f5f4a-105">Οι πραγματικές τιμές του έργου μπορούν να επισημανθούν στα έγγραφα προέλευσης.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="f5f4a-106">Στα εν λόγω έγγραφα προέλευσης περιλαμβάνονται καταχωρήσεις χρόνου, εξόδων και ημερολογίου καθώς επίσης και τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Πώς ανιχνεύονται οι πραγματικές τιμές του έργου στα έγγραφα προέλευσης](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="f5f4a-108">Υποβολή χρονικής καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="f5f4a-108">Submitting a time entry</span></span>

<span data-ttu-id="f5f4a-109">Στο PSA, όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="f5f4a-110">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="f5f4a-111">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="f5f4a-112">Η λογική για την εισαγωγή προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="f5f4a-113">Όλες οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="f5f4a-114">Αυτά τα πεδία περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="f5f4a-115">Τα πεδία που επηρεάζουν τις προεπιλεγμένες τιμές, όπως ο **Ρόλος** και η **Οργανική μονάδα** προκαλούν την εισαγωγή μιας κατάλληλης τιμής από προεπιλογή στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="f5f4a-116">Εάν προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση ώρας και θέλετε η τιμή του πεδίου να μεταδοθεί στα πραγματικά στοιχεία, δημιουργήστε το πεδίο στην οντότητα "πραγματικές τιμές" και χρησιμοποιήστε αντιστοιχίσεις πεδίων για να αντιγράψετε το πεδίο από την καταχώρηση χρόνου στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="f5f4a-117">Υποβολή μιας καταχώρησης εξόδων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-117">Submitting an expense entry</span></span>

<span data-ttu-id="f5f4a-118">Στο PSA, όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="f5f4a-119">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="f5f4a-120">Όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="f5f4a-121">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα βασίζεται στην κατηγορία εξόδων που έχει επιλεγεί στη σελίδα **Καταχώρηση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="f5f4a-122">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="f5f4a-123">Ωστόσο, για την ίδια την τιμή, το ποσό που εισήγαγε ο χρήστης ορίζεται απευθείας στις σχετικές γραμμές ημερολογίου εξόδων για το κόστος και τις πωλήσεις από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="f5f4a-124">Στην τρέχουσα έκδοση του PSA, η καταχώρηση με βάση την κατηγορία των προεπιλεγμένων τιμών ανά μονάδα σε καταχωρήσεις εξόδων δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="f5f4a-125">Χρήση ημερολογίων για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="f5f4a-125">Using journals to record costs</span></span>

<span data-ttu-id="f5f4a-126">Στο PSA, τα ημερολόγια σάς επιτρέπουν να καταγράφετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, το χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="f5f4a-127">Ένα ημερολόγιο έχει κεφαλίδα, γραμμές και μια **Επιβεβαίωση** ενέργειας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="f5f4a-128">Ακολουθούν ορισμένα σενάρια στα οποία μπορείτε να χρησιμοποιήσετε ένα ημερολόγιο:</span><span class="sxs-lookup"><span data-stu-id="f5f4a-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="f5f4a-129">Πρέπει να καταγράψετε το πραγματικό κόστος υλικού και τις πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="f5f4a-130">Πρέπει να μετακινήσετε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο PSA.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="f5f4a-131">Πρέπει να καταγράψετε το κόστος που σημειώθηκε σε ένα άλλο σύστημα, για παράδειγμα, το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="f5f4a-132">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-132">Recording actuals based on project events</span></span>

<span data-ttu-id="f5f4a-133">Το PSA καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="f5f4a-134">Αυτές οι συναλλαγές καταγράφονται ως **πραγματικές τιμές**.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="f5f4a-135">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="f5f4a-136">**Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="f5f4a-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="f5f4a-137">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="f5f4a-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="f5f4a-138">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="f5f4a-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="f5f4a-139">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="f5f4a-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="f5f4a-140">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="f5f4a-141">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="f5f4a-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="f5f4a-142">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="f5f4a-143">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="f5f4a-143">Actuals</span></span></th>
<th><span data-ttu-id="f5f4a-144">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f5f4a-144">Transaction currency</span></span></th>
<th><span data-ttu-id="f5f4a-145">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-145">Fixed price</span></span></th>
<th><span data-ttu-id="f5f4a-146">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f5f4a-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="f5f4a-147">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="f5f4a-148">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f5f4a-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-149">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="f5f4a-150">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f5f4a-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f5f4a-151">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f5f4a-152">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-152">Cost actual</span></span></td>
<td><span data-ttu-id="f5f4a-153">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-154">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-155">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="f5f4a-156">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-157">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-158">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="f5f4a-159">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f5f4a-160">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f5f4a-161">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-161">Cost actual</span></span></td>
<td><span data-ttu-id="f5f4a-162">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-163">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-164">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-165">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-166">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-167">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-168">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-169">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-170">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f5f4a-171">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f5f4a-172">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f5f4a-173">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-174">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-175">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-176">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-177">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-178">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-178">Billed sales</span></span></td>
<td><span data-ttu-id="f5f4a-179">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f5f4a-180">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f5f4a-181">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f5f4a-182">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-183">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-184">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-185">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-186">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-187">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-188">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-189">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-190">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f5f4a-191">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f5f4a-192">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f5f4a-193">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="f5f4a-194">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="f5f4a-195">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="f5f4a-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="f5f4a-196">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-197">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-198">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-199">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-199">Billed sales</span></span></td>
<td><span data-ttu-id="f5f4a-200">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f5f4a-201">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f5f4a-202">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f5f4a-203">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-204">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-205">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-206">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-207">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="f5f4a-208">**Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="f5f4a-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="f5f4a-209">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="f5f4a-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="f5f4a-210">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="f5f4a-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="f5f4a-211">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="f5f4a-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="f5f4a-212">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="f5f4a-213">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="f5f4a-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="f5f4a-214">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="f5f4a-215">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="f5f4a-215">Actuals</span></span></th>
<th><span data-ttu-id="f5f4a-216">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f5f4a-216">Transaction currency</span></span></th>
<th><span data-ttu-id="f5f4a-217">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-217">Fixed price</span></span></th>
<th><span data-ttu-id="f5f4a-218">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f5f4a-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="f5f4a-219">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="f5f4a-220">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f5f4a-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-221">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="f5f4a-222">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f5f4a-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="f5f4a-223">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f5f4a-224">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-224">Cost actual</span></span></td>
<td><span data-ttu-id="f5f4a-225">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="f5f4a-226">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="f5f4a-227">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="f5f4a-228">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="f5f4a-229">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-230">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="f5f4a-231">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-232">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="f5f4a-233">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-234">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="f5f4a-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="f5f4a-235">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="f5f4a-236">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f5f4a-237">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-237">Cost actual</span></span></td>
<td><span data-ttu-id="f5f4a-238">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-239">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-240">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-241">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-242">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f5f4a-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-243">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="f5f4a-244">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-245">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="f5f4a-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="f5f4a-246">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f5f4a-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-247">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-248">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-249">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-250">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f5f4a-251">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f5f4a-252">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f5f4a-253">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-254">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-255">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-256">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="f5f4a-257">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-258">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-258">Billed sales</span></span></td>
<td><span data-ttu-id="f5f4a-259">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f5f4a-260">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f5f4a-261">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f5f4a-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-263">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-264">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-265">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f5f4a-266">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-267">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-268">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-269">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-270">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f5f4a-271">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f5f4a-272">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f5f4a-273">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="f5f4a-274">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f5f4a-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="f5f4a-275">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="f5f4a-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="f5f4a-276">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-277">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="f5f4a-278">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f5f4a-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-279">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f5f4a-279">Billed sales</span></span></td>
<td><span data-ttu-id="f5f4a-280">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f5f4a-281">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f5f4a-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f5f4a-282">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f5f4a-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f5f4a-283">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-284">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f5f4a-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="f5f4a-285">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f5f4a-286">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f5f4a-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="f5f4a-287">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f5f4a-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
