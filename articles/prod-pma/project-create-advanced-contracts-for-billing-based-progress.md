---
title: Δημιουργία σύνθετων συμβάσεων για χρέωση με βάση την πρόοδο
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας συμβάσεων έργου έτσι ώστε να μπορείτε να δημιουργήσετε τιμολόγια για πελάτες, με βάση ένα ποσοστό ολοκληρωμένης εργασίας.
author: RadhikaRS
manager: AnnBe
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1a83785a9db4dffc4585acf11ef971c08594f312
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077045"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="e0176-103">Δημιουργία σύνθετων συμβάσεων για χρέωση με βάση την πρόοδο</span><span class="sxs-lookup"><span data-stu-id="e0176-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="e0176-104">Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας συμβάσεων έργου έτσι ώστε να μπορείτε να δημιουργήσετε τιμολόγια για πελάτες, με βάση ένα ποσοστό ολοκληρωμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="e0176-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="e0176-105">Τα ποσά τιμολογίων υπολογίζονται αυτόματα για τις κατηγορίες προϋπολογισμού του έργου που ορίζετε για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="e0176-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="e0176-106">Ο χρόνος τιμολόγησης ορίζεται όταν διαπραγματεύεστε τη σύμβαση έργου με τον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="e0176-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="e0176-107">Χρησιμοποιήστε τις διαδικασίες σε αυτό το θέμα για να δημιουργήσετε μια σύμβαση, ένα συσχετισμένο έργο και τους κανόνες χρέωσης που υπολογίζουν ποσά τιμολογίων για τις κατηγορίες προϋπολογισμού της εργασίας που ορίζετε για το έργο.</span><span class="sxs-lookup"><span data-stu-id="e0176-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="e0176-108">Αφού δημιουργήσετε τη σύμβαση και το έργο, μπορείτε να δημιουργήσετε τις λεπτομέρειες του έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="e0176-109">Για παράδειγμα, μπορείτε να καθορίσετε τις δραστηριότητες και να αναθέσετε εργαζομένους στο έργο.</span><span class="sxs-lookup"><span data-stu-id="e0176-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="e0176-110">Παράδειγμα</span><span class="sxs-lookup"><span data-stu-id="e0176-110">Example</span></span>

<span data-ttu-id="e0176-111">Ο οργανισμός σας είναι μια εταιρεία ανάπτυξης λογισμικού.</span><span class="sxs-lookup"><span data-stu-id="e0176-111">Your organization is a software development firm.</span></span> <span data-ttu-id="e0176-112">Συμφωνείτε να αναπτύξετε ένα πακέτο λογαριασμών μισθοδοσίας για έναν πελάτη με συνολικό κόστος 20.000 δολάρια ΗΠΑ (USD).</span><span class="sxs-lookup"><span data-stu-id="e0176-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="e0176-113">Ο οργανισμός σας συμφωνεί με την τιμολόγηση του πελάτη καθώς ολοκληρώνετε συγκεκριμένα ποσοστά του έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="e0176-114">Μπορείτε να ορίσετε τις παρακάτω κατηγορίες έργου για την εργασία, έτσι ώστε να μπορείτε να τις χρησιμοποιήσετε στη διαδικασία χρέωσης:</span><span class="sxs-lookup"><span data-stu-id="e0176-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="e0176-115">Συμβουλευτικές υπηρεσίες</span><span class="sxs-lookup"><span data-stu-id="e0176-115">Consulting</span></span>
- <span data-ttu-id="e0176-116">Σχεδίαση</span><span class="sxs-lookup"><span data-stu-id="e0176-116">Design</span></span>
- <span data-ttu-id="e0176-117">Εγκατάσταση</span><span class="sxs-lookup"><span data-stu-id="e0176-117">Installation</span></span>

<span data-ttu-id="e0176-118">Μπορείτε επίσης να ορίσετε κανόνες χρέωσης που υπολογίζουν αυτόματα τα ποσά τιμολόγησης για το ποσοστό της εργασίας έργου που ολοκληρώνεται για κάθε κατηγορία.</span><span class="sxs-lookup"><span data-stu-id="e0176-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="e0176-119">Η διαχείριση προϋπολογισμού δημιουργεί έναν προϋπολογισμό για τις κατηγορίες έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="e0176-120">Ο όγκος της ολοκληρωμένης εργασίας υπολογίζεται αυτόματα ως ποσοστό της πραγματικής εργασίας σε σύγκριση με τα προϋπολογισμένα ποσά.</span><span class="sxs-lookup"><span data-stu-id="e0176-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0176-121">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="e0176-121">Prerequisites</span></span>

<span data-ttu-id="e0176-122">Για να δημιουργήσετε ένα έργο που χρησιμοποιεί κανόνες χρέωσης, πρέπει να ορίσετε τις ακολουθίες αριθμών για τους κανόνες χρέωσης και ένα ημερολόγιο τελών που χρησιμοποιείται για την καταχώρηση των χρεώσεων προόδου.</span><span class="sxs-lookup"><span data-stu-id="e0176-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="e0176-123">Μεταβείτε στη **Διαχείριση έργου και λογιστική** \> **Ρύθμιση** \> **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="e0176-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="e0176-124">Στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής** , στην καρτέλα **Ακολουθίες αριθμών** , ρυθμίστε την ακολουθία αριθμών που θέλετε να χρησιμοποιήσετε όταν δημιουργούνται οι κανόνες χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="e0176-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="e0176-125">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** \> **Ημερολόγια** \> **Χρέωση**.</span><span class="sxs-lookup"><span data-stu-id="e0176-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="e0176-126">Στη σελίδα **Ημερολόγιο τελών** , επιλέξτε **Δημιουργία** και καταχωρίστε το όνομα του ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="e0176-126">On the **Fee journal** page, select **New** , and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="e0176-127">Δημιουργία σύμβασης για τις χρεώσεις προόδου</span><span class="sxs-lookup"><span data-stu-id="e0176-127">Create a contract for progress billings</span></span>

<span data-ttu-id="e0176-128">Χρησιμοποιήστε αυτήν τη διαδικασία για να δημιουργήσετε μια σύμβαση έργου για ένα έργο με προκαθορισμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="e0176-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="e0176-129">Δημιουργείτε ένα τιμολόγιο έργου όταν η εργασία που ολοκληρώνεται στο έργο φθάνει σε ένα καθορισμένο ποσοστό.</span><span class="sxs-lookup"><span data-stu-id="e0176-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="e0176-130">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** \> **Έργα** \> **Συμβάσεις έργου**.</span><span class="sxs-lookup"><span data-stu-id="e0176-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="e0176-131">Στη σελίδα **Συμβάσεις έργου** , επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="e0176-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="e0176-132">Στο παράθυρο διαλόγου **Νέα σύμβαση έργου** , ορίστε τα ακόλουθα πεδία:</span><span class="sxs-lookup"><span data-stu-id="e0176-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="e0176-133">**Όνομα**.</span><span class="sxs-lookup"><span data-stu-id="e0176-133">**Name**</span></span>
    - <span data-ttu-id="e0176-134">**Τύπος χρηματοδότησης**</span><span class="sxs-lookup"><span data-stu-id="e0176-134">**Funding type**</span></span>
    - <span data-ttu-id="e0176-135">**Προέλευση χρηματοδότησης**</span><span class="sxs-lookup"><span data-stu-id="e0176-135">**Funding source**</span></span>
    - <span data-ttu-id="e0176-136">**Νόμισμα πωλήσεων** – Από προεπιλογή, αυτή η νομισματική μονάδα χρησιμοποιείται για τιμολόγια πελατών που σχετίζονται με τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="e0176-137">Ωστόσο, μπορείτε να αλλάξετε τη νομισματική μονάδα πωλήσεων σε ένα συγκεκριμένο τιμολόγιο πελάτη.</span><span class="sxs-lookup"><span data-stu-id="e0176-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="e0176-138">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="e0176-138">Select **OK**.</span></span> <span data-ttu-id="e0176-139">Οι πληροφορίες αντιγράφονται στην κεφαλίδα της σελίδας **Συμβάσεις έργου**.</span><span class="sxs-lookup"><span data-stu-id="e0176-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="e0176-140">Στη σελίδα **Συμβάσεις έργου** , συμπληρώστε τις υπόλοιπες απαιτούμενες πληροφορίες για το έργο.</span><span class="sxs-lookup"><span data-stu-id="e0176-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="e0176-141">Δημιουργία έργου για τις χρεώσεις προόδου</span><span class="sxs-lookup"><span data-stu-id="e0176-141">Create a project for progress billings</span></span>

<span data-ttu-id="e0176-142">Ακολουθήστε τα παρακάτω βήματα για να δημιουργήσετε ένα έργο και τυχόν δευτερεύοντα έργα που σχετίζονται με μια σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="e0176-143">Μεταβείτε στην επλογή **Διαχείριση έργου και λογιστική** \> **Έργα** \> **Όλα τα έργα**.</span><span class="sxs-lookup"><span data-stu-id="e0176-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="e0176-144">Στη σελίδα **Όλα τα έργα** επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="e0176-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="e0176-145">Στο παράθυρο διαλόγου **Νέο έργο** , στο πεδίο **Τύπος έργου** , επιλέξτε **Χρόνος και υλικό**.</span><span class="sxs-lookup"><span data-stu-id="e0176-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="e0176-146">Επιλέξτε μια ομάδα έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-146">Select a project group.</span></span> <span data-ttu-id="e0176-147">Μια ομάδα έργου καθορίζει τις πληροφορίες καταχώρησης για τα έργα που έχουν ανατεθεί στην ομάδα.</span><span class="sxs-lookup"><span data-stu-id="e0176-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="e0176-148">Επιλέξτε **Δημιουργία έργου**.</span><span class="sxs-lookup"><span data-stu-id="e0176-148">Select **Create project**.</span></span>
6. <span data-ttu-id="e0176-149">Μετά τη δημιουργία του έργου, ορίστε το στάδιο έργου **Σε εξέλιξη**.</span><span class="sxs-lookup"><span data-stu-id="e0176-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="e0176-150">Δημιουργία προϋπολογισμού για ένα έργο</span><span class="sxs-lookup"><span data-stu-id="e0176-150">Create a budget for a project</span></span>

<span data-ttu-id="e0176-151">Οι κατηγορίες προϋπολογισμού χρησιμοποιούνται για τον αυτόματο υπολογισμό των ποσών τιμολόγησης για το ποσοστό της εργασίας που ολοκληρώνεται για κάθε κατηγορία.</span><span class="sxs-lookup"><span data-stu-id="e0176-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="e0176-152">Ακολουθήστε τα παρακάτω βήματα για να δημιουργήσετε κατηγορίες προϋπολογισμού για τις εκτιμώμενες δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="e0176-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="e0176-153">Μεταβείτε στην επλογή **Διαχείριση έργου και λογιστική** \> **Έργα** \> **Όλα τα έργα**.</span><span class="sxs-lookup"><span data-stu-id="e0176-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="e0176-154">Στη σελίδα **Όλα τα έργα** , επιλέξτε και ανοίξτε το έργο που θέλετε.</span><span class="sxs-lookup"><span data-stu-id="e0176-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="e0176-155">Στη σελίδα **Έργα** , στο τμήμα παραθύρου ενεργειών, στην καρτέλα **Σχέδιο** , στην ομάδα **Προϋπολογισμός** επιλέξτε **Προϋπολογισμός έργου**.</span><span class="sxs-lookup"><span data-stu-id="e0176-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="e0176-156">Στη σελίδα **Προϋπολογισμός έργου** , καταγράψτε ένα εκτιμώμενο κόστος για κάθε κατηγορία του έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="e0176-157">Δημιουργία κανόνων χρέωσης για χρεώσεις προόδου</span><span class="sxs-lookup"><span data-stu-id="e0176-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="e0176-158">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** \> **Έργα** \> **Συμβάσεις έργου**.</span><span class="sxs-lookup"><span data-stu-id="e0176-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="e0176-159">Στη σελίδα **Συμβάσεις έργου** επιλέξτε και ανοίξτε μια σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="e0176-160">Στη σελίδα σύμβασης έργου, στη συνοπτική καρτέλα **Κανόνες χρέωσης** , επιλέξτε **Προσθήκη**.</span><span class="sxs-lookup"><span data-stu-id="e0176-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="e0176-161">Στη σελίδα **Κανόνας χρέωσης** , στο πεδίο **Τύπος γραμμής** , επιλέξτε **Πρόοδος**.</span><span class="sxs-lookup"><span data-stu-id="e0176-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="e0176-162">Στη συνοπτική καρτέλα **Λεπτομέρειες γραμμής κανόνα χρέωσης** , στο πεδίο **Τιμή σύμβασης** , καταγράψτε τη συνολική αξία της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="e0176-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="e0176-163">Στο πεδίο **Κατηγορία** , επιλέξτε την κατηγορία στην οποία θα καταχωρείται η συναλλαγή τέλους.</span><span class="sxs-lookup"><span data-stu-id="e0176-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="e0176-164">Στο πεδίο **Έργο** , επιλέξτε το έργο που χρησιμοποιεί αυτόν τον κανόνα χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="e0176-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="e0176-165">Προαιρετικό: εκχωρήστε τον κανόνα χρέωσης σε πρόσθετα έργα.</span><span class="sxs-lookup"><span data-stu-id="e0176-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="e0176-166">Στη συνοπτική καρτέλα **Έργο** στην ενότητα **Διαθέσιμα έργα** , επιλέξτε ένα έργο και, στη συνέχεια, κάντε κλικ στο κουμπί δεξιού βέλους για να προσθέσετε το έργο στην ενότητα **Επιλεγμένα έργα**.</span><span class="sxs-lookup"><span data-stu-id="e0176-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="e0176-167">Προαιρετικό: Υπολογίστε το ποσοστιαίο ποσό που παρακρατεί ο πελάτης από τις πληρωμές σε ένα τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e0176-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="e0176-168">Στη συνοπτική καρτέλα **Όροι κράτησης πληρωμής** , επιλέξτε την προέλευση χρηματοδότησης και, στη συνέχεια, στο πεδίο **Ποσοστό κράτησης** , καταγράψτε το ποσοστό κράτησης.</span><span class="sxs-lookup"><span data-stu-id="e0176-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="e0176-169">Επαναλάβετε αυτά τα βήματα για να δημιουργήσετε πρόσθετους κανόνες χρέωσης για τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e0176-169">Repeat these steps to create additional billing rules for the project contract.</span></span>