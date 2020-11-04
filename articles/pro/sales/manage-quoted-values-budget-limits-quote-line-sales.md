---
title: Γραμμές προσφοράς βάσει έργου (Pro)
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076846"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="e1f69-104">Γραμμές προσφοράς βάσει έργου (Pro)</span><span class="sxs-lookup"><span data-stu-id="e1f69-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="e1f69-105">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="e1f69-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e1f69-106">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="e1f69-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="e1f69-107">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="e1f69-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="e1f69-108">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="e1f69-108">Billing Method</span></span>
- <span data-ttu-id="e1f69-109">Αντιστοίχιση έργου και εργασιών</span><span class="sxs-lookup"><span data-stu-id="e1f69-109">Project and Task Mapping</span></span>
- <span data-ttu-id="e1f69-110">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="e1f69-110">Included Transaction classes</span></span>
- <span data-ttu-id="e1f69-111">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="e1f69-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="e1f69-112">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="e1f69-112">Chargeability setup</span></span>
- <span data-ttu-id="e1f69-113">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="e1f69-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="e1f69-114">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="e1f69-114">Quote line Customers</span></span>

<span data-ttu-id="e1f69-115">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="e1f69-116">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="e1f69-117">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="e1f69-117">**Field**</span></span> | <span data-ttu-id="e1f69-118">**Συνάφεια, σκοπός και καθοδήγηση**</span><span class="sxs-lookup"><span data-stu-id="e1f69-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="e1f69-119">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="e1f69-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e1f69-120">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="e1f69-120">Name</span></span> | <span data-ttu-id="e1f69-121">Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="e1f69-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="e1f69-122">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-123">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="e1f69-123">Billing Method</span></span> | <span data-ttu-id="e1f69-124">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="e1f69-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="e1f69-125">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια συμβαλλόμενα μοντέλα που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="e1f69-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="e1f69-126">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="e1f69-126">- Fixed price</span></span></br><span data-ttu-id="e1f69-127">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="e1f69-127">- Time and material.</span></span>| <span data-ttu-id="e1f69-128">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-129">Project</span><span class="sxs-lookup"><span data-stu-id="e1f69-129">Project</span></span> | <span data-ttu-id="e1f69-130">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="e1f69-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="e1f69-131">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="e1f69-132">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="e1f69-133">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="e1f69-134">Εργασίες που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="e1f69-134">Included Tasks</span></span> | <span data-ttu-id="e1f69-135">Υποδεικνύει εάν αυτή η γραμμή προσφοράς χρησιμοποιείται για όλες ή ορισμένες από τις εργασίες έργου του επιλεγμένου έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="e1f69-136">Το πεδίο αυτό έχει τις ακόλουθες πιθανές τιμές:</span><span class="sxs-lookup"><span data-stu-id="e1f69-136">This field has the following possible values:</span></span></br><span data-ttu-id="e1f69-137">- Όλες οι εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="e1f69-137">- All project tasks</span></span></br><span data-ttu-id="e1f69-138">- Επιλεγμένες εργασίες έργου μόνο</span><span class="sxs-lookup"><span data-stu-id="e1f69-138">- Selected project tasks only</span></span></br><span data-ttu-id="e1f69-139">Μια κενή τιμή σε αυτό το πεδίο ισοδυναμεί με την επιλογή **Όλες οι εργασίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="e1f69-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="e1f69-140">Όταν επιλέξετε **Μόνο επιλεγμένες εργασίες έργου** , στη συνέχεια, στη σελίδα έργου, η καρτέλα **Ρύθμιση χρέωσης εργασιών** σάς δίνει τη δυνατότητα να επιλέξετε συγκεκριμένες εργασίες για να τις συσχετίσετε με αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="e1f69-141">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-142">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="e1f69-142">Include Time</span></span> | <span data-ttu-id="e1f69-143">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-144">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-145">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e1f69-146">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-147">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="e1f69-147">Include Expense</span></span> | <span data-ttu-id="e1f69-148">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-149">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-150">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e1f69-151">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-152">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="e1f69-152">Include Fee</span></span> | <span data-ttu-id="e1f69-153">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-154">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e1f69-155">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e1f69-156">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-157">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="e1f69-157">Quoted Amount</span></span> | <span data-ttu-id="e1f69-158">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="e1f69-159">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="e1f69-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="e1f69-160">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="e1f69-161">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-162">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="e1f69-162">Estimated Tax</span></span> | <span data-ttu-id="e1f69-163">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="e1f69-164">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="e1f69-165">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-166">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="e1f69-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="e1f69-167">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="e1f69-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="e1f69-168">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="e1f69-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="e1f69-169">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-170">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="e1f69-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="e1f69-171">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="e1f69-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="e1f69-172">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e1f69-173">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="e1f69-173">Customer Budget</span></span> | <span data-ttu-id="e1f69-174">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="e1f69-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="e1f69-175">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="e1f69-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="e1f69-176">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="e1f69-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="e1f69-177">**Κανόνας 1** : Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου** , το έργο περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-177">**Rule 1** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project is included in the quote line.</span></span>

<span data-ttu-id="e1f69-178">**Κανόνας 2** : Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου** , ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-178">**Rule 2** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="e1f69-179">**Κανόνας 3** : Εάν το πεδίο **Εργασίες που περιλαμβάνονται** έχει οριστεί σε **Μόνο επιλεγμένες εργασίες έργου** , ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν σε πολλές γραμμές προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="e1f69-179">**Rule 3** : If the **Included Tasks** field is set to **Selected project tasks only** , a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="e1f69-180">**Κανόνας 4** : Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="e1f69-180">**Rule 4** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="e1f69-181">**Κανόνας 5** : Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="e1f69-181">**Rule 5** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="e1f69-182">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="e1f69-183">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e1f69-184">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e1f69-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="e1f69-186">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="e1f69-187">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="e1f69-188">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e1f69-189">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="e1f69-190">
                    <strong>Χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="e1f69-191">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="e1f69-192">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1f69-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-193">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-194">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-195">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-196">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-197">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-198">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-199">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-200">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-201">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="e1f69-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-202">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-202">Violation of Rule #2.</span></span> <span data-ttu-id="e1f69-203">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-204">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-205">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-206">QL2</span><span class="sxs-lookup"><span data-stu-id="e1f69-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-207">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-208">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-209">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-210">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-211">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-211">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="e1f69-212">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-213">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-214">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-215">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-216">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-217">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-218">No</span><span class="sxs-lookup"><span data-stu-id="e1f69-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-220">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="e1f69-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-221">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-221">Violation of Rule #2.</span></span> <span data-ttu-id="e1f69-222">Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-223">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-224">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-225">QL2</span><span class="sxs-lookup"><span data-stu-id="e1f69-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-226">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-227">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-228">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-229">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-230">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-230">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-231">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-232">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-233">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-234">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-235">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-236">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-237">No</span><span class="sxs-lookup"><span data-stu-id="e1f69-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-239">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="e1f69-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="e1f69-240">Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.</span><span class="sxs-lookup"><span data-stu-id="e1f69-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="e1f69-241">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="e1f69-242">Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς και είναι έγκυρη.</span><span class="sxs-lookup"><span data-stu-id="e1f69-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-243">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-244">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-245">QL2</span><span class="sxs-lookup"><span data-stu-id="e1f69-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-246">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-247">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-248">No</span><span class="sxs-lookup"><span data-stu-id="e1f69-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-250">No</span><span class="sxs-lookup"><span data-stu-id="e1f69-250">No</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="e1f69-251">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-252">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-253">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-254">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-255">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="e1f69-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-258">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-259">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="e1f69-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-260">Παραβίαση του Κανόνα #2 παραπάνω</span><span class="sxs-lookup"><span data-stu-id="e1f69-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="e1f69-261">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="e1f69-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="e1f69-262">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.</span><span class="sxs-lookup"><span data-stu-id="e1f69-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-263">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-264">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-265">QL2</span><span class="sxs-lookup"><span data-stu-id="e1f69-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-266">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-267">Κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-268">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-269">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-270">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-270">Yes</span></span> </p>
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
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-271">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-272">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-273">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-274">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-275">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="e1f69-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-276">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-277">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-278">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-279">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="e1f69-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-280">Σύμφωνα με τον Κανόνα #3 παραπάνω,</span><span class="sxs-lookup"><span data-stu-id="e1f69-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="e1f69-281">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="e1f69-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="e1f69-282">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="e1f69-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="e1f69-283">Η μόνη πρόσθετη επικύρωση είναι για το υποσύνολο των εργασιών στο QL1 που είναι διαφορετικές από το υποσύνολο των εργασιών στο QL2.</span><span class="sxs-lookup"><span data-stu-id="e1f69-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="e1f69-284">Με αυτόν τον τρόπο εξασφαλίζεται ότι δεν υπάρχουν επικαλύψεις.</span><span class="sxs-lookup"><span data-stu-id="e1f69-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="e1f69-285">Αυτό γίνεται από το σύστημα όταν σχετίζονται οι εργασίες.</span><span class="sxs-lookup"><span data-stu-id="e1f69-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-286">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-287">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-288">QL2</span><span class="sxs-lookup"><span data-stu-id="e1f69-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-289">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-290">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="e1f69-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-291">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-292">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-293">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-293">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="e1f69-294">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-295">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-296">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-297">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-298">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-299">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-300">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-301">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e1f69-302">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="e1f69-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-303">Με βάση τον κανόνα #5, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-304">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-305">Τ2</span><span class="sxs-lookup"><span data-stu-id="e1f69-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-306">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-307">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-308">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-309">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-310">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-311">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-311">Yes</span></span> </p>
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
            <td width="90" valign="top">
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
<span data-ttu-id="e1f69-312">O1</span><span class="sxs-lookup"><span data-stu-id="e1f69-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-313">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-314">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-315">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-316">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-317">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-318">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-319">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e1f69-320">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="e1f69-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e1f69-321">Με βάση τον κανόνα #4, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="e1f69-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e1f69-322">O2</span><span class="sxs-lookup"><span data-stu-id="e1f69-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e1f69-323">Τ1</span><span class="sxs-lookup"><span data-stu-id="e1f69-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-324">QL1</span><span class="sxs-lookup"><span data-stu-id="e1f69-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-325">Π1</span><span class="sxs-lookup"><span data-stu-id="e1f69-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="e1f69-326">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="e1f69-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-327">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e1f69-328">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e1f69-329">Ναι</span><span class="sxs-lookup"><span data-stu-id="e1f69-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e1f69-330">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="e1f69-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

