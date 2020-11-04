---
title: Επιβεβαίωση προτιμολογίου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την επιβεβαίωση ενός προτιμολογίου.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 560bb68cba865a6af60504114126ae6ea73dde2d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076761"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="a77ad-103">Επιβεβαίωση προτιμολογίου</span><span class="sxs-lookup"><span data-stu-id="a77ad-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="a77ad-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="a77ad-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a77ad-105">Αφού επιβεβαιωθεί ένα προτιμολόγιο, η κατάσταση των ενημερώσεων του τιμολογίου έργου θα είναι **Επιβεβαιώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="a77ad-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="a77ad-106">Όταν επιβεβαιώνεται ένα τιμολόγιο, γίνεται μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="a77ad-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="a77ad-107">Προχωρώντας, το τιμολόγιο μπορεί να διορθωθεί μόνο εάν υπάρχουν διορθώσεις ή πιστώσεις που έχουν προετοιμαστεί από τον πελάτη ή όταν έχει επισημανθεί ως πληρωμένο.</span><span class="sxs-lookup"><span data-stu-id="a77ad-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="a77ad-108">Στον ακόλουθο πίνακα παρουσιάζονται οι πραγματικές τιμές που δημιουργούνται από το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="a77ad-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="a77ad-109">Αυτές οι πραγματικές τιμές δημιουργούνται όταν εκτελούνται συγκεκριμένες λειτουργίες στο προσχέδιο τιμολογίου πριν επιβεβαιωθεί.</span><span class="sxs-lookup"><span data-stu-id="a77ad-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="a77ad-110">
                    <strong>Σενάριο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a77ad-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="a77ad-111">
                    <strong>Πραγματικές τιμές που δημιουργήθηκαν κατά την επιβεβαίωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a77ad-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a77ad-112">Τιμολόγηση μιας συναλλαγής χρόνου χωρίς καμία επεξεργασία στο προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-113">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-114">Η πραγματική τιμολογημένη πώληση για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a77ad-115">Τιμολόγηση μιας συναλλαγής χρόνου που έχει υποστεί επεξεργασία για τη μείωση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="a77ad-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-116">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-117">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-118">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης είναι μη χρεώσιμη για τις υπόλοιπες ώρες και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a77ad-119">Τιμολόγηση μιας συναλλαγής χρόνου που έχει υποστεί επεξεργασία για την αύξηση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="a77ad-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-120">Η αντιστροφή των μη τιμολογημένων πωλήσεων για τις ώρες και το ποσό της αρχικής έγκρισης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-121">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για τις ώρες και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a77ad-122">Τιμολόγηση μιας συναλλαγής εξόδων χωρίς καμία επεξεργασία στο προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-123">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-124">Η τιμολογημένη πραγματική πώληση για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a77ad-125">Τιμολόγηση μιας συναλλαγής εξόδων που έχει υποστεί επεξεργασία για τη μείωση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="a77ad-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-126">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-127">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-128">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης είναι μη χρεώσιμη για την υπόλοιπη ποσότητα και το ποσό μετά την αφαίρεση των διορθωμένων αριθμών στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a77ad-129">Τιμολόγηση μιας συναλλαγής εξόδων που έχει υποστεί επεξεργασία για την αύξηση της ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="a77ad-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-130">Η αντιστροφή των μη τιμολογημένων πωλήσεων για την ποσότητα και το ποσό της αρχικής έγκρισης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-131">Μια νέα μη τιμολογημένη πραγματική τιμή πώλησης με χρέωση για την ποσότητα και το ποσό στην επεξεργασμένη λεπτομέρεια γραμμής τιμολογίου, μια αντιστροφή της πραγματικής μη τιμολογημένης πώλησης και ένα ισοδύναμο τιμολογημένο πραγματικό πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="a77ad-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a77ad-132">Τιμολόγηση μιας αμοιβής.</span><span class="sxs-lookup"><span data-stu-id="a77ad-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-133">Η αντιστροφή των μη τιμολογημένων πωλήσεων για το ποσό αμοιβής στην αρχική γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-134">Η τιμολογημένη πραγματική πώληση για την ποσότητα και το ποσό της αρχικής γραμμής ημερολογίου αμοιβής.</span><span class="sxs-lookup"><span data-stu-id="a77ad-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a77ad-135">Τιμολόγηση ενός ορόσημου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a77ad-136">Η τιμολογημένη πραγματική πώληση για το ποσό ορόσημου στο αρχικό ορόσημο στη γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="a77ad-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
