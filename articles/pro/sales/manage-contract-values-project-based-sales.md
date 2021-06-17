---
title: Επισκόπηση γραμμών σύμβασης βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με γραμμές σύμβασης βάσει έργου.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8af32b0475650db9c5862ea23d185588a631ade6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003136"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="4277d-103">Επισκόπηση γραμμών σύμβασης βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="4277d-103">Project-based contract lines overview</span></span>

<span data-ttu-id="4277d-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="4277d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4277d-105">Οι γραμμές σύμβασης βάσει έργου στο Dynamics 365 Project Operations έχουν σχεδιαστεί για τη διατήρηση των συμβάσεων εκτίμησης και χρέωσης για συγκεκριμένα στοιχεία της εργασίας έργου σε μια δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="4277d-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="4277d-106">Η δομή μιας γραμμής σύμβασης βάσει έργου επεκτείνεται για εκτιμήσεις έργων και σενάρια χρέωσης με τις ακόλουθες έννοιες:</span><span class="sxs-lookup"><span data-stu-id="4277d-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="4277d-107">Μέθοδος χρέωσης</span><span class="sxs-lookup"><span data-stu-id="4277d-107">Billing method</span></span>
- <span data-ttu-id="4277d-108">Αντιστοίχιση έργου και εργασιών</span><span class="sxs-lookup"><span data-stu-id="4277d-108">Project and task mapping</span></span>
- <span data-ttu-id="4277d-109">Κατηγορίες συναλλαγής που περιλαμβάνονται</span><span class="sxs-lookup"><span data-stu-id="4277d-109">Included transaction classes</span></span>
- <span data-ttu-id="4277d-110">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="4277d-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="4277d-111">Ρύθμιση χρέωσης</span><span class="sxs-lookup"><span data-stu-id="4277d-111">Chargeability setup</span></span>
- <span data-ttu-id="4277d-112">Εκτιμήσεις χρησιμοποιώντας τις λεπτομέρειες γραμμής σύμβασης</span><span class="sxs-lookup"><span data-stu-id="4277d-112">Estimates using contract line details</span></span>
- <span data-ttu-id="4277d-113">Πελάτης γραμμής σύμβασης</span><span class="sxs-lookup"><span data-stu-id="4277d-113">Contract line customers</span></span>

<span data-ttu-id="4277d-114">Ο παρακάτω πίνακας περιλαμβάνει τα πεδία στην καρτέλα **Γενικά** των γραμμών σύμβασης βάσει έργου που σας βοηθούν να ορίσετε τη βάση μιας λεπτομερούς εκτίμησης, της αρχικής εκτίμησης και των λεπτομερειών χρέωσης για την εργασία βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="4277d-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="4277d-115">Πεδίο</span><span class="sxs-lookup"><span data-stu-id="4277d-115">Field</span></span> | <span data-ttu-id="4277d-116">Περιγραφή</span><span class="sxs-lookup"><span data-stu-id="4277d-116">Description</span></span> | <span data-ttu-id="4277d-117">Κατάντη επίπτωση</span><span class="sxs-lookup"><span data-stu-id="4277d-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4277d-118">**Όνομα**.</span><span class="sxs-lookup"><span data-stu-id="4277d-118">**Name**</span></span> | <span data-ttu-id="4277d-119">Όνομα της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-119">Name of the contract line.</span></span> <span data-ttu-id="4277d-120">Με αυτόν τον τρόπο προσδιορίζεται το διακριτό στοιχείο της σύμβασης που εκτιμάται.</span><span class="sxs-lookup"><span data-stu-id="4277d-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="4277d-121">Για μια σύμβαση έργου που έχει δημιουργηθεί από μια προσφορά, αυτή η τιμή αντιγράφεται από μια αντίστοιχη τιμή της γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="4277d-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="4277d-122">Το όνομα που αντιγράφηκε στη γραμμή τιμολογίου βάσει έργου που δημιουργείται από αυτήν τη γραμμή σύμβασης κατά τη δημιουργία του τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="4277d-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="4277d-123">**Μέθοδος χρέωσης**</span><span class="sxs-lookup"><span data-stu-id="4277d-123">**Billing Method**</span></span> | <span data-ttu-id="4277d-124">Σε μια σύμβαση έργου που έχει δημιουργηθεί από μια προσφορά, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="4277d-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="4277d-125">Πρόκειται για ένα σύνολο επιλογών που αντιπροσωπεύει τα δύο κύρια συμβαλλόμενα μοντέλα που υποστηρίζονται από το Project Operations:</span><span class="sxs-lookup"><span data-stu-id="4277d-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="4277d-126">- **Σταθερή τιμή**</span><span class="sxs-lookup"><span data-stu-id="4277d-126">- **Fixed Price**</span></span></br><span data-ttu-id="4277d-127">- **Χρόνος και υλικό**</span><span class="sxs-lookup"><span data-stu-id="4277d-127">- **Time and Material**</span></span> | <span data-ttu-id="4277d-128">Με βάση τη μέθοδο χρέωσης της γραμμής σύμβασης αναφοράς, η πραγματική συναλλαγή θα διεκπεραιωθεί.</span><span class="sxs-lookup"><span data-stu-id="4277d-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="4277d-129">Εάν η γραμμή σύμβασης στην οποία γίνεται αναφορά από την πραγματική τιμή έχει μια μέθοδο χρέωσης χρόνου και υλικού, δημιουργούνται καρτέλες πραγματικών μη τιμολογημένων πωλήσεων και κόστους.</span><span class="sxs-lookup"><span data-stu-id="4277d-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="4277d-130">Εάν η γραμμή σύμβασης στην οποία γίνεται αναφορά από την πραγματική τιμή έχει μια μέθοδο χρέωσης με σταθερή τιμή, δημιουργείται μόνο μια πραγματική δαπάνη.</span><span class="sxs-lookup"><span data-stu-id="4277d-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="4277d-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="4277d-131">**Project**</span></span> | <span data-ttu-id="4277d-132">Χρησιμοποιήστε αυτό το πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση.</span><span class="sxs-lookup"><span data-stu-id="4277d-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="4277d-133">Αυτή η τιμή θα χρησιμοποιηθεί σε συνδυασμό με τις **εργασίες που περιλαμβάνονται** και τις **κλάσεις συναλλαγών που περιλαμβάνονται** για την επίλυση της αναφοράς γραμμής σύμβασης σε μια πραγματική καρτέλα ή μια καρτέλα γραμμής εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="4277d-134">**Εργασίες που περιλαμβάνονται**</span><span class="sxs-lookup"><span data-stu-id="4277d-134">**Included Tasks**</span></span> | <span data-ttu-id="4277d-135">Υποδεικνύει εάν αυτή η γραμμή σύμβασης περιλαμβάνει όλες τις εργασίες έργου για το επιλεγμένο έργο ή μόνο ένα υποσύνολο των εργασιών.</span><span class="sxs-lookup"><span data-stu-id="4277d-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="4277d-136">Πρόκειται για μια σύνολο επιλογών που έχει τις ακόλουθες πιθανές τιμές:</span><span class="sxs-lookup"><span data-stu-id="4277d-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="4277d-137">- **Όλες οι εργασίες έργων**</span><span class="sxs-lookup"><span data-stu-id="4277d-137">- **All Project Tasks**</span></span></br><span data-ttu-id="4277d-138">- **Επιλεγμένες εργασίες έργου μόνο**.</span><span class="sxs-lookup"><span data-stu-id="4277d-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="4277d-139">Μια κενή τιμή σε αυτό το πεδίο ισούται με την επιλογή **Όλες οι εργασίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="4277d-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="4277d-140">Εάν έχετε επιλέξει **Μόνο οι επιλεγμένες εργασίες**, μπορείτε να επιλέξετε συγκεκριμένες εργασίες και να τις συσχετίσετε με αυτήν τη γραμμή σύμβασης στην καρτέλα **Ρύθμιση χρέωσης εργασίας** στη σελίδα **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="4277d-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="4277d-141">Αυτή η τιμή θα χρησιμοποιηθεί σε συνδυασμό με τις κατηγορίες **Έργο** και **Συναλλαγή που περιλαμβάνεται** για την επίλυση της αναφοράς γραμμής σύμβασης σε μια καρτέλα πραγματικής τιμής ή γραμμής εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="4277d-142">**Συμπερίληψη χρόνου**</span><span class="sxs-lookup"><span data-stu-id="4277d-142">**Include Time**</span></span> | <span data-ttu-id="4277d-143">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας στο επιλεγμένο έργο θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="4277d-144">Μια τιμή **Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="4277d-145">Μια τιμή **Ναι** υποδεικνύει ότι αυτό θα γίνει.</span><span class="sxs-lookup"><span data-stu-id="4277d-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="4277d-146">Αυτή η τιμή χρησιμοποιείται σε συνδυασμό με το έργο για την επίλυση της αναφοράς γραμμής σύμβασης σε μια πραγματική ή μια εκτιμώμενη γραμμή εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="4277d-147">**Συμπερίληψη εξόδου**</span><span class="sxs-lookup"><span data-stu-id="4277d-147">**Include Expense**</span></span> | <span data-ttu-id="4277d-148">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη εξόδων στο επιλεγμένο έργο θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="4277d-149">Μια τιμή **Όχι** υποδεικνύει ότι τα κόστη δεν θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="4277d-150">Μια τιμή **Ναι** υποδεικνύει ότι αυτό θα γίνει.</span><span class="sxs-lookup"><span data-stu-id="4277d-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="4277d-151">Αυτή η τιμή χρησιμοποιείται σε συνδυασμό με το έργο για την επίλυση της αναφοράς γραμμής σύμβασης σε μια πραγματική ή μια εκτιμώμενη γραμμή εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="4277d-152">**Συμπερίληψη υλικών**</span><span class="sxs-lookup"><span data-stu-id="4277d-152">**Include Materials**</span></span> | <span data-ttu-id="4277d-153">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη υλικού στο επιλεγμένο έργο θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="4277d-154">Μια τιμή **Όχι** υποδεικνύει ότι τα κόστη υλικού δεν θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="4277d-155">Μια τιμή **Ναι** υποδεικνύει ότι αυτό θα γίνει.</span><span class="sxs-lookup"><span data-stu-id="4277d-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="4277d-156">Αυτή η τιμή χρησιμοποιείται σε συνδυασμό με το έργο για την επίλυση της αναφοράς γραμμής σύμβασης σε μια πραγματική ή μια εκτιμώμενη γραμμή εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="4277d-157">**Συμπερίληψη χρέωσης**</span><span class="sxs-lookup"><span data-stu-id="4277d-157">**Include Fee**</span></span> | <span data-ttu-id="4277d-158">Μια τιμή **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις στο επιλεγμένο έργο θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="4277d-159">Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν σε αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="4277d-160">Μια τιμή **Ναι** υποδεικνύει ότι αυτό θα γίνει.</span><span class="sxs-lookup"><span data-stu-id="4277d-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="4277d-161">Αυτή η τιμή χρησιμοποιείται σε συνδυασμό με το έργο για την επίλυση της αναφοράς γραμμής σύμβασης σε μια πραγματική ή μια εκτιμώμενη γραμμή εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="4277d-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="4277d-162">**Συμβατικό ποσό**</span><span class="sxs-lookup"><span data-stu-id="4277d-162">**Contracted Amount**</span></span> | <span data-ttu-id="4277d-163">Σε μια γραμμή σύμβασης με προκαθορισμένη τιμή, αυτό το ποσό είναι η τιμή που έχει συμφωνηθεί και η οποία θα τιμολογηθεί στον πελάτη για όλα τα στοιχεία εργασίας που σχετίζονται με αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="4277d-164">Σε μια γραμμή σύμβασης χρόνου και υλικού, αυτό το ποσό είναι μια εκτιμώμενη τιμή η οποία θα τιμολογηθεί στον πελάτη για όλα τα στοιχεία εργασίας που σχετίζονται με αυτήν τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="4277d-165">Σε μια σύμβαση έργου που έχει δημιουργηθεί από μια προσφορά, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο της γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="4277d-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="4277d-166">Όταν μια γραμμή σύμβασης με βάση ένα έργο έχει λεπτομέρειες σχετικά με τη γραμμή, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="4277d-167">Όταν η γραμμή σύμβασης περιέχει λεπτομέρειες σχετικά με τη γραμμή, αυτή η τιμή μπορεί να τροποποιηθεί με την αλλαγή των ποσών στις λεπτομέρειες της γραμμής.</span><span class="sxs-lookup"><span data-stu-id="4277d-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="4277d-168">Σε μια γραμμή σύμβασης με προκαθορισμένη τιμή, αυτή η τιμή χρησιμοποιείται για τη δημιουργία του ποσού πριν από τη φορολόγηση των περιοδικών ορόσημων χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="4277d-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="4277d-169">**Εκτιμώμενος φόρος**</span><span class="sxs-lookup"><span data-stu-id="4277d-169">**Estimated Tax**</span></span> | <span data-ttu-id="4277d-170">Ο χρήστης μπορεί να επεξεργαστεί αυτό το πεδίο για να εισαγαγάγει το υπολογιζόμενο ποσό φόρου στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="4277d-171">Όταν μια γραμμή σύμβασης με βάση ένα έργο έχει λεπτομέρειες σχετικά με τη γραμμή, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="4277d-172">Όταν η γραμμή σύμβασης περιέχει λεπτομέρειες σχετικά με τη γραμμή, αυτή η τιμή μπορεί να τροποποιηθεί με την αλλαγή των ποσών φόρου στις λεπτομέρειες της γραμμής.</span><span class="sxs-lookup"><span data-stu-id="4277d-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="4277d-173">Σε μια γραμμή σύμβασης με προκαθορισμένη τιμή, αυτή η τιμή χρησιμοποιείται για τη δημιουργία του φόρου σε περιοδικά ορόσημα χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="4277d-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="4277d-174">**Συμβατικό ποσό μετά από φόρο**</span><span class="sxs-lookup"><span data-stu-id="4277d-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="4277d-175">Το ποσό γραμμής σύμβασης μετά από φόρο.</span><span class="sxs-lookup"><span data-stu-id="4277d-175">The contract line amount after tax.</span></span> <span data-ttu-id="4277d-176">Αυτό το πεδίο είναι μόνο για ανάγνωση και υπολογίζεται ως **Ποσό σύμβασης + Φόρος**.</span><span class="sxs-lookup"><span data-stu-id="4277d-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="4277d-177">Σε μια γραμμή σύμβασης με προκαθορισμένη τιμή, αυτή η τιμή χρησιμοποιείται για τη δημιουργία περιοδικών ορόσημων χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="4277d-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="4277d-178">**Όριο που δεν πρέπει να υπερβαίνεται**</span><span class="sxs-lookup"><span data-stu-id="4277d-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="4277d-179">Ο χρήστης μπορεί να επεξεργαστεί αυτό το πεδίο και είναι διαθέσιμο μόνο σε γραμμές σύμβασης βάσει έργου που έχουν ορίσει τη μέθοδο χρέωσης ως ώρα και υλικό.</span><span class="sxs-lookup"><span data-stu-id="4277d-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="4277d-180">Ο χρήστης μπορεί να επεξεργαστεί αυτό το πεδίο.</span><span class="sxs-lookup"><span data-stu-id="4277d-180">The user can edit this field.</span></span> <span data-ttu-id="4277d-181">Όταν μια πραγματική για την ώρα και το υλικό αναφέρεται σε αυτήν τη γραμμή σύμβασης για τον χρόνο και το υλικό, το ποσό στην πραγματική τιμή αξιολογείται με βάση το όριο που δεν πρέπει να υπερβαίνει τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="4277d-182">Αυτή η αξιολόγηση ολοκληρώνεται αφού καταληφθούν τα ποσά που έχουν ήδη δαπανηθεί και δεσμευτεί.</span><span class="sxs-lookup"><span data-stu-id="4277d-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="4277d-183">**Προϋπολογισμός πελάτη**</span><span class="sxs-lookup"><span data-stu-id="4277d-183">**Customer Budget**</span></span> | <span data-ttu-id="4277d-184">Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή σύμβασης αν η σύμβαση έχει δημιουργηθεί από μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="4277d-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="4277d-185">Αυτό το πεδίο χρησιμοποιείται μόνο για πληροφορίες και δεν έχει καμία κατάντη σημασία.</span><span class="sxs-lookup"><span data-stu-id="4277d-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="4277d-186">Κανόνες επικύρωσης για τις επιλογές στην καρτέλα "Γενικά" των γραμμών σύμβασης βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="4277d-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="4277d-187">Κανόνας 1: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή έχει οριστεί σε **Όλες οι εργασίες έργου**, όλες οι εργασίες του έργου περιλαμβάνονται στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="4277d-188">Κανόνας 2: Όταν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή ορίζεται ρητά στο στοιχείο **Όλες οι εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής είναι δυνατό να συμπεριληφθούν μόνο σε μια γραμμή σύμβασης βάσει έργου μιας σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="4277d-189">Κανόνας 3: Όταν το πεδίο **Εργασίες που περιλαμβάνονται** ορίζεται στο στοιχείο **Επιλεγμένες εργασίες έργου μόνο**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής είναι δυνατό να συμπεριληφθούν μόνο πολλαπλές γραμμές σύμβασης βάσει έργου μιας σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="4277d-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="4277d-190">
                    <strong>Σύμβαση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="4277d-191">
                    <strong>Γραμμή σύμβασης</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4277d-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="4277d-193">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="4277d-194">
                    <strong>Συμπερίληψη χρόνου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="4277d-195">
                    <strong>Συμπερίληψη εξόδου</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4277d-196">
                    <strong>Συμπερίληψη υλικών</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="4277d-197">
                    <strong>Συμπερίληψη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="4277d-198">
                    <strong>Χρέωση</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="4277d-199">
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="4277d-200">
                    <strong>Αιτία</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4277d-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-201">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-202">CL1</span><span class="sxs-lookup"><span data-stu-id="4277d-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-203">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-204">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-205">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-206">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-207">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-208">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-209">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="4277d-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-210">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="4277d-210">Violation of Rule #2.</span></span> <span data-ttu-id="4277d-211">Ο χρόνος, το έξοδο, τα υλικά και οι χρεώσεις για το έργο P1 περιλαμβάνονται και στις δύο γραμμές σύμβασης CL1 και CL2.</span><span class="sxs-lookup"><span data-stu-id="4277d-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-212">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-213">CL2</span><span class="sxs-lookup"><span data-stu-id="4277d-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-214">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-215">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-216">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-217">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-218">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-220">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-221">CL1</span><span class="sxs-lookup"><span data-stu-id="4277d-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-222">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-223">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-224">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-225">No</span><span class="sxs-lookup"><span data-stu-id="4277d-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-226">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-227">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-228">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="4277d-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-229">Παραβίαση του Κανόνα #2.</span><span class="sxs-lookup"><span data-stu-id="4277d-229">Violation of Rule #2.</span></span> <span data-ttu-id="4277d-230">Ο χρόνος, τα υλικά και οι χρεώσεις για το έργο P1 περιλαμβάνονται και στις δύο γραμμές σύμβασης CL1 και CL2.</span><span class="sxs-lookup"><span data-stu-id="4277d-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-231">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-232">CL2</span><span class="sxs-lookup"><span data-stu-id="4277d-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-233">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-234">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-235">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-236">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-238">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-239">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-240">CL1</span><span class="sxs-lookup"><span data-stu-id="4277d-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-241">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-242">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-243">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-244">No</span><span class="sxs-lookup"><span data-stu-id="4277d-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-245">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-246">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-247">Έγκυρη</span><span class="sxs-lookup"><span data-stu-id="4277d-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-248">Ο χρόνος, τα υλικά και οι χρεώσεις για το έργο P1 περιλαμβάνονται στο CL1.</span><span class="sxs-lookup"><span data-stu-id="4277d-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="4277d-249">Η δαπάνη στο έργο P1 περιλαμβάνεται στο CL2.</span><span class="sxs-lookup"><span data-stu-id="4277d-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="4277d-250">Δεν υπάρχει επικάλυψη σε ό,τι περιλαμβάνεται σε κάθε γραμμή σύμβασης και επομένως είναι έγκυρο.</span><span class="sxs-lookup"><span data-stu-id="4277d-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-251">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-252">CL2</span><span class="sxs-lookup"><span data-stu-id="4277d-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-253">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-254">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-255">No</span><span class="sxs-lookup"><span data-stu-id="4277d-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-256">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-257">No</span><span class="sxs-lookup"><span data-stu-id="4277d-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-258">No</span><span class="sxs-lookup"><span data-stu-id="4277d-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-259">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-260">CL1</span><span class="sxs-lookup"><span data-stu-id="4277d-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-261">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-262">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="4277d-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-263">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-264">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-265">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-266">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-267">Μη έγκυρο</span><span class="sxs-lookup"><span data-stu-id="4277d-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-268">Παραβίαση του Κανόνα #2</span><span class="sxs-lookup"><span data-stu-id="4277d-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="4277d-269">Το C1 περιλαμβάνει χρόνο, υλικά, δαπάνες και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="4277d-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4277d-270">Το CL2 περιλαμβάνει χρόνο, υλικά, δαπάνες και χρεώσεις για ολόκληρο το έργο P1 και ως εκ τούτου επικαλύπτεται με αυτά που περιλαμβάνονται στο C1.</span><span class="sxs-lookup"><span data-stu-id="4277d-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-271">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-272">CL2</span><span class="sxs-lookup"><span data-stu-id="4277d-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-273">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-274">Κενό</span><span class="sxs-lookup"><span data-stu-id="4277d-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-275">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-276">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-277">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-278">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-279">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-280">CL1</span><span class="sxs-lookup"><span data-stu-id="4277d-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-281">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-282">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="4277d-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-283">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-284">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-285">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-286">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-287">Έγκυρη</span><span class="sxs-lookup"><span data-stu-id="4277d-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4277d-288">Σύμφωνα με τον κανόνα #3</span><span class="sxs-lookup"><span data-stu-id="4277d-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="4277d-289">Το C1 περιλαμβάνει χρόνο, έξοδαμ υλικά και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="4277d-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4277d-290">Το CL2 περιλαμβάνει χρόνο, έξοδαμ υλικά και χρεώσεις για ένα υποσύνολο εργασιών στο έργο P1.</span><span class="sxs-lookup"><span data-stu-id="4277d-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="4277d-291">Η μόνη πρόσθετη επικύρωση είναι γύρω από το υποσύνολο εργασιών στο CL1 και διαφέρει από το υποσύνολο εργασιών στο CL2, ώστε να διασφαλιστεί ότι δεν υπάρχουν επικαλύπτονται εκεί.</span><span class="sxs-lookup"><span data-stu-id="4277d-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="4277d-292">Αυτό γίνεται από το σύστημα όταν σχετίζονται οι εργασίες.</span><span class="sxs-lookup"><span data-stu-id="4277d-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="4277d-293">C1</span><span class="sxs-lookup"><span data-stu-id="4277d-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="4277d-294">CL2</span><span class="sxs-lookup"><span data-stu-id="4277d-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-295">Π1</span><span class="sxs-lookup"><span data-stu-id="4277d-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="4277d-296">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="4277d-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-297">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="4277d-298">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-299">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="4277d-300">Ναι</span><span class="sxs-lookup"><span data-stu-id="4277d-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
