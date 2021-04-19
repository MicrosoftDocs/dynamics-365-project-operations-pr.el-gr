---
title: Ρύθμιση παραμέτρων χρεώσιμων στοιχείων μιας γραμμής σύμβασης βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο προσθήκης χρεώσιμων στοιχείων σε γραμμές σύμβασης στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858473"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="ee136-103">Ρύθμιση παραμέτρων χρεώσιμων στοιχείων μιας γραμμής σύμβασης βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="ee136-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="ee136-104">_**Ισχύει για:** ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση, Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="ee136-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ee136-105">Μια γραμμή σύμβασης βάσει έργου έχει την έννοια των *περιλαμβανόμενων* στοιχείων και των *χρεώσιμων* στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="ee136-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="ee136-106">Τα στοιχεία που περιλαμβάνονται είναι στοιχεία τα οποία υπόκεινται σε:</span><span class="sxs-lookup"><span data-stu-id="ee136-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="ee136-107">Μέθοδος χρέωσης και διαιρέσεις πελάτη</span><span class="sxs-lookup"><span data-stu-id="ee136-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="ee136-108">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="ee136-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="ee136-109">Ρυθμίσεις συχνότητας τιμολογίου που καθορίζονται στη γραμμή σύμβασης βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="ee136-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="ee136-110">Ένα υποσύνολο των περιλαμβανόμενων στοιχείων μπορεί να επισημανθεί ως χρεώσιμο με χρήση του πεδίου **Τύπος χρέωσης**.</span><span class="sxs-lookup"><span data-stu-id="ee136-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="ee136-111">Το πεδίο **Τύπος χρέωσης** είναι ένα σύνολο επιλογών που επιτρέπει τις παρακάτω τιμές στο περιβάλλον μιας γραμμής σύμβασης:</span><span class="sxs-lookup"><span data-stu-id="ee136-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="ee136-112">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-112">Chargeable</span></span>
  - <span data-ttu-id="ee136-113">Μη χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-113">Non-chargeable</span></span>

<span data-ttu-id="ee136-114">Τα χρεώσιμα στοιχεία μπορούν να οριστούν σε εργασίες, ρόλους και κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="ee136-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="ee136-115">Η χρεωσιμότητα καθορίζεται στις εργασίες για μια γραμμή σύμβασης έργου και ισχύει για όλες τις κλάσεις συναλλαγής που περιλαμβάνονται στη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="ee136-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="ee136-116">Εάν το πεδίο **Συμπερίληψη εργασιών** σε μια γραμμή σύμβασης είναι κενό ή έχει οριστεί σε **Ολόκληρο το έργο** ή παραμένει κενό, η καρτέλα **Χρεώσιμες εργασίες** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="ee136-117">Η χρεωσιμότητα καθορίζεται σε ρόλους για μια γραμμή σύμβασης έργου και ισχύει μόνο για την κλάση συναλλαγής **Χρόνος**.</span><span class="sxs-lookup"><span data-stu-id="ee136-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="ee136-118">Εάν το πεδίο **Συμπερίληψη χρόνου** σε μια γραμμή σύμβασης έχει οριστεί σε **Όχι** σε μια γραμμή προσφοράς έργου, η καρτέλα **Χρεώσιμοι ρόλοι** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="ee136-119">Η χρεωσιμότητα καθορίζεται σε κατηγορίες συναλλαγής για μια γραμμή σύμβασης έργου και ισχύει μόνο για την κλάση συναλλαγής **Έξοδο**.</span><span class="sxs-lookup"><span data-stu-id="ee136-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="ee136-120">Εάν το πεδίο **Συμπερίληψη εξόδων** σε μια γραμμή σύμβασης έχει οριστεί σε **Όχι** σε μια γραμμή προσφοράς έργου, η καρτέλα **Χρεώσιμες κατηγορίες** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="ee136-121">Ενημέρωση μιας εργασίας έργου ώστε να χρεώσιμη ή μη χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="ee136-122">Μια εργασία έργου μπορεί να είναι χρεώσιμη ή μη χρεώσιμη σε μια συγκεκριμένη γραμμή σύμβασης, γεγονός που καθιστά δυνατή την ακόλουθη ρύθμιση:</span><span class="sxs-lookup"><span data-stu-id="ee136-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="ee136-123">Εάν μια γραμμή σύμβασης που βασίζεται σε ένα έργο περιλαμβάνει **Χρόνο** και μια συγκεκριμένη εργασία, το **Τ1** σχετίζεται με αυτό ως χρεώσιμο.</span><span class="sxs-lookup"><span data-stu-id="ee136-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="ee136-124">Εάν υπάρχει μια δεύτερη γραμμή σύμβασης που περιλαμβάνει **Έξοδα**, μπορείτε να συσχετίσετε την εργασία Τ1 στη γραμμή σύμβασης ως μη χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="ee136-125">Το αποτέλεσμα είναι ότι όλος ο χρόνος που καταγράφηκε στην εργασία είναι χρεώσιμος και όλα τα έξοδα που καταγράφονται στην εργασία δεν είναι χρεώσιμα.</span><span class="sxs-lookup"><span data-stu-id="ee136-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="ee136-126">Ο τύπος χρέωσης μιας εργασίας μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμες εργασίες** της γραμμής σύμβασης, ενημερώνοντας το πεδίο **Τύπος χρέωσης** στο υποπλέγμα εργασιών της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="ee136-127">Εναλλακτικά, μπορείτε να ενημερώσετε το πεδίο **Τύπος χρέωσης** στο υποπλέγμα της ρύθμισης χρέωσης εργασιών ενός έργου που εμφανίζει τις γραμμές σύμβασης που σχετίζονται με μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="ee136-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="ee136-128">Ενημέρωση ενός ρόλου ώστε να χρεώσιμος ή μη χρεώσιμος</span><span class="sxs-lookup"><span data-stu-id="ee136-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="ee136-129">Ένας ρόλος μπορεί να είναι χρεώσιμος ή μη χρεώσιμος σε μια συγκεκριμένη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="ee136-130">Ο τύπος χρέωσης ενός ρόλου μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμοι ρόλοι** μιας γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="ee136-131">Για να το κάνετε αυτό, ενημερώστε το πεδίο **Τύπος χρέωσης** στο υποπλέγμα **Χρεώσιμοι ρόλοι**.</span><span class="sxs-lookup"><span data-stu-id="ee136-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="ee136-132">Ενημέρωση μιας κατηγορίας συναλλαγής ώστε να χρεώσιμη ή μη χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="ee136-133">Μια κατηγορία συναλλαγής μπορεί να είναι χρεώσιμη ή μη χρεώσιμη σε μια συγκεκριμένη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="ee136-134">Ο τύπος χρέωσης μιας συναλλαγής μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμες κατηγορίες** μιας γραμμής σύμβασης βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="ee136-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="ee136-135">Για να το κάνετε αυτό, ενημερώστε το πεδίο **Τύπος χρέωσης** στο υποπλέγμα **Χρεώσιμες κατηγορίες**.</span><span class="sxs-lookup"><span data-stu-id="ee136-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="ee136-136">Επίλυση χρεωσιμότητας</span><span class="sxs-lookup"><span data-stu-id="ee136-136">Resolve chargeability</span></span>

<span data-ttu-id="ee136-137">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για χρόνο θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="ee136-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="ee136-138">**Ο χρόνος** περιλαμβάνεται στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="ee136-139">**Ο ρόλος** ρυθμίζεται ως χρεώσιμος στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="ee136-140">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένες εργασίες** στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="ee136-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="ee136-141">Εάν αυτά τα τρία πράγματα είναι αληθή, η εργασία ρυθμίζεται ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="ee136-142">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για έξοδο θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="ee136-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="ee136-143">**Το έξοδο** περιλαμβάνεται στη γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="ee136-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="ee136-144">**Η κατηγορία συναλλαγής** ρυθμίζεται ως χρεώσιμη στη γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="ee136-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="ee136-145">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένη εργασία** στη γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="ee136-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="ee136-146">Εάν αυτά τα τρία πράγματα είναι αληθή, η **εργασία** ρυθμίζεται ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="ee136-147">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για υλικό θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="ee136-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="ee136-148">**Τα υλικά** περιλαμβάνονται στη γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="ee136-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="ee136-149">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένες εργασίες** στη γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="ee136-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="ee136-150">Εάν αυτά τα δύο πράγματα είναι αληθή, η **εργασία** ρυθμίζεται ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="ee136-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-151">
                    <strong>Συμπεριλαμβάνει χρόνο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="ee136-152">
                    <strong>Συμπεριλαμβάνει έξοδο</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="ee136-153">
                    <strong>Περιλαμβάνει υλικά</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="ee136-154">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-155">
                    <strong>Ρόλος</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-156">
                    <strong>Κατηγορία</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-157">
                    <strong>Κλείσιμο εργασίας</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="ee136-158">
                    <strong>Επίδραση δυνατότητας χρέωσης</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-159">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-160">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-161">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-162">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-163">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-164">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-165">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-166">Τιμολόγηση σε μια πραγματική τιμή χρόνου: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-167">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-168">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-169">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-170">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-171">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-172">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="ee136-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-173">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-174">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-175">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-176">Τιμολόγηση σε μια πραγματική τιμή χρόνου: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-177">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-178">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-179">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-180">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-181">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-182">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="ee136-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-183">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-184">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-185">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-186">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-187">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="ee136-188">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-189">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-190">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-191">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-192">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="ee136-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-193">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-194">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-195">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-196">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-197">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-198">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-199">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-200">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-201">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-202">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="ee136-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-203">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-204">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-205">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-206">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-207">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-208">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-209">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-210">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-211">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-212">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="ee136-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-213">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-214">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-215">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-216">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-217">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong> Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-218">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-220">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-221">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-222">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-223">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-224">
                    <strong>Χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-225">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-226">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-227">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="ee136-228">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-230">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-231">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-232">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-233">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-234">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-235">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-236">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-237">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong> Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-238">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="ee136-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-241">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-242">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-243">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-244">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-245">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-246">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="ee136-247">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-248">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="ee136-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="ee136-251">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-252">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-253">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-254">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-255">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-256">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-257">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-258">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="ee136-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-259">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-260">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="ee136-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-262">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-263">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-264">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-265">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-266">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="ee136-267">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="ee136-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="ee136-268">Τύπος τιμολόγησης σε πραγματική τιμή υλικού:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="ee136-269">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="ee136-270">Ναι</span><span class="sxs-lookup"><span data-stu-id="ee136-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="ee136-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="ee136-272">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="ee136-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="ee136-273">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="ee136-274">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="ee136-275">Δεν μπορεί να οριστεί</span><span class="sxs-lookup"><span data-stu-id="ee136-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="ee136-276">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-277">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη χρεώσιμη </strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="ee136-278">Τύπος τιμολόγησης σε πραγματική τιμή υλικού:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ee136-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
