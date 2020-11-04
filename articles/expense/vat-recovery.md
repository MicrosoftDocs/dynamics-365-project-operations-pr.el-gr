---
title: Επιστροφή ΦΠΑ στη διαχείριση εξόδων
description: Αυτό το θέμα επεξηγεί τον τρόπο λήψης των επιστροφών στις συναλλαγές με επιλέξιμο φόρο προστιθέμενης αξίας (ΦΠΑ).
author: suvaidya
manager: AnnBe
ms.date: 10/10/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 2c20e4a7fa9748e03bf1729fc2f7bdbfc2f292d1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076784"
---
# <a name="vat-recovery-in-expense-management"></a><span data-ttu-id="1ec39-103">Επιστροφή ΦΠΑ στη διαχείριση εξόδων</span><span class="sxs-lookup"><span data-stu-id="1ec39-103">VAT recovery in Expense management</span></span>

<span data-ttu-id="1ec39-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="1ec39-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1ec39-105">Για τη λήψη επιστροφών για συναλλαγές με επιλέξιμο φόρο προστιθέμενης αξίας (ΦΠΑ), μια εταιρεία ή ένας οργανισμός πρέπει να αναγνωρίζει, να συλλέγει, να επαληθεύει και να υποβάλλει ακριβείς πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="1ec39-105">To receive refunds on eligible value-added tax (VAT) transactions, a company or organization must identify, collect, verify, and submit accurate information.</span></span> <span data-ttu-id="1ec39-106">Αυτή η διεργασία περιλαμβάνει πολλές εργασίες και, ανάλογα με το μέγεθος της εταιρείας σας, μπορεί να περιλαμβάνει αρκετούς υπαλλήλους ή ρόλους.</span><span class="sxs-lookup"><span data-stu-id="1ec39-106">This process includes multiple tasks and, depending on the size of your company, can include several employees or roles.</span></span>

<span data-ttu-id="1ec39-107">Για επιστροφή ΦΠΑ στη λειτουργική μονάδα **Διαχείριση εξόδων** , πρέπει να ολοκληρωθούν οι ακόλουθες προϋποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="1ec39-107">To recover VAT in the **Expense management** module, the following prerequisites must be completed:</span></span>

- <span data-ttu-id="1ec39-108">Πρέπει να δημιουργηθούν κωδικοί φόρων για τις χώρες/περιοχές που έχουν εκχωρηθεί σε κατηγορίες δαπανών.</span><span class="sxs-lookup"><span data-stu-id="1ec39-108">Tax codes must be created for countries/regions that are allocated to expense categories.</span></span>
- <span data-ttu-id="1ec39-109">Πρέπει να δημιουργηθεί μια ομάδα φόρου πωλήσεων για κάθε φορολογικό κώδικα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-109">A sales tax group must be created for each tax code.</span></span>
- <span data-ttu-id="1ec39-110">Πρέπει να κωδικός φόρου πώλησης στοιχείου για κάθε ομάδα φόρου πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="1ec39-110">An item sales tax code must be created for each sales tax group.</span></span>

<span data-ttu-id="1ec39-111">Μετά την ολοκλήρωση των προϋποθέσεων, πρέπει να ολοκληρωθούν τα παρακάτω βήματα για να ζητηθεί επιστροφή χρημάτων για τις συναλλαγές ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-111">After the prerequisites are completed, the following steps must be completed to request refunds for VAT transactions.</span></span>

1. <span data-ttu-id="1ec39-112">Σε μια αναφορά εξόδων, καταχωρείτε πληροφορίες φόρου σχετικά με τις συναλλαγές με πιστωτικές κάρτες για τον προσδιορισμό των επιλέξιμων επιστροφών ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-112">On an expense report, enter tax information about credit card transactions to identify eligible VAT refunds.</span></span>
2. <span data-ttu-id="1ec39-113">Επαληθεύστε ότι όλες οι πληροφορίες φόρων είναι συμπληρωμένες και, στη συνέχεια, καταχωρήστε την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="1ec39-113">Verify that all tax information is complete, and then post the expense report.</span></span>
3. <span data-ttu-id="1ec39-114">Έξοδα διεργασίας που δικαιούνται διεθνή επιστροφή ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-114">Process expenses that are eligible for international VAT recovery.</span></span>
4. <span data-ttu-id="1ec39-115">Αποστείλετε τα δεδομένα επιστροφής ΦΠΑ στον τρίτο προμηθευτή για να υποβάλετε τις διεθνείς επιστροφές.</span><span class="sxs-lookup"><span data-stu-id="1ec39-115">Send VAT recovery data to the third-party vendor to file international recovery returns.</span></span>
5. <span data-ttu-id="1ec39-116">Έξοδα διεργασίας για εγχώρια επιστροφή ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-116">Process expenses for domestic VAT recovery.</span></span>

<span data-ttu-id="1ec39-117">Οι παρακάτω ενότητες παρέχουν παραδείγματα που δείχνουν τον τρόπο με τον οποίο οι υπάλληλοι της Contoso ολοκληρώνουν κάθε βήμα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-117">The following sections provide examples that show how Contoso employees complete each step.</span></span>

## <a name="enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a><span data-ttu-id="1ec39-118">Καταχωρίστε πληροφορίες φόρου σχετικά με τις συναλλαγές με πιστωτικές κάρτες για τον προσδιορισμό των επιλέξιμων επιστροφών ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-118">Enter tax information about credit card transactions to identify eligible VAT refunds</span></span>

<span data-ttu-id="1ec39-119">Η Δήμητρα, μια αντιπρόσωπος πωλήσεων της Contoso που εδρεύει στις Ηνωμένες Πολιτείες, επέστρεψε πρόσφατα από ένα ταξίδι πωλήσεων στο Ηνωμένο Βασίλειο.</span><span class="sxs-lookup"><span data-stu-id="1ec39-119">Nancy, a Contoso sales representative who is based in the United States, recently returned from a sales trip to the United Kingdom.</span></span> <span data-ttu-id="1ec39-120">Κατά τη διάρκεια του ταξιδιού η Δήμητρα έκανε ορισμένα προσωπικά έξοδα μέσω της πιστωτικής της κάρτας για γεύματα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-120">Durinthe trip, Nancy incurred some personal credit card expenses for meals.</span></span> <span data-ttu-id="1ec39-121">Η Δήμητρα πρέπει τώρα να δημιουργήσει μια αναφορά εξόδων για να συμβιβάσει τα έξοδα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-121">Nancy must now create an expense report to reconcile the expenses.</span></span>

<span data-ttu-id="1ec39-122">Όταν η Δήμητρα εισαγάγει πληροφορίες σχετικά με την αναφορά εξόδων, επιλέγει **Ηνωμένο Βασίλειο** στο πεδίο **Χώρα/περιοχή** στη σελίδα **Επεξεργασία αναφοράς εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-122">When Nancy enters information on the expense report, she selects **United Kingdom** in the **Country/region** field on the **Edit expense report** page.</span></span> <span data-ttu-id="1ec39-123">Στη συνέχεια, φιλτράρεται η λίστα με τις ομάδες φόρου πωλήσεων έτσι, ώστε να εμφανίζει μόνο τις ομάδες που ισχύουν για το Ηνωμένο Βασίλειο.</span><span class="sxs-lookup"><span data-stu-id="1ec39-123">The list of sales tax groups is then filtered so that it shows only the groups that apply to the United Kingdom.</span></span> <span data-ttu-id="1ec39-124">Η Δήμητρα επιλέγει την ομάδα φορολογίας πωλήσεων **Ηνωμένο Βασίλειο 001** και, στη συνέχεια, επιλέγει την ομάδα φόρου πωλήσεων ειδών **Γεύματα**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-124">Nancy selects the **United Kingdom 001** sales tax group and then selects the **Meals** item sales tax group.</span></span> <span data-ttu-id="1ec39-125">Στη συνέχεια, η Δήμητρα προσθέτει μια νέα συναλλαγή για διαμονή.</span><span class="sxs-lookup"><span data-stu-id="1ec39-125">Next, Nancy adds a new transaction for lodging.</span></span> <span data-ttu-id="1ec39-126">Επειδή υπάρχει μόνο μία ομάδα φόρου πωλήσεων και μια ομάδα φόρου πωλήσεων ειδών για διαμονή στο Ηνωμένο Βασίλειο, οι πληροφορίες αυτές συμπληρώνονται αυτόματα στην αναφορά εξόδων της Δήμητρας.</span><span class="sxs-lookup"><span data-stu-id="1ec39-126">Because there is only one sales tax group and one item sales tax group for lodging in the United Kingdom, this information is automatically filled in on Nancy's expense report.</span></span>

<span data-ttu-id="1ec39-127">Σύμφωνα με την πολιτική της Contoso, όλα τα έξοδα πρέπει να έχουν μια αντίστοιχη απόδειξη.</span><span class="sxs-lookup"><span data-stu-id="1ec39-127">Per Contoso policy, all expenses must have a matching receipt.</span></span> <span data-ttu-id="1ec39-128">Επομένως, όταν η Δήμητρα αποθηκεύει την αναφορά εξόδων, λαμβάνει ένα μήνυμα που αναφέρει ότι πρέπει να επισυνάψει ένα αποδεικτικό για κάθε συναλλαγή που αναγράφεται στην αναφορά εξόδων της.</span><span class="sxs-lookup"><span data-stu-id="1ec39-128">Therefore, when Nancy saves the expense report, she receives a message that states that she must attach a receipt for each transaction that she listed on her expense report.</span></span> <span data-ttu-id="1ec39-129">Η Δήμητρα επιβεβαιώνει ότι έχει επισυνάψει μια ψηφιακή εικόνα κάθε απόδειξης συναλλαγής στην αναφορά εξόδων της και, στη συνέχεια, υποβάλλει την αναφορά της για έγκριση.</span><span class="sxs-lookup"><span data-stu-id="1ec39-129">Nancy verifies that she has attached a digital image of each transaction receipt to her expense report and then submits her report for approval.</span></span> <span data-ttu-id="1ec39-130">Στη συνέχεια, στέλνει τις έγγραφες αποδείξεις στην ομάδα επεξεργασίας υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="1ec39-130">She then sends the paper receipts to the back-office processing team.</span></span> <span data-ttu-id="1ec39-131">Αυτή η ομάδα θα στείλει τα δεδομένα επιστροφής ΦΠΑ στον τρίτο προμηθευτή που αρχειοθετεί τις διεθνείς επιστροφές ΦΠΑ για την Contoso.</span><span class="sxs-lookup"><span data-stu-id="1ec39-131">This team will send the VAT recovery data to the third-party vendor that files international VAT recovery returns for Contoso.</span></span>

## <a name="verify-tax-information-and-post-an-expense-report"></a><span data-ttu-id="1ec39-132">Επαλήθευση φορολογικών πληροφοριών και καταχώρηση μιας αναφοράς εξόδων</span><span class="sxs-lookup"><span data-stu-id="1ec39-132">Verify tax information and post an expense report</span></span>

<span data-ttu-id="1ec39-133">Για να μπορέσει η Ιωάννα, η συντονίστρια πληρωτέων λογαριασμών για την Contoso, να καταχωρήσει μια αναφορά εξόδων θα πρέπει να καταχωρήσει τυχόν πληροφορίες φόρων που λείπουν από αυτήν.</span><span class="sxs-lookup"><span data-stu-id="1ec39-133">Before April, the Accounts payable coordinator for Contoso, can post an expense report, she must enter any tax information that is missing from it.</span></span> <span data-ttu-id="1ec39-134">Ανοίγει τη σελίδα **Λεπτομέρειες αναφοράς εξόδων** και βλέπει την εγκεκριμένη αναφορά δαπανών της Δήμητρας.</span><span class="sxs-lookup"><span data-stu-id="1ec39-134">She opens the **Expense report details** page and sees Nancy's approved expense report.</span></span> <span data-ttu-id="1ec39-135">Η Ιωάννα ανοίγει την αναφορά εξόδων για να προβάλει τις λεπτομέρειες των συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="1ec39-135">April then opens the expense report to view the details of the transactions.</span></span> <span data-ttu-id="1ec39-136">Βλέπει ότι η Δήμητρα δεν έχει εισαγάγει μια ομάδα φόρου πωλήσεων ειδών για μία από τις συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="1ec39-136">She sees that Nancy didn't enter an item sales tax group for one of the transactions.</span></span> <span data-ttu-id="1ec39-137">Επειδή αυτές οι πληροφορίες δεν παρέχονται, η Ιωάννα δεν μπορεί να καταχωρήσει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="1ec39-137">Because this information isn't provided, April can't post the expense report.</span></span> <span data-ttu-id="1ec39-138">Ως εκ τούτου, βλέπει τη σελίδα **Ρυθμίσεις φόρου** στη διαχείριση εξόδων και βρίσκει την κατάλληλη ομάδα φόρου πωλήσεων ειδών για τη χώρα/περιοχή και τον τύπο συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="1ec39-138">Therefore, she looks on the **Tax configurations** page in Expense management, and finds the appropriate item sales tax group for the country/region and the transaction type.</span></span> <span data-ttu-id="1ec39-139">Η Ιωάννα μπορεί πλέον να καταχωρήσει την αναφορά εξόδων στο γενικό καθολικό.</span><span class="sxs-lookup"><span data-stu-id="1ec39-139">April can now post the expense report to the general ledger.</span></span>

<span data-ttu-id="1ec39-140">Όταν η Ιωάννα καταχωρεί την αναφορά εξόδων, δημιουργείται ένα στοιχείο εργασίας με δυνατότητα επιστροφής ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-140">When April posts the expense report, a VAT recoverable work item is created.</span></span> <span data-ttu-id="1ec39-141">Αυτό το στοιχείο εργασίας ανατίθεται σε ένα μέλος της ομάδας επεξεργασίας υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="1ec39-141">This work item is assigned to a member of the back-office processing team.</span></span> <span data-ttu-id="1ec39-142">Η Ιωάννα λαμβάνει ένα μήνυμα που επιβεβαιώνει ότι η καταχώρηση ήταν επιτυχής.</span><span class="sxs-lookup"><span data-stu-id="1ec39-142">April receives a message that confirms that posting was successful.</span></span> <span data-ttu-id="1ec39-143">Αυτό το μήνυμα αναφέρει επίσης τον αριθμό των συναλλαγών ΦΠΑ που αναγνωρίστηκαν για επιστροφή.</span><span class="sxs-lookup"><span data-stu-id="1ec39-143">This message also lists the number of VAT transactions that were identified for recovery.</span></span>

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a><span data-ttu-id="1ec39-144">Έξοδα διεργασίας που δικαιούνται διεθνή επιστροφή ΦΠΑ.</span><span class="sxs-lookup"><span data-stu-id="1ec39-144">Process expenses that are eligible for international VAT recovery</span></span>

<span data-ttu-id="1ec39-145">Ο Αλέξης, μέλος της ομάδας επεξεργασίας υποστήριξης της Contoso, είναι υπεύθυνος να επαληθεύσει ότι όλες οι απαιτούμενες πληροφορίες για την επιστροφή ΦΠΑ περιλαμβάνονται στις αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="1ec39-145">Arnie, a member of Contoso's back-office processing team, is responsible for verifying that all the required information for VAT recovery is included on expense reports.</span></span> <span data-ttu-id="1ec39-146">Ανοίγει τη σελίδα **Επιστροφή φόρου εξόδων** και επιλέγει την αναφορά εξόδων που υπέβαλε η Δήμητρα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-146">He opens the **Expense tax recovery** page and selects the expense report that Nancy submitted.</span></span> <span data-ttu-id="1ec39-147">Στη συνέχεια, ο Αλέξης επιβεβαιώνει ότι έχουν επισυναφθεί όλες οι απαιτούμενες αποδείξεις και ότι έχουν καταχωρηθεί οι σωστές ομάδες φόρου πωλήσεων και οι κωδικοί φόρου πωλήσεων ειδών.</span><span class="sxs-lookup"><span data-stu-id="1ec39-147">Arnie then verifies that all the required receipts are attached, and that the correct sales tax group and item sales tax codes were entered.</span></span>

<span data-ttu-id="1ec39-148">Όταν ο Αλέξης λάβει τις έγγραφες αποδείξεις από τη Δήμητρα, τις επιβεβαιώνει έναντι των ψηφιακών αποδείξεων και, στη συνέχεια, αλλάζει την κατάσταση της αναφοράς εξόδων σε **Έτοιμο για επιστροφή**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-148">When Arnie receives the paper receipts from Nancy, he verifies them against the digital receipts and then changes the status of the expense report to **Ready for recovery**.</span></span>

## <a name="send-vat-recovery-data-to-the-third-party-vendor"></a><span data-ttu-id="1ec39-149">Αποστολή δεδομένων επιστροφής ΦΠΑ στον τρίτο προμηθευτή</span><span class="sxs-lookup"><span data-stu-id="1ec39-149">Send VAT recovery data to the third-party vendor</span></span>

<span data-ttu-id="1ec39-150">Όταν ο Αλέξης είναι έτοιμος να στείλει τα δεδομένα αναφοράς εξόδων στον τρίτο προμηθευτή που θα καταθέσει τις επιστροφές ΦΠΑ, ανοίγει τη σελίδα **Ανάκτηση φόρων εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-150">When Arnie is ready to send the expense report data to the third-party vendor that will file the VAT recovery returns, he opens the **Expense tax recovery** page.</span></span> <span data-ttu-id="1ec39-151">Φιλτράρει τη σελίδα έτσι, ώστε να εμφανίζει μόνο τις αναφορές εξόδων που έχουν επισημανθεί ως **Έτοιμο για επιστροφή**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-151">He filters the page so that it shows only the expense reports that are marked as **Ready for recovery**.</span></span> <span data-ttu-id="1ec39-152">Στη συνέχεια, ο Αλέξης επιλέγει **Αρχείο** &gt; **Εξαγωγή σε Excel**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-152">Arnie then selects **File** &gt; **Export to Excel**.</span></span> <span data-ttu-id="1ec39-153">Οι πληροφορίες ΦΠΑ από τις αναφορές εξόδων εξάγονται σε ένα Microsoft Excel φύλλο εργασίας.</span><span class="sxs-lookup"><span data-stu-id="1ec39-153">The VAT information from the expense reports is exported to a Microsoft Excel worksheet.</span></span> <span data-ttu-id="1ec39-154">Ο Αλέξης καταχωρεί αυτό το φύλλο εργασίας στον τρίτο προμηθευτή και περιλαμβάνει ένα μήνυμα που αναφέρει ότι οι αποδείξεις εγγράφου έχουν αποσταλεί από τον ταχυμεταφορέα.</span><span class="sxs-lookup"><span data-stu-id="1ec39-154">Arnie submits this worksheet to the third-party vendor and includes a message that states that the paper receipts have been sent by courier.</span></span>

## <a name="process-expenses-for-domestic-vat-recovery"></a><span data-ttu-id="1ec39-155">Έξοδα διεργασίας για εγχώρια επιστροφή ΦΠΑ</span><span class="sxs-lookup"><span data-stu-id="1ec39-155">Process expenses for domestic VAT recovery</span></span>

<span data-ttu-id="1ec39-156">Ο Αλέξης πρέπει να επαληθεύσει ότι οι συναλλαγές αναφοράς εξόδων είναι επιλέξιμες για επιστροφή ΦΠΑ και ότι οι ψηφιακές αποδείξεις επισυνάπτονται στις αναφορές.</span><span class="sxs-lookup"><span data-stu-id="1ec39-156">Arnie must verify that the expense report transactions are eligible for VAT recovery, and that the digital receipts are attached to the reports.</span></span> <span data-ttu-id="1ec39-157">Για να ξεκινήσετε την επεξεργασία των επιλέξιμων δαπανών για εγχώρια επιστροφή, ο Αλέξης ανοίγει τη σελίδα **Ανάκτηση φόρων εξόδων** και επιλέγει την αναφορά εξόδων που απαιτεί επαλήθευση.</span><span class="sxs-lookup"><span data-stu-id="1ec39-157">To start to process eligible expenses for domestic recovery, Arnie opens the **Expense tax recovery** page and selects the expense report that requires verification.</span></span> <span data-ttu-id="1ec39-158">Επιβεβαιώνει ότι οι αποδείξεις βρίσκονται στο όνομα της εταιρείας αντί του υπαλλήλου.</span><span class="sxs-lookup"><span data-stu-id="1ec39-158">He verifies that receipts are in the name of the company instead of the employee.</span></span> <span data-ttu-id="1ec39-159">(Για επιστροφή ΦΠΑ, οι αποδείξεις πρέπει να είναι στο όνομα της εταιρείας). Ο Αλέξης επιβεβαιώνει ότι έχουν καταχωριστεί η σωστή ομάδα φόρου πωλήσεων και οι σωστοί κωδικοί φόρου πωλήσεων ειδών.</span><span class="sxs-lookup"><span data-stu-id="1ec39-159">(For VAT recovery, receipts must be in the name of the company.) Arnie then verifies that the correct sales tax group and item sales tax codes were entered.</span></span>

<span data-ttu-id="1ec39-160">Όταν ο Αλέξης λάβει τις έγγραφες αποδείξεις αλλάζει την κατάσταση της αναφοράς εξόδων σε **Έτοιμο για επιστροφή**.</span><span class="sxs-lookup"><span data-stu-id="1ec39-160">When Arnie receives the paper receipts, he changes the status of the expense report to **Ready for recovery**.</span></span> <span data-ttu-id="1ec39-161">Στη συνέχεια, μπορεί να καταθέσει την επιστροφή στην αρμόδια φορολογική αρχή.</span><span class="sxs-lookup"><span data-stu-id="1ec39-161">He can then file the return with the appropriate tax authority.</span></span> <span data-ttu-id="1ec39-162">Σε αυτήν την περίπτωση, η αρμόδια φορολογική αρχή στις Ηνωμένες Πολιτείες είναι η φορολογική υπηρεσία (IRS).</span><span class="sxs-lookup"><span data-stu-id="1ec39-162">In this case, the appropriate tax authority in the United States is the Internal Revenue Service (IRS).</span></span>