---
title: Δημιουργία διορθωτικών τιμολογίων βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα διορθωτικά τιμολόγια στο Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0423fe9895b91431b2a83a8fff81118205b0736
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001614"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="e0f62-103">Δημιουργία διορθωτικών τιμολογίων βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="e0f62-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="e0f62-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="e0f62-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e0f62-105">Ένα επιβεβαιωμένο τιμολόγιο έργου μπορεί να διορθωθεί για την επεξεργασία αλλαγών ή πιστώσεων σύμφωνα με τις διαπραγματεύσεις του πελάτη και του υπεύθυνου έργου.</span><span class="sxs-lookup"><span data-stu-id="e0f62-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="e0f62-106">Για να κάνετε αλλαγές σε ένα επιβεβαιωμένο τιμολόγιο, ανοίξτε το επιβεβαιωμένο τιμολόγιο και επιλέξτε **Διόρθωση αυτού του τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="e0f62-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="e0f62-107">Αυτή η επιλογή δεν είναι διαθέσιμη, εκτός εάν επιβεβαιωθεί ένα τιμολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="e0f62-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="e0f62-108">Δημιουργείται ένα νέο προσχέδιο τιμολογίου από το επιβεβαιωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="e0f62-109">Όλες οι λεπτομέρειες της γραμμής τιμολογίων από το τιμολόγιο που έχει ήδη επιβεβαιωθεί αντιγράφονται στο νέο προσχέδιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="e0f62-110">Ακολουθούν ορισμένα βασικά σημεία που θα σας βοηθήσουν να κατανοήσετε περισσότερα σχετικά με τις λεπτομέρειες γραμμής στο νέο διορθωμένο τιμολόγιο:</span><span class="sxs-lookup"><span data-stu-id="e0f62-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="e0f62-111">Όλες οι ποσότητες ενημερώνονται στο μηδέν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-111">All quantities are updated to zero.</span></span> <span data-ttu-id="e0f62-112">Αυτό προϋποθέτει ότι όλα τα στοιχεία που έχουν τιμολογηθεί έχουν πιστωθεί πλήρως.</span><span class="sxs-lookup"><span data-stu-id="e0f62-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="e0f62-113">Εάν χρειάζεται, μπορείτε να ενημερώσετε με μη αυτόματο τρόπο αυτές τις ποσότητες ώστε να αντικατοπτρίζουν την ποσότητα που τιμολογείται και όχι την ποσότητα που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="e0f62-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="e0f62-114">Με βάση την ποσότητα που καταχωρείτε, η εφαρμογή υπολογίζει την πιστωθείσα ποσότητα.</span><span class="sxs-lookup"><span data-stu-id="e0f62-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="e0f62-115">Αυτό το ποσό αντικατοπτρίζεται στις πραγματικές τιμές που δημιουργούνται όταν επιβεβαιώνεται το διορθωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="e0f62-116">Εάν πραγματοποιείτε αλλαγές στο ποσό του φόρου, πρέπει να εισαγάγετε το σωστό ποσό φόρου και όχι το ποσό του φόρου που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="e0f62-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="e0f62-117">Οι διορθώσεις ορόσημων διεκπεραιώνονται πάντα ως πλήρεις πιστώσεις.</span><span class="sxs-lookup"><span data-stu-id="e0f62-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="e0f62-118">Τα ποσά προκαταβολής μπορούν να διορθωθούν εάν ο πελάτης τιμολογηθεί για εσφαλμένο ποσό.</span><span class="sxs-lookup"><span data-stu-id="e0f62-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="e0f62-119">Οι συμφωνίες προκαταβολών είναι δυνατό να διορθωθούν εάν χρησιμοποιήθηκε εσφαλμένο ποσό για τη συμφωνία σε σχέση με χρεώσεις σε ένα τιμολόγιο που έχει ήδη επιβεβαιωθεί.</span><span class="sxs-lookup"><span data-stu-id="e0f62-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e0f62-120">Οι λεπτομέρειες γραμμής τιμολογίου που είναι διορθώσεις σε άλλες ήδη τιμολογημένες χρεώσεις, έχουν ορίσει το πεδίο **Διόρθωση** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="e0f62-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="e0f62-121">Τα τιμολόγια που έχουν διορθωμένες τις λεπτομέρειες της γραμμής τιμολογίου έχουν ένα πεδίο που ονομάζεται **Έχει διορθώσεις** που έχει οριστεί επίσης σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="e0f62-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="e0f62-122">Πραγματικές τιμές που δημιουργήθηκαν με την επιβεβαίωση του διορθωτικού τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="e0f62-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="e0f62-123">Ο παρακάτω πίνακας περιλαμβάνει τις πραγματικές τιμές που δημιουργούνται όταν επιβεβαιωθεί ένα διορθωτικό τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="e0f62-124">
                    <strong>Σενάριο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e0f62-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="e0f62-125">
                    <strong>Πραγματικές τιμές που δημιουργήθηκαν κατά την επιβεβαίωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e0f62-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="e0f62-126">Επιβεβαιώστε τη διόρθωση μιας τιμολογημένης προκαταβολής.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e0f62-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-127">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e0f62-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="e0f62-128">Αυτό το ποσό είναι θετικό, επειδή έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν τιμολογήθηκε η προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="e0f62-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-129">Δημιουργείται μια πραγματική αντίστροφη τιμή τιμολογημένων πωλήσεων για το ποσό της προκαταβολής με σκοπό την αντιστροφή των αρχικών πωλήσεων που έχουν τιμολογηθεί.</span><span class="sxs-lookup"><span data-stu-id="e0f62-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-130">Δημιουργείται μια νέα πραγματική τιμή τιμολόγησης πωλήσεων για το διορθωμένο ποσό στη γραμμή διορθωμένου τιμολογίου βάσει προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="e0f62-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-131">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού της γραμμής διορθωμένου τιμολογίου βάσει προκαταβολής που θα χρησιμοποιηθεί για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e0f62-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="e0f62-132">Επιβεβαίωση της διόρθωσης μιας προηγούμενης συμφωνίας προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="e0f62-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-133">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e0f62-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="e0f62-134">Αυτό το ποσό είναι θετικό και έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν παρουσιάστηκε προηγούμενη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e0f62-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-135">Αντίστροφη πραγματική τιμή τιμολογημένων πωλήσεων για το ποσό στο προηγούμενο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-136">Δημιουργείται μια νέα πραγματική τιμή τιμολόγησης πωλήσεων για το διορθωμένο ποσό προκαταβολής στο διορθωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-137">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού από τη διορθωμένη προκαταβολή που θα χρησιμοποιηθεί για συμφωνία σε μετέπειτα τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="e0f62-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e0f62-138">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-139">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-140">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e0f62-141">Τιμολόγηση της μερικής πίστωσης σε μια συναλλαγή χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e0f62-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-142">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-143">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e0f62-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-144">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις υπολειπόμενες ώρες και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="e0f62-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e0f62-145">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-146">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e0f62-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-147">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e0f62-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e0f62-148">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-149">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e0f62-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-150">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e0f62-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-151">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την υπολειπόμενη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="e0f62-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e0f62-152">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-153">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e0f62-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-154">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e0f62-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e0f62-155">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-156">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e0f62-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-157">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e0f62-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e0f62-158">Η τιμολόγηση της πλήρους πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-159">Η αντιστροφή των τιμολογημένων πωλήσεων για το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="e0f62-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="e0f62-160">Η κατάσταση τιμολογίου για το ορόσημο ενημερώνεται από το <b>Αναρτημένο τιμολόγιο πελάτη</b> στο <b>Έτοιμο για τιμολόγηση</b>.</span><span class="sxs-lookup"><span data-stu-id="e0f62-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e0f62-161">Η τιμολόγηση της μερικής πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e0f62-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e0f62-162">Δεν υποστηρίζονται</span><span class="sxs-lookup"><span data-stu-id="e0f62-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
