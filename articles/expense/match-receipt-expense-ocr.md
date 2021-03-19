---
title: Καταγραφή απόδειξης με χρήση OCR
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την επεξεργασία οπτικής αναγνώρισης χαρακτήρων (OCR) για αποδείξεις.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: fd0cb0fb094260fa3e82d7a2f200f328a39dd7a1
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "5499851"
---
# <a name="capture-a-receipt-using-ocr"></a><span data-ttu-id="de04d-103">Καταγραφή απόδειξης με χρήση OCR</span><span class="sxs-lookup"><span data-stu-id="de04d-103">Capture a receipt using OCR</span></span>

<span data-ttu-id="de04d-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="de04d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="de04d-105">Η καταχώρηση εξόδων έχει ενισχυθεί με την εισαγωγή της επεξεργασίας οπτικής αναγνώρισης χαρακτήρων (OCR) για αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="de04d-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="de04d-106">Αυτή η λειτουργικότητα έχει σχεδιαστεί για τη βελτίωση της εμπειρίας του χρήστη κατά τη δημιουργία αναφορών εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="de04d-107">Δυνατότητες κλειδιά</span><span class="sxs-lookup"><span data-stu-id="de04d-107">Key features</span></span>

- <span data-ttu-id="de04d-108">Το σύστημα εξάγει το όνομα του εμπόρου, την ημερομηνία και το συνολικό ποσό από τις αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="de04d-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="de04d-109">Το σύστημα θα προσπαθεί να αντιστοιχίσει μη συνημμένες αποδείξεις με μη προσαρτημένες συναλλαγές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="de04d-110">Μπορείτε να δημιουργήσετε καταχωρημένες συναλλαγές εξόδων με μη αυτόματο τρόπο από αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="de04d-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="de04d-111">Επισύναψη αποδείξεων σε μια αναφορά εξόδων</span><span class="sxs-lookup"><span data-stu-id="de04d-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="de04d-112">Για την αυτόματη προσάρτηση αποδείξεων που περιλαμβάνουν συναλλαγές με πιστωτικές κάρτες όταν δημιουργείται μια αναφορά εξόδων, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="de04d-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="de04d-113">Ανοίξτε το χώρο εργασίας **Διαχείριση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="de04d-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="de04d-114">Στη σελίδα **Αποδείξεις**, επαληθεύστε ότι υπάρχουν αποδεικτικά που δεν έχουν επισυναφθεί.</span><span class="sxs-lookup"><span data-stu-id="de04d-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="de04d-115">Μπορείτε, επίσης, να αποστείλετε αποδείξεις στην καρτέλα **Αποδείξεις**.</span><span class="sxs-lookup"><span data-stu-id="de04d-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="de04d-116">Στη καρτέλα **Έξοδα**, επαληθεύστε ότι υπάρχουν έξοδα που δεν έχουν επισυναφθεί.</span><span class="sxs-lookup"><span data-stu-id="de04d-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="de04d-117">Κατά κανόνα, ο διαχειριστής εξόδων εισαγάγει αυτά τα έξοδα από τον παροχέα της πιστωτικής κάρτας.</span><span class="sxs-lookup"><span data-stu-id="de04d-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="de04d-118">Επιλέξτε **Νέα αναφορά εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="de04d-118">Select **New expense report**.</span></span> <span data-ttu-id="de04d-119">Λάβετε υπόψη ότι τώρα μπορείτε να συμπεριλάβετε έξοδα και αποδείξεις, επίσης όταν δημιουργείτε μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="de04d-120">Εάν προσθέσετε και έξοδα και αποδείξεις, ενεργοποιείται η αυτόματη αντιστοίχιση των αποδείξεων με τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="de04d-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="de04d-121">Δημιουργία ή αντιστοίχηση αποδείξεων σε μια αναφορά εξόδων</span><span class="sxs-lookup"><span data-stu-id="de04d-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="de04d-122">Για να δημιουργήσετε ένα έξοδο ή να αντιστοιχίσετε ένα έξοδο από μια απόδειξη, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="de04d-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="de04d-123">Σε μια αναφορά εξόδων, στην καρτέλα **Αποδείξεις**, επισυνάψτε μια απόδειξη επιλέγοντας **Προσθήκη αποδείξεων**.</span><span class="sxs-lookup"><span data-stu-id="de04d-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="de04d-124">Κάτω από την ληφθείσα εικόνα της απόδειξης, προσέξτε τις επιλογές **Δημιουργία** και **Αντιστοίχιση**.</span><span class="sxs-lookup"><span data-stu-id="de04d-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="de04d-125">Επιλέξτε **Δημιουργία** για να δημιουργήσετε μια συναλλαγή εξόδων που καταχωρείται με μη αυτόματο τρόπο και συμπληρώστε τις τιμές που έχουν εξαχθεί από την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="de04d-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="de04d-126">Εάν επιλέξετε **Αντιστοίχηση**, το σύστημα θα επιχειρήσει να αντιστοιχίσει ένα υφιστάμενο έξοδο με την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="de04d-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="de04d-127">Εγκατάσταση</span><span class="sxs-lookup"><span data-stu-id="de04d-127">Installation</span></span>

<span data-ttu-id="de04d-128">Για να χρησιμοποιήσετε αυτές τις προηγμένες δυνατότητες εξόδων, εγκαταστήστε το πρόσθετο Υπηρεσίας Διαχείρισης Εξόδων για το Microsoft Dynamics 365 Finance και ενεργοποιήστε τις δυνατότητες που υπάρχουν στην παρουσία σας.</span><span class="sxs-lookup"><span data-stu-id="de04d-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="de04d-129">Μπορείτε να αποκτήσετε πρόσβαση στο πρόσθετο από το έργο σας στο Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="de04d-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="de04d-130">Πραγματοποιήστε είσοδο στο LCS και ανοίξτε το επιθυμητό περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="de04d-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="de04d-131">Μεταβείτε στην επιλογή **Πλήρεις λεπτομέρειες**.</span><span class="sxs-lookup"><span data-stu-id="de04d-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="de04d-132">Επιλέξτε **Συντήρηση** ή κάντε κύλιση προς τα κάτω στη συνοπτική καρτέλα **Πρόσθετα περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="de04d-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="de04d-133">Επιλέξτε **Εγκατάσταση νέου πρόσθετου**.</span><span class="sxs-lookup"><span data-stu-id="de04d-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="de04d-134">Επιλέξτε **Υπηρεσία Διαχείρισης Εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="de04d-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="de04d-135">Ακολουθήστε τον οδηγό εγκατάστασης και αποδεχτείτε τους όρους και τις προϋποθέσεις.</span><span class="sxs-lookup"><span data-stu-id="de04d-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="de04d-136">Επιλέξτε **Εγκατάσταση**.</span><span class="sxs-lookup"><span data-stu-id="de04d-136">Select **Install**.</span></span>

<span data-ttu-id="de04d-137">Στο χώρο εργασίας **Διαχείρισης δυνατοτήτων**, ενεργοποιήστε τις ακόλουθες δυνατότητες:</span><span class="sxs-lookup"><span data-stu-id="de04d-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="de04d-138">Νέα σύλληψη αναφορών εξόδων</span><span class="sxs-lookup"><span data-stu-id="de04d-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="de04d-139">Αυτόματη αντιστοίχηση και δημιουργία εξόδου από την απόδειξη</span><span class="sxs-lookup"><span data-stu-id="de04d-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="de04d-140">Όταν ενεργοποιείτε αυτές τις δυνατότητες, γίνονται οι εξής ενέργειες:</span><span class="sxs-lookup"><span data-stu-id="de04d-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="de04d-141">Ο υπάρχων χώρος εργασίας **Διαχείριση εξόδων** αντικαθίσταται με το νέο χώρο εργασίας.</span><span class="sxs-lookup"><span data-stu-id="de04d-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="de04d-142">Προστίθεται ένα νέο στοιχείο μενού για την προβολή του πεδίου εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="de04d-143">Εξακολουθείτε να μπορείτε να ανοίξετε την παλιά σελίδα **Αναφορές εξόδων** μεταβαίνοντας στη **Διαχείριση εξόδων > Τα έξοδά μου > Αναφορές εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="de04d-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="de04d-144">Οι ροές εργασιών και τυχόν εγκρίσεις σάς μεταφέρουν ακόμα στη σελίδα με τις υπάρχουσες αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="de04d-145">Οι αποδείξεις θα υποβληθούν σε επεξεργασία μέσω Microsoft Azure Cognitive Services και τα μετα-δεδομένα θα εξαχθούν και θα προστεθούν.</span><span class="sxs-lookup"><span data-stu-id="de04d-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="de04d-146">Προστίθεται μια επιλογή που σας δίνει τη δυνατότητα να δημιουργήσετε μια αναφορά εξόδων που περιλαμβάνει αντιστοιχισμένες αλλά μη προσαρτημένες αποδείξεις.</span><span class="sxs-lookup"><span data-stu-id="de04d-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="de04d-147">Μια επιλογή που προστίθεται στις αναφορές εξόδων, σάς δίνει τη δυνατότητα να δημιουργήσετε μια γραμμή εξόδων από μια απόδειξη ή επιχειρεί να αντιστοιχίσει μια υπάρχουσα απόδειξη με μια υπάρχουσα γραμμή εξόδων.</span><span class="sxs-lookup"><span data-stu-id="de04d-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="de04d-148">Συνήθεις ερωτήσεις</span><span class="sxs-lookup"><span data-stu-id="de04d-148">Frequently asked questions</span></span>

<span data-ttu-id="de04d-149">**Η Microsoft χρησιμοποιεί τα δεδομένα μου για τα μοντέλα της;**</span><span class="sxs-lookup"><span data-stu-id="de04d-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="de04d-150">Όχι, η Microsoft έχει δημιουργήσει ένα γενικό μοντέλο εκμάθησης μηχανής για την υπηρεσία επεξεργασίας αποδείξεων.</span><span class="sxs-lookup"><span data-stu-id="de04d-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="de04d-151">Αυτό το μοντέλο δεν βασίζεται στις αποδείξεις που αποστέλλετε.</span><span class="sxs-lookup"><span data-stu-id="de04d-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="de04d-152">**Πού είναι διαθέσιμη αυτή η δυνατότητα και πού γίνεται επεξεργασία της;**</span><span class="sxs-lookup"><span data-stu-id="de04d-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="de04d-153">Προς το παρόν, υποστηρίζονται οι Ηνωμένες Πολιτείες.</span><span class="sxs-lookup"><span data-stu-id="de04d-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="de04d-154">**Πού καταλήγουν οι αποδείξεις μου;**</span><span class="sxs-lookup"><span data-stu-id="de04d-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="de04d-155">Το Finance θα επικοινωνήσει με το Cognitive Services για την εξαγωγή των δεδομένων πεδίων.</span><span class="sxs-lookup"><span data-stu-id="de04d-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="de04d-156">Οι Cognitive Services θα διατηρήσουν ένα αντίγραφο της απόδειξής σας για 24 ώρες, ενώ γίνεται η επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="de04d-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="de04d-157">Μετά την ολοκλήρωση της επεξεργασίας, οι Cognitive Services θα αφαιρέσουν την απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="de04d-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="de04d-158">Οι αποδείξεις παραμένουν αποθηκευμένες στο Finance.</span><span class="sxs-lookup"><span data-stu-id="de04d-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="de04d-159">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση κατανόησης αποδείξεων με τη νέα δυνατότητα Αναγνώρισης φορμών](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="de04d-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
