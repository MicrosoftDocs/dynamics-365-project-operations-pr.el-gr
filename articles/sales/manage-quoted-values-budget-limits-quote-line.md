---
title: Επισκόπηση γραμμών προσφοράς έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς έργου για εργασία έργου.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa48a90c275eae1b0c0dbce685ae718dd9674c88
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858023"
---
# <a name="project-quote-lines-overview"></a><span data-ttu-id="b1845-103">Επισκόπηση γραμμών προσφοράς έργου</span><span class="sxs-lookup"><span data-stu-id="b1845-103">Project quote lines overview</span></span>

<span data-ttu-id="b1845-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="b1845-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b1845-105">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="b1845-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="b1845-106">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="b1845-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="b1845-107">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="b1845-107">Billing Method</span></span>
- <span data-ttu-id="b1845-108">Αντιστοίχιση έργου</span><span class="sxs-lookup"><span data-stu-id="b1845-108">Project Mapping</span></span>
- <span data-ttu-id="b1845-109">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="b1845-109">Included Transaction classes</span></span>
- <span data-ttu-id="b1845-110">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="b1845-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="b1845-111">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="b1845-111">Chargeability setup</span></span>
- <span data-ttu-id="b1845-112">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="b1845-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="b1845-113">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="b1845-113">Quote line Customers</span></span>

<span data-ttu-id="b1845-114">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="b1845-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="b1845-115">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="b1845-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="b1845-116">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="b1845-116">**Field**</span></span> | <span data-ttu-id="b1845-117">**Περιγραφή**</span><span class="sxs-lookup"><span data-stu-id="b1845-117">**Description**</span></span> | <span data-ttu-id="b1845-118">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="b1845-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="b1845-119">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="b1845-119">Name</span></span> | <span data-ttu-id="b1845-120">Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="b1845-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="b1845-121">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-122">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="b1845-122">Billing Method</span></span> | <span data-ttu-id="b1845-123">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="b1845-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="b1845-124">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια μοντέλα ανάθεσης συμβάσεων που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="b1845-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="b1845-125">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="b1845-125">- Fixed price</span></span></br><span data-ttu-id="b1845-126">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="b1845-126">- Time and material.</span></span>| <span data-ttu-id="b1845-127">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-128">Project</span><span class="sxs-lookup"><span data-stu-id="b1845-128">Project</span></span> | <span data-ttu-id="b1845-129">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="b1845-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="b1845-130">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="b1845-131">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="b1845-132">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-133">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="b1845-133">Include Time</span></span> | <span data-ttu-id="b1845-134">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-135">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-136">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b1845-137">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-138">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="b1845-138">Include Expense</span></span> | <span data-ttu-id="b1845-139">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-140">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-141">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b1845-142">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-143">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="b1845-143">Include Fee</span></span> | <span data-ttu-id="b1845-144">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-145">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b1845-146">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b1845-147">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-148">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="b1845-148">Quoted Amount</span></span> | <span data-ttu-id="b1845-149">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="b1845-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="b1845-150">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="b1845-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="b1845-151">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="b1845-152">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-153">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="b1845-153">Estimated Tax</span></span> | <span data-ttu-id="b1845-154">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="b1845-155">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="b1845-156">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-157">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="b1845-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="b1845-158">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b1845-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="b1845-159">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="b1845-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="b1845-160">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-161">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="b1845-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="b1845-162">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="b1845-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="b1845-163">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b1845-164">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="b1845-164">Customer Budget</span></span> | <span data-ttu-id="b1845-165">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="b1845-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="b1845-166">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b1845-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="b1845-167">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="b1845-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="b1845-168">**Κανόνας 1**: Μια συγκεκριμένη κλάση συναλλαγής στο επιλεγμένο έργο μπορεί να συμπεριληφθεί μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b1845-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="b1845-169">**Κανόνας 2**: Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="b1845-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="b1845-170">**Κανόνας 3**: Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="b1845-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="b1845-171">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="b1845-172">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b1845-173">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b1845-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="b1845-175">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="b1845-176">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b1845-177">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="b1845-178">
                    <strong>χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="b1845-179">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="b1845-180">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b1845-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-181">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-182">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-183">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-184">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-185">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-186">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-187">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-188">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="b1845-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-189">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="b1845-189">Violation of Rule #1.</span></span> <span data-ttu-id="b1845-190">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="b1845-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-191">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-192">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-193">QL2</span><span class="sxs-lookup"><span data-stu-id="b1845-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-194">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-195">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-196">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-197">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-197">Yes</span></span> </p>
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
<span data-ttu-id="b1845-198">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-199">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-200">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-201">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-202">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-203">No</span><span class="sxs-lookup"><span data-stu-id="b1845-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-204">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-205">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="b1845-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-206">Παραβίαση του Κανόνα #1.</span><span class="sxs-lookup"><span data-stu-id="b1845-206">Violation of Rule #1.</span></span> <span data-ttu-id="b1845-207">Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="b1845-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-208">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-209">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-210">QL2</span><span class="sxs-lookup"><span data-stu-id="b1845-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-211">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-212">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-213">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-214">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-214">Yes</span></span> </p>
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
<span data-ttu-id="b1845-215">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-216">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-217">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-218">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-220">No</span><span class="sxs-lookup"><span data-stu-id="b1845-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-221">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-222">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="b1845-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="b1845-223">Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.</span><span class="sxs-lookup"><span data-stu-id="b1845-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="b1845-224">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.</span><span class="sxs-lookup"><span data-stu-id="b1845-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="b1845-225">Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς, ώστε να είναι έγκυρη.</span><span class="sxs-lookup"><span data-stu-id="b1845-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-226">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-227">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-228">QL2</span><span class="sxs-lookup"><span data-stu-id="b1845-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-229">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-230">No</span><span class="sxs-lookup"><span data-stu-id="b1845-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-231">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-232">No</span><span class="sxs-lookup"><span data-stu-id="b1845-232">No</span></span> </p>
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
<span data-ttu-id="b1845-233">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-234">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-235">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-236">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-240">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="b1845-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-241">Παραβίαση του Κανόνα #1 παραπάνω</span><span class="sxs-lookup"><span data-stu-id="b1845-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="b1845-242">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1.</span><span class="sxs-lookup"><span data-stu-id="b1845-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="b1845-243">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.</span><span class="sxs-lookup"><span data-stu-id="b1845-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-244">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-245">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-246">QL2</span><span class="sxs-lookup"><span data-stu-id="b1845-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-247">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-248">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-250">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-250">Yes</span></span> </p>
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
<span data-ttu-id="b1845-251">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-252">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-253">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-254">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-255">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b1845-258">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="b1845-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-259">Με βάση τον κανόνα #2, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="b1845-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-260">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-261">Τ2</span><span class="sxs-lookup"><span data-stu-id="b1845-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-262">QL1 σε Q2</span><span class="sxs-lookup"><span data-stu-id="b1845-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-263">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-264">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-265">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-266">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-266">Yes</span></span> </p>
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
<span data-ttu-id="b1845-267">O1</span><span class="sxs-lookup"><span data-stu-id="b1845-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-268">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-269">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-270">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-271">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-272">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-273">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b1845-274">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="b1845-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b1845-275">Με βάση τον κανόνα #3, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="b1845-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b1845-276">O2</span><span class="sxs-lookup"><span data-stu-id="b1845-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b1845-277">Τ1</span><span class="sxs-lookup"><span data-stu-id="b1845-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-278">QL1</span><span class="sxs-lookup"><span data-stu-id="b1845-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-279">Π1</span><span class="sxs-lookup"><span data-stu-id="b1845-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-280">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b1845-281">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b1845-282">Ναι</span><span class="sxs-lookup"><span data-stu-id="b1845-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b1845-283">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="b1845-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
