---
title: Πραγματικές τιμές
description: Αυτό θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εργασίας με τις πραγματικές τιμές στο Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9e046602a3005930c41ab8c50472d5b1a72303c6
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368611"
---
# <a name="actuals"></a><span data-ttu-id="d66af-103">Πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="d66af-103">Actuals</span></span> 

<span data-ttu-id="d66af-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="d66af-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d66af-105">Οι πραγματικές τιμές αντιπροσωπεύουν την ελεγμένη και εγκεκριμένη οικονομική πρόοδο και την πρόοδο χρονοδιαγράμματος ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="d66af-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="d66af-106">Αυτά δημιουργούνται ως αποτέλεσμα της έγκρισης χρόνου, δαπανών, καταχωρήσεων χρήσης υλικού και καταχωρήσεων ημερολογίου και τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="d66af-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="d66af-107">Γραμμές ημερολογίου και υποβολή χρόνου</span><span class="sxs-lookup"><span data-stu-id="d66af-107">Journal lines and time submission</span></span>

<span data-ttu-id="d66af-108">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση χρόνου, ανατρέξτε στο θέμα [Επισκόπηση καταχώρησης χρόνου](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d66af-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="d66af-109">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="d66af-109">Time and materials</span></span>

<span data-ttu-id="d66af-110">Όταν μια καταχώρηση χρόνου που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="d66af-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="d66af-111">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-111">Fixed price</span></span>

<span data-ttu-id="d66af-112">Όταν υποβάλλεται μια καταχώρηση χρόνου για ένα έργο που έχει συνδεθεί με μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου μόνο για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="d66af-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="d66af-113">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="d66af-113">Default pricing</span></span>

<span data-ttu-id="d66af-114">Η λογική για τη δημιουργία προεπιλεγμένων τιμών βρίσκεται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="d66af-115">Οι τιμές πεδίου από μια καταχώρηση χρόνου αντιγράφονται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="d66af-116">Αυτές οι τιμές περιλαμβάνουν την ημερομηνία της συναλλαγής, τη γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και το αποτέλεσμα της νομισματικής μονάδας στον κατάλληλο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="d66af-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="d66af-117">Τα πεδία που επηρεάζουν την προεπιλεγμένη τιμολόγηση, όπως ο **Ρόλος** και η **Μονάδα πόρων** , χρησιμοποιούνται για τον καθορισμό της κατάλληλης τιμής στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="d66af-118">Μπορείτε να προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση χρόνου.</span><span class="sxs-lookup"><span data-stu-id="d66af-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="d66af-119">Εάν θέλετε η τιμή πεδίου να μεταδοθεί σε πραγματικές τιμές, δημιουργήστε το πεδίο στους πίνακες **Πραγματικές τιμές** και **Γραμμή ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="d66af-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="d66af-120">Χρησιμοποιήστε προσαρμοσμένο κώδικα για τη μετάδοση της επιλεγμένης τιμής πεδίου από την καταχώρηση ώρας στις πραγματικές τιμές μέσω της γραμμής ημερολογίου χρησιμοποιώντας προελεύσεις συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d66af-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="d66af-121">Για περισσότερες πληροφορίες σχετικά με τις προελεύσεις συναλλαγών και τις συνδέσεις, ανατρέξτε στο θέμα [Σύνδεση πραγματικών τιμών με τις αρχικές καρτέλες](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="d66af-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="d66af-122">Γραμμές ημερολογίου και υποβολή βασικών εξόδων</span><span class="sxs-lookup"><span data-stu-id="d66af-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="d66af-123">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση εξόδων, ανατρέξτε στο θέμα [Επισκόπηση εξόδων](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d66af-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="d66af-124">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="d66af-124">Time and materials</span></span>

<span data-ttu-id="d66af-125">Όταν μια καταχώρηση βασικών εξόδων που υποβάλλεται συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης χρόνου και υλικών, το σύστημα δημιουργεί δύο γραμμές εγγραφών, μία για το κόστος και μία για τις μη χρεώσιμες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="d66af-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="d66af-126">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-126">Fixed price</span></span>

<span data-ttu-id="d66af-127">Όταν μια υποβεβλημένη καταχώρηση βασικών εξόδων συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="d66af-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="d66af-128">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="d66af-128">Default pricing</span></span>

<span data-ttu-id="d66af-129">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για τα έξοδα γίνεται με βάση την κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="d66af-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="d66af-130">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="d66af-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="d66af-131">Τα πεδία που επηρεάζουν την προεπιλεγμένη τιμολόγηση, όπως η **Κατηγορία συναλλαγών** και η **Μονάδα** , χρησιμοποιούνται για τον καθορισμό της κατάλληλης τιμής στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="d66af-132">Ωστόσο, αυτό λειτουργεί μόνο όταν η μέθοδος τιμολόγησης στον τιμοκατάλογο είναι **Τιμή ανά μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="d66af-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="d66af-133">Εάν η μέθοδος τιμολόγησης είναι **Στο κόστος** ή **Αύξηση επί του κόστους**, η τιμή που καταχωρείται όταν δημιουργείται η καταχώρηση δαπανών χρησιμοποιείται για το κόστος και η τιμή στη γραμμή του ημερολογίου πωλήσεων υπολογίζεται με βάση τη μέθοδο τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="d66af-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="d66af-134">Μπορείτε να προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση δαπανών.</span><span class="sxs-lookup"><span data-stu-id="d66af-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="d66af-135">Εάν θέλετε η τιμή πεδίου να μεταδοθεί σε πραγματικές τιμές, δημιουργήστε το πεδίο στους πίνακες **Πραγματικές τιμές** και **Γραμμή ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="d66af-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="d66af-136">Χρησιμοποιήστε προσαρμοσμένο κώδικα για τη μετάδοση της επιλεγμένης τιμής πεδίου από την καταχώρηση ώρας στις πραγματικές τιμές μέσω της γραμμής ημερολογίου χρησιμοποιώντας προελεύσεις συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d66af-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="d66af-137">Για περισσότερες πληροφορίες σχετικά με τις προελεύσεις συναλλαγών και τις συνδέσεις, ανατρέξτε στο θέμα [Σύνδεση πραγματικών τιμών με τις αρχικές καρτέλες](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="d66af-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="d66af-138">Γραμμές ημερολογίου και υποβολή αρχείου καταγραφής χρήσης υλικού</span><span class="sxs-lookup"><span data-stu-id="d66af-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="d66af-139">Για περισσότερες πληροφορίες σχετικά με την καταχώρηση δαπανών, ανατρέξτε στο [Αρχείο καταγραφής χρήσης υλικού](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="d66af-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="d66af-140">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="d66af-140">Time and materials</span></span>

<span data-ttu-id="d66af-141">Όταν μια υποβελβημένη καταχώρηση αρχείου καταγραφής χρήσης υλικού συνδέεται με ένα έργο που αντιστοιχίζεται σε μια γραμμή σύμβασης χρόνου και υλικού, το σύστημα δημιουργεί δύο γραμμές ημερολογίου, μία για το κόστος και μία για μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="d66af-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="d66af-142">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-142">Fixed price</span></span>

<span data-ttu-id="d66af-143">Όταν μια υποβεβλημένη καταχώρηση αρχείου καταχώρησης χρήσης υλικού συνδέεται με ένα έργο που έχει αντιστοιχιστεί σε μια γραμμή σύμβασης σταθερής τιμής, το σύστημα δημιουργεί μια γραμμή ημερολογίου για το κόστος.</span><span class="sxs-lookup"><span data-stu-id="d66af-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="d66af-144">Προεπιλεγμένη τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="d66af-144">Default pricing</span></span>

<span data-ttu-id="d66af-145">Η λογική για την εισαγωγή προεπιλεγμένων τιμών για το υλικό βασίζεται στο συνδυασμό προϊόντων και μονάδων.</span><span class="sxs-lookup"><span data-stu-id="d66af-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="d66af-146">Η ημερομηνία της συναλλαγής, η γραμμή σύμβασης με την οποία έχει αντιστοιχιστεί το έργο και η νομισματική μονάδα χρησιμοποιούνται για τον καθορισμό του κατάλληλου τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="d66af-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="d66af-147">Τα πεδία που επηρεάζουν την προεπιλεγμένη τιμολόγηση, όπως το **Αναγνωριστικό προϊόντων** και η **Μονάδα** , χρησιμοποιούνται για τον καθορισμό της κατάλληλης τιμής στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="d66af-148">Ωστόσο, αυτό λειτουργεί μόνο για προϊόντα καταλόγου.</span><span class="sxs-lookup"><span data-stu-id="d66af-148">However, this only works for catalog products.</span></span> <span data-ttu-id="d66af-149">Για τα εγγεγραμμένα προϊόντα, η τιμή που καταχωρείται όταν δημιουργείται η καταχώρηση του αρχείου καταγραφής χρήσης υλικού χρησιμοποιείται για την τιμή κόστους και πωλήσεων στις γραμμές ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="d66af-150">Μπορείτε να προσθέσετε ένα προσαρμοσμένο πεδίο στην καταχώρηση **Αρχείο καταγραφής χρήσης υλικού**.</span><span class="sxs-lookup"><span data-stu-id="d66af-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="d66af-151">Εάν θέλετε η τιμή πεδίου να μεταδοθεί σε πραγματικές τιμές, δημιουργήστε το πεδίο στους πίνακες **Πραγματικές τιμές** και **Γραμμή ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="d66af-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="d66af-152">Χρησιμοποιήστε προσαρμοσμένο κώδικα για τη μετάδοση της επιλεγμένης τιμής πεδίου από την καταχώρηση ώρας στις πραγματικές τιμές μέσω της γραμμής ημερολογίου χρησιμοποιώντας προελεύσεις συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="d66af-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="d66af-153">Για περισσότερες πληροφορίες σχετικά με τις προελεύσεις συναλλαγών και τις συνδέσεις, ανατρέξτε στο θέμα [Σύνδεση πραγματικών τιμών με τις αρχικές καρτέλες](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="d66af-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="d66af-154">Χρήση ημερολογίων εγγραφών για την καταγραφή του κόστους</span><span class="sxs-lookup"><span data-stu-id="d66af-154">Use entry journals to record costs</span></span>

<span data-ttu-id="d66af-155">Μπορείτε να χρησιμοποιήσετε ημερολόγια εγγραφών για να καταγράψετε το κόστος ή τα έσοδα στο υλικό, την αμοιβή, το χρόνο, τη δαπάνη ή τις φορολογικές κατηγορίες.</span><span class="sxs-lookup"><span data-stu-id="d66af-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="d66af-156">Τα ημερολόγια μπορούν να χρησιμοποιηθούν για τους εξής σκοπούς:</span><span class="sxs-lookup"><span data-stu-id="d66af-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="d66af-157">Μετακινήστε τα πραγματικά στοιχεία των συναλλαγών από ένα άλλο σύστημα στο Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="d66af-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="d66af-158">Για να καταγράψετε κόστη που έγιναν σε ένα άλλο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="d66af-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="d66af-159">Αυτά τα κόστη μπορεί να περιλαμβάνουν το κόστος προμηθειών ή υπεργολαβίας.</span><span class="sxs-lookup"><span data-stu-id="d66af-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d66af-160">Η εφαρμογή δεν επικυρώνει τον τύπο της γραμμής ημερολογίου ή τη σχετική τιμολόγηση που καταχωρείται στη γραμμή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="d66af-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="d66af-161">Επομένως, μόνο ένας χρήστης που γνωρίζει πλήρως το λογιστικό αντίκτυπο που έχουν τα πραγματικά στοιχεία στο έργο θα πρέπει να χρησιμοποιεί ημερολόγια εγγραφών για τη δημιουργία πραγματικών στοιχείων.</span><span class="sxs-lookup"><span data-stu-id="d66af-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="d66af-162">Λόγω της επίδρασης αυτού του τύπου ημερολογίου, θα πρέπει να επιλέξετε προσεκτικά ποιος έχει πρόσβαση για τη δημιουργία ημερολογίων εγγραφών.</span><span class="sxs-lookup"><span data-stu-id="d66af-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="d66af-163">Καταγραφή πραγματικών στοιχείων με βάση τα συμβάντα έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-163">Record actuals based on project events</span></span>

<span data-ttu-id="d66af-164">Το Project Operations καταγράφει όλες οι οικονομικές συναλλαγές που πραγματοποιούνται κατά τη διάρκεια ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="d66af-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="d66af-165">Αυτές οι συναλλαγές καταγράφονται ως πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="d66af-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="d66af-166">Στον ακόλουθο πίνακα παρουσιάζονται οι διαφορετικοί τύποι πραγματικών τιμών που δημιουργούνται, ανάλογα με το εάν το έργο είναι έργο χρόνου και υλικού, έργο σταθερής τιμής ή εσωτερικό έργο ή εάν βρίσκεται στο στάδιο προπώλησης.</span><span class="sxs-lookup"><span data-stu-id="d66af-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="d66af-167">Ο πόρος ανήκει στην ίδια οργανωτική μονάδα με τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d66af-168">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="d66af-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d66af-169">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="d66af-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d66af-170">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="d66af-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d66af-171">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="d66af-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d66af-172">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="d66af-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d66af-173">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d66af-174">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="d66af-174">Actuals</span></span></th>
<th><span data-ttu-id="d66af-175">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="d66af-175">Transaction currency</span></span></th>
<th><span data-ttu-id="d66af-176">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-176">Fixed price</span></span></th>
<th><span data-ttu-id="d66af-177">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="d66af-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d66af-178">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="d66af-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d66af-179">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="d66af-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-180">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="d66af-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d66af-181">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="d66af-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d66af-182">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="d66af-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d66af-183">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-183">Cost actual</span></span></td>
<td><span data-ttu-id="d66af-184">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-185">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-186">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="d66af-187">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-188">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-189">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="d66af-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d66af-190">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d66af-191">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="d66af-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d66af-192">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-192">Cost actual</span></span></td>
<td><span data-ttu-id="d66af-193">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-194">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-195">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-196">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-197">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-198">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-199">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-200">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-201">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d66af-202">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="d66af-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d66af-203">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d66af-204">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-205">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="d66af-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-206">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-207">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-208">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-209">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-209">Billed sales</span></span></td>
<td><span data-ttu-id="d66af-210">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d66af-211">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="d66af-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d66af-212">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d66af-213">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-214">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-215">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-216">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-217">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-218">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-219">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-220">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-221">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d66af-222">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="d66af-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d66af-223">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="d66af-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d66af-224">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d66af-225">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="d66af-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d66af-226">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="d66af-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d66af-227">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-228">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-229">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-230">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-230">Billed sales</span></span></td>
<td><span data-ttu-id="d66af-231">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d66af-232">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="d66af-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d66af-233">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="d66af-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d66af-234">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-235">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-236">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-237">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-238">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="d66af-239">Ο πόρος ανήκει σε μια οργανωτική μονάδα που διαφέρει από τη συμβαλλόμενη μονάδα του έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="d66af-240">Συμβάν</span><span class="sxs-lookup"><span data-stu-id="d66af-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="d66af-241">Χρεώσιμο έργο ή έργο πώλησης</span><span class="sxs-lookup"><span data-stu-id="d66af-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="d66af-242">Έργο στο στάδιο προπώλησης</span><span class="sxs-lookup"><span data-stu-id="d66af-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="d66af-243">Εσωτερικό έργο</span><span class="sxs-lookup"><span data-stu-id="d66af-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="d66af-244">Χρόνος και υλικό</span><span class="sxs-lookup"><span data-stu-id="d66af-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="d66af-245">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="d66af-246">Πραγματικές τιμές </span><span class="sxs-lookup"><span data-stu-id="d66af-246">Actuals</span></span></th>
<th><span data-ttu-id="d66af-247">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="d66af-247">Transaction currency</span></span></th>
<th><span data-ttu-id="d66af-248">Σταθερή τιμή</span><span class="sxs-lookup"><span data-stu-id="d66af-248">Fixed price</span></span></th>
<th><span data-ttu-id="d66af-249">Νόμισμα συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="d66af-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="d66af-250">Δημιουργήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="d66af-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="d66af-251">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="d66af-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-252">Υποβλήθηκε μια χρονική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="d66af-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="d66af-253">Καμία δραστηριότητα στην οντότητα "πραγματικές τιμές"</span><span class="sxs-lookup"><span data-stu-id="d66af-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="d66af-254">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="d66af-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d66af-255">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-255">Cost actual</span></span></td>
<td><span data-ttu-id="d66af-256">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d66af-257">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d66af-258">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="d66af-259">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="d66af-260">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-261">Πραγματικό μη χρεώσιμο ποσό πωλήσεων - Χρεώσιμο</span><span class="sxs-lookup"><span data-stu-id="d66af-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="d66af-262">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-263">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="d66af-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d66af-264">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="d66af-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-265">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="d66af-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d66af-266">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="d66af-267">Ο χρόνος έχει εγκριθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες κατά την έγκριση.</span><span class="sxs-lookup"><span data-stu-id="d66af-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="d66af-268">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-268">Cost actual</span></span></td>
<td><span data-ttu-id="d66af-269">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-270">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-271">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-272">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-273">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="d66af-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-274">Κόστος μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="d66af-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="d66af-275">Νόμισμα μονάδας πόρων</span><span class="sxs-lookup"><span data-stu-id="d66af-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-276">Πωλήσεις μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="d66af-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="d66af-277">Νόμισμα μονάδας συμβάσεων</span><span class="sxs-lookup"><span data-stu-id="d66af-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-278">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-279">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-280">Πραγματική μη χρεώσιμη ποσότητα πωλήσεων - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-281">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d66af-282">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία αλλαγή ή αύξηση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="d66af-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d66af-283">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d66af-284">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-285">Πωλήσεις με χρέωση για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="d66af-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-286">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-287">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="d66af-288">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-289">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-289">Billed sales</span></span></td>
<td><span data-ttu-id="d66af-290">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d66af-291">Ένα τιμολόγιο έχει επιβεβαιωθεί και δεν γίνεται καμία μείωση στις χρεώσιμες ώρες.</span><span class="sxs-lookup"><span data-stu-id="d66af-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="d66af-292">Καθολικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="d66af-293">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-294">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-295">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-296">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="d66af-297">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-298">Χρεώσιμες πωλήσεις - Χρεώσιμη για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-299">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-300">Χρεώσιμες πωλήσεις - Μη χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-301">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="d66af-302">Ένα τιμολόγιο διορθώνεται με την αύξηση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="d66af-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d66af-303">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="d66af-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d66af-304">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="d66af-305">Αντιστροφή χρεώσιμων πωλήσεων για ορόσημο</span><span class="sxs-lookup"><span data-stu-id="d66af-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="d66af-306">Αλλαγή της κατάστασης "ορόσημο" από <strong>Τιμολογήθηκε</strong> σε <strong>Έτοιμο για τιμολόγιο</strong></span><span class="sxs-lookup"><span data-stu-id="d66af-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="d66af-307">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-308">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="d66af-309">Δεν ισχύει</span><span class="sxs-lookup"><span data-stu-id="d66af-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-310">Χρεωμένες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="d66af-310">Billed sales</span></span></td>
<td><span data-ttu-id="d66af-311">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="d66af-312">Ένα τιμολόγιο διορθώνεται με τη μείωση της φορολογήσιμης ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="d66af-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="d66af-313">Χρεώσιμες πωλήσεις - Αντιστροφή</span><span class="sxs-lookup"><span data-stu-id="d66af-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="d66af-314">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-315">Χρεώσιμες πωλήσεις για νέα ποσότητα</span><span class="sxs-lookup"><span data-stu-id="d66af-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="d66af-316">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="d66af-317">Μη χρεώσιμες πωλήσεις - Χρεώσιμη για τη διαφορά</span><span class="sxs-lookup"><span data-stu-id="d66af-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="d66af-318">Νόμισμα σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d66af-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
