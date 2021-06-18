---
title: Διορθωτικά τιμολόγια βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας και επιβεβαίωσης διορθωτικών τιμολογίων βάσει έργου στο Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012271"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="aafe2-103">Διορθωτικά τιμολόγια βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="aafe2-103">Corrective project-based invoices</span></span>

<span data-ttu-id="aafe2-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="aafe2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="aafe2-105">Ένα επιβεβαιωμένο τιμολόγιο έργου μπορεί να διορθωθεί για την επεξεργασία αλλαγών ή πιστώσεων σύμφωνα με τις διαπραγματεύσεις του πελάτη και του υπεύθυνου έργου.</span><span class="sxs-lookup"><span data-stu-id="aafe2-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="aafe2-106">Για να κάνετε αλλαγές σε ένα επιβεβαιωμένο τιμολόγιο, ανοίξτε το επιβεβαιωμένο τιμολόγιο και επιλέξτε **Διόρθωση αυτού του τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="aafe2-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="aafe2-107">Αυτή η επιλογή δεν είναι διαθέσιμη εκτός εάν επιβεβαιωθεί ένα τιμολόγιο έργου ή εάν το τιμολόγιο βάσει έργου έχει προκαταβολές ή διευθετήσεις προκαταβολών.</span><span class="sxs-lookup"><span data-stu-id="aafe2-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="aafe2-108">Δημιουργείται ένα νέο προσχέδιο τιμολογίου από το επιβεβαιωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="aafe2-109">Όλες οι λεπτομέρειες της γραμμής τιμολογίων από το τιμολόγιο που έχει ήδη επιβεβαιωθεί αντιγράφονται στο νέο προσχέδιο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="aafe2-110">Ακολουθούν ορισμένα από τα βασικά σημεία που πρέπει να κατανοήσετε σχετικά με τις λεπτομέρειες της γραμμής στο νέο διορθωμένο τιμολόγιο:</span><span class="sxs-lookup"><span data-stu-id="aafe2-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="aafe2-111">Όλες οι ποσότητες ενημερώνονται στο μηδέν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-111">All quantities are updated to zero.</span></span> <span data-ttu-id="aafe2-112">Το Dynamics 365 Project Operations προϋποθέτει ότι όλα τα στοιχεία που έχουν τιμολογηθεί έχουν πιστωθεί πλήρως.</span><span class="sxs-lookup"><span data-stu-id="aafe2-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="aafe2-113">Εάν χρειάζεται, μπορείτε να ενημερώσετε με μη αυτόματο τρόπο αυτές τις ποσότητες ώστε να αντικατοπτρίζουν την ποσότητα που τιμολογείται και όχι την ποσότητα που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="aafe2-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="aafe2-114">Με βάση την ποσότητα που καταχωρείτε, η εφαρμογή υπολογίζει την πιστωθείσα ποσότητα.</span><span class="sxs-lookup"><span data-stu-id="aafe2-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="aafe2-115">Αυτό το ποσό αντικατοπτρίζεται στις πραγματικές τιμές που δημιουργούνται όταν επιβεβαιώνεται το διορθωμένο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="aafe2-116">Εάν πραγματοποιείτε αλλαγές στο ποσό του φόρου, πρέπει να εισαγάγετε το σωστό ποσό φόρου και όχι το ποσό του φόρου που πιστώνεται.</span><span class="sxs-lookup"><span data-stu-id="aafe2-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="aafe2-117">Οι διορθώσεις ορόσημων διεκπεραιώνονται πάντα ως πλήρεις πιστώσεις.</span><span class="sxs-lookup"><span data-stu-id="aafe2-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="aafe2-118">Για λεπτομέρειες γραμμής τιμολογίου που είναι διορθώσεις σε άλλες ήδη τιμολογημένες χρεώσεις, το πεδίο **Διόρθωση** ορίζεται σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="aafe2-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="aafe2-119">Για τιμολόγια που έχουν διορθωμένες λεπτομέρειες γραμμής τιμολογίου το πεδίο **Έχει διορθώσεις** ορίζεται σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="aafe2-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="aafe2-120">Πραγματικές τιμές που δημιουργήθηκαν όταν επιβεβαιώθηκε ένα διορθωτικό τιμολόγιο</span><span class="sxs-lookup"><span data-stu-id="aafe2-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="aafe2-121">Ο παρακάτω πίνακας περιλαμβάνει τις πραγματικές τιμές που δημιουργούνται όταν επιβεβαιωθεί ένα διορθωτικό τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="aafe2-122">
                    <strong>Σενάριο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="aafe2-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="aafe2-123">
                    <strong>Πραγματικές τιμές που δημιουργήθηκαν κατά την επιβεβαίωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="aafe2-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="aafe2-124">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-125">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-126">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για τις ώρες και το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="aafe2-127">Τιμολόγηση της μερικής πίστωσης σε μια συναλλαγή χρόνου.</span><span class="sxs-lookup"><span data-stu-id="aafe2-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-128">Η αντιστροφή των τιμολογημένων πωλήσεων για τις ώρες και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για το χρόνο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-129">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="aafe2-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-130">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις υπολειπόμενες ώρες και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="aafe2-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="aafe2-131">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-132">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="aafe2-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-133">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="aafe2-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="aafe2-134">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής δαπανών που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-135">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="aafe2-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-136">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="aafe2-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-137">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την υπολειπόμενη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="aafe2-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="aafe2-138">Τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής υλικού που είχε τιμολογηθεί προηγουμένως.</span><span class="sxs-lookup"><span data-stu-id="aafe2-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-139">Μια αντιστροφή τιμολογημένων πωλήσεων για την ποσότητα και το ποσό στη λεπτομέρεια της γραμμής του αρχικού τιμολογίου για υλικά.</span><span class="sxs-lookup"><span data-stu-id="aafe2-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-140">Μια νέα πραγματική τιμή μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό στη λεπτομέρεια της γραμμής του αρχικού τιμολογίου για υλικά.</span><span class="sxs-lookup"><span data-stu-id="aafe2-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="aafe2-141">Τιμολόγηση της μερικής πίστωσης σε μια σημαντική συναλλαγή.</span><span class="sxs-lookup"><span data-stu-id="aafe2-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-142">Μια αντιστροφή τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκαν στη λεπτομέρεια της γραμμής του αρχικού τιμολογίου για υλικά.</span><span class="sxs-lookup"><span data-stu-id="aafe2-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-143">Ένα νέο μη τιμολογημένο πραγματικό ποσό πωλήσεων που μπορεί να χρεωθεί για την ποσότητα και το ποσό στη λεπτομέρεια της γραμμής επεξεργασμένου τιμολογίου, μια αντιστροφή για αυτό και μια ισοδύναμη πραγματική τιμή τιμολογημένων πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="aafe2-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-144">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την υπολειπόμενη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στη λεπτομέρεια της γραμμής τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="aafe2-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="aafe2-145">Η τιμολόγηση της πλήρους πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-146">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="aafe2-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-147">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="aafe2-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="aafe2-148">Η τιμολόγηση της μερικής πίστωσης μιας συναλλαγής που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-149">Η αντιστροφή των τιμολογημένων πωλήσεων για την ποσότητα και το ποσό που τιμολογήθηκε στην αρχική λεπτομέρεια της γραμμής τιμολογίου για τη χρέωση.</span><span class="sxs-lookup"><span data-stu-id="aafe2-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-150">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στη διορθωμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή αυτού και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="aafe2-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="aafe2-151">Η τιμολόγηση της πλήρους πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-152">Η αντιστροφή των τιμολογημένων πωλήσεων για το ποσό της αρχικής λεπτομέρειας της γραμμής τιμολογίου για το ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="aafe2-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="aafe2-153">Η κατάσταση τιμολογίου του ορόσημου ενημερώνεται από το <b>Αναρτημένο τιμολόγιο πελάτη</b> στο <b>Έτοιμο για τιμολόγηση</b>.</span><span class="sxs-lookup"><span data-stu-id="aafe2-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="aafe2-154">Η τιμολόγηση της μερικής πίστωσης ενός ορόσημου που έχει τιμολογηθεί στο παρελθόν.</span><span class="sxs-lookup"><span data-stu-id="aafe2-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="aafe2-155">Αυτό το σενάριο δεν υποστηρίζεται.</span><span class="sxs-lookup"><span data-stu-id="aafe2-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
