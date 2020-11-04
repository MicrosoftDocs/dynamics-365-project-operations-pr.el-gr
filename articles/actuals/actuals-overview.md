---
title: Πραγματικές τιμές
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με πραγματικές τιμές στο Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 93a945ffbe9c6dd998456b506b95e717ab8fbab7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076906"
---
# <a name="actuals"></a><span data-ttu-id="04dbd-103">Πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="04dbd-103">Actuals</span></span> 

<span data-ttu-id="04dbd-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="04dbd-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="04dbd-105">Οι πραγματικές τιμές είναι ο όγκος εργασίας που έχει ολοκληρωθεί σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="04dbd-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="04dbd-106">Δημιουργούνται ως αποτέλεσμα των καταχωρήσεων χρόνου και εξόδων και των ημερολογιακών εγγραφών και των τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="04dbd-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="04dbd-107">Γραμμές ημερολογίου και υποβολή χρόνου</span><span class="sxs-lookup"><span data-stu-id="04dbd-107">Journal lines and time submission</span></span>

<span data-ttu-id="04dbd-108">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση χρόνου, ανατρέξτε στο θέμα [Επισκόπηση καταχώρησης χρόνου](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="04dbd-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="04dbd-109">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="04dbd-109">Time and materials</span></span>

<span data-ttu-id="04dbd-110">Όταν μια καταχώρηση χρόνου που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="04dbd-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="04dbd-111">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-111">Fixed price</span></span>

<span data-ttu-id="04dbd-112">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει συνδεθεί με μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="04dbd-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="04dbd-113">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="04dbd-113">Default pricing</span></span>

<span data-ttu-id="04dbd-114">Η λογική για τη δημιουργία προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="04dbd-115">Οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="04dbd-116">Αυτές οι τιμές περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="04dbd-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="04dbd-117">Τα πεδία που επηρεάζουν την προεπιλεγμένη τιμολόγηση, όπως ο **Ρόλος** και η **Οργανική μονάδα** χρησιμοποιούνται για τον καθορισμό της κατάλληλης τιμής στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-117">The fields that affect default pricing, such as **Role** and **Org Unit** , are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="04dbd-118">Μπορείτε να προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση χρόνου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="04dbd-119">Αν θέλετε η τιμή του πεδίου να εφαρμοστεί στα πραγματικά στοιχεία, δημιουργήστε το πεδίο στην οντότητα "πραγματικές τιμές" και χρησιμοποιήστε αντιστοιχίσεις πεδίων για να αντιγράψετε το πεδίο από την καταχώρηση χρόνου στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="04dbd-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="04dbd-120">Γραμμές ημερολογίου και υποβολή βασικών εξόδων</span><span class="sxs-lookup"><span data-stu-id="04dbd-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="04dbd-121">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση εξόδων, ανατρέξτε στο θέμα [Επισκόπηση εξόδων](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="04dbd-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="04dbd-122">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="04dbd-122">Time and materials</span></span>

<span data-ttu-id="04dbd-123">Όταν μια καταχώρηση βασικών εξόδων που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="04dbd-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="04dbd-124">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-124">Fixed price</span></span>

<span data-ttu-id="04dbd-125">Όταν υποβάλλεται μια καταχώρηση βασικών εξόδων για ένα έργο που έχει συνδεθεί με μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="04dbd-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="04dbd-126">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="04dbd-126">Default pricing</span></span>

<span data-ttu-id="04dbd-127">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα γίνεται με βάση την κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="04dbd-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="04dbd-128">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="04dbd-129">Ωστόσο, από προεπιλογή, το ποσό που εισήγαγε ο χρήστης για την ίδια την τιμή ορίζεται απευθείας στις σχετικές γραμμές ημερολογίου εξόδων για το κόστος και τις πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="04dbd-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="04dbd-130">Η καταχώρηση με βάση την κατηγορία των προεπιλεγμένων τιμών ανά μονάδα σε καταχωρήσεις εξόδων δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="04dbd-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="04dbd-131">Χρήση ημερολογίων εγγραφών για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="04dbd-131">Use entry journals to record costs</span></span>

<span data-ttu-id="04dbd-132">Μπορείτε να χρησιμοποιήσετε ημερολόγια εγγραφών για να καταγράψετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, το χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="04dbd-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="04dbd-133">Τα ημερολόγια μπορούν να χρησιμοποιηθούν για τους εξής σκοπούς:</span><span class="sxs-lookup"><span data-stu-id="04dbd-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="04dbd-134">Για να καταγράψετε το πραγματικό κόστος υλικού και τις πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="04dbd-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="04dbd-135">Για να μετακινήσετε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="04dbd-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="04dbd-136">Για να καταγράψετε κόστη που έγιναν σε ένα άλλο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="04dbd-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="04dbd-137">Αυτά τα κόστη μπορεί να περιλαμβάνουν το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="04dbd-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="04dbd-138">Η εφαρμογή δεν επικυρώνει τον τύπο της γραμμής ημερολογίου ή τη σχετική τιμολόγηση που καταχωρείται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="04dbd-139">Επομένως, μόνο ένας χρήστης που γνωρίζει πλήρως το λογιστικό αντίκτυπο που έχουν τα πραγματικά στοιχεία στο έργο θα πρέπει να χρησιμοποιεί ημερολόγια εγγραφών για τη δημιουργία πραγματικών στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="04dbd-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="04dbd-140">Λόγω της επίδρασης αυτού του τύπου ημερολογίου, θα πρέπει να επιλέξετε προσεκτικά ποιος έχει πρόσβαση για τη δημιουργία ημερολογίων εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="04dbd-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="04dbd-141">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-141">Record actuals based on project events</span></span>

<span data-ttu-id="04dbd-142">Το Project Operations καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="04dbd-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="04dbd-143">Αυτές οι συναλλαγές καταγράφονται ως πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="04dbd-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="04dbd-144">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="04dbd-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="04dbd-145">Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="04dbd-146">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="04dbd-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="04dbd-147">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="04dbd-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="04dbd-148">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="04dbd-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="04dbd-149">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="04dbd-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="04dbd-150">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="04dbd-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="04dbd-151">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="04dbd-152">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="04dbd-152">Actuals</span></span></th>
<th><span data-ttu-id="04dbd-153">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="04dbd-153">Transaction currency</span></span></th>
<th><span data-ttu-id="04dbd-154">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-154">Fixed price</span></span></th>
<th><span data-ttu-id="04dbd-155">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="04dbd-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="04dbd-156">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="04dbd-157">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="04dbd-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-158">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="04dbd-159">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="04dbd-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="04dbd-160">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="04dbd-161">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-161">Cost actual</span></span></td>
<td><span data-ttu-id="04dbd-162">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-163">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-164">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="04dbd-165">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-166">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-167">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="04dbd-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="04dbd-168">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="04dbd-169">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="04dbd-170">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-170">Cost actual</span></span></td>
<td><span data-ttu-id="04dbd-171">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-172">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-173">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-174">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-175">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-176">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-177">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-178">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-179">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="04dbd-180">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="04dbd-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="04dbd-181">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="04dbd-182">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-183">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="04dbd-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-184">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-185">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-186">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-187">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-187">Billed sales</span></span></td>
<td><span data-ttu-id="04dbd-188">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="04dbd-189">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="04dbd-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="04dbd-190">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="04dbd-191">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-192">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-193">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-194">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-195">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-196">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-197">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-198">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-199">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="04dbd-200">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="04dbd-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="04dbd-201">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="04dbd-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="04dbd-202">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="04dbd-203">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="04dbd-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="04dbd-204">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="04dbd-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="04dbd-205">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-206">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-207">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-208">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-208">Billed sales</span></span></td>
<td><span data-ttu-id="04dbd-209">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="04dbd-210">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="04dbd-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="04dbd-211">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="04dbd-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="04dbd-212">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-213">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-214">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-215">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-216">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="04dbd-217">Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="04dbd-218">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="04dbd-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="04dbd-219">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="04dbd-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="04dbd-220">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="04dbd-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="04dbd-221">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="04dbd-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="04dbd-222">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="04dbd-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="04dbd-223">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="04dbd-224">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="04dbd-224">Actuals</span></span></th>
<th><span data-ttu-id="04dbd-225">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="04dbd-225">Transaction currency</span></span></th>
<th><span data-ttu-id="04dbd-226">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="04dbd-226">Fixed price</span></span></th>
<th><span data-ttu-id="04dbd-227">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="04dbd-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="04dbd-228">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="04dbd-229">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="04dbd-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-230">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="04dbd-231">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="04dbd-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="04dbd-232">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="04dbd-233">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-233">Cost actual</span></span></td>
<td><span data-ttu-id="04dbd-234">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="04dbd-235">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="04dbd-236">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="04dbd-237">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="04dbd-238">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-239">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="04dbd-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="04dbd-240">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-241">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="04dbd-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="04dbd-242">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="04dbd-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-243">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="04dbd-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="04dbd-244">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="04dbd-245">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="04dbd-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="04dbd-246">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-246">Cost actual</span></span></td>
<td><span data-ttu-id="04dbd-247">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-248">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-249">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-250">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-251">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04dbd-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-252">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="04dbd-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="04dbd-253">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="04dbd-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-254">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="04dbd-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="04dbd-255">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="04dbd-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-256">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-257">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-258">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-259">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="04dbd-260">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="04dbd-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="04dbd-261">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="04dbd-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-263">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="04dbd-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-264">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-265">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="04dbd-266">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-267">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-267">Billed sales</span></span></td>
<td><span data-ttu-id="04dbd-268">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="04dbd-269">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="04dbd-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="04dbd-270">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="04dbd-271">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-272">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-273">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-274">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="04dbd-275">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-276">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-277">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-278">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-279">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="04dbd-280">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="04dbd-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="04dbd-281">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="04dbd-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="04dbd-282">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="04dbd-283">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="04dbd-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="04dbd-284">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="04dbd-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="04dbd-285">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-286">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="04dbd-287">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="04dbd-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-288">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04dbd-288">Billed sales</span></span></td>
<td><span data-ttu-id="04dbd-289">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="04dbd-290">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="04dbd-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="04dbd-291">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="04dbd-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="04dbd-292">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-293">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="04dbd-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="04dbd-294">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="04dbd-295">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="04dbd-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="04dbd-296">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="04dbd-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
