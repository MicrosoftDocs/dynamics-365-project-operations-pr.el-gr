---
title: Εισαγωγή και διατήρηση συναλλαγών με πιστωτικές κάρτες
description: Αυτό το θέμα επεξηγεί τον τρόπο εισαγωγής και διατήρησης των συναλλαγών με πιστωτικές κάρτες που σχετίζονται με έξοδα. Αυτές οι συναλλαγές μπορούν να ρυθμιστούν έτσι ώστε να εισαγάγονται αυτόματα σε ένα επαναλαμβανόμενο χρονοδιάγραμμα ή μπορούν να εισαχθούν με μη αυτόματο τρόπο, όπως απαιτείται.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: df5c6bce8a534f4f8b1872e2bd5cc8a58ef11189
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271578"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="735eb-104">Εισαγωγή και διατήρηση συναλλαγών με πιστωτικές κάρτες</span><span class="sxs-lookup"><span data-stu-id="735eb-104">Import and maintain credit card transactions</span></span>

<span data-ttu-id="735eb-105">Οι συναλλαγές με πιστωτική κάρτα που σχετίζονται με έξοδα μπορούν να ρυθμιστούν με τρόπο ώστε να εισάγονται αυτόματα σε επαναλαμβανόμενο χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="735eb-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="735eb-106">Εναλλακτικά, οι συναλλαγές μπορούν να εισαχθούν με μη αυτόματο τρόπο, όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="735eb-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="735eb-107">Οι συναλλαγές με πιστωτικές κάρτες εισάγονται μέσω της οντότητας Δεδομένων συναλλαγών με πιστωτικές κάρτες.</span><span class="sxs-lookup"><span data-stu-id="735eb-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="735eb-108">Για περισσότερες πληροφορίες σχετικά με τις οντότητες δεδομένων, ανατρέξτε στο θέμα [Οντότητες δεδομένων](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span><span class="sxs-lookup"><span data-stu-id="735eb-108">For more information about data entities, see [Data entities](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="735eb-109">Εισαγωγή συναλλαγών με πιστωτικές κάρτες</span><span class="sxs-lookup"><span data-stu-id="735eb-109">Import credit card transactions</span></span>

1. <span data-ttu-id="735eb-110">Στη σελίδα **Συναλλαγές με πιστωτικές κάρτες**, επιλέξτε **Εισαγωγή συναλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="735eb-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="735eb-111">Εάν ανοίγετε τη διαχείριση δεδομένων για πρώτη φορά, το σύστημα πρέπει να ενημερώσει τη λίστα οντοτήτων δεδομένων πριν να μπορέσετε να συνεχίσετε.</span><span class="sxs-lookup"><span data-stu-id="735eb-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="735eb-112">Στο πεδίο **Όνομα**, εισαγάγετε μια μοναδική περιγραφή της εργασίας εισαγωγής.</span><span class="sxs-lookup"><span data-stu-id="735eb-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="735eb-113">Στο πεδίο **Μορφή δεδομένων προέλευσης**, επιλέξτε τη μορφή του αρχείου που περιέχει τις συναλλαγές με πιστωτικές κάρτες προς εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="735eb-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="735eb-114">Επιλέξτε **Αποστολή** και, στη συνέχεια, εντοπίστε και επιλέξτε το αρχείο προς εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="735eb-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="735eb-115">Μετά την αποστολή του αρχείου, επικυρώστε την αντιστοίχιση του αρχείου συναλλαγών με την πιστωτική κάρτα και τις στήλες της οντότητας Δεδομένων συναλλαγών με πιστωτικές κάρτες επιλέγοντας τη σύνδεση **Προβολή χάρτη** στο πλακίδιο.</span><span class="sxs-lookup"><span data-stu-id="735eb-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="735eb-116">Εάν υπάρχουν σφάλματα αντιστοίχισης ή εάν πρέπει να αλλάξετε την αντιστοίχιση, πραγματοποιήστε τις αλλαγές αντιστοίχισης είτε από την καρτέλα **Απεικόνιση αντιστοίχισης** είτε από την καρτέλα **Λεπτομέρειες αντιστοίχισης**.</span><span class="sxs-lookup"><span data-stu-id="735eb-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="735eb-117">Για να αυτοματοποιήσετε τις συναλλαγές με πιστωτικές κάρτες, επιλέξτε **Δημιουργία επαναλαμβανόμενων εργασιών δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="735eb-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="735eb-118">Στη συνέχεια, μπορείτε να ορίσετε την περιοδικότητα που καθορίζει τη συχνότητα με την οποία θα πρέπει να εισαχθούν οι συναλλαγές με πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="735eb-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="735eb-119">Όταν ολοκληρώσετε, επιλέξτε **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="735eb-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="735eb-120">Για να εισαγάγετε τώρα το επιλεγμένο αρχείο , επιλέξτε **Εισαγωγή**.</span><span class="sxs-lookup"><span data-stu-id="735eb-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="735eb-121">Εάν παρουσιαστούν σφάλματα κατά την εισαγωγή, μπορείτε να προβάλετε το αρχείο καταγραφής εκτέλεσης ή τα δεδομένα δημιουργίας σταδίων για να δείτε τα σφάλματα που πρέπει να διορθώσετε για να εξασφαλίσετε την επιτυχή εισαγωγή.</span><span class="sxs-lookup"><span data-stu-id="735eb-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="735eb-122">Εάν πρέπει να εισαγάγετε περισσότερες από μία μορφές αρχείων, πρέπει να δημιουργήσετε ξεχωριστές εργασίες εισαγωγής για κάθε τύπο μορφής.</span><span class="sxs-lookup"><span data-stu-id="735eb-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="735eb-123">Εκχωρήστε εκ νέου τις συναλλαγές με πιστωτικές κάρτες για τους εργαζομένους που έχουν απομακρυνθεί</span><span class="sxs-lookup"><span data-stu-id="735eb-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="735eb-124">Μετά τον τερματισμό μιας καρτέλας υπαλλήλου, ο λογαριασμός Active Directory Domain Services (AD DS) του υπαλλήλου απενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="735eb-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="735eb-125">Ωστόσο, ενδέχεται να υπάρχουν ενεργές συναλλαγές με πιστωτικές κάρτες που θα πρέπει ακόμα να χρεωθούν και να καταβληθούν.</span><span class="sxs-lookup"><span data-stu-id="735eb-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="735eb-126">Από τη σελίδα **Συναλλαγές με πιστωτική κάρτα**, μπορείτε να αναθέσετε εκ νέου τον εργαζόμενο για κάθε συναλλαγή με πιστωτική κάρτα, στην οποία συσχετισμένος εργαζόμενος έχει απομακρυνθεί.</span><span class="sxs-lookup"><span data-stu-id="735eb-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="735eb-127">Επιλέξτε μία ή περισσότερες συναλλαγές με πιστωτικές κάρτες και, στη συνέχεια, επιλέξτε **Ανάθεση εκ νέου συναλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="735eb-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="735eb-128">Στη συνέχεια, μπορείτε να επιλέξετε άλλο υπάλληλο στον οποίο θα αναθέσετε τις συναλλαγές με πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="735eb-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="735eb-129">Αφού εκχωρηθούν οι συναλλαγές με πιστωτική κάρτα, μπορούν να επιλεγούν για μια αναφορά εξόδων και να πληρωθούν μέσω της συνηθισμένης διαδικασίας για την πληρωμή της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="735eb-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]