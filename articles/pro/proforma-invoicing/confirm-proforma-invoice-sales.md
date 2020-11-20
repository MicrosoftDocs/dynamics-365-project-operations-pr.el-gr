---
title: Επιβεβαίωση προτιμολογίου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την επιβεβαίωση προτιμολογίων στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 02b671e4ad327b2448529d7119211613f3a9cb27
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176521"
---
# <a name="confirm-a-proforma-invoice---lite"></a><span data-ttu-id="7135c-103">Επιβεβαίωση προτιμολογίου - lite</span><span class="sxs-lookup"><span data-stu-id="7135c-103">Confirm a proforma invoice - lite</span></span>

<span data-ttu-id="7135c-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="7135c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="7135c-105">Αφού επιβεβαιωθεί ένα προτιμολόγιο, η κατάσταση των ενημερώσεων του τιμολογίου έργου θα είναι **Επιβεβαιώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="7135c-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="7135c-106">Όταν επιβεβαιώνεται ένα τιμολόγιο, γίνεται μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="7135c-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="7135c-107">Προχωρώντας, το τιμολόγιο μπορεί να διορθωθεί μόνο εάν υπάρχουν διορθώσεις ή πιστώσεις που έχουν προετοιμαστεί από τον πελάτη ή όταν έχει επισημανθεί ως πληρωμένο.</span><span class="sxs-lookup"><span data-stu-id="7135c-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="7135c-108">Στον ακόλουθο πίνακα παρουσιάζονται οι πραγματικές τιμές που δημιουργούνται από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="7135c-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="7135c-109">Αυτές οι πραγματικές τιμές δημιουργούνται όταν εκτελούνται συγκεκριμένες λειτουργίες στο προσχέδιο τιμολογίου πριν επιβεβαιωθεί.</span><span class="sxs-lookup"><span data-stu-id="7135c-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="7135c-110">
                    <strong>Σενάριο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7135c-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="7135c-111">
                    <strong>Πραγματικές τιμές που δημιουργήθηκαν κατά την επιβεβαίωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7135c-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-112">Τιμολόγηση προκαταβολής ή προπληρωμής</span><span class="sxs-lookup"><span data-stu-id="7135c-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-113">Μια πραγματική τιμολογημένη πώληση τύπου <strong>Προκαταβολή</strong> δημιουργείται για το ποσό της προκαταβολής ή της προπληρωμής.</span><span class="sxs-lookup"><span data-stu-id="7135c-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-114">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού της προκαταβολής ή της προπληρωμής που θα χρησιμοποιηθεί για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="7135c-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-115">Αφού γίνει πλήρης συμφωνία μιας προκαταβολής ή μιας προπληρωμής σε ένα τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="7135c-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-116">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="7135c-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="7135c-117">Αυτό το ποσό είναι θετικό, επειδή έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν τιμολογήθηκε η προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="7135c-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-118">Πραγματική τιμολογημένη πώληση για το ποσό σε αυτό το τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="7135c-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="7135c-119">Αφού γίνει μερική συμφωνία μιας προκαταβολής ή μιας προπληρωμής σε ένα τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="7135c-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-120">Μια αντιστροφή των πωλήσεων που δεν έχουν τιμολογηθεί για την προκαταβολή που δημιουργήθηκε για τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="7135c-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="7135c-121">Αυτό το ποσό είναι θετικό, επειδή έχει ως στόχο την ακύρωση του αρνητικού που δημιουργήθηκε όταν τιμολογήθηκε η προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="7135c-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-122">Πραγματική τιμολογημένη πώληση για το ποσό σε αυτό το τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="7135c-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-123">Μια μη τιμολογημένη πραγματική τιμή πώλησης αρνητικού ποσού της υπόλοιπης προκαταβολής ή της προπληρωμής που θα χρησιμοποιηθεί για τη συμφωνία σε μελλοντικά τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="7135c-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-124">Τιμολόγηση μιας συναλλαγής χρόνου χωρίς καμία επεξεργασία στο προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="7135c-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-125">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="7135c-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-126">Η πραγματική τιμολογημένη πώληση για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="7135c-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="7135c-127">Τιμολόγηση μιας συναλλαγής χρόνου που έχει υποστεί επεξεργασία για τη μείωση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="7135c-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-128">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="7135c-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-129">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-130">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης είναι μη χρεώσιμη για τις υπόλοιπες ώρες και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-131">Τιμολόγηση μιας συναλλαγής χρόνου που έχει υποστεί επεξεργασία για την αύξηση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="7135c-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-132">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="7135c-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-133">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-134">Τιμολόγηση μιας συναλλαγής εξόδων χωρίς καμία επεξεργασία στο προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="7135c-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-135">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="7135c-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-136">Η τιμολογημένη πραγματική πώληση για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="7135c-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="7135c-137">Τιμολόγηση μιας συναλλαγής εξόδων που έχει υποστεί επεξεργασία για τη μείωση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="7135c-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-138">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="7135c-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-139">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-140">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης είναι μη χρεώσιμη για την υπόλοιπη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-141">Τιμολόγηση μιας συναλλαγής εξόδων που έχει υποστεί επεξεργασία για την αύξηση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="7135c-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-142">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="7135c-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-143">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="7135c-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7135c-144">Τιμολόγηση μιας αμοιβής.</span><span class="sxs-lookup"><span data-stu-id="7135c-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-145">Η αντιστροφή των μη τιμολογημένων πωλήσεων για το ποσό αμοιβής στην αρχική γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="7135c-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-146">Η τιμολογημένη πραγματική πώληση για την ποσότητα και το ποσό της αρχικής γραμμής ημερολογίου αμοιβής.</span><span class="sxs-lookup"><span data-stu-id="7135c-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="7135c-147">Τιμολόγηση ενός ορόσημου.</span><span class="sxs-lookup"><span data-stu-id="7135c-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-148">Η τιμολογημένη πραγματική πώληση για το ποσό ορόσημου στο αρχικό ορόσημο στη γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="7135c-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="7135c-149">Τιμολόγηση γραμμής σύμβασης βάσει προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="7135c-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7135c-150">Μια τιμολογημένη πραγματική πώληση για τη γραμμή προϊόντων με την ποσότητα και το ποσό που προέρχεται από τη γραμμή σύμβασης με βάση τα προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="7135c-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
