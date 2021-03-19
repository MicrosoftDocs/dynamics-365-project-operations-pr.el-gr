---
title: Επισκόπηση γραμμών προσφοράς βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e61a9fbf357123884397b930662d11f22bfdeaa0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277788"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="23be1-103">Επισκόπηση γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="23be1-103">Project-based quote lines overview</span></span>

<span data-ttu-id="23be1-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="23be1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="23be1-105">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="23be1-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="23be1-106">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="23be1-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="23be1-107">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="23be1-107">Billing Method</span></span>
- <span data-ttu-id="23be1-108">Αντιστοίχιση έργου</span><span class="sxs-lookup"><span data-stu-id="23be1-108">Project Mapping</span></span>
- <span data-ttu-id="23be1-109">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="23be1-109">Included Transaction classes</span></span>
- <span data-ttu-id="23be1-110">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="23be1-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="23be1-111">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="23be1-111">Chargeability setup</span></span>
- <span data-ttu-id="23be1-112">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="23be1-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="23be1-113">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="23be1-113">Quote line Customers</span></span>

<span data-ttu-id="23be1-114">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="23be1-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="23be1-115">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="23be1-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="23be1-116">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="23be1-116">**Field**</span></span> | <span data-ttu-id="23be1-117">**Περιγραφή**</span><span class="sxs-lookup"><span data-stu-id="23be1-117">**Description**</span></span> | <span data-ttu-id="23be1-118">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="23be1-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="23be1-119">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="23be1-119">Name</span></span> | <span data-ttu-id="23be1-120">Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="23be1-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="23be1-121">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-122">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="23be1-122">Billing Method</span></span> | <span data-ttu-id="23be1-123">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="23be1-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="23be1-124">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια μοντέλα ανάθεσης συμβάσεων που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="23be1-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="23be1-125">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="23be1-125">- Fixed price</span></span></br><span data-ttu-id="23be1-126">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="23be1-126">- Time and material.</span></span>| <span data-ttu-id="23be1-127">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-128">Project</span><span class="sxs-lookup"><span data-stu-id="23be1-128">Project</span></span> | <span data-ttu-id="23be1-129">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="23be1-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="23be1-130">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="23be1-131">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="23be1-132">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-133">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="23be1-133">Include Time</span></span> | <span data-ttu-id="23be1-134">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-135">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-136">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="23be1-137">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-138">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="23be1-138">Include Expense</span></span> | <span data-ttu-id="23be1-139">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-140">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-141">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="23be1-142">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-143">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="23be1-143">Include Fee</span></span> | <span data-ttu-id="23be1-144">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-145">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="23be1-146">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="23be1-147">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-148">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="23be1-148">Quoted Amount</span></span> | <span data-ttu-id="23be1-149">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="23be1-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="23be1-150">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="23be1-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="23be1-151">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="23be1-152">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-153">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="23be1-153">Estimated Tax</span></span> | <span data-ttu-id="23be1-154">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="23be1-155">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="23be1-156">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-157">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="23be1-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="23be1-158">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="23be1-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="23be1-159">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="23be1-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="23be1-160">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-161">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="23be1-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="23be1-162">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="23be1-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="23be1-163">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="23be1-164">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="23be1-164">Customer Budget</span></span> | <span data-ttu-id="23be1-165">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="23be1-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="23be1-166">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="23be1-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="23be1-167">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="23be1-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="23be1-168">**Κανόνας 1**: Μια συγκεκριμένη κλάση συναλλαγής στο επιλεγμένο έργο μπορεί να συμπεριληφθεί μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="23be1-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="23be1-169">**Κανόνας 2**: Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="23be1-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="23be1-170">**Κανόνας 3**: Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="23be1-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="23be1-171">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="23be1-172">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="23be1-173">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="23be1-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="23be1-175">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="23be1-176">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="23be1-177">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="23be1-178">
                    <strong>χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="23be1-179">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="23be1-180">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="23be1-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-181">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-182">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-183">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-184">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-185">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-186">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-187">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-188">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="23be1-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-189">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="23be1-189">Violation of Rule #1.</span></span> <span data-ttu-id="23be1-190">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="23be1-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-191">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-192">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-193">QL2</span><span class="sxs-lookup"><span data-stu-id="23be1-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-194">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-195">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-196">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-197">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-197">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-198">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-199">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-200">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-201">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-202">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-203">No</span><span class="sxs-lookup"><span data-stu-id="23be1-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-204">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-205">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="23be1-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-206">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="23be1-206">Violation of Rule #1.</span></span> <span data-ttu-id="23be1-207">Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="23be1-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-208">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-209">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-210">QL2</span><span class="sxs-lookup"><span data-stu-id="23be1-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-211">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-212">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-213">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-214">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-214">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-215">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-216">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-217">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-218">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-220">No</span><span class="sxs-lookup"><span data-stu-id="23be1-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-221">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-222">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="23be1-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="23be1-223">Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.</span><span class="sxs-lookup"><span data-stu-id="23be1-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="23be1-224">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.</span><span class="sxs-lookup"><span data-stu-id="23be1-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="23be1-225">Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς, ώστε να είναι έγκυρη.</span><span class="sxs-lookup"><span data-stu-id="23be1-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-226">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-227">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-228">QL2</span><span class="sxs-lookup"><span data-stu-id="23be1-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-229">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-230">No</span><span class="sxs-lookup"><span data-stu-id="23be1-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-231">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-232">No</span><span class="sxs-lookup"><span data-stu-id="23be1-232">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-233">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-234">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-235">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-236">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-240">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="23be1-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-241">Παραβίαση του Κανόνα #1 παραπάνω</span><span class="sxs-lookup"><span data-stu-id="23be1-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="23be1-242">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1.</span><span class="sxs-lookup"><span data-stu-id="23be1-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="23be1-243">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.</span><span class="sxs-lookup"><span data-stu-id="23be1-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-244">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-245">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-246">QL2</span><span class="sxs-lookup"><span data-stu-id="23be1-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-247">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-248">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-250">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-250">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-251">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-252">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-253">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-254">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-255">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="23be1-258">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="23be1-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-259">Με βάση τον κανόνα #2, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="23be1-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-260">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-261">Τ2</span><span class="sxs-lookup"><span data-stu-id="23be1-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-262">QL1 σε Q2</span><span class="sxs-lookup"><span data-stu-id="23be1-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-263">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-264">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-265">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-266">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-266">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-267">O1</span><span class="sxs-lookup"><span data-stu-id="23be1-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-268">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-269">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-270">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-271">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-272">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-273">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="23be1-274">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="23be1-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="23be1-275">Με βάση τον κανόνα #3, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="23be1-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="23be1-276">O2</span><span class="sxs-lookup"><span data-stu-id="23be1-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="23be1-277">Τ1</span><span class="sxs-lookup"><span data-stu-id="23be1-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-278">QL1</span><span class="sxs-lookup"><span data-stu-id="23be1-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-279">Π1</span><span class="sxs-lookup"><span data-stu-id="23be1-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-280">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="23be1-281">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="23be1-282">Ναι</span><span class="sxs-lookup"><span data-stu-id="23be1-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="23be1-283">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="23be1-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]