---
title: Επισκόπηση γραμμών προσφοράς βάσει έργου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: be1663c0d226fa19fe4b9df566e16d215f1fc08e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181092"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="885d0-104">Επισκόπηση γραμμών προσφοράς βάσει έργου - lite</span><span class="sxs-lookup"><span data-stu-id="885d0-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="885d0-105">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="885d0-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="885d0-106">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="885d0-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="885d0-107">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="885d0-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="885d0-108">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="885d0-108">Billing Method</span></span>
- <span data-ttu-id="885d0-109">Αντιστοίχιση έργου και εργασιών</span><span class="sxs-lookup"><span data-stu-id="885d0-109">Project and Task Mapping</span></span>
- <span data-ttu-id="885d0-110">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="885d0-110">Included Transaction classes</span></span>
- <span data-ttu-id="885d0-111">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="885d0-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="885d0-112">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="885d0-112">Chargeability setup</span></span>
- <span data-ttu-id="885d0-113">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="885d0-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="885d0-114">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="885d0-114">Quote line Customers</span></span>

<span data-ttu-id="885d0-115">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="885d0-116">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="885d0-117">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="885d0-117">**Field**</span></span> | <span data-ttu-id="885d0-118">**Περιγραφή**</span><span class="sxs-lookup"><span data-stu-id="885d0-118">**Description**</span></span> | <span data-ttu-id="885d0-119">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="885d0-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="885d0-120">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="885d0-120">Name</span></span> | <span data-ttu-id="885d0-121">Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="885d0-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="885d0-122">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-123">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="885d0-123">Billing Method</span></span> | <span data-ttu-id="885d0-124">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="885d0-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="885d0-125">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια συμβαλλόμενα μοντέλα που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="885d0-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="885d0-126">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="885d0-126">- Fixed price</span></span></br><span data-ttu-id="885d0-127">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="885d0-127">- Time and material.</span></span>| <span data-ttu-id="885d0-128">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-129">Project</span><span class="sxs-lookup"><span data-stu-id="885d0-129">Project</span></span> | <span data-ttu-id="885d0-130">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="885d0-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="885d0-131">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="885d0-132">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="885d0-133">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="885d0-134">Εργασίες που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="885d0-134">Included Tasks</span></span> | <span data-ttu-id="885d0-135">Υποδεικνύει εάν αυτή η γραμμή προσφοράς χρησιμοποιείται για όλες ή ορισμένες από τις εργασίες έργου του επιλεγμένου έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="885d0-136">Το πεδίο αυτό έχει τις ακόλουθες πιθανές τιμές:</span><span class="sxs-lookup"><span data-stu-id="885d0-136">This field has the following possible values:</span></span></br><span data-ttu-id="885d0-137">- Όλες οι εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="885d0-137">- All project tasks</span></span></br><span data-ttu-id="885d0-138">- Επιλεγμένες εργασίες έργου μόνο</span><span class="sxs-lookup"><span data-stu-id="885d0-138">- Selected project tasks only</span></span></br><span data-ttu-id="885d0-139">Μια κενή τιμή σε αυτό το πεδίο ισοδυναμεί με την επιλογή **Όλες οι εργασίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="885d0-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="885d0-140">Όταν επιλέξετε **Μόνο επιλεγμένες εργασίες έργου**, στη συνέχεια, στη σελίδα έργου, η καρτέλα **Ρύθμιση χρέωσης εργασιών** σάς δίνει τη δυνατότητα να επιλέξετε συγκεκριμένες εργασίες για να τις συσχετίσετε με αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="885d0-141">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-142">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="885d0-142">Include Time</span></span> | <span data-ttu-id="885d0-143">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-144">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-145">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="885d0-146">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-147">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="885d0-147">Include Expense</span></span> | <span data-ttu-id="885d0-148">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-149">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-150">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="885d0-151">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-152">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="885d0-152">Include Fee</span></span> | <span data-ttu-id="885d0-153">Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-154">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="885d0-155">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="885d0-156">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-157">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="885d0-157">Quoted Amount</span></span> | <span data-ttu-id="885d0-158">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="885d0-159">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="885d0-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="885d0-160">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="885d0-161">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-162">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="885d0-162">Estimated Tax</span></span> | <span data-ttu-id="885d0-163">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="885d0-164">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="885d0-165">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-166">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="885d0-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="885d0-167">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="885d0-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="885d0-168">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="885d0-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="885d0-169">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-170">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="885d0-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="885d0-171">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="885d0-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="885d0-172">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="885d0-173">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="885d0-173">Customer Budget</span></span> | <span data-ttu-id="885d0-174">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="885d0-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="885d0-175">Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="885d0-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="885d0-176">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="885d0-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="885d0-177">**Κανόνας 1**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, το έργο περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="885d0-178">**Κανόνας 2**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="885d0-179">**Κανόνας 3**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** έχει οριστεί σε **Μόνο επιλεγμένες εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν σε πολλές γραμμές προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="885d0-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="885d0-180">**Κανόνας 4**: Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="885d0-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="885d0-181">**Κανόνας 5**: Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="885d0-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="885d0-182">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="885d0-183">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="885d0-184">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="885d0-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="885d0-186">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="885d0-187">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="885d0-188">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="885d0-189">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="885d0-190">
                    <strong>Χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="885d0-191">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="885d0-192">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="885d0-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-193">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-194">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-195">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-196">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-197">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-198">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-199">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-200">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-201">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="885d0-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-202">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="885d0-202">Violation of Rule #2.</span></span> <span data-ttu-id="885d0-203">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="885d0-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-204">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-205">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-206">QL2</span><span class="sxs-lookup"><span data-stu-id="885d0-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-207">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-208">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-209">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-210">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-211">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-211">Yes</span></span> </p>
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
<span data-ttu-id="885d0-212">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-213">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-214">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-215">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-216">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-217">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-218">No</span><span class="sxs-lookup"><span data-stu-id="885d0-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-220">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="885d0-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-221">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="885d0-221">Violation of Rule #2.</span></span> <span data-ttu-id="885d0-222">Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.</span><span class="sxs-lookup"><span data-stu-id="885d0-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-223">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-224">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-225">QL2</span><span class="sxs-lookup"><span data-stu-id="885d0-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-226">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-227">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-228">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-229">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-230">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-230">Yes</span></span> </p>
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
<span data-ttu-id="885d0-231">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-232">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-233">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-234">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-235">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-236">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-237">No</span><span class="sxs-lookup"><span data-stu-id="885d0-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-239">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="885d0-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="885d0-240">Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.</span><span class="sxs-lookup"><span data-stu-id="885d0-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="885d0-241">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.</span><span class="sxs-lookup"><span data-stu-id="885d0-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="885d0-242">Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς και είναι έγκυρη.</span><span class="sxs-lookup"><span data-stu-id="885d0-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-243">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-244">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-245">QL2</span><span class="sxs-lookup"><span data-stu-id="885d0-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-246">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-247">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-248">No</span><span class="sxs-lookup"><span data-stu-id="885d0-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-250">No</span><span class="sxs-lookup"><span data-stu-id="885d0-250">No</span></span> </p>
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
<span data-ttu-id="885d0-251">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-252">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-253">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-254">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-255">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="885d0-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-258">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-259">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="885d0-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-260">Παραβίαση του Κανόνα #2 παραπάνω</span><span class="sxs-lookup"><span data-stu-id="885d0-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="885d0-261">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="885d0-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="885d0-262">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.</span><span class="sxs-lookup"><span data-stu-id="885d0-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-263">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-264">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-265">QL2</span><span class="sxs-lookup"><span data-stu-id="885d0-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-266">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-267">Κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-268">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-269">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-270">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-270">Yes</span></span> </p>
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
<span data-ttu-id="885d0-271">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-272">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-273">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-274">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-275">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="885d0-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-276">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-277">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-278">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-279">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="885d0-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-280">Σύμφωνα με τον Κανόνα #3 παραπάνω,</span><span class="sxs-lookup"><span data-stu-id="885d0-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="885d0-281">Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="885d0-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="885d0-282">Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="885d0-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="885d0-283">Η μόνη πρόσθετη επικύρωση είναι για το υποσύνολο των εργασιών στο QL1 που είναι διαφορετικές από το υποσύνολο των εργασιών στο QL2.</span><span class="sxs-lookup"><span data-stu-id="885d0-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="885d0-284">Με αυτόν τον τρόπο εξασφαλίζεται ότι δεν υπάρχουν επικαλύψεις.</span><span class="sxs-lookup"><span data-stu-id="885d0-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="885d0-285">Αυτό γίνεται από το σύστημα όταν σχετίζονται οι εργασίες.</span><span class="sxs-lookup"><span data-stu-id="885d0-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-286">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-287">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-288">QL2</span><span class="sxs-lookup"><span data-stu-id="885d0-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-289">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-290">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="885d0-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-291">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-292">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-293">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-293">Yes</span></span> </p>
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
<span data-ttu-id="885d0-294">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-295">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-296">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-297">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-298">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-299">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-300">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-301">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="885d0-302">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="885d0-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-303">Με βάση τον κανόνα #5, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-304">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-305">Τ2</span><span class="sxs-lookup"><span data-stu-id="885d0-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-306">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-307">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-308">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-309">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-310">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-311">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-311">Yes</span></span> </p>
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
<span data-ttu-id="885d0-312">O1</span><span class="sxs-lookup"><span data-stu-id="885d0-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-313">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-314">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-315">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-316">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-317">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-318">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-319">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="885d0-320">Έγκυρα</span><span class="sxs-lookup"><span data-stu-id="885d0-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="885d0-321">Με βάση τον κανόνα #4, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="885d0-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="885d0-322">O2</span><span class="sxs-lookup"><span data-stu-id="885d0-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="885d0-323">Τ1</span><span class="sxs-lookup"><span data-stu-id="885d0-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-324">QL1</span><span class="sxs-lookup"><span data-stu-id="885d0-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-325">Π1</span><span class="sxs-lookup"><span data-stu-id="885d0-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="885d0-326">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="885d0-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-327">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="885d0-328">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="885d0-329">Ναι</span><span class="sxs-lookup"><span data-stu-id="885d0-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="885d0-330">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="885d0-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

