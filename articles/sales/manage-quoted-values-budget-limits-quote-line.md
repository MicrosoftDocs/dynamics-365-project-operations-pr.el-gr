---
title: Γραμμές προσφοράς βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 06a47c45dc3b3b174658e2fba14d3d2050aabf85
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076783"
---
# <a name="project-based-quote-lines"></a><span data-ttu-id="d5635-103">Γραμμές προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="d5635-103">Project-based quote lines</span></span>

<span data-ttu-id="d5635-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="d5635-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d5635-105">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="d5635-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="d5635-106">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="d5635-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="d5635-107">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="d5635-107">Billing Method</span></span>
- <span data-ttu-id="d5635-108">Αντιστοίχιση έργου</span><span class="sxs-lookup"><span data-stu-id="d5635-108">Project Mapping</span></span>
- <span data-ttu-id="d5635-109">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="d5635-109">Included Transaction classes</span></span>
- <span data-ttu-id="d5635-110">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="d5635-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="d5635-111">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="d5635-111">Chargeability setup</span></span>
- <span data-ttu-id="d5635-112">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="d5635-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="d5635-113">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="d5635-113">Quote line Customers</span></span>

<span data-ttu-id="d5635-114">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="d5635-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="d5635-115">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="d5635-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="d5635-116">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="d5635-116">**Field**</span></span> | <span data-ttu-id="d5635-117">**Συνάφεια, σκοπός και καθοδήγηση**</span><span class="sxs-lookup"><span data-stu-id="d5635-117">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="d5635-118">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="d5635-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d5635-119">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="d5635-119">Name</span></span> | <span data-ttu-id="d5635-120">Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="d5635-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="d5635-121">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-122">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="d5635-122">Billing Method</span></span> | <span data-ttu-id="d5635-123">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="d5635-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="d5635-124">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια συμβαλλόμενα μοντέλα που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="d5635-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="d5635-125">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="d5635-125">- Fixed price</span></span></br><span data-ttu-id="d5635-126">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="d5635-126">- Time and material.</span></span>| <span data-ttu-id="d5635-127">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-128">Project</span><span class="sxs-lookup"><span data-stu-id="d5635-128">Project</span></span> | <span data-ttu-id="d5635-129">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="d5635-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="d5635-130">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="d5635-131">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="d5635-132">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-133">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="d5635-133">Include Time</span></span> | <span data-ttu-id="d5635-134">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-135">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-136">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d5635-137">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-138">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="d5635-138">Include Expense</span></span> | <span data-ttu-id="d5635-139">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-140">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-141">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d5635-142">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-143">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="d5635-143">Include Fee</span></span> | <span data-ttu-id="d5635-144">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-145">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d5635-146">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d5635-147">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-148">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="d5635-148">Quoted Amount</span></span> | <span data-ttu-id="d5635-149">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="d5635-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="d5635-150">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="d5635-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="d5635-151">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="d5635-152">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-153">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="d5635-153">Estimated Tax</span></span> | <span data-ttu-id="d5635-154">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="d5635-155">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="d5635-156">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-157">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="d5635-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="d5635-158">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="d5635-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="d5635-159">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="d5635-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="d5635-160">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-161">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="d5635-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="d5635-162">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="d5635-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="d5635-163">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d5635-164">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="d5635-164">Customer Budget</span></span> | <span data-ttu-id="d5635-165">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="d5635-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="d5635-166">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="d5635-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="d5635-167">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="d5635-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="d5635-168">**Κανόνας 1** : Μια συγκεκριμένη κλάση συναλλαγής στο επιλεγμένο έργο μπορεί να συμπεριληφθεί μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d5635-168">**Rule 1** : A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="d5635-169">**Κανόνας 2** : Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d5635-169">**Rule 2** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="d5635-170">**Κανόνας 3** : Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d5635-170">**Rule 3** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="d5635-171">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="d5635-172">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d5635-173">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d5635-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d5635-175">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d5635-176">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d5635-177">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="d5635-178">
                    <strong>χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="d5635-179">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="d5635-180">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d5635-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-181">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-182">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-183">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-184">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-185">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-186">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-187">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-188">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="d5635-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-189">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="d5635-189">Violation of Rule #1.</span></span> <span data-ttu-id="d5635-190">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="d5635-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-191">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-192">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-193">QL2</span><span class="sxs-lookup"><span data-stu-id="d5635-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-194">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-195">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-196">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-197">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-197">Yes</span></span> </p>
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
<span data-ttu-id="d5635-198">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-199">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-200">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-201">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-202">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-203">No</span><span class="sxs-lookup"><span data-stu-id="d5635-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-204">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-205">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="d5635-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-206">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="d5635-206">Violation of Rule #1.</span></span> <span data-ttu-id="d5635-207">Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="d5635-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-208">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-209">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-210">QL2</span><span class="sxs-lookup"><span data-stu-id="d5635-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-211">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-212">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-213">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-214">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-214">Yes</span></span> </p>
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
<span data-ttu-id="d5635-215">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-216">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-217">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-218">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-220">No</span><span class="sxs-lookup"><span data-stu-id="d5635-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-221">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-222">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="d5635-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="d5635-223">Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.</span><span class="sxs-lookup"><span data-stu-id="d5635-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="d5635-224">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.</span><span class="sxs-lookup"><span data-stu-id="d5635-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="d5635-225">Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς, ώστε να είναι έγκυρη.</span><span class="sxs-lookup"><span data-stu-id="d5635-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-226">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-227">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-228">QL2</span><span class="sxs-lookup"><span data-stu-id="d5635-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-229">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-230">No</span><span class="sxs-lookup"><span data-stu-id="d5635-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-231">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-232">No</span><span class="sxs-lookup"><span data-stu-id="d5635-232">No</span></span> </p>
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
<span data-ttu-id="d5635-233">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-234">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-235">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-236">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-240">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="d5635-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-241">Παραβίαση του Κανόνα #1 παραπάνω</span><span class="sxs-lookup"><span data-stu-id="d5635-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="d5635-242">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1.</span><span class="sxs-lookup"><span data-stu-id="d5635-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="d5635-243">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.</span><span class="sxs-lookup"><span data-stu-id="d5635-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-244">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-245">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-246">QL2</span><span class="sxs-lookup"><span data-stu-id="d5635-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-247">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-248">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-250">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-250">Yes</span></span> </p>
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
<span data-ttu-id="d5635-251">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-252">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-253">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-254">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-255">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d5635-258">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="d5635-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-259">Με βάση τον κανόνα #2, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="d5635-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-260">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-261">Τ2</span><span class="sxs-lookup"><span data-stu-id="d5635-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-262">QL1 σε Q2</span><span class="sxs-lookup"><span data-stu-id="d5635-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-263">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-264">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-265">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-266">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-266">Yes</span></span> </p>
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
<span data-ttu-id="d5635-267">O1</span><span class="sxs-lookup"><span data-stu-id="d5635-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-268">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-269">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-270">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-271">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-272">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-273">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d5635-274">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="d5635-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d5635-275">Με βάση τον κανόνα #3, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="d5635-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d5635-276">O2</span><span class="sxs-lookup"><span data-stu-id="d5635-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d5635-277">Τ1</span><span class="sxs-lookup"><span data-stu-id="d5635-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-278">QL1</span><span class="sxs-lookup"><span data-stu-id="d5635-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-279">Π1</span><span class="sxs-lookup"><span data-stu-id="d5635-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-280">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d5635-281">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d5635-282">Ναι</span><span class="sxs-lookup"><span data-stu-id="d5635-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d5635-283">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="d5635-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

