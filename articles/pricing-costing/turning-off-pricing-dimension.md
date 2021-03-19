---
title: Απενεργοποίηση μιας διάστασης τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την απενεργοποίηση των διαστάσεων τιμολόγησης.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d2e10c9ce782697fa4cbbe6eb63491ebb573a6f6
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274728"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="f53c5-103">Απενεργοποίηση μιας διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="f53c5-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="f53c5-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="f53c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f53c5-105">Μπορεί να χρειαστεί να εξετάζετε και να ενημερώνετε τη στρατηγική τιμολόγησης κάθε λίγα χρόνια.</span><span class="sxs-lookup"><span data-stu-id="f53c5-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="f53c5-106">Τυχόν ενημερώσεις που κάνετε μπορεί να απαιτούν να απενεργοποιήσετε μια υπάρχουσα διάσταση τιμολόγησης και να δημιουργήσετε μια νέα.</span><span class="sxs-lookup"><span data-stu-id="f53c5-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="f53c5-107">Για παράδειγμα, μπορεί να έχετε ήδη κοστολογήσει τον **Ρόλο** σας αλλά τώρα έχετε αποφασίσει να τιμολογήσετε την **Εμπειρία εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="f53c5-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="f53c5-108">Αυτό μπορεί να απαιτεί την απενεργοποίηση του **Ρόλου** ως διάσταση τιμολόγησης και τη δημιουργία **Εμπειρίας εργασίας** ως νέας διάστασης τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="f53c5-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="f53c5-109">Η απενεργοποίηση μιας διάστασης τιμολόγησης, ανεξάρτητα από το εάν είναι εκτός ελέγχου ή προσαρμοσμένη, μπορεί να γίνει με τον ορισμό των πεδίων **Ισχύει για το κόστος** και **Ισχύει για τις πωλήσεις** της διάστασης τιμολόγησης σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="f53c5-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="f53c5-110">Ωστόσο, όταν το κάνετε αυτό, μπορείτε να λάβετε το μήνυμα σφάλματος **Η διάσταση τιμολόγησης δεν μπορεί να ενημερωθεί ή να διαγραφεί εάν υπάρχουν συσχετισμένες καρτέλες τιμών.**</span><span class="sxs-lookup"><span data-stu-id="f53c5-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

![Πιθανό σφάλμα επιχειρηματικής διαδικασίας κατά την απενεργοποίηση μιας διάστασης τιμολόγησης](media/Business-Process-Error.png)

<span data-ttu-id="f53c5-112">Αυτό το μήνυμα σφάλματος υποδεικνύει ότι υπάρχουν καρτέλες τιμών που είχαν ρυθμιστεί προηγουμένως για τη διάσταση που απενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="f53c5-112">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="f53c5-113">Όλες οι καρτέλες **Τιμή ρόλου** και **Αύξηση τιμής ρόλου** που αναφέρονται σε μια διάσταση πρέπει να διαγραφούν προτού η δυνατότητα εφαρμογής της διάστασης οριστεί σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="f53c5-113">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="f53c5-114">Αυτός ο κανόνας ισχύει τόσο για τις έτοιμες διαστάσεις τιμολόγησης όσο και για τυχόν προσαρμοσμένες διαστάσεις τιμολόγησης που μπορεί να έχετε δημιουργήσει.</span><span class="sxs-lookup"><span data-stu-id="f53c5-114">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="f53c5-115">Ο λόγος για αυτήν την επικύρωση είναι επειδή κάθε καρτέλα **Τιμή ρόλου** πρέπει να έχει ένα μοναδικό συνδυασμό διαστάσεων.</span><span class="sxs-lookup"><span data-stu-id="f53c5-115">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="f53c5-116">Για παράδειγμα, σε έναν τιμοκατάλογο που ονομάζεται **Τιμές κόστους ΗΠΑ 2018**, έχετε τις παρακάτω σειρές **Τιμής ρόλων**.</span><span class="sxs-lookup"><span data-stu-id="f53c5-116">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="f53c5-117">Τυπικός τίτλος</span><span class="sxs-lookup"><span data-stu-id="f53c5-117">Standard Title</span></span>         | <span data-ttu-id="f53c5-118">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="f53c5-118">Org Unit</span></span>    |<span data-ttu-id="f53c5-119">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="f53c5-119">Unit</span></span>   |<span data-ttu-id="f53c5-120">Τιμή</span><span class="sxs-lookup"><span data-stu-id="f53c5-120">Price</span></span>  |<span data-ttu-id="f53c5-121">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="f53c5-121">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="f53c5-122">Μηχανικός συστημάτων</span><span class="sxs-lookup"><span data-stu-id="f53c5-122">Systems Engineer</span></span>|<span data-ttu-id="f53c5-123">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f53c5-123">Contoso US</span></span>|<span data-ttu-id="f53c5-124">Hour</span><span class="sxs-lookup"><span data-stu-id="f53c5-124">Hour</span></span>| <span data-ttu-id="f53c5-125">100</span><span class="sxs-lookup"><span data-stu-id="f53c5-125">100</span></span>|<span data-ttu-id="f53c5-126">USD</span><span class="sxs-lookup"><span data-stu-id="f53c5-126">USD</span></span>|
| <span data-ttu-id="f53c5-127">Επικεφαλής μηχανικός συστημάτων</span><span class="sxs-lookup"><span data-stu-id="f53c5-127">Senior Systems Engineer</span></span>|<span data-ttu-id="f53c5-128">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f53c5-128">Contoso US</span></span>|<span data-ttu-id="f53c5-129">Hour</span><span class="sxs-lookup"><span data-stu-id="f53c5-129">Hour</span></span>| <span data-ttu-id="f53c5-130">150</span><span class="sxs-lookup"><span data-stu-id="f53c5-130">150</span></span>| <span data-ttu-id="f53c5-131">USD</span><span class="sxs-lookup"><span data-stu-id="f53c5-131">USD</span></span>|


<span data-ttu-id="f53c5-132">Όταν απενεργοποιείτε τον **Τυπικό τίτλο** ως διάσταση τιμολόγησης και ο μηχανισμός τιμολόγησης αναζητά μια τιμή, θα χρησιμοποιήσει μόνο την τιμή **Οργανωτική μονάδα** από το περιβάλλον εισόδου.</span><span class="sxs-lookup"><span data-stu-id="f53c5-132">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="f53c5-133">Εάν η **Οργανωτική μονάδα** του περιβάλλοντος εισόδου είναι "Contoso US", το αποτέλεσμα θα είναι μη καθοριστικό επειδή και οι δύο γραμμές θα είναι ίδιες.</span><span class="sxs-lookup"><span data-stu-id="f53c5-133">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="f53c5-134">Για να αποφύγετε αυτό το σενάριο, όταν δημιουργείτε καρτέλες **Τιμή ρόλου**, το σύστημα επικυρώνει ότι ο συνδυασμός των διαστάσεων είναι μοναδικός.</span><span class="sxs-lookup"><span data-stu-id="f53c5-134">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="f53c5-135">Εάν η διάσταση είναι απενεργοποιημένη μετά τη δημιουργία καρτελών **Τιμή ρόλου** αυτός ο περιορισμός μπορεί να παραβιαστεί.</span><span class="sxs-lookup"><span data-stu-id="f53c5-135">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="f53c5-136">Ως εκ τούτου, απαιτείται πριν να απενεργοποιήσετε μια διάσταση, να διαγράψετε όλες τις σειρές **Τιμή ρόλου** και **Αύξηση τιμής ρόλου** που έχουν ως συμπληρωμένο αυτόν τον κωδικό διάστασης.</span><span class="sxs-lookup"><span data-stu-id="f53c5-136">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]