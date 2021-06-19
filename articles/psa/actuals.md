---
title: Επισκόπηση πραγματικών τιμών
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις πραγματικές τιμές έργου.
author: rumant
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
ms.openlocfilehash: 73f1b14bbb4cc53111a1b3a93756a86db04475ab
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014656"
---
# <a name="actuals-overview"></a><span data-ttu-id="f2688-103">Επισκόπηση πραγματικών τιμών</span><span class="sxs-lookup"><span data-stu-id="f2688-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f2688-104">Οι πραγματικές τιμές είναι ο όγκος εργασίας που έχει ολοκληρωθεί σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f2688-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="f2688-105">Οι πραγματικές τιμές του έργου μπορούν να επισημανθούν στα έγγραφα προέλευσης.</span><span class="sxs-lookup"><span data-stu-id="f2688-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="f2688-106">Στα εν λόγω έγγραφα προέλευσης περιλαμβάνονται καταχωρήσεις χρόνου, εξόδων και ημερολογίου καθώς επίσης και τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="f2688-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Πώς ανιχνεύονται οι πραγματικές τιμές του έργου στα έγγραφα προέλευσης](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="f2688-108">Υποβολή χρονικής καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="f2688-108">Submitting a time entry</span></span>

<span data-ttu-id="f2688-109">Στο PSA, όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="f2688-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="f2688-110">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="f2688-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="f2688-111">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="f2688-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="f2688-112">Η λογική για την εισαγωγή προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f2688-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="f2688-113">Όλες οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f2688-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="f2688-114">Αυτά τα πεδία περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="f2688-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="f2688-115">Τα πεδία που επηρεάζουν τις προεπιλεγμένες τιμές, όπως ο **Ρόλος** και η **Οργανική μονάδα** προκαλούν την εισαγωγή μιας κατάλληλης τιμής από προεπιλογή στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f2688-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="f2688-116">Εάν προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση ώρας και θέλετε η τιμή του πεδίου να μεταδοθεί στα πραγματικά στοιχεία, δημιουργήστε το πεδίο στην οντότητα "πραγματικές τιμές" και χρησιμοποιήστε αντιστοιχίσεις πεδίων για να αντιγράψετε το πεδίο από την καταχώρηση χρόνου στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="f2688-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="f2688-117">Υποβολή μιας καταχώρησης εξόδων</span><span class="sxs-lookup"><span data-stu-id="f2688-117">Submitting an expense entry</span></span>

<span data-ttu-id="f2688-118">Στο PSA, όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης "χρόνος και υλικά", δημιουργούνται δύο γραμμές εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="f2688-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="f2688-119">Μια γραμμή είναι για το κόστος και η άλλη γραμμή είναι για τις μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="f2688-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="f2688-120">Όταν υποβάλλεται μια καταχώρηση εξόδων για ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, δημιουργείται μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="f2688-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="f2688-121">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα βασίζεται στην κατηγορία εξόδων που έχει επιλεγεί στη σελίδα **Καταχώρηση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="f2688-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="f2688-122">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="f2688-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="f2688-123">Ωστόσο, για την ίδια την τιμή, το ποσό που εισήγαγε ο χρήστης ορίζεται απευθείας στις σχετικές γραμμές ημερολογίου εξόδων για το κόστος και τις πωλήσεις από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="f2688-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="f2688-124">Στην τρέχουσα έκδοση του PSA, η καταχώρηση με βάση την κατηγορία των προεπιλεγμένων τιμών ανά μονάδα σε καταχωρήσεις εξόδων δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="f2688-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="f2688-125">Χρήση ημερολογίων εγγραφών για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="f2688-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="f2688-126">Στο PSA, τα ημερολόγια εγγραφών σάς επιτρέπουν να καταγράφετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, τον χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="f2688-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="f2688-127">Ένα ημερολόγιο έχει κεφαλίδα, γραμμές και μια **Επιβεβαίωση** ενέργειας.</span><span class="sxs-lookup"><span data-stu-id="f2688-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="f2688-128">Ακολουθούν ορισμένα σενάρια στα οποία μπορείτε να χρησιμοποιήσετε ένα ημερολόγιο:</span><span class="sxs-lookup"><span data-stu-id="f2688-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="f2688-129">Πρέπει να καταγράψετε το πραγματικό κόστος υλικού και τις πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f2688-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="f2688-130">Πρέπει να μετακινήσετε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο PSA.</span><span class="sxs-lookup"><span data-stu-id="f2688-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="f2688-131">Πρέπει να καταγράψετε το κόστος που σημειώθηκε σε ένα άλλο σύστημα, για παράδειγμα, το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="f2688-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f2688-132">Η χρήση ημερολογίων εγγραφών για τη δημιουργία πραγματικών στοιχείων πρέπει να γίνεται μόνο από έναν χρήστη ο οποίος γνωρίζει πλήρως τις λογιστικές επιπτώσεις που έχουν οι πραγματικές τιμές για το έργο.</span><span class="sxs-lookup"><span data-stu-id="f2688-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="f2688-133">Αυτό οφείλεται στο γεγονός ότι η εφαρμογή δεν επικυρώνει τον τύπο της γραμμής ημερολογίου ή τη σχετική τιμολόγηση που καταχωρείται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="f2688-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="f2688-134">Λόγω της επίδρασης αυτού του τύπου ημερολογίου, δείξτε επαρκή προσοχή στο άτομο το οποίο έχει πρόσβαση για τη δημιουργία ημερολογίων εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="f2688-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="f2688-135">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-135">Recording actuals based on project events</span></span>

<span data-ttu-id="f2688-136">Το PSA καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="f2688-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="f2688-137">Αυτές οι συναλλαγές καταγράφονται ως **πραγματικές τιμές**.</span><span class="sxs-lookup"><span data-stu-id="f2688-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="f2688-138">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="f2688-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="f2688-139">**Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="f2688-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="f2688-140">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="f2688-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="f2688-141">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="f2688-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="f2688-142">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="f2688-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="f2688-143">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="f2688-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="f2688-144">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="f2688-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="f2688-145">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f2688-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="f2688-146">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="f2688-146">Actuals</span></span></th>
<th><span data-ttu-id="f2688-147">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f2688-147">Transaction currency</span></span></th>
<th><span data-ttu-id="f2688-148">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f2688-148">Fixed price</span></span></th>
<th><span data-ttu-id="f2688-149">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f2688-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="f2688-150">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f2688-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="f2688-151">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f2688-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-152">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f2688-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="f2688-153">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f2688-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f2688-154">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f2688-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f2688-155">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-155">Cost actual</span></span></td>
<td><span data-ttu-id="f2688-156">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-157">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-158">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="f2688-159">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-160">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-161">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f2688-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="f2688-162">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f2688-163">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f2688-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f2688-164">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-164">Cost actual</span></span></td>
<td><span data-ttu-id="f2688-165">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-166">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-167">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-168">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-169">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-170">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-171">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-172">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-173">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f2688-174">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f2688-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f2688-175">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f2688-176">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-177">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f2688-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-178">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-179">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-180">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-181">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-181">Billed sales</span></span></td>
<td><span data-ttu-id="f2688-182">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f2688-183">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f2688-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f2688-184">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f2688-185">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-186">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-187">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-188">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-189">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-190">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-191">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-192">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-193">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f2688-194">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f2688-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f2688-195">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f2688-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f2688-196">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="f2688-197">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f2688-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="f2688-198">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="f2688-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="f2688-199">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-200">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-201">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-202">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-202">Billed sales</span></span></td>
<td><span data-ttu-id="f2688-203">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f2688-204">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f2688-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f2688-205">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f2688-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f2688-206">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-207">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-208">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-209">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-210">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="f2688-211">**Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου**</span><span class="sxs-lookup"><span data-stu-id="f2688-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="f2688-212">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="f2688-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="f2688-213">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="f2688-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="f2688-214">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="f2688-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="f2688-215">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="f2688-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="f2688-216">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="f2688-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="f2688-217">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f2688-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="f2688-218">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="f2688-218">Actuals</span></span></th>
<th><span data-ttu-id="f2688-219">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f2688-219">Transaction currency</span></span></th>
<th><span data-ttu-id="f2688-220">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="f2688-220">Fixed price</span></span></th>
<th><span data-ttu-id="f2688-221">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="f2688-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="f2688-222">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f2688-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="f2688-223">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f2688-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-224">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="f2688-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="f2688-225">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="f2688-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="f2688-226">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f2688-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f2688-227">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-227">Cost actual</span></span></td>
<td><span data-ttu-id="f2688-228">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="f2688-229">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="f2688-230">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="f2688-231">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="f2688-232">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-233">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f2688-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="f2688-234">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-235">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f2688-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="f2688-236">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f2688-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-237">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="f2688-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="f2688-238">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="f2688-239">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="f2688-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="f2688-240">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-240">Cost actual</span></span></td>
<td><span data-ttu-id="f2688-241">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-242">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-243">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-244">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-245">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="f2688-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-246">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f2688-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="f2688-247">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="f2688-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-248">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="f2688-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="f2688-249">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="f2688-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-250">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-251">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-252">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-253">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f2688-254">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f2688-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f2688-255">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f2688-256">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-257">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f2688-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-258">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-259">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="f2688-260">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-261">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-261">Billed sales</span></span></td>
<td><span data-ttu-id="f2688-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f2688-263">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="f2688-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="f2688-264">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="f2688-265">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-266">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-267">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-268">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="f2688-269">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-270">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-271">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-272">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-273">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="f2688-274">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f2688-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f2688-275">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f2688-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f2688-276">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="f2688-277">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="f2688-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="f2688-278">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="f2688-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="f2688-279">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-280">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="f2688-281">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="f2688-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-282">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="f2688-282">Billed sales</span></span></td>
<td><span data-ttu-id="f2688-283">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="f2688-284">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="f2688-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="f2688-285">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="f2688-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="f2688-286">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-287">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="f2688-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="f2688-288">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="f2688-289">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="f2688-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="f2688-290">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="f2688-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]