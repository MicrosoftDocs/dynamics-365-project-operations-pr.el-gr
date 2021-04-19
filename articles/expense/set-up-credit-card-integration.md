---
title: Ρύθμιση ενοποίησης πιστωτικών καρτών
description: Αυτό θέμα εξηγεί τον τρόπο εργασίας με συναλλαγές πιστωτικής κάρτας που σχετίζονται με δαπάνες.
author: suvaidya
manager: AnnBe
ms.date: 04/02/2021
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
ms.openlocfilehash: 72ff98f5985af4362cde3c9914e0d20247f1f09a
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866683"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="cfa2d-103">Ρύθμιση ενοποίησης πιστωτικών καρτών</span><span class="sxs-lookup"><span data-stu-id="cfa2d-103">Set up credit card integration</span></span>

<span data-ttu-id="cfa2d-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="cfa2d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cfa2d-105">Οι συναλλαγές με πιστωτική κάρτα που σχετίζονται με έξοδα μπορούν να ρυθμιστούν με τρόπο ώστε να εισάγονται αυτόματα σε επαναλαμβανόμενο χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="cfa2d-106">Εναλλακτικά, οι συναλλαγές μπορούν να εισαχθούν με μη αυτόματο τρόπο, όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="cfa2d-107">Οι συναλλαγές με πιστωτικές κάρτες εισάγονται μέσω της οντότητας Δεδομένων συναλλαγών με πιστωτικές κάρτες.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="cfa2d-108">Εισαγωγή συναλλαγών με πιστωτικές κάρτες</span><span class="sxs-lookup"><span data-stu-id="cfa2d-108">Import credit card transactions</span></span>

<span data-ttu-id="cfa2d-109">Για την εισαγωγή συναλλαγών με πιστωτική κάρτα, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="cfa2d-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="cfa2d-110">Στη σελίδα **Συναλλαγές με πιστωτικές κάρτες**, επιλέξτε **Εισαγωγή συναλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="cfa2d-111">Εάν ανοίγετε τη διαχείριση δεδομένων για πρώτη φορά, το σύστημα πρέπει να ενημερώσει τη λίστα οντοτήτων δεδομένων πριν να μπορέσετε να συνεχίσετε.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="cfa2d-112">Στο πεδίο **Όνομα**, εισαγάγετε μια μοναδική περιγραφή για την εργασία εισαγωγής.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="cfa2d-113">Στο πεδίο **Μορφή δεδομένων προέλευσης**, επιλέξτε τη μορφή του αρχείου που περιέχει τις συναλλαγές με πιστωτικές κάρτες προς εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="cfa2d-114">Επιλέξτε **Αποστολή** και, στη συνέχεια, εντοπίστε και επιλέξτε το αρχείο προς εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="cfa2d-115">Μετά την αποστολή του αρχείου, επικυρώστε την αντιστοίχιση του αρχείου συναλλαγών με την πιστωτική κάρτα και τις στήλες της οντότητας Δεδομένων συναλλαγών με πιστωτικές κάρτες επιλέγοντας τη σύνδεση **Προβολή χάρτη** στο πλακίδιο.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="cfa2d-116">Εάν υπάρχουν σφάλματα αντιστοίχισης ή εάν πρέπει να αλλάξετε την αντιστοίχιση, πραγματοποιήστε τις αλλαγές αντιστοίχισης είτε από την καρτέλα **Απεικόνιση αντιστοίχισης** είτε από την καρτέλα **Λεπτομέρειες αντιστοίχισης**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="cfa2d-117">Για να αυτοματοποιήσετε τις συναλλαγές με πιστωτικές κάρτες, επιλέξτε **Δημιουργία επαναλαμβανόμενων εργασιών δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="cfa2d-118">Στη συνέχεια, μπορείτε να ορίσετε την περιοδικότητα που καθορίζει τη συχνότητα με την οποία θα πρέπει να εισαχθούν οι συναλλαγές με πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="cfa2d-119">Όταν ολοκληρώσετε, επιλέξτε **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="cfa2d-120">Για να εισαγάγετε τώρα το επιλεγμένο αρχείο , επιλέξτε **Εισαγωγή**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="cfa2d-121">Εάν προκύψουν σφάλματα κατά την εισαγωγή, μπορείτε να προβάλετε το αρχείοπ καταγραφής εκτέλεσης ή τα δεδομένα προεργασίας για να δείτε τα σφάλματα που πρέπει να διορθώσετε, ώστε να εξασφαλίσετε μια επιτυχή εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="cfa2d-122">Εάν θέλετε να εισαγάγετε περισσότερες από μία μορφές αρχείων, πρέπει να δημιουργήσετε ξεχωριστές εργασίες εισαγωγής για κάθε τύπο μορφής.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="cfa2d-123">Εκχωρήστε εκ νέου τις συναλλαγές με πιστωτικές κάρτες για τους εργαζομένους που έχουν απομακρυνθεί</span><span class="sxs-lookup"><span data-stu-id="cfa2d-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="cfa2d-124">Μετά τον τερματισμό μιας καρτέλας υπαλλήλου, ο λογαριασμός Active Directory Domain Services (AD DS) του υπαλλήλου απενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="cfa2d-125">Ωστόσο, ενδέχεται να υπάρχουν ενεργές συναλλαγές με πιστωτικές κάρτες που θα πρέπει ακόμα να χρεωθούν και να καταβληθούν.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="cfa2d-126">Στη σελίδα **Συναλλαγές με πιστωτική κάρτα**, μπορείτε να αναθέσετε εκ νέου τον υπάλληλο σε οποιαδήποτε συναλλαγή με πιστωτική κάρτα, όπου ο συσχετισμένος υπάλληλος έχει τερματιστεί.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="cfa2d-127">Επιλέξτε μία ή περισσότερες συναλλαγές με πιστωτικές κάρτες και, στη συνέχεια, επιλέξτε **Ανάθεση εκ νέου συναλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="cfa2d-128">Στη συνέχεια, μπορείτε να επιλέξετε άλλο υπάλληλο στον οποίο θα αναθέσετε τις συναλλαγές με πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="cfa2d-129">Αφού εκχωρηθούν οι συναλλαγές με πιστωτική κάρτα, μπορούν να επιλεγούν για μια αναφορά εξόδων και να πληρωθούν μέσω της συνηθισμένης διαδικασίας για την πληρωμή της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="cfa2d-130">Διαγραφή συναλλαγών με πιστωτική κάρτα</span><span class="sxs-lookup"><span data-stu-id="cfa2d-130">Delete credit card transactions</span></span> 

<span data-ttu-id="cfa2d-131">Ορισμένες φορές, μετά την εισαγωγή των συναλλαγών με πιστωτική κάρτα, ενδέχεται να χρειάζεται να διαγραφούν ορισμένες συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="cfa2d-132">Αυτό ενδέχεται να συμβαίνει επειδή οι συναλλαγές είναι διπλότυπες ή επειδή τα δεδομένα ενδεχομένως να μην είναι ακριβή.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="cfa2d-133">Οι διαχειριστές μπορούν να χρησιμοποιήσουν τη δυνατότητα **Διαγραφή συναλλαγών με πιστωτική κάρτα** για να επιλέξουν και να διαγράψουν συναλλαγές με πιστωτικές κάρτες που **δεν επισυνάπτονται** σε μια αναφορά δαπανών.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="cfa2d-134">Μετάβαση στην επιλογή **Περιοδικές εργασίες** > **Διαγραφή συναλλαγών με πιστωτική κάρτα**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="cfa2d-135">Επιλέξτε **Φίλτρο** και παράσχετε πληροφορίες για τον προσδιορισμό των καρτελών που θα συμπεριληφθούν.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="cfa2d-136">Για να διαγράψετε τις καρτέλες, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="cfa2d-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
