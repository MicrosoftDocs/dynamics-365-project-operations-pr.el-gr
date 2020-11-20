---
title: Διορθωμένα τιμολόγια - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα διορθωμένα τιμολόγια στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 55bec8ad1d9c2b55cabb453321f13df8b7cd1614
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176431"
---
# <a name="corrected-invoices---lite"></a><span data-ttu-id="e1a53-103">Διορθωμένα τιμολόγια - lite</span><span class="sxs-lookup"><span data-stu-id="e1a53-103">Corrected invoices - lite</span></span>

<span data-ttu-id="e1a53-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="e1a53-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e1a53-105">Ένα επιβεβαιωμένο τιμολόγιο έργου μπορεί να διορθωθεί για την επεξεργασία αλλαγών ή πιστώσεων σύμφωνα με τις διαπραγματεύσεις του πελάτη και του υπεύθυνου έργου.</span><span class="sxs-lookup"><span data-stu-id="e1a53-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="e1a53-106">Για να κάνετε αλλαγές σε ένα επιβεβαιωμένο τιμολόγιο, ανοίξτε το επιβεβαιωμένο τιμολόγιο και επιλέξτε **Διόρθωση αυτού του τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="e1a53-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="e1a53-107">Αυτή η επιλογή δεν είναι διαθέσιμη, εκτός εάν επιβεβαιωθεί ένα τιμολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="e1a53-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="e1a53-108">Δημιουργείται ένα νέο προσχέδιο τιμολογίου από το επιβεβαιωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="e1a53-109">Όλες οι λεπτομέρειες της γραμμής τιμολογίων από το τιμολόγιο που έχει ήδη επιβεβαιωθεί αντιγράφονται στο νέο προσχέδιο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="e1a53-110">Ακολουθούν ορισμένα από τα βασικά σημεία που πρέπει να κατανοήσετε σχετικά με τις λεπτομέρειες της γραμμής στο νέο διορθωμένο τιμολόγιο:</span><span class="sxs-lookup"><span data-stu-id="e1a53-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="e1a53-111">Όλες οι ποσότητες ενημερώνονται στο μηδέν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-111">All quantities are updated to zero.</span></span> <span data-ttu-id="e1a53-112">Η εφαρμογή προϋποθέτει ότι όλα τα τιμολογημένα στοιχεία πιστώνονται πλήρως.</span><span class="sxs-lookup"><span data-stu-id="e1a53-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="e1a53-113">Εάν χρειάζεται, μπορείτε να ενημερώσετε με μη αυτόματο τρόπο αυτές τις ποσότητες ώστε να αντικατοπτρίζουν την ποσότητα που τιμολογείται και όχι την ποσότητα που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="e1a53-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="e1a53-114">Με βάση την ποσότητα που καταχωρείτε, η εφαρμογή υπολογίζει την πιστωθείσα ποσότητα.</span><span class="sxs-lookup"><span data-stu-id="e1a53-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="e1a53-115">Αυτό το ποσό αντικατοπτρίζεται στις πραγματικές τιμές που δημιουργούνται όταν επιβεβαιώνεται το διορθωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="e1a53-116">Εάν πραγματοποιείτε αλλαγές στο ποσό του φόρου, πρέπει να εισαγάγετε το σωστό ποσό φόρου και όχι το ποσό του φόρου που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="e1a53-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="e1a53-117">Οι γραμμές σύμβασης που έχουν επιβεβαιωθεί προηγουμένως με βάση τα προϊόντα δεν αντιγράφονται.</span><span class="sxs-lookup"><span data-stu-id="e1a53-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="e1a53-118">Η επεξεργασία διορθώσεων σε ένα τιμολόγιο έργου που βασίζεται σε προϊόν δεν υποστηρίζεται.</span><span class="sxs-lookup"><span data-stu-id="e1a53-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="e1a53-119">Οι διορθώσεις ορόσημων διεκπεραιώνονται πάντα ως πλήρεις πιστώσεις.</span><span class="sxs-lookup"><span data-stu-id="e1a53-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="e1a53-120">Τα ποσά προκαταβολής μπορούν να διορθωθούν εάν ο πελάτης τιμολογηθεί για εσφαλμένο ποσό.</span><span class="sxs-lookup"><span data-stu-id="e1a53-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="e1a53-121">Οι συμφωνίες προκαταβολών είναι δυνατό να διορθωθούν εάν χρησιμοποιήθηκε εσφαλμένο ποσό για τη συμφωνία σε σχέση με χρεώσεις σε ένα τιμολόγιο που έχει ήδη επιβεβαιωθεί.</span><span class="sxs-lookup"><span data-stu-id="e1a53-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e1a53-122">Οι λεπτομέρειες της γραμμής τιμολογίου που είναι διορθώσεις σε άλλες ήδη τιμολογημένες χρεώσεις έχουν οριστεί σε **Ναι** στο πεδίο **Διόρθωση**.</span><span class="sxs-lookup"><span data-stu-id="e1a53-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="e1a53-123">Τα τιμολόγια που έχουν διορθωμένες τις λεπτομέρειες της γραμμής τιμολογίου έχουν ένα πεδίο που ονομάζεται **Έχει διορθώσεις** που έχει οριστεί επίσης σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="e1a53-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="e1a53-124">Πραγματικές τιμές που δημιουργήθηκαν με την επιβεβαίωση του διορθωτικού τιμολογίου:</span><span class="sxs-lookup"><span data-stu-id="e1a53-124">Actuals created on Confirmation of a corrective invoice:</span></span>

<span data-ttu-id="e1a53-125">Ακολουθούν οι πραγματικές τιμές που δημιουργήθηκαν από την εφαρμογή κατά την επιβεβαίωση μιας διόρθωσης με βάση τις εργασίες που πραγματοποιήθηκαν στο προσχέδιο διορθωτικού τιμολογίου πριν από την επιβεβαίωση.</span><span class="sxs-lookup"><span data-stu-id="e1a53-125">Below are the actuals created by the application on confirmation of a corrective based on the operations performed on the draft corrective invoice before confirmation.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="e1a53-126">
                    <strong>Σενάριο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1a53-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="e1a53-127">
                    <strong>Πραγματικές τιμές που δημιουργήθηκαν κατά την επιβεβαίωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1a53-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="e1a53-128">Επιβεβαιώστε τη διόρθωση μιας τιμολογημένης προκαταβολής.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1a53-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-129">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e1a53-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="e1a53-130">Αυτό το ποσό είναι θετικό, επειδή έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν τιμολογήθηκε η προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="e1a53-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-131">Δημιουργείται μια πραγματική αντίστροφη τιμή τιμολογημένων πωλήσεων για το ποσό της προκαταβολής με σκοπό την αντιστροφή των αρχικών πωλήσεων που έχουν τιμολογηθεί.</span><span class="sxs-lookup"><span data-stu-id="e1a53-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-132">Δημιουργείται μια νέα πραγματική τιμή τιμολόγησης πωλήσεων για το διορθωμένο ποσό στη γραμμή διορθωμένου τιμολογίου βάσει προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="e1a53-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-133">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού της γραμμής διορθωμένου τιμολογίου βάσει προκαταβολής που θα χρησιμοποιηθεί για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e1a53-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="e1a53-134">Επιβεβαίωση της διόρθωσης μιας προηγούμενης συμφωνίας προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="e1a53-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-135">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e1a53-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="e1a53-136">Αυτό το ποσό είναι θετικό και έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν παρουσιάστηκε προηγούμενη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="e1a53-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-137">Αντίστροφη πραγματική τιμή τιμολογημένων πωλήσεων για το ποσό στο προηγούμενο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-138">Δημιουργείται μια νέα πραγματική τιμή τιμολόγησης πωλήσεων για το διορθωμένο ποσό προκαταβολής στο διορθωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-139">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού από τη διορθωμένη προκαταβολή που θα χρησιμοποιηθεί για συμφωνία σε μετέπειτα τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="e1a53-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1a53-140">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-141">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-142">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e1a53-143">Τιμολόγηση της μερικής πίστωσης σε μια συναλλαγή χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e1a53-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-144">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-145">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e1a53-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-146">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις υπολειπόμενες ώρες και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="e1a53-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1a53-147">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-148">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e1a53-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-149">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e1a53-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="e1a53-150">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-151">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="e1a53-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-152">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e1a53-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-153">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την υπολειπόμενη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="e1a53-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1a53-154">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-154">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-155">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e1a53-155">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-156">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e1a53-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1a53-157">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-157">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-158">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="e1a53-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-159">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="e1a53-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e1a53-160">Η τιμολόγηση της πλήρους πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-160">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-161">Η αντιστροφή των τιμολογημένων πωλήσεων για το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="e1a53-161">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="e1a53-162">Το τιμολόγιο ορόσημου ή η κατάσταση χρέωσης στη γραμμή σύμβασης έργου ενημερώνονται ώστε να είναι **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="e1a53-162">The milestone invoice or billing status on the project contract line is updated to **Ready to Invoice**.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e1a53-163">Η τιμολόγηση της μερικής πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="e1a53-163">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-164">Δεν υποστηρίζονται</span><span class="sxs-lookup"><span data-stu-id="e1a53-164">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="e1a53-165">Πιστώσεις και διορθώσεις μιας ήδη τιμολογημένης γραμμής σύμβασης βασισμένης σε προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="e1a53-165">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="e1a53-166">Δεν υποστηρίζονται</span><span class="sxs-lookup"><span data-stu-id="e1a53-166">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>
