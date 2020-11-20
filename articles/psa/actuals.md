---
title: Επισκόπηση πραγματικών τιμών
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις πραγματικές τιμές έργου.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: cf9e36c99790b77f0ed6490f49b4ebeb043bcdf6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129768"
---
# <a name="actuals-overview"></a><span data-ttu-id="4f9fe-103">Επισκόπηση πραγματικών τιμών</span><span class="sxs-lookup"><span data-stu-id="4f9fe-103">Actuals overview</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4f9fe-104">Οι πραγματικές τιμές είναι ο όγκος εργασίας που έχει ολοκληρωθεί σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="4f9fe-105">Οι πραγματικές τιμές του έργου μπορούν να επισημανθούν στα έγγραφα προέλευσης.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="4f9fe-106">Στα εν λόγω έγγραφα προέλευσης περιλαμβάνονται καταχωρήσεις χρόνου, εξόδων και ημερολογίου καθώς επίσης και τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Πώς ανιχνεύονται οι πραγματικές τιμές του έργου στα έγγραφα προέλευσης](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="4f9fe-108">Υποβολή χρονικής καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="4f9fe-108">Submitting a time entry</span></span>

<span data-ttu-id="4f9fe-109">Στο PSA, όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4f9fe-110">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4f9fe-111">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="4f9fe-112">Η λογική για την εισαγωγή προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="4f9fe-113">Όλες οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="4f9fe-114">Αυτά τα πεδία περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="4f9fe-115">Τα πεδία που επηρεάζουν τις προεπιλεγμένες τιμές, όπως ο **Ρόλος** και η **Οργανική μονάδα** προκαλούν την εισαγωγή μιας κατάλληλης τιμής από προεπιλογή στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="4f9fe-116">Εάν προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση ώρας και θέλετε η τιμή του πεδίου να μεταδοθεί στα πραγματικά στοιχεία, δημιουργήστε το πεδίο στην οντότητα "πραγματικές τιμές" και χρησιμοποιήστε αντιστοιχίσεις πεδίων για να αντιγράψετε το πεδίο από την καταχώρηση χρόνου στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="4f9fe-117">Υποβολή μιας καταχώρησης εξόδων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-117">Submitting an expense entry</span></span>

<span data-ttu-id="4f9fe-118">Στο PSA, όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4f9fe-119">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4f9fe-120">Όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="4f9fe-121">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα βασίζεται στην κατηγορία εξόδων που έχει επιλεγεί στη σελίδα **Καταχώρηση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="4f9fe-122">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="4f9fe-123">Ωστόσο, για την ίδια την τιμή, το ποσό που εισήγαγε ο χρήστης ορίζεται απευθείας στις σχετικές γραμμές ημερολογίου εξόδων για το κόστος και τις πωλήσεις από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="4f9fe-124">Στην τρέχουσα έκδοση του PSA, η καταχώρηση με βάση την κατηγορία των προεπιλεγμένων τιμών ανά μονάδα σε καταχωρήσεις εξόδων δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="4f9fe-125">Χρήση ημερολογίων εγγραφών για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="4f9fe-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="4f9fe-126">Στο PSA, τα ημερολόγια εγγραφών σάς επιτρέπουν να καταγράφετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, τον χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="4f9fe-127">Ένα ημερολόγιο έχει κεφαλίδα, γραμμές και μια **Επιβεβαίωση** ενέργειας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="4f9fe-128">Ακολουθούν ορισμένα σενάρια στα οποία μπορείτε να χρησιμοποιήσετε ένα ημερολόγιο:</span><span class="sxs-lookup"><span data-stu-id="4f9fe-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="4f9fe-129">Πρέπει να καταγράψετε το πραγματικό κόστος υλικού και τις πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="4f9fe-130">Πρέπει να μετακινήσετε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο PSA.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="4f9fe-131">Πρέπει να καταγράψετε το κόστος που σημειώθηκε σε ένα άλλο σύστημα, για παράδειγμα, το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4f9fe-132">Η χρήση ημερολογίων εγγραφών για τη δημιουργία πραγματικών στοιχείων πρέπει να γίνεται μόνο από έναν χρήστη ο οποίος γνωρίζει πλήρως τις λογιστικές επιπτώσεις που έχουν οι πραγματικές τιμές για το έργο.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="4f9fe-133">Αυτό οφείλεται στο γεγονός ότι η εφαρμογή δεν επικυρώνει τον τύπο της γραμμής ημερολογίου ή τη σχετική τιμολόγηση που καταχωρείται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="4f9fe-134">Λόγω της επίδρασης αυτού του τύπου ημερολογίου, δείξτε επαρκή προσοχή στο άτομο το οποίο έχει πρόσβαση για τη δημιουργία ημερολογίων εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="4f9fe-135">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-135">Recording actuals based on project events</span></span>

<span data-ttu-id="4f9fe-136">Το PSA καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="4f9fe-137">Αυτές οι συναλλαγές καταγράφονται ως **πραγματικές τιμές**.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="4f9fe-138">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="4f9fe-139">**Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="4f9fe-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4f9fe-140">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="4f9fe-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4f9fe-141">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="4f9fe-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4f9fe-142">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="4f9fe-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4f9fe-143">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4f9fe-144">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="4f9fe-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4f9fe-145">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4f9fe-146">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="4f9fe-146">Actuals</span></span></th>
<th><span data-ttu-id="4f9fe-147">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="4f9fe-147">Transaction currency</span></span></th>
<th><span data-ttu-id="4f9fe-148">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-148">Fixed price</span></span></th>
<th><span data-ttu-id="4f9fe-149">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="4f9fe-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4f9fe-150">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4f9fe-151">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="4f9fe-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-152">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4f9fe-153">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="4f9fe-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4f9fe-154">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4f9fe-155">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-155">Cost actual</span></span></td>
<td><span data-ttu-id="4f9fe-156">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-157">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-158">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="4f9fe-159">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-160">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-161">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4f9fe-162">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4f9fe-163">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4f9fe-164">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-164">Cost actual</span></span></td>
<td><span data-ttu-id="4f9fe-165">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-166">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-167">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-168">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-169">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-170">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-171">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-172">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-173">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4f9fe-174">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4f9fe-175">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4f9fe-176">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-177">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-178">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-179">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-180">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-181">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-181">Billed sales</span></span></td>
<td><span data-ttu-id="4f9fe-182">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4f9fe-183">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4f9fe-184">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4f9fe-185">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-186">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-187">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-188">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-189">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-190">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-191">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-192">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-193">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4f9fe-194">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4f9fe-195">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4f9fe-196">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4f9fe-197">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4f9fe-198">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="4f9fe-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4f9fe-199">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-200">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-201">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-202">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-202">Billed sales</span></span></td>
<td><span data-ttu-id="4f9fe-203">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4f9fe-204">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4f9fe-205">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4f9fe-206">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-207">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-208">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-209">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-210">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="4f9fe-211">**Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="4f9fe-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4f9fe-212">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="4f9fe-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4f9fe-213">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="4f9fe-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4f9fe-214">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="4f9fe-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4f9fe-215">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4f9fe-216">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="4f9fe-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4f9fe-217">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4f9fe-218">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="4f9fe-218">Actuals</span></span></th>
<th><span data-ttu-id="4f9fe-219">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="4f9fe-219">Transaction currency</span></span></th>
<th><span data-ttu-id="4f9fe-220">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-220">Fixed price</span></span></th>
<th><span data-ttu-id="4f9fe-221">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="4f9fe-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4f9fe-222">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4f9fe-223">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="4f9fe-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-224">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4f9fe-225">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="4f9fe-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="4f9fe-226">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4f9fe-227">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-227">Cost actual</span></span></td>
<td><span data-ttu-id="4f9fe-228">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4f9fe-229">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4f9fe-230">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4f9fe-231">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4f9fe-232">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-233">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4f9fe-234">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-235">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4f9fe-236">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-237">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="4f9fe-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4f9fe-238">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="4f9fe-239">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4f9fe-240">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-240">Cost actual</span></span></td>
<td><span data-ttu-id="4f9fe-241">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-242">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-243">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-244">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-245">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="4f9fe-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-246">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4f9fe-247">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-248">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="4f9fe-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4f9fe-249">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="4f9fe-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-250">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-251">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-252">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-253">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4f9fe-254">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4f9fe-255">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4f9fe-256">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-257">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-258">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-259">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4f9fe-260">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-261">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-261">Billed sales</span></span></td>
<td><span data-ttu-id="4f9fe-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4f9fe-263">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4f9fe-264">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4f9fe-265">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-266">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-267">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-268">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4f9fe-269">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-270">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-271">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-272">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-273">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4f9fe-274">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4f9fe-275">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4f9fe-276">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4f9fe-277">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="4f9fe-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4f9fe-278">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="4f9fe-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4f9fe-279">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-280">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4f9fe-281">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="4f9fe-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-282">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="4f9fe-282">Billed sales</span></span></td>
<td><span data-ttu-id="4f9fe-283">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4f9fe-284">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="4f9fe-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4f9fe-285">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="4f9fe-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4f9fe-286">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-287">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="4f9fe-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4f9fe-288">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4f9fe-289">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="4f9fe-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4f9fe-290">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="4f9fe-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
