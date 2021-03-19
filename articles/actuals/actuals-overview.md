---
title: Πραγματικές τιμές
description: Αυτό θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εργασίας με τις πραγματικές τιμές στο Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 6a94bd143b0d0dad2a08511a34e592a057b6d2a1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291799"
---
# <a name="actuals"></a><span data-ttu-id="38ab8-103">Πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="38ab8-103">Actuals</span></span> 

<span data-ttu-id="38ab8-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="38ab8-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="38ab8-105">Οι πραγματικές τιμές είναι ο όγκος εργασίας που έχει ολοκληρωθεί σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="38ab8-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="38ab8-106">Δημιουργούνται ως αποτέλεσμα των καταχωρήσεων χρόνου και εξόδων και των ημερολογιακών εγγραφών και των τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="38ab8-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="38ab8-107">Γραμμές ημερολογίου και υποβολή χρόνου</span><span class="sxs-lookup"><span data-stu-id="38ab8-107">Journal lines and time submission</span></span>

<span data-ttu-id="38ab8-108">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση χρόνου, ανατρέξτε στο θέμα [Επισκόπηση καταχώρησης χρόνου](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="38ab8-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="38ab8-109">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="38ab8-109">Time and materials</span></span>

<span data-ttu-id="38ab8-110">Όταν μια καταχώρηση χρόνου που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="38ab8-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="38ab8-111">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-111">Fixed price</span></span>

<span data-ttu-id="38ab8-112">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει συνδεθεί με μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="38ab8-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="38ab8-113">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="38ab8-113">Default pricing</span></span>

<span data-ttu-id="38ab8-114">Η λογική για τη δημιουργία προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="38ab8-115">Οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="38ab8-116">Αυτές οι τιμές περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="38ab8-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="38ab8-117">Τα πεδία που επηρεάζουν την προεπιλεγμένη τιμολόγηση, όπως ο **Ρόλος** και η **Οργανική μονάδα** χρησιμοποιούνται για τον καθορισμό της κατάλληλης τιμής στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="38ab8-118">Μπορείτε να προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση χρόνου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="38ab8-119">Αν θέλετε η τιμή του πεδίου να εφαρμοστεί στα πραγματικά στοιχεία, δημιουργήστε το πεδίο στην οντότητα "πραγματικές τιμές" και χρησιμοποιήστε αντιστοιχίσεις πεδίων για να αντιγράψετε το πεδίο από την καταχώρηση χρόνου στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="38ab8-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="38ab8-120">Γραμμές ημερολογίου και υποβολή βασικών εξόδων</span><span class="sxs-lookup"><span data-stu-id="38ab8-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="38ab8-121">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση εξόδων, ανατρέξτε στο θέμα [Επισκόπηση εξόδων](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="38ab8-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="38ab8-122">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="38ab8-122">Time and materials</span></span>

<span data-ttu-id="38ab8-123">Όταν μια καταχώρηση βασικών εξόδων που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="38ab8-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="38ab8-124">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-124">Fixed price</span></span>

<span data-ttu-id="38ab8-125">Όταν υποβάλλεται μια καταχώρηση βασικών εξόδων για ένα έργο που έχει συνδεθεί με μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="38ab8-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="38ab8-126">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="38ab8-126">Default pricing</span></span>

<span data-ttu-id="38ab8-127">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα γίνεται με βάση την κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="38ab8-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="38ab8-128">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="38ab8-129">Ωστόσο, από προεπιλογή, το ποσό που εισήγαγε ο χρήστης για την ίδια την τιμή ορίζεται απευθείας στις σχετικές γραμμές ημερολογίου εξόδων για το κόστος και τις πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="38ab8-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="38ab8-130">Η καταχώρηση με βάση την κατηγορία των προεπιλεγμένων τιμών ανά μονάδα σε καταχωρήσεις εξόδων δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="38ab8-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="38ab8-131">Χρήση ημερολογίων εγγραφών για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="38ab8-131">Use entry journals to record costs</span></span>

<span data-ttu-id="38ab8-132">Μπορείτε να χρησιμοποιήσετε ημερολόγια εγγραφών για να καταγράψετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, το χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="38ab8-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="38ab8-133">Τα ημερολόγια μπορούν να χρησιμοποιηθούν για τους εξής σκοπούς:</span><span class="sxs-lookup"><span data-stu-id="38ab8-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="38ab8-134">Για να καταγράψετε το πραγματικό κόστος υλικού και τις πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="38ab8-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="38ab8-135">Μετακινήστε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="38ab8-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="38ab8-136">Για να καταγράψετε κόστη που έγιναν σε ένα άλλο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="38ab8-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="38ab8-137">Αυτά τα κόστη μπορεί να περιλαμβάνουν το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="38ab8-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="38ab8-138">Η εφαρμογή δεν επικυρώνει τον τύπο της γραμμής ημερολογίου ή τη σχετική τιμολόγηση που καταχωρείται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="38ab8-139">Επομένως, μόνο ένας χρήστης που γνωρίζει πλήρως το λογιστικό αντίκτυπο που έχουν τα πραγματικά στοιχεία στο έργο θα πρέπει να χρησιμοποιεί ημερολόγια εγγραφών για τη δημιουργία πραγματικών στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="38ab8-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="38ab8-140">Λόγω της επίδρασης αυτού του τύπου ημερολογίου, θα πρέπει να επιλέξετε προσεκτικά ποιος έχει πρόσβαση για τη δημιουργία ημερολογίων εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="38ab8-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="38ab8-141">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-141">Record actuals based on project events</span></span>

<span data-ttu-id="38ab8-142">Το Project Operations καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="38ab8-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="38ab8-143">Αυτές οι συναλλαγές καταγράφονται ως πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="38ab8-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="38ab8-144">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="38ab8-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="38ab8-145">Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="38ab8-146">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="38ab8-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="38ab8-147">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="38ab8-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="38ab8-148">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="38ab8-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="38ab8-149">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="38ab8-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="38ab8-150">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="38ab8-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="38ab8-151">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="38ab8-152">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="38ab8-152">Actuals</span></span></th>
<th><span data-ttu-id="38ab8-153">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="38ab8-153">Transaction currency</span></span></th>
<th><span data-ttu-id="38ab8-154">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-154">Fixed price</span></span></th>
<th><span data-ttu-id="38ab8-155">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="38ab8-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="38ab8-156">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="38ab8-157">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="38ab8-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-158">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="38ab8-159">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="38ab8-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="38ab8-160">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="38ab8-161">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-161">Cost actual</span></span></td>
<td><span data-ttu-id="38ab8-162">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-163">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-164">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="38ab8-165">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-166">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-167">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="38ab8-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="38ab8-168">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="38ab8-169">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="38ab8-170">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-170">Cost actual</span></span></td>
<td><span data-ttu-id="38ab8-171">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-172">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-173">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-174">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-175">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-176">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-177">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-178">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-179">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="38ab8-180">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="38ab8-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="38ab8-181">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="38ab8-182">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-183">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="38ab8-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-184">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-185">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-186">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-187">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-187">Billed sales</span></span></td>
<td><span data-ttu-id="38ab8-188">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="38ab8-189">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="38ab8-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="38ab8-190">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="38ab8-191">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-192">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-193">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-194">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-195">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-196">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-197">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-198">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-199">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="38ab8-200">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="38ab8-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="38ab8-201">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="38ab8-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="38ab8-202">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="38ab8-203">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="38ab8-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="38ab8-204">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="38ab8-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="38ab8-205">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-206">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-207">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-208">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-208">Billed sales</span></span></td>
<td><span data-ttu-id="38ab8-209">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="38ab8-210">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="38ab8-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="38ab8-211">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="38ab8-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="38ab8-212">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-213">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-214">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-215">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-216">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="38ab8-217">Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="38ab8-218">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="38ab8-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="38ab8-219">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="38ab8-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="38ab8-220">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="38ab8-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="38ab8-221">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="38ab8-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="38ab8-222">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="38ab8-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="38ab8-223">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="38ab8-224">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="38ab8-224">Actuals</span></span></th>
<th><span data-ttu-id="38ab8-225">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="38ab8-225">Transaction currency</span></span></th>
<th><span data-ttu-id="38ab8-226">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="38ab8-226">Fixed price</span></span></th>
<th><span data-ttu-id="38ab8-227">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="38ab8-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="38ab8-228">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="38ab8-229">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="38ab8-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-230">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="38ab8-231">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="38ab8-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="38ab8-232">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="38ab8-233">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-233">Cost actual</span></span></td>
<td><span data-ttu-id="38ab8-234">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="38ab8-235">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="38ab8-236">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="38ab8-237">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="38ab8-238">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-239">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="38ab8-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="38ab8-240">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-241">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="38ab8-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="38ab8-242">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="38ab8-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-243">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="38ab8-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="38ab8-244">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="38ab8-245">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="38ab8-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="38ab8-246">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-246">Cost actual</span></span></td>
<td><span data-ttu-id="38ab8-247">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-248">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-249">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-250">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-251">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="38ab8-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-252">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="38ab8-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="38ab8-253">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="38ab8-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-254">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="38ab8-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="38ab8-255">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="38ab8-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-256">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-257">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-258">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-259">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="38ab8-260">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="38ab8-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="38ab8-261">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="38ab8-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-263">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="38ab8-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-264">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-265">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="38ab8-266">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-267">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-267">Billed sales</span></span></td>
<td><span data-ttu-id="38ab8-268">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="38ab8-269">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="38ab8-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="38ab8-270">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="38ab8-271">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-272">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-273">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-274">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="38ab8-275">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-276">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-277">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-278">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-279">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="38ab8-280">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="38ab8-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="38ab8-281">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="38ab8-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="38ab8-282">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="38ab8-283">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="38ab8-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="38ab8-284">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="38ab8-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="38ab8-285">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-286">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="38ab8-287">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="38ab8-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-288">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="38ab8-288">Billed sales</span></span></td>
<td><span data-ttu-id="38ab8-289">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="38ab8-290">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="38ab8-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="38ab8-291">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="38ab8-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="38ab8-292">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-293">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="38ab8-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="38ab8-294">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="38ab8-295">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="38ab8-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="38ab8-296">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="38ab8-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]