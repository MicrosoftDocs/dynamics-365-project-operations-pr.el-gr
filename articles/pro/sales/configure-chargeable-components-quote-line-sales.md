---
title: Ρύθμιση παραμέτρων των χρεώσιμων στοιχείων μιας γραμμής προσφοράς
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη ρύθμιση των χρεώσιμων και μη χρεώσιμων στοιχείων σε μια γραμμή προσφοράς βάσει έργου.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858293"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="f6801-103">Ρύθμιση παραμέτρων των χρεώσιμων στοιχείων μιας γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="f6801-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="f6801-104">_**Ισχύει για:** ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση, Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="f6801-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f6801-105">Μια γραμμή προσφοράς βάσει έργου έχει την έννοια των *περιλαμβανόμενων* στοιχείων και των *χρεώσιμων* στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="f6801-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="f6801-106">Τα στοιχεία που περιλαμβάνονται υπόκεινται στις εξής επιλογές:</span><span class="sxs-lookup"><span data-stu-id="f6801-106">Included components are subject to:</span></span>

  - <span data-ttu-id="f6801-107">Μέθοδος χρέωσης και διαιρέσεις πελάτη</span><span class="sxs-lookup"><span data-stu-id="f6801-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="f6801-108">Όριο που δεν πρέπει να υπερβαίνεται</span><span class="sxs-lookup"><span data-stu-id="f6801-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="f6801-109">Ρυθμίσεις συχνότητας τιμολογίου που καθορίζονται στη γραμμή προσφοράς βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="f6801-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="f6801-110">Ένα υποσύνολο των περιλαμβανόμενων στοιχείων μπορεί να επισημανθεί ως χρεώσιμο με χρήση του πεδίου **Τύπος χρέωσης**.</span><span class="sxs-lookup"><span data-stu-id="f6801-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="f6801-111">Το πεδίο **Τύπος χρέωσης** είναι ένα σύνολο επιλογών που επιτρέπει τις παρακάτω τιμές στο περιβάλλον μιας γραμμής προσφοράς:</span><span class="sxs-lookup"><span data-stu-id="f6801-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="f6801-112">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-112">Chargeable</span></span>
  - <span data-ttu-id="f6801-113">Μη χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-113">Non-chargeable</span></span>

<span data-ttu-id="f6801-114">Τα χρεώσιμα στοιχεία μπορούν να οριστούν σε εργασίες, ρόλους και κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="f6801-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="f6801-115">Η χρεωσιμότητα καθορίζεται στις εργασίες για μια γραμμή προσφοράς και ισχύει για όλες τις κλάσεις συναλλαγής που περιλαμβάνονται σε αυτήν τη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="f6801-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="f6801-116">Εάν το πεδίο **Συμπερίληψη εργασιών** έχει οριστεί σε **Ολόκληρο το έργο** ή παραμένει κενό, η καρτέλα **Χρεώσιμες εργασίες** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="f6801-117">Η χρεωσιμότητα καθορίζεται σε ρόλους για μια γραμμή προσφοράς και ισχύει μόνο για την κλάση συναλλαγής **Χρόνος**.</span><span class="sxs-lookup"><span data-stu-id="f6801-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="f6801-118">Εάν το πεδίο **Συμπερίληψη χρόνου** έχει οριστεί σε **Όχι** σε μια γραμμή προσφοράς έργου, η καρτέλα **Χρεώσιμοι ρόλοι** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="f6801-119">Η χρεωσιμότητα καθορίζεται σε κατηγορίες συναλλαγής για μια γραμμή προσφοράς και ισχύει μόνο για την κλάση συναλλαγής **Έξοδο**.</span><span class="sxs-lookup"><span data-stu-id="f6801-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="f6801-120">Εάν το πεδίο **Συμπερίληψη εξόδων** έχει οριστεί σε **Όχι** σε μια γραμμή προσφοράς έργου, η καρτέλα **Χρεώσιμες κατηγορίες** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="f6801-121">Ενημέρωση μιας εργασίας έργου ώστε να χρεώσιμη ή μη χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="f6801-122">Μια εργασία έργου μπορεί να είναι χρεώσιμη ή μη χρεώσιμη στο περιβάλλον μιας συγκεκριμένης γραμμής προσφοράς βάσει έργου, γεγονός που καθιστά δυνατή την ακόλουθη ρύθμιση.</span><span class="sxs-lookup"><span data-stu-id="f6801-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="f6801-123">Εάν μια γραμμή προσφοράς βάσει έργου περιλαμβάνει **Χρόνο** και την εργασία **Τ1**, η εργασία συσχετίζεται με τη γραμμή προσφοράς ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="f6801-124">Εάν υπάρχει μια δεύτερη γραμμή προσφοράς που περιλαμβάνει **Έξοδα**, μπορείτε να συσχετίσετε την εργασία **Τ1** στη γραμμή προσφοράς ως μη χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="f6801-125">Το αποτέλεσμα είναι ότι όλος ο χρόνος που καταγράφηκε στην εργασία είναι χρεώσιμος και όλα τα έξοδα που καταγράφονται στην εργασία δεν είναι χρεώσιμα.</span><span class="sxs-lookup"><span data-stu-id="f6801-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="f6801-126">Ο τύπος χρέωσης μιας εργασίας μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμες εργασίες** της γραμμής προσφοράς βάσει έργου ενημερώνοντας το πεδίο **Τύπος χρέωσης** στο υποπλέγμα **Εργασίες γραμμής προσφοράς**.</span><span class="sxs-lookup"><span data-stu-id="f6801-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="f6801-127">Εναλλακτικά, μπορείτε να ενημερώσετε τον τύπο χρέωσης για μια εργασία έργου στο πεδίο **Τύπος χρέωσης** στο υποπλέγμα της ρύθμισης χρέωσης εργασίας ενός έργου που εμφανίζει τις γραμμές προσφοράς που σχετίζονται με μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="f6801-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="f6801-128">Ενημέρωση ενός ρόλου ώστε να χρεώσιμος ή μη χρεώσιμος</span><span class="sxs-lookup"><span data-stu-id="f6801-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="f6801-129">Ένας ρόλος μπορεί να είναι χρεώσιμος ή μη χρέωσιμος στο περιβάλλον μιας συγκεκριμένης γραμμής προσφοράς βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="f6801-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="f6801-130">Ο τύπος χρέωσης ενός ρόλου μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμοι ρόλοι** της γραμμής προσφοράς βάσει έργου ενημερώνοντας το πεδίο **Τύπος χρέωσης** στο υποπλέγμα **Χρεώσιμοι ρόλοι**.</span><span class="sxs-lookup"><span data-stu-id="f6801-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="f6801-131">Ενημέρωση μιας κατηγορίας συναλλαγής ώστε να χρεώσιμη ή μη χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="f6801-132">Μια κατηγορία συναλλαγής μπορεί να είναι χρεώσιμη ή μη χρεώσιμη σε μια συγκεκριμένη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="f6801-133">Ο τύπος χρέωσης μιας συναλλαγής μπορεί να ρυθμιστεί στην καρτέλα **Χρεώσιμες κατηγορίες** της γραμμής προσφοράς βάσει έργου ενημερώνοντας το πεδίο **Τύπος χρέωσης** στο υποπλέγμα **Χρεώσιμες κατηγορίες**.</span><span class="sxs-lookup"><span data-stu-id="f6801-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="f6801-134">Επίλυση χρεωσιμότητας</span><span class="sxs-lookup"><span data-stu-id="f6801-134">Resolve chargeability</span></span>
<span data-ttu-id="f6801-135">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για χρόνο θα θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="f6801-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="f6801-136">**Ο χρόνος** περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="f6801-137">**Ο ρόλος** ρυθμίζεται ως χρεώσιμος στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="f6801-138">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένες εργασίες** στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="f6801-139">Εάν αυτά τα τρία πράγματα είναι αληθή, η **εργασία** ρυθμίζεται επίσης ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="f6801-140">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για έξοδο θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="f6801-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="f6801-141">**Το έξοδο** περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="f6801-142">**Η κατηγορία συναλλαγής** ρυθμίζεται ως χρεώσιμη στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="f6801-143">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένες εργασίες** στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="f6801-144">Εάν αυτά τα τρία πράγματα είναι αληθή, η **εργασία** ρυθμίζεται επίσης ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="f6801-145">Μια εκτίμηση ή πραγματική τιμή που δημιουργήθηκε για υλικό θα θεωρείται χρεώσιμη μόνο εάν:</span><span class="sxs-lookup"><span data-stu-id="f6801-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="f6801-146">**Το υλικό** περιλαμβάνεται στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="f6801-147">**Οι εργασίες που περιλαμβάνονται** ορίζονται σε **Επιλεγμένες εργασίες** στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f6801-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="f6801-148">Εάν αυτά τα δύο πράγματα είναι αληθή, η **εργασία** θα πρέπει να ρυθμίζεται επίσης ως χρεώσιμη.</span><span class="sxs-lookup"><span data-stu-id="f6801-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-149">
                    <strong>Συμπεριλαμβάνει χρόνο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="f6801-150">
                    <strong>Συμπεριλαμβάνει έξοδο</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="f6801-151">
                    <strong>Περιλαμβάνει υλικά</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="f6801-152">
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-153">
                    <strong>Ρόλος</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-154">
                    <strong>Κατηγορία</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-155">
                    <strong>Κλείσιμο εργασίας</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="f6801-156">
                    <strong>Επίδραση δυνατότητας χρέωσης</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-157">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-158">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-159">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-160">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-161">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-162">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-163">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-164">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-165">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-166">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-167">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-168">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-169">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-170">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="f6801-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-171">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-172">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-173">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-174">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-175">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-176">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-177">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-178">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-179">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-180">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="f6801-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-181">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-182">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-183">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-184">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-185">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-186">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-187">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-188">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-189">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-190">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="f6801-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-191">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-192">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-193">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-194">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-195">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-196">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-197">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-198">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-199">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-200">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="f6801-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-201">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-202">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-203">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-204">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-205">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-206">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-207">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-208">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-209">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-210">Επιλεγμένες εργασίες μόνο</span><span class="sxs-lookup"><span data-stu-id="f6801-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-211">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-212">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-213">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-214">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-215">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong> Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-216">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-218">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-220">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-221">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-222">
                    <strong>Χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-223">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-224">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-225">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-226">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-228">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-229">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-230">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-231">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-232">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-233">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-234">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-235">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου: <strong> Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-236">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-237">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="f6801-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-239">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-240">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-241">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-242">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-243">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-244">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-245">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-246">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-247">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="f6801-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="f6801-249">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-250">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-251">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-252">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-253">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-254">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-255">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-256">Τύπος τιμολόγησης σε πραγματική τιμή υλικού: Χρεώσιμη</span><span class="sxs-lookup"><span data-stu-id="f6801-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-257">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-258">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="f6801-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-260">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-261">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-262">Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-263">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-264">Τιμολόγηση σε ένα πραγματικό χρόνο: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-265">Τύπος χρέωσης με πραγματική δαπάνη: Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="f6801-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="f6801-266">Τύπος τιμολόγησης σε πραγματική τιμή υλικού:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="f6801-267">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="f6801-268">Ναι</span><span class="sxs-lookup"><span data-stu-id="f6801-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="f6801-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="f6801-270">Ολόκληρο το έργο</span><span class="sxs-lookup"><span data-stu-id="f6801-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="f6801-271">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="f6801-272">
                    <strong>Μη χρεώσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="f6801-273">Δεν είναι δυνατός ο ορισμός</span><span class="sxs-lookup"><span data-stu-id="f6801-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="f6801-274">Τιμολόγηση σε πραγματική τιμή χρόνου: <strong>Μη χρεώσιμη</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-275">Τύπος τιμολόγησης σε πραγματική τιμή εξόδου:<strong> Μη χρεώσιμη </strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="f6801-276">Τύπος τιμολόγησης σε πραγματική τιμή υλικού:<strong> Μη διαθέσιμο</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f6801-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
