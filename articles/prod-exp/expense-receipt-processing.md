---
title: Επεξεργασία αποδείξεων εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την επεξεργασία οπτικής αναγνώρισης χαρακτήρων (OCR) για αποδείξεις. Αυτή η δυνατότητα έχει σχεδιαστεί για τη βελτίωση της εμπειρίας του χρήστη κατά τη δημιουργία αναφορών εξόδων στο Microsoft Dynamics 365 Finance.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: ed9c97ba9cc505106599c2896dc2112358d0c408
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993506"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="ca9ee-104">Επεξεργασία αποδείξεων εξόδων</span><span class="sxs-lookup"><span data-stu-id="ca9ee-104">Expense receipt processing</span></span>

<span data-ttu-id="ca9ee-105">Η καταχώρηση εξόδων έχει ενισχυθεί με την εισαγωγή της επεξεργασίας οπτικής αναγνώρισης χαρακτήρων (OCR) για αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="ca9ee-106">Αυτή η δυνατότητα έχει σχεδιαστεί για τη βελτίωση της εμπειρίας του χρήστη κατά τη δημιουργία αναφορών εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="ca9ee-107">Δυνατότητες κλειδιά</span><span class="sxs-lookup"><span data-stu-id="ca9ee-107">Key features</span></span>

- <span data-ttu-id="ca9ee-108">Το σύστημα εξάγει το όνομα του εμπόρου, την ημερομηνία και το συνολικό ποσό από τις αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="ca9ee-109">Αυτή η δυνατότητα προσπαθεί να αντιστοιχίσει μη συνημμένες αποδείξεις με μη προσαρτημένες συναλλαγές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="ca9ee-110">Οι χρήστες μπορούν να δημιουργήσουν καταχωρημένες συναλλαγές εξόδων με μη αυτόματο τρόπο από αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="ca9ee-111">Παραδείγματα χρήσης</span><span class="sxs-lookup"><span data-stu-id="ca9ee-111">Usage examples</span></span>

<span data-ttu-id="ca9ee-112">Για την αυτόματη προσάρτηση αποδείξεων που περιλαμβάνουν συναλλαγές με πιστωτικές κάρτες όταν δημιουργείται μια αναφορά εξόδων, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ca9ee-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="ca9ee-113">Ανοίξτε το χώρο εργασίας **Διαχείριση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="ca9ee-114">Στη σελίδα **Αποδείξεις**, επαληθεύστε ότι υπάρχουν αποδεικτικά που δεν έχουν επισυναφθεί.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="ca9ee-115">Μπορείτε, επίσης, να αποστείλετε αποδείξεις στην καρτέλα **Αποδείξεις**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="ca9ee-116">Στη καρτέλα **Έξοδα**, επαληθεύστε ότι υπάρχουν έξοδα που δεν έχουν επισυναφθεί.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="ca9ee-117">Κατά κανόνα, ο διαχειριστής εξόδων εισαγάγει αυτά τα έξοδα από τον παροχέα της πιστωτικής κάρτας.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="ca9ee-118">Επιλέξτε **Νέα αναφορά εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-118">Select **New expense report**.</span></span> <span data-ttu-id="ca9ee-119">Λάβετε υπόψη ότι τώρα μπορείτε να συμπεριλάβετε έξοδα και αποδείξεις, επίσης όταν δημιουργείτε μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="ca9ee-120">Εάν προσθέσετε και έξοδα και αποδείξεις, ενεργοποιείται η αυτόματη αντιστοίχιση των αποδείξεων με τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="ca9ee-121">Για να δημιουργήσετε ένα έξοδο ή να αντιστοιχίσετε ένα έξοδο από μια απόδειξη, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="ca9ee-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="ca9ee-122">Σε μια αναφορά εξόδων, στην καρτέλα **Αποδείξεις**, επισυνάψτε μια απόδειξη επιλέγοντας **Προσθήκη αποδείξεων**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="ca9ee-123">Κάτω από την ληφθείσα εικόνα της απόδειξης, προσέξτε τις επιλογές **Δημιουργία** και **Αντιστοίχιση**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="ca9ee-124">Επιλέξτε **Δημιουργία** για να δημιουργήσετε μια συναλλαγή εξόδων που καταχωρείται με μη αυτόματο τρόπο και συμπληρώστε τις τιμές που έχουν εξαχθεί από την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="ca9ee-125">Εάν επιλέξετε **Αντιστοίχηση**, το σύστημα θα επιχειρήσει να αντιστοιχίσει ένα υφιστάμενο έξοδο με την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="ca9ee-126">Εγκατάσταση</span><span class="sxs-lookup"><span data-stu-id="ca9ee-126">Installation</span></span>

<span data-ttu-id="ca9ee-127">Αυτή η δυνατότητα λειτουργεί σε συνδυασμό με τη δυνατότητα **Επανασχεδιασμός αναφορών εξόδων** για να σας βοηθήσει να απλοποιήσετε την εμπειρία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="ca9ee-128">Αυτή η δυνατότητα είναι διαθέσιμη μόνο για περιβάλλοντα επιπέδου 2+, τα οποία είναι προστατευμένης εκτέλεσης και παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="ca9ee-129">Για να χρησιμοποιήσετε αυτές τις προηγμένες δυνατότητες εξόδων, εγκαταστήστε το πρόσθετο Υπηρεσίας Διαχείρισης Εξόδων για το Microsoft Dynamics 365 Finance και ενεργοποιήστε τις δυνατότητες που υπάρχουν στην παρουσία σας.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="ca9ee-130">Μπορείτε να αποκτήσετε πρόσβαση στο πρόσθετο από το έργο σας στο Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="ca9ee-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="ca9ee-131">Πραγματοποιήστε είσοδο στο LCS και ανοίξτε το επιθυμητό περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="ca9ee-132">Μεταβείτε στην επιλογή **Πλήρεις λεπτομέρειες**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="ca9ee-133">Επιλέξτε **Συντήρηση** ή κάντε κύλιση προς τα κάτω στη συνοπτική καρτέλα **Πρόσθετα περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="ca9ee-134">Επιλέξτε **Εγκατάσταση νέου πρόσθετου**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="ca9ee-135">Επιλέξτε **Υπηρεσία Διαχείρισης Εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="ca9ee-136">Ακολουθήστε τον οδηγό εγκατάστασης και αποδεχτείτε τους όρους και τις προϋποθέσεις.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="ca9ee-137">Επιλέξτε **Εγκατάσταση**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-137">Select **Install**.</span></span>

<span data-ttu-id="ca9ee-138">Στο χώρο εργασίας **Διαχείρισης δυνατοτήτων**, ενεργοποιήστε τις ακόλουθες δυνατότητες:</span><span class="sxs-lookup"><span data-stu-id="ca9ee-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="ca9ee-139">Νέα σύλληψη αναφορών εξόδων</span><span class="sxs-lookup"><span data-stu-id="ca9ee-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="ca9ee-140">Αυτόματη αντιστοίχηση και δημιουργία εξόδου από την απόδειξη</span><span class="sxs-lookup"><span data-stu-id="ca9ee-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="ca9ee-141">Όταν ενεργοποιείτε αυτές τις δυνατότητες, γίνονται οι εξής ενέργειες:</span><span class="sxs-lookup"><span data-stu-id="ca9ee-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="ca9ee-142">Ο υπάρχων χώρος εργασίας **Διαχείριση εξόδων** αντικαθίσταται με το νέο χώρο εργασίας.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="ca9ee-143">Προστίθεται ένα νέο στοιχείο μενού για την προβολή του πεδίου εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="ca9ee-144">Εξακολουθείτε να μπορείτε να ανοίξετε την παλιά σελίδα **Αναφορές εξόδων** μεταβαίνοντας στη **Διαχείριση εξόδων > Τα έξοδά μου > Αναφορές εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="ca9ee-145">Οι ροές εργασιών και τυχόν εγκρίσεις σάς μεταφέρουν ακόμα στη σελίδα με τις υπάρχουσες αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="ca9ee-146">Οι αποδείξεις θα υποβληθούν σε επεξεργασία μέσω Microsoft Azure Cognitive Services και τα μετα-δεδομένα θα εξαχθούν και θα προστεθούν.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="ca9ee-147">Προστίθεται μια επιλογή που σας δίνει τη δυνατότητα να δημιουργήσετε μια αναφορά εξόδων που περιλαμβάνει αντιστοιχισμένες αλλά μη προσαρτημένες αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="ca9ee-148">Μια επιλογή που προστίθεται στις αναφορές εξόδων, σάς δίνει τη δυνατότητα να δημιουργήσετε μια γραμμή εξόδων από μια απόδειξη ή επιχειρεί να αντιστοιχίσει μια υπάρχουσα απόδειξη με μια υπάρχουσα γραμμή εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="ca9ee-149">Για περισσότερες πληροφορίες σχετικά με τη δυνατότητα Επανασχεδιασμός αναφορών εξόδων, ανατρέξτε στην ενότητα [Επανασχεδιασμός αναφορών εξόδων](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="ca9ee-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="ca9ee-150">Συνήθεις ερωτήσεις</span><span class="sxs-lookup"><span data-stu-id="ca9ee-150">Frequently asked questions</span></span>

<span data-ttu-id="ca9ee-151">**Η Microsoft χρησιμοποιεί τα δεδομένα μου για τα μοντέλα της;**</span><span class="sxs-lookup"><span data-stu-id="ca9ee-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="ca9ee-152">Όχι, η Microsoft έχει δημιουργήσει ένα γενικό μοντέλο εκμάθησης μηχανής για την υπηρεσία επεξεργασίας αποδείξεων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="ca9ee-153">Αυτό το μοντέλο δεν βασίζεται στις αποδείξεις που αποστέλλετε.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="ca9ee-154">**Πού είναι διαθέσιμη αυτή η δυνατότητα και πού γίνεται επεξεργασία της;**</span><span class="sxs-lookup"><span data-stu-id="ca9ee-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="ca9ee-155">Προς το παρόν, υποστηρίζονται οι Ηνωμένες Πολιτείες.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="ca9ee-156">**Πού καταλήγουν οι αποδείξεις μου;**</span><span class="sxs-lookup"><span data-stu-id="ca9ee-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="ca9ee-157">Το Finance θα επικοινωνήσει με το Cognitive Services για την εξαγωγή των δεδομένων πεδίων.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="ca9ee-158">Οι Cognitive Services θα διατηρήσουν ένα αντίγραφο της απόδειξής σας για 24 ώρες, ενώ γίνεται η επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="ca9ee-159">Μετά την ολοκλήρωση της επεξεργασίας, οι Cognitive Services θα αφαιρέσουν την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="ca9ee-160">Οι αποδείξεις παραμένουν αποθηκευμένες στο Finance.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="ca9ee-161">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση κατανόησης αποδείξεων με τη νέα δυνατότητα Αναγνώρισης φορμών](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="ca9ee-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]