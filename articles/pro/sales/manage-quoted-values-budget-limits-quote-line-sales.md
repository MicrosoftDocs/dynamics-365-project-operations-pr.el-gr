---
title: Επισκόπηση γραμμών προσφοράς βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32337b05f09ef7c5b84fdff9870744d6367e2693
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994856"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="2e4c8-103">Επισκόπηση γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="2e4c8-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="2e4c8-104">_**Ισχύει για:** ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση, Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="2e4c8-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2e4c8-105">Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="2e4c8-106">Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="2e4c8-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="2e4c8-107">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="2e4c8-107">Billing Method</span></span>
- <span data-ttu-id="2e4c8-108">Αντιστοίχιση έργου και εργασιών</span><span class="sxs-lookup"><span data-stu-id="2e4c8-108">Project and Task Mapping</span></span>
- <span data-ttu-id="2e4c8-109">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="2e4c8-109">Included Transaction classes</span></span>
- <span data-ttu-id="2e4c8-110">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="2e4c8-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="2e4c8-111">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="2e4c8-111">Chargeability setup</span></span>
- <span data-ttu-id="2e4c8-112">Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="2e4c8-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="2e4c8-113">Πελάτες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="2e4c8-113">Quote line Customers</span></span>

<span data-ttu-id="2e4c8-114">Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="2e4c8-115">Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="2e4c8-116">**Πεδίο**</span><span class="sxs-lookup"><span data-stu-id="2e4c8-116">**Field**</span></span> | <span data-ttu-id="2e4c8-117">**Περιγραφή**</span><span class="sxs-lookup"><span data-stu-id="2e4c8-117">**Description**</span></span> | <span data-ttu-id="2e4c8-118">**Κατάντη επίπτωση**</span><span class="sxs-lookup"><span data-stu-id="2e4c8-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="2e4c8-119">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="2e4c8-119">Name</span></span> | <span data-ttu-id="2e4c8-120">Το όνομα της γραμμής προσφοράς που σας βοηθά να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που υπολογίζεται.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="2e4c8-121">Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-122">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="2e4c8-122">Billing Method</span></span> | <span data-ttu-id="2e4c8-123">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="2e4c8-124">Αυτό το πεδίο περιλαμβάνει τα δύο κύρια μοντέλα ανάθεσης συμβάσεων που υποστηρίζονται από το Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="2e4c8-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="2e4c8-125">- Προκαθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="2e4c8-125">- Fixed price</span></span></br><span data-ttu-id="2e4c8-126">- Χρόνος και υλικό.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-126">- Time and material.</span></span>| <span data-ttu-id="2e4c8-127">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-128">Project</span><span class="sxs-lookup"><span data-stu-id="2e4c8-128">Project</span></span> | <span data-ttu-id="2e4c8-129">Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="2e4c8-130">Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="2e4c8-131">Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="2e4c8-132">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="2e4c8-133">Εργασίες που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="2e4c8-133">Included Tasks</span></span> | <span data-ttu-id="2e4c8-134">Υποδεικνύει εάν αυτή η γραμμή προσφοράς χρησιμοποιείται για όλες ή ορισμένες από τις εργασίες έργου του επιλεγμένου έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="2e4c8-135">Το πεδίο αυτό έχει τις ακόλουθες πιθανές τιμές:</span><span class="sxs-lookup"><span data-stu-id="2e4c8-135">This field has the following possible values:</span></span></br><span data-ttu-id="2e4c8-136">- Όλες οι εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="2e4c8-136">- All project tasks</span></span></br><span data-ttu-id="2e4c8-137">- Επιλεγμένες εργασίες έργου μόνο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-137">- Selected project tasks only</span></span></br><span data-ttu-id="2e4c8-138">Μια κενή τιμή σε αυτό το πεδίο ισοδυναμεί με την επιλογή **Όλες οι εργασίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="2e4c8-139">Όταν επιλέγεται το **μόνο επιλεγμένες εργασίες έργου** στη σελίδα έργου, η καρτέλα **Ρύθμιση χρέωσης εργασίας** σάς επιτρέπει να επιλέξετε συγκεκριμένες εργασίες για να τις συσχετίσετε με αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="2e4c8-140">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-141">Συμπερίληψη χρόνου</span><span class="sxs-lookup"><span data-stu-id="2e4c8-141">Include Time</span></span> | <span data-ttu-id="2e4c8-142">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας στο επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-143">Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-144">Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2e4c8-145">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-146">Συμπερίληψη εξόδου</span><span class="sxs-lookup"><span data-stu-id="2e4c8-146">Include Expense</span></span> | <span data-ttu-id="2e4c8-147">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν το κόστος δαπανών στο επιλεγμένο έργο θα συμπεριληφθεί στην εκτίμηση στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-148">Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-149">Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2e4c8-150">Αυτή η τιμή αντιγράφεται πάνω από τη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-151">Συμπερίληψη υλικού</span><span class="sxs-lookup"><span data-stu-id="2e4c8-151">Include Material</span></span> | <span data-ttu-id="2e4c8-152">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν το κόστος υλικού στο επιλεγμένο έργο θα συμπεριληφθεί στην εκτίμηση στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-153">Μια τιμή **Όχι** υποδεικνύει ότι τα κόστη υλικού δεν θα συμπεριληφθούν στη εκτίμηση για αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-154">Μια τιμή **Ναι** υποδεικνύει ότι τα κόστη υλικού θα συμπεριληφθούν στη εκτίμηση για αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2e4c8-155">Αυτή η τιμή αντιγράφεται πάνω από τη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-156">Συμπερίληψη χρέωσης</span><span class="sxs-lookup"><span data-stu-id="2e4c8-156">Include Fee</span></span> | <span data-ttu-id="2e4c8-157">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-158">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2e4c8-159">Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2e4c8-160">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης Έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-161">Ποσό προσφοράς</span><span class="sxs-lookup"><span data-stu-id="2e4c8-161">Quoted Amount</span></span> | <span data-ttu-id="2e4c8-162">Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλη την εργασία που προβλέπεται σε αυτήν τη γραμμή προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="2e4c8-163">Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="2e4c8-164">Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="2e4c8-165">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-166">Εκτιμώμενος φόρος</span><span class="sxs-lookup"><span data-stu-id="2e4c8-166">Estimated Tax</span></span> | <span data-ttu-id="2e4c8-167">Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="2e4c8-168">Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="2e4c8-169">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-170">Ποσό προσφοράς μετά από φόρο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="2e4c8-171">Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="2e4c8-172">Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="2e4c8-173">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-174">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="2e4c8-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="2e4c8-175">Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="2e4c8-176">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2e4c8-177">Προϋπολογισμός πελάτη</span><span class="sxs-lookup"><span data-stu-id="2e4c8-177">Customer Budget</span></span> | <span data-ttu-id="2e4c8-178">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="2e4c8-179">Αυτή η τιμή αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζετε την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="2e4c8-180">Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="2e4c8-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="2e4c8-181">**Κανόνας 1**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, το έργο περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="2e4c8-182">**Κανόνας 2**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="2e4c8-183">**Κανόνας 3**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** έχει οριστεί σε **Μόνο επιλεγμένες εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν σε πολλές γραμμές προσφοράς βάσει έργου μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="2e4c8-184">**Κανόνας 4**: Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="2e4c8-185">**Κανόνας 5**: Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="2e4c8-186">
                    <strong>Ευκαιρία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="2e4c8-187">
                    <strong>Προσφορά</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="2e4c8-188">
                    <strong>Γραμμή προσφοράς</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="2e4c8-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="2e4c8-190">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="2e4c8-191">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="2e4c8-192">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="2e4c8-193">
                    <strong>Συμπερίληψη υλικού</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="2e4c8-194">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="2e4c8-195">
                    <strong>Χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="2e4c8-196">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="2e4c8-197">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2e4c8-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-198">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-199">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-200">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-201">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-202">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-203">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-204">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-205">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-206">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-207">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-208">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-208">Violation of Rule #2.</span></span> <span data-ttu-id="2e4c8-209">Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-210">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-211">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-212">QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-213">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-214">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-215">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-216">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-217">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-218">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-219">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-220">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-221">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-222">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-223">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-224">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-225">No</span><span class="sxs-lookup"><span data-stu-id="2e4c8-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-226">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-227">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-228">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-229">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-229">Violation of Rule #2.</span></span> <span data-ttu-id="2e4c8-230">Ο χρόνος, το υλικό και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-231">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-232">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-233">QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-234">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-235">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-236">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-240">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-241">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-242">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-243">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-244">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-245">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-246">No</span><span class="sxs-lookup"><span data-stu-id="2e4c8-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-247">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-248">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-249">Έγκυρη</span><span class="sxs-lookup"><span data-stu-id="2e4c8-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-250">Ο χρόνος, το υλικό και οι χρεώσεις για το έργο P1 περιλαμβάνονται στο QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="2e4c8-251">Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="2e4c8-252">Δεν υπάρχει επικάλυψη σε ό,τι περιλαμβάνεται σε κάθε γραμμή προσφοράς και επομένως είναι έγκυρο.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-253">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-254">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-255">QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-256">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-257">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-258">No</span><span class="sxs-lookup"><span data-stu-id="2e4c8-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-259">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-260">No</span><span class="sxs-lookup"><span data-stu-id="2e4c8-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-261">No</span><span class="sxs-lookup"><span data-stu-id="2e4c8-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-262">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-263">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-264">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-265">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-266">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-267">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-268">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-269">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-270">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-271">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-272">Παραβίαση του Κανόνα #2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="2e4c8-273">Το πρώτο τρίμηνο1 περιλαμβάνει χρόνο, υλικό, δαπάνες και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="2e4c8-274">Το δεύτερο τρίμηνο2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και, επομένως, επικαλύπτεται με τα στοιχεία που περιλαμβάνονται στο πρώτο τρίμηνο.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-275">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-276">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-277">QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-278">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-279">Κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-280">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-281">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-282">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-283">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-284">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-285">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-286">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-287">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-288">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-289">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-290">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-291">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-292">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-293">Έγκυρη</span><span class="sxs-lookup"><span data-stu-id="2e4c8-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-294">Σύμφωνα με τον κανόνα #3,</span><span class="sxs-lookup"><span data-stu-id="2e4c8-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="2e4c8-295">Το Q1 περιλαμβάνει χρόνο, υλικό, δαπάνες και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="2e4c8-296">Το QL2 περιλαμβάνει χρόνο, υλικό, έξοδα και χρεώσεις για ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="2e4c8-297">Η μόνη πρόσθετη επικύρωση είναι γύρω από το υποσύνολο εργασιών στο QL1 που διαφέρει από το υποσύνολο εργασιών στο QL2, ώστε να διασφαλιστεί ότι δεν υπάρχει επικάλυψη.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="2e4c8-298">Αυτό γίνεται από το σύστημα όταν σχετίζονται οι εργασίες.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-299">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-300">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-301">QL2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-302">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-303">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-304">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-305">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-306">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-307">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-308">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-309">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-310">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-311">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-312">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-313">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-314">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-315">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-316">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-317">Έγκυρη</span><span class="sxs-lookup"><span data-stu-id="2e4c8-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-318">Σύμφωνα με #5, το πρώτο και το δεύτερο τρίμηνο είναι δύο προσφορές στην ίδια ευκαιρία, ώστε να μπορούν και τα δύο να υπολογίσουν τα ίδια στοιχεία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-319">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-320">Τ2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-321">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-322">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-323">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-324">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-325">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-326">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-327">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-328">O1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-329">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-330">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-331">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-332">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-333">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-334">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-335">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-336">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-337">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="2e4c8-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2e4c8-338">Σύμφωνα με #4, το πρώτο και το δεύτερο τρίμηνο είναι δύο προσφορές σε διαφορετικές ευκαιρίες, ώστε να μην μπορούν να υπολογίσουν τα ίδια στοιχεία του ίδιου έργου.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="2e4c8-339">O2</span><span class="sxs-lookup"><span data-stu-id="2e4c8-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="2e4c8-340">Τ1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="2e4c8-341">QL1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-342">Π1</span><span class="sxs-lookup"><span data-stu-id="2e4c8-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="2e4c8-343">Όλες οι εργασίες έργου ή κενό</span><span class="sxs-lookup"><span data-stu-id="2e4c8-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="2e4c8-344">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="2e4c8-345">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="2e4c8-346">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2e4c8-347">Ναι</span><span class="sxs-lookup"><span data-stu-id="2e4c8-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
