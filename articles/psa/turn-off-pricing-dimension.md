---
title: Απενεργοποίηση διάστασης τιμολόγησης
description: Αυτό το θέμα δείχνει πώς μπορείτε να ορίσετε διαστάσεις τιμολόγησης στη λύση Project Service.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 6e4b80b9c4b1b0f57d04079c9d2f84051b451d29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281838"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="4f2e2-103">Απενεργοποίηση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="4f2e2-103">Turn off a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="4f2e2-104">Μπορεί να χρειαστεί να εξετάζετε και να ενημερώνετε τη στρατηγική τιμολόγησης κάθε λίγα χρόνια.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="4f2e2-105">Τυχόν ενημερώσεις που κάνετε μπορεί να απαιτούν να απενεργοποιήσετε μια υπάρχουσα διάσταση τιμολόγησης και να δημιουργήσετε μια νέα.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="4f2e2-106">Για παράδειγμα, μπορεί να έχετε ήδη κοστολογήσει τον **Ρόλο** σας αλλά τώρα έχετε αποφασίσει να τιμολογήσετε την **Εμπειρία εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="4f2e2-107">Αυτό μπορεί να απαιτεί την απενεργοποίηση του **Ρόλου** ως διάσταση τιμολόγησης και τη δημιουργία **Εμπειρίας εργασίας** ως νέας διάστασης τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="4f2e2-108">Η απενεργοποίηση μιας διάστασης τιμολόγησης, ανεξάρτητα από το εάν είναι εκτός ελέγχου ή προσαρμοσμένη, μπορεί να γίνει με τον ορισμό των πεδίων **Ισχύει για το κόστος** και **Ισχύει για τις πωλήσεις** της διάστασης τιμολόγησης σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="4f2e2-109">Ωστόσο, όταν το κάνετε αυτό, ενδέχεται να εμφανιστεί το ακόλουθο μήνυμα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-109">However, when you do this, you might receive the following error message.</span></span>

![Πιθανό σφάλμα επιχειρηματικής διαδικασίας κατά την απενεργοποίηση μιας διάστασης τιμολόγησης](media/Business-Process-Error.png)


<span data-ttu-id="4f2e2-111">Αυτό το μήνυμα σφάλματος υποδεικνύει ότι υπάρχουν καρτέλες τιμών που είχαν ρυθμιστεί προηγουμένως για τη διάσταση που απενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="4f2e2-112">Όλες οι καρτέλες **Τιμή ρόλου** και **Αύξηση τιμής ρόλου** που αναφέρονται σε μια διάσταση πρέπει να διαγραφούν προτού η δυνατότητα εφαρμογής της διάστασης οριστεί σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="4f2e2-113">Αυτός ο κανόνας ισχύει τόσο για τις έτοιμες διαστάσεις τιμολόγησης όσο και για τυχόν προσαρμοσμένες διαστάσεις τιμολόγησης που μπορεί να έχετε δημιουργήσει.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="4f2e2-114">Ο λόγος για αυτήν την επικύρωση είναι επειδή το Project Service έχει έναν περιορισμό ότι κάθε καρτέλα **Τιμή ρόλου** πρέπει να έχει ένα μοναδικό συνδυασμό διαστάσεων.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="4f2e2-115">Για παράδειγμα, σε έναν τιμοκατάλογο που ονομάζεται **Τιμές κόστους ΗΠΑ 2018**, έχετε τις παρακάτω σειρές **Τιμής ρόλων**.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="4f2e2-116">Τυπικός τίτλος</span><span class="sxs-lookup"><span data-stu-id="4f2e2-116">Standard Title</span></span>         | <span data-ttu-id="4f2e2-117">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="4f2e2-117">Org Unit</span></span>    |<span data-ttu-id="4f2e2-118">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="4f2e2-118">Unit</span></span>   |<span data-ttu-id="4f2e2-119">Τιμή</span><span class="sxs-lookup"><span data-stu-id="4f2e2-119">Price</span></span>  |<span data-ttu-id="4f2e2-120">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="4f2e2-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="4f2e2-121">Μηχανικός συστημάτων</span><span class="sxs-lookup"><span data-stu-id="4f2e2-121">Systems Engineer</span></span>|<span data-ttu-id="4f2e2-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="4f2e2-122">Contoso US</span></span>|<span data-ttu-id="4f2e2-123">Hour</span><span class="sxs-lookup"><span data-stu-id="4f2e2-123">Hour</span></span>| <span data-ttu-id="4f2e2-124">100</span><span class="sxs-lookup"><span data-stu-id="4f2e2-124">100</span></span>|<span data-ttu-id="4f2e2-125">USD</span><span class="sxs-lookup"><span data-stu-id="4f2e2-125">USD</span></span>|
| <span data-ttu-id="4f2e2-126">Επικεφαλής μηχανικός συστημάτων</span><span class="sxs-lookup"><span data-stu-id="4f2e2-126">Senior Systems Engineer</span></span>|<span data-ttu-id="4f2e2-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="4f2e2-127">Contoso US</span></span>|<span data-ttu-id="4f2e2-128">Hour</span><span class="sxs-lookup"><span data-stu-id="4f2e2-128">Hour</span></span>| <span data-ttu-id="4f2e2-129">150</span><span class="sxs-lookup"><span data-stu-id="4f2e2-129">150</span></span>| <span data-ttu-id="4f2e2-130">USD</span><span class="sxs-lookup"><span data-stu-id="4f2e2-130">USD</span></span>|


<span data-ttu-id="4f2e2-131">Όταν απενεργοποιείτε τον **Τυπικό τίτλο** ως διάσταση τιμολόγησης και ο μηχανισμός τιμολόγησης Project Service αναζητά μια τιμή, θα χρησιμοποιήσει μόνο την τιμή **Οργανωτική μονάδα** από το περιβάλλον εισόδου.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="4f2e2-132">Εάν η **Οργανωτική μονάδα** του περιβάλλοντος εισόδου είναι "Contoso US", το αποτέλεσμα θα είναι μη καθοριστικό επειδή και οι δύο γραμμές θα είναι ίδιες.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="4f2e2-133">Για να αποφύγετε αυτό το σενάριο, όταν δημιουργείτε καρτέλες **Τιμή ρόλου**, το Project Service επικυρώνει ότι ο συνδυασμός των διαστάσεων είναι μοναδικός.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="4f2e2-134">Εάν η διάσταση είναι απενεργοποιημένη μετά τη δημιουργία καρτελών **Τιμή ρόλου** αυτός ο περιορισμός μπορεί να παραβιαστεί.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="4f2e2-135">Ως εκ τούτου, απαιτείται πριν να απενεργοποιήσετε μια διάσταση, να διαγράψετε όλες τις σειρές **Τιμή ρόλου** και **Αύξηση τιμής ρόλου** που έχουν ως συμπληρωμένο αυτόν τον κωδικό διάστασης.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]