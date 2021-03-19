---
title: Ρύθμιση παραμέτρων διαχείρισης εξόδων
description: Σε αυτό το άρθρο περιγράφονται τα ζητήματα και οι αποφάσεις που πρέπει να πάρετε κατά τη διαδικασία σχεδιασμού πριν ρυθμίσετε τη διαχείριση εξόδων στο Microsoft Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 74a8435464c8573ca831b7886f00c2695fd29827
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271353"
---
# <a name="configure-expense-management"></a><span data-ttu-id="62948-103">Ρύθμιση παραμέτρων διαχείρισης εξόδων</span><span class="sxs-lookup"><span data-stu-id="62948-103">Configure expense management</span></span>

<span data-ttu-id="62948-104">Σε αυτό το θέμα περιγράφονται τα ζητήματα και οι αποφάσεις που πρέπει να πάρετε κατά τη διαδικασία σχεδιασμού πριν ρυθμίσετε τη διαχείριση εξόδων.</span><span class="sxs-lookup"><span data-stu-id="62948-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="62948-105">Στη διαχείριση εξόδων, μπορείτε να αποθηκεύσετε πληροφορίες σχετικά με μεθόδους πληρωμής, αιτήσεις για ταξίδια, αναφορές εξόδων, πολιτικές και ούτω καθεξής.</span><span class="sxs-lookup"><span data-stu-id="62948-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="62948-106">Επειδή πολλές από τις αποφάσεις που λαμβάνετε όταν προγραμματίζετε τη ρύθμιση παραμέτρων για τη διαχείριση εξόδων βασίζονται στην ιεραρχία και την οικονομική δομή του οργανισμού σας, πρέπει να ανατρέξετε στα έγγραφα σχεδιασμού για αυτές τις περιοχές.</span><span class="sxs-lookup"><span data-stu-id="62948-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="62948-107">Διεταιρικές δαπάνες</span><span class="sxs-lookup"><span data-stu-id="62948-107">Intercompany expenses</span></span>

<span data-ttu-id="62948-108">Όταν ενεργοποιείτε τις διεταιρικές δαπάνες, επιτρέπετε σε νομικές οντότητες και εργαζομένους να επιβαρύνονται με έξοδα εκ μέρους άλλης νομικής οντότητας και να εισπράττουν πληρωμές από τη νομική οντότητα απασχόλησης εντός του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="62948-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="62948-109">Για παράδειγμα, ένας εργαζόμενος στη νομική οντότητα Α ολοκληρώνει ένα έργο για τη νομική οντότητα Β και το έργο επιβαρύνεται με έξοδα ταξιδίου.</span><span class="sxs-lookup"><span data-stu-id="62948-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="62948-110">Εάν τα διεταιρικά έξοδα είναι ενεργοποιημένα, ο εργαζόμενος μπορεί να καταχωρήσει μια αναφορά εξόδων που θα κοινοποιήσει τη δαπάνη στη νομική οντότητα Β και, στη συνέχεια, η δαπάνη θα πρέπει να καταβληθεί από την νομική οντότητα Α. Εάν ο οργανισμός σας δεν διαθέτει πολλές νομικές οντότητες, δεν χρειάζεται να ενεργοποιήσετε τις διεταιρικές δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="62948-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="62948-111">**Απόφαση:** Θέλετε να ενεργοποιήσετε τις διεταιρικές δαπάνες;</span><span class="sxs-lookup"><span data-stu-id="62948-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="62948-112">Χρηματοοικονομική διαχείριση</span><span class="sxs-lookup"><span data-stu-id="62948-112">Financial management</span></span>

<span data-ttu-id="62948-113">Η διαχείριση δαπανών είναι άρρηκτα ενσωματωμένη με τη χρηματοοικονομική διαχείριση του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="62948-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="62948-114">Σε μεγάλο βαθμό, η ρύθμιση των παραμέτρων για τη διαχείριση εξόδων θα βασίζεται στις αποφάσεις που έχετε λάβει σχετικά με τα οικονομικά του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="62948-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="62948-115">Οι παρακάτω ενότητες περιγράφουν τις διάφορες περιοχές που απαιτούν προγραμματισμό και αποφάσεις, βάσει των οικονομικών αποφάσεων και της καθοδήγησης του οργανισμού σας από την ηγετική σας ομάδα.</span><span class="sxs-lookup"><span data-stu-id="62948-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="62948-116">Ημερήσιες αποζημιώσεις</span><span class="sxs-lookup"><span data-stu-id="62948-116">Per diems</span></span>

<span data-ttu-id="62948-117">Πρέπει να καθορίσετε τις ημερήσιες αποζημιώσεις εργαζόμενου που παρέχει ο οργανισμός σας.</span><span class="sxs-lookup"><span data-stu-id="62948-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="62948-118">Επειδή οι ημερήσιες αποζημιώσεις χρησιμοποιούνται συνήθως για την κάλυψη εξόδων όπως τα γεύματα, η στέγαση και άλλα παρεπόμενα έξοδα, μπορείτε να δημιουργήσετε κανόνες για τις ημερήσιες αποζημιώσεις που προσφέρει ο οργανισμός σας.</span><span class="sxs-lookup"><span data-stu-id="62948-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="62948-119">Οι τιμές ημερήσιας αποζημίωσης βασίζονται στην εποχή του χρόνου, στην τοποθεσία ταξιδίου ή και στα δύο.</span><span class="sxs-lookup"><span data-stu-id="62948-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="62948-120">Όταν καθορίζετε έναν κανόνα ημερήσιας αποζημίωσης, μπορείτε να προσδιορίσετε ότι ένα ποσοστό της ημερήσιας αποζημίωσης θα παρακρατηθεί εάν ο εργαζόμενος λάβει δωρεάν γεύματα ή υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="62948-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="62948-121">Μπορείτε, επίσης, να ορίσετε τα επίπεδα ανά ποσοστό ημερήσιας αποζημίωσης για να ορίσετε τον ελάχιστο και τον μέγιστο αριθμό ωρών όπου θα ισχύει η τιμή της ημερήσιας αποζημίωσης για τα ταξίδια του εργαζομένου.</span><span class="sxs-lookup"><span data-stu-id="62948-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="62948-122">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-122">**Decisions:**</span></span>

- <span data-ttu-id="62948-123">Προεπιλεγμένοι κανόνες ημερήσιας αποζημίωσης για την πρώτη και την τελευταία ημέρα:</span><span class="sxs-lookup"><span data-stu-id="62948-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="62948-124">Ποιος είναι ο ελάχιστος αριθμός ωρών που μπορεί να διεκδικήσει ένας εργαζόμενος για μια ημέρα και να εξακολουθεί να λαμβάνει ημερήσια αποζημίωση;</span><span class="sxs-lookup"><span data-stu-id="62948-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="62948-125">Υπάρχει μείωση του ποσού που προσφέρεται για τα γεύματα για την πρώτη ημέρα και την τελευταία ημέρα;</span><span class="sxs-lookup"><span data-stu-id="62948-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="62948-126">Σε περίπτωση μείωσης, ποιο είναι το ποσοστό της μείωσης;</span><span class="sxs-lookup"><span data-stu-id="62948-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="62948-127">Υπάρχει μείωση του ποσού που προσφέρεται από ένα ξενοδοχείο για την πρώτη ημέρα και την τελευταία ημέρα;</span><span class="sxs-lookup"><span data-stu-id="62948-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="62948-128">Σε περίπτωση μείωσης, ποιο είναι το ποσοστό της μείωσης;</span><span class="sxs-lookup"><span data-stu-id="62948-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="62948-129">Υπάρχει μείωση του ποσού που προσφέρεται για άλλα έξοδα που προκύπτουν την πρώτη ημέρα και την τελευταία ημέρα;</span><span class="sxs-lookup"><span data-stu-id="62948-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="62948-130">Σε περίπτωση μείωσης, ποιο είναι το ποσοστό της μείωσης;</span><span class="sxs-lookup"><span data-stu-id="62948-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="62948-131">Προεπιλεγμένοι κανόνες ανά ημερήσια αποζημίωση:</span><span class="sxs-lookup"><span data-stu-id="62948-131">Default per diem rules:</span></span>

    - <span data-ttu-id="62948-132">Υπάρχει ποσοστό μείωσης της ημερήσιας αποζημίωσης για κάθε γεύμα, εάν, για παράδειγμα, το γεύμα είναι δωρεάν;</span><span class="sxs-lookup"><span data-stu-id="62948-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="62948-133">Σε περίπτωση μείωσης, ποιο είναι το ποσοστό της μείωσης για κάθε γεύμα;</span><span class="sxs-lookup"><span data-stu-id="62948-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="62948-134">Η μείωση του γεύματος υπολογίζεται ανά ημέρα, ανά ταξίδι ή με βάση τον αριθμό των γευμάτων ανά ημέρα;</span><span class="sxs-lookup"><span data-stu-id="62948-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="62948-135">Οι ημερήσιες ποσότητες πρέπει να στρογγυλοποιούνται με τον κανονικό τρόπο ή να στρογγυλοποιούνται προς τα πάνω;</span><span class="sxs-lookup"><span data-stu-id="62948-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="62948-136">Οι ημερήσιες αποζημιώσεις υπολογίζονται σε μια διάρκεια 24 ωρών ή σε μια ημερολογιακή ημέρα;</span><span class="sxs-lookup"><span data-stu-id="62948-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="62948-137">Οι κανόνες ημερήσιας αποζημίωσης βασίζονται στην τοποθεσία:</span><span class="sxs-lookup"><span data-stu-id="62948-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="62948-138">Οι ημερήσιες αποζημιώσεις ποικίλλουν ανάλογα με την τοποθεσία;</span><span class="sxs-lookup"><span data-stu-id="62948-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="62948-139">Ποιες τοποθεσίες περιλαμβάνονται;</span><span class="sxs-lookup"><span data-stu-id="62948-139">What locations are included?</span></span>
    - <span data-ttu-id="62948-140">Εάν οι ημερήσιες αποζημιώσεις ποικίλλουν ανάλογα με την τοποθεσία, για κάθε τοποθεσία, ποιο είναι το ποσοστό που παρέχεται για τους ακόλουθους τύπους δαπανών:</span><span class="sxs-lookup"><span data-stu-id="62948-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="62948-141">Γεύματα</span><span class="sxs-lookup"><span data-stu-id="62948-141">Meals</span></span>
        - <span data-ttu-id="62948-142">Ξενοδοχείο</span><span class="sxs-lookup"><span data-stu-id="62948-142">Hotel</span></span>
        - <span data-ttu-id="62948-143">Άλλα έξοδα</span><span class="sxs-lookup"><span data-stu-id="62948-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="62948-144">Ημερολόγια διαχείρισης εξόδων και λογαριασμοί</span><span class="sxs-lookup"><span data-stu-id="62948-144">Expense management journals and accounts</span></span>

<span data-ttu-id="62948-145">Η διαχείριση εξόδων απαιτεί τη χρήση πολλών ημερολογίων και λογαριασμών.</span><span class="sxs-lookup"><span data-stu-id="62948-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="62948-146">Πρέπει να αποφασίσετε, για παράδειγμα, εάν ο ίδιος λογαριασμός χρησιμοποιείται για προκαταβολές μετρητών και διενέξεις πιστωτικών καρτών.</span><span class="sxs-lookup"><span data-stu-id="62948-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="62948-147">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-147">**Decisions:**</span></span>

- <span data-ttu-id="62948-148">Σε ποιο ημερολόγιο καθολικού καταχωρίζονται οι αναφορές εγκεκριμένων δαπανών;</span><span class="sxs-lookup"><span data-stu-id="62948-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="62948-149">Ποιος λογαριασμός χρησιμοποιείται για προκαταβολές μετρητών;</span><span class="sxs-lookup"><span data-stu-id="62948-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="62948-150">Θα πρέπει να καταχωρηθούν αμέσως προκαταβολές μετρητών;</span><span class="sxs-lookup"><span data-stu-id="62948-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="62948-151">Μέθοδοι πληρωμής</span><span class="sxs-lookup"><span data-stu-id="62948-151">Payment methods</span></span>

<span data-ttu-id="62948-152">Όταν επιτρέπετε στους εργαζομένους να επιβαρύνονται με έξοδα εκ μέρους της επιχείρησής σας, πρέπει να ορίσετε τις μεθόδους πληρωμής που επιτρέπεται να χρησιμοποιούν οι υπάλληλοι.</span><span class="sxs-lookup"><span data-stu-id="62948-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="62948-153">Για παράδειγμα, μπορείτε να επιτρέψετε στους εργαζομένους να χρησιμοποιούν μετρητά ή μια εταιρική πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="62948-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="62948-154">Επίσης, θα μπορούσατε να επιτρέψετε στους εργαζομένους να χρησιμοποιούν προσωπικές πιστωτικές κάρτες και, στη συνέχεια, να αποζημιώνετε τους εργαζομένους.</span><span class="sxs-lookup"><span data-stu-id="62948-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="62948-155">Πρέπει να λάβετε τις παρακάτω αποφάσεις για κάθε μέθοδο πληρωμής που θα επιτρέψετε.</span><span class="sxs-lookup"><span data-stu-id="62948-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="62948-156">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-156">**Decisions:**</span></span>

- <span data-ttu-id="62948-157">Ποιες μέθοδοι πληρωμής επιτρέπονται;</span><span class="sxs-lookup"><span data-stu-id="62948-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="62948-158">Σε ποιον ανήκουν οι δαπάνες μεθόδου πληρωμής;</span><span class="sxs-lookup"><span data-stu-id="62948-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="62948-159">Υπάρχει τύπος λογαριασμού αντιστάθμισης;</span><span class="sxs-lookup"><span data-stu-id="62948-159">Is there an offset account type?</span></span> <span data-ttu-id="62948-160">Εάν υπάρχει τύπος λογαριασμού αντιστάθμισης, τι είναι;</span><span class="sxs-lookup"><span data-stu-id="62948-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="62948-161">Εάν υπάρχει τύπος λογαριασμού αντιστάθμισης, ποιος είναι ο λογαριασμός;</span><span class="sxs-lookup"><span data-stu-id="62948-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="62948-162">Εάν ο τρόπος πληρωμής είναι μια πιστωτική κάρτα, θα πρέπει να χρησιμοποιείται η μέθοδος πληρωμής μόνο με εισαγόμενες συναλλαγές;</span><span class="sxs-lookup"><span data-stu-id="62948-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="62948-163">Κατηγορίες εξόδων και κοινόχρηστες κατηγορίες</span><span class="sxs-lookup"><span data-stu-id="62948-163">Expense categories and shared categories</span></span>

<span data-ttu-id="62948-164">Όταν οι υπάλληλοι δημιουργούν μια αναφορά εξόδων, κάθε δαπάνη την οποία καταγράφουν πρέπει να συσχετίζεται με μια κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="62948-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="62948-165">Οι κατηγορίες δαπανών προέρχονται από κοινόχρηστες κατηγορίες, οι οποίες είναι δυνατό να χρησιμοποιηθούν από κοινού σε όλες τις νομικές οντότητες του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="62948-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="62948-166">Αυτές οι κατηγορίες είναι επίσης δυνατό να χρησιμοποιηθούν από κοινού στη διαχείριση έργου και στη λογιστική, ανάλογα με τον τρόπο με τον οποίο καθορίζεται ο οργανισμός σας.</span><span class="sxs-lookup"><span data-stu-id="62948-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="62948-167">Με βάση τον ορισμό του οργανισμού σας και την καθοδήγησή σας από την ομάδα υλοποίησης, πρέπει να καθορίσετε εάν οι κατηγορίες που χρησιμοποιούνται στη διαχείριση δαπανών θα χρησιμοποιηθούν μόνο στη διαχείριση εξόδων ή θα πρέπει να είναι κοινόχρηστες μεταξύ της διαχείρισης έργων και λογιστικής και της διαχείρισης δαπανών.</span><span class="sxs-lookup"><span data-stu-id="62948-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="62948-168">Λάβετε υπόψη ότι αυτές οι κατηγορίες είναι δυνατό να είναι κοινόχρηστες μεταξύ του έργου και των εξόδων ή του έργου και της παραγωγής αλλά όχι μεταξύ των εξόδων και της παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="62948-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="62948-169">Πρέπει να λάβετε τις παρακάτω αποφάσεις για κάθε κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="62948-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="62948-170">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-170">**Decisions:**</span></span>

- <span data-ttu-id="62948-171">Ποια είναι η κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-171">What is the expense category?</span></span> <span data-ttu-id="62948-172">Τα παραδείγματα περιλαμβάνουν κατηγορίες για πτήσεις, ξενοδοχεία ή χιλιόμετρα.</span><span class="sxs-lookup"><span data-stu-id="62948-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="62948-173">Μπορεί η κατηγορία εξόδων να χρησιμοποιηθεί και στη διαχείριση έργου και στη λογιστική;</span><span class="sxs-lookup"><span data-stu-id="62948-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="62948-174">Ποιος είναι ο τύπος εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-174">What is the expense type?</span></span>
- <span data-ttu-id="62948-175">Ποια είναι η προεπιλεγμένη μέθοδος πληρωμής για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="62948-176">Οι δαπάνες στην κατηγορία εξόδων πρέπει να είναι αναλυτικές;</span><span class="sxs-lookup"><span data-stu-id="62948-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="62948-177">Ποιος είναι ο κύριος προεπιλεγμένος λογαριασμός για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="62948-178">Ποια είναι η προεπιλεγμένη ομάδα φόρου πωλήσεων είδους για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="62948-179">Επιτρέπονται επιπλέον μέθοδοι πληρωμής για την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="62948-180">Εάν επιτρέπονται επιπλέον μέθοδοι πληρωμής, ποιες είναι;</span><span class="sxs-lookup"><span data-stu-id="62948-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="62948-181">Υπάρχουν υποκατηγορίες σε αυτήν την κατηγορία εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="62948-182">Αν υπάρχουν υποκατηγορίες, πρέπει να έχετε αποφασίσει για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="62948-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="62948-183">Αποκλείεται καμία από τις υποκατηγορίες από την είσπραξη φόρων;</span><span class="sxs-lookup"><span data-stu-id="62948-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="62948-184">Ποια είναι η ομάδα φόρου πωλήσεων ειδών στις υποκατηγορίες;</span><span class="sxs-lookup"><span data-stu-id="62948-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="62948-185">Εάν η κατηγορία εξόδων χρησιμοποιείται επίσης στη διαχείριση έργου και στη λογιστική, απαντήστε στις υπόλοιπες ερωτήσεις.</span><span class="sxs-lookup"><span data-stu-id="62948-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="62948-186">Διαφορετικά, μεταβείτε στην επόμενη ενότητα.</span><span class="sxs-lookup"><span data-stu-id="62948-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="62948-187">Ποιοι λογαριασμοί κόστους θα χρησιμοποιηθούν για τις ακόλουθες δαπάνες;</span><span class="sxs-lookup"><span data-stu-id="62948-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="62948-188">Κόστος</span><span class="sxs-lookup"><span data-stu-id="62948-188">Cost</span></span>
    - <span data-ttu-id="62948-189">Εκχώρηση μισθοδοσίας</span><span class="sxs-lookup"><span data-stu-id="62948-189">Payroll allocation</span></span>
    - <span data-ttu-id="62948-190">WIP-τιμή κόστους</span><span class="sxs-lookup"><span data-stu-id="62948-190">WIP-cost value</span></span>
    - <span data-ttu-id="62948-191">Κόστος-στοιχείο</span><span class="sxs-lookup"><span data-stu-id="62948-191">Cost-item</span></span>
    - <span data-ttu-id="62948-192">WIP-τιμή κόστους-στοιχείο</span><span class="sxs-lookup"><span data-stu-id="62948-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="62948-193">Συσσωρευμένη απώλεια</span><span class="sxs-lookup"><span data-stu-id="62948-193">Accrued loss</span></span>
    - <span data-ttu-id="62948-194">WIP-συσσωρευμένη απώλεια</span><span class="sxs-lookup"><span data-stu-id="62948-194">WIP-accrued loss</span></span>

- <span data-ttu-id="62948-195">Ποιοι λογαριασμοί εσόδων θα χρησιμοποιηθούν για τα ακόλουθα;</span><span class="sxs-lookup"><span data-stu-id="62948-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="62948-196">Τιμολογημένα έσοδα</span><span class="sxs-lookup"><span data-stu-id="62948-196">Invoiced revenue</span></span>
    - <span data-ttu-id="62948-197">Συσσωρευμένα έσοδα - τιμή πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="62948-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="62948-198">WIP-τιμή πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="62948-198">WIP-sales value</span></span>
    - <span data-ttu-id="62948-199">Συσσωρευμένα έσοδα-παραγωγή</span><span class="sxs-lookup"><span data-stu-id="62948-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="62948-200">WIP-παραγωγή</span><span class="sxs-lookup"><span data-stu-id="62948-200">WIP-production</span></span>
    - <span data-ttu-id="62948-201">Συσσωρευμένα έσοδα-κέρδος</span><span class="sxs-lookup"><span data-stu-id="62948-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="62948-202">WIP-κέρδος</span><span class="sxs-lookup"><span data-stu-id="62948-202">WIP-profit</span></span>
    - <span data-ttu-id="62948-203">Συσσωρευμένα έσοδα-συνδρομή</span><span class="sxs-lookup"><span data-stu-id="62948-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="62948-204">WIP-συνδρομή</span><span class="sxs-lookup"><span data-stu-id="62948-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="62948-205">Φόροι</span><span class="sxs-lookup"><span data-stu-id="62948-205">Taxes</span></span>

<span data-ttu-id="62948-206">Για τους φόρους που σχετίζονται με τα έξοδα, πρέπει να καθορίσετε τι περιλαμβάνεται ή τι είναι ενεργοποιημένο στις αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="62948-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="62948-207">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-207">**Decisions:**</span></span>

- <span data-ttu-id="62948-208">Ο φόρος πωλήσεων περιλαμβάνεται στα ποσά εξόδων;</span><span class="sxs-lookup"><span data-stu-id="62948-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="62948-209">Θα πρέπει να ενεργοποιηθεί η είσπραξη φόρων στις δαπάνες;</span><span class="sxs-lookup"><span data-stu-id="62948-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="62948-210">Όταν σχεδιάζετε τη γενική λογιστική, εάν αποφασίσατε να εφαρμόσετε φόρο πωλήσεων στις ΗΠΑ και να χρησιμοποιήσετε φορολογικούς κανόνες, δεν μπορείτε να ενεργοποιήσετε την είσπραξη φόρων στις δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="62948-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="62948-211">(Για την εφαρμογή του φόρου πωλήσεων στις ΗΠΑ και τη χρήση φορολογικών κανόνων, ορίστε την επιλογή **Εφαρμογή κανόνων φορολόγησης φόρων πωλήσεων** σε **Ναι**.)</span><span class="sxs-lookup"><span data-stu-id="62948-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="62948-212">Πολιτικές</span><span class="sxs-lookup"><span data-stu-id="62948-212">Policies</span></span>

<span data-ttu-id="62948-213">Δημιουργώντας πολιτικές αναφοράς δαπανών, μπορείτε να βοηθήσετε τον οργανισμό σας να εξοικονομήσει χρόνο και χρήμα, όταν οι υπάλληλοι επιβαρύνονται με έξοδα για λογαριασμό του.</span><span class="sxs-lookup"><span data-stu-id="62948-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="62948-214">Οι πολιτικές εγγυώνται ότι οι υπάλληλοι παραμένουν εντός προϋπολογισμού, παρέχουν όλες τις απαιτούμενες πληροφορίες και δαπανούν χρήματα μόνο εφόσον απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="62948-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="62948-215">Πρέπει να λάβετε τις παρακάτω αποφάσεις για κάθε πολιτική αναφοράς εξόδων και για κάθε πολιτική έγκρισης εξόδων αναφοράς που δημιουργείτε.</span><span class="sxs-lookup"><span data-stu-id="62948-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="62948-216">**Αποφάσεις:**</span><span class="sxs-lookup"><span data-stu-id="62948-216">**Decisions:**</span></span>

- <span data-ttu-id="62948-217">Ποιο είναι το όνομα της πολιτικής;</span><span class="sxs-lookup"><span data-stu-id="62948-217">What is the name of the policy?</span></span>
- <span data-ttu-id="62948-218">Σε τι χρησιμεύει η πολιτική δαπανών;</span><span class="sxs-lookup"><span data-stu-id="62948-218">What is the expense policy for?</span></span>
- <span data-ttu-id="62948-219">Εάν αποφασίσατε προηγουμένως να ενεργοποιήσετε τις διεταιρικές δαπάνες, σε ποιες εταιρείες του οργανισμού σας θα ισχύει αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="62948-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="62948-220">Πότε η πολιτική είναι αποτελεσματική;</span><span class="sxs-lookup"><span data-stu-id="62948-220">When does the policy become effective?</span></span>
- <span data-ttu-id="62948-221">Πότε λήγει η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="62948-221">When does the policy expire?</span></span>
- <span data-ttu-id="62948-222">Ποιος είναι ο κανόνας πολιτικής;</span><span class="sxs-lookup"><span data-stu-id="62948-222">What is the policy rule?</span></span>
- <span data-ttu-id="62948-223">Ποιο είναι το αποτέλεσμα του κανόνα πολιτικής;</span><span class="sxs-lookup"><span data-stu-id="62948-223">What is the outcome of the policy rule?</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]