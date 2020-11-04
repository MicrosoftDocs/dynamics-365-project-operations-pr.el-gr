---
title: Δημιουργία και επιβεβαίωση Ημερολογίων διορθώσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας και επιβεβαίωσης ενός ημερολογίου διορθώσεων.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 855593df1ea14827f06961dda5b4becd2fa75c18
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076913"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="31ee7-103">Δημιουργία και επιβεβαίωση Ημερολογίων διορθώσεων</span><span class="sxs-lookup"><span data-stu-id="31ee7-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="31ee7-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="31ee7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="31ee7-105">Περιστασιακά, μια καταχώρηση ώρας ή εξόδων μπορεί να καταχωρηθεί εσφαλμένα.</span><span class="sxs-lookup"><span data-stu-id="31ee7-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="31ee7-106">Για παράδειγμα, ένας σύμβουλος μπορεί να επιλέξει τη λανθασμένη ημερομηνία κατά τη δημιουργία μιας καταχώρησης ώρας ή μπορεί να αλλάξει τη θέση των αριθμών κατά την εισαγωγή ενός εξόδου.</span><span class="sxs-lookup"><span data-stu-id="31ee7-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="31ee7-107">Εάν ένας σύμβουλος δεν μπορεί να πραγματοποιήσει τις ενημερώσεις στις καταχωρήσεις που υποβλήθηκαν, ένας διαχειριστής μπορεί να διορθώσει απευθείας την καταχώρηση για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="31ee7-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="31ee7-108">Για να ολοκληρώσετε τις διαδικασίες σε αυτό το θέμα, θα χρειαστείτε δικαιώματα διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="31ee7-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="31ee7-109">Σωστές εγκεκριμένες καταχωρήσεις ώρας</span><span class="sxs-lookup"><span data-stu-id="31ee7-109">Correct approved time entries</span></span>     

<span data-ttu-id="31ee7-110">Ολοκληρώστε τα παρακάτω βήματα για να διορθώσετε μεμονωμένες ή πολλαπλές καταχωρήσεις ώρας για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="31ee7-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="31ee7-111">Στην περιοχή **Πωλήσεις** , επιλέξτε **Συναλλαγές** κι, έπειτα, επιλέξτε **Εγκεκριμένη ώρα**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-111">In the **Sales** area, select **Transactions** , and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="31ee7-112">Στη λίστα **Εγκεκριμένη ώρα** , εντοπίστε και επιλέξτε μία ή περισσότερες εγκεκριμένες καταχωρήσεις ώρας για διόρθωση.</span><span class="sxs-lookup"><span data-stu-id="31ee7-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="31ee7-113">Μπορείτε να χρησιμοποιήσετε το φίλτρο για να εντοπίσετε σχετικές καταχωρήσεις.</span><span class="sxs-lookup"><span data-stu-id="31ee7-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="31ee7-114">Για παράδειγμα, μπορεί να φιλτράρετε ένα αναγνωριστικό έργου και να επιλέξετε όλες τις εγκεκριμένες καταχωρήσεις ώρας με αυτό το αναγνωριστικό έργου.</span><span class="sxs-lookup"><span data-stu-id="31ee7-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="31ee7-115">Επιλέξτε **Σωστές καταχωρήσεις**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-115">Select **Correct entries**.</span></span> <span data-ttu-id="31ee7-116">Δημιουργείται αυτόματα ένα νέο ημερολόγιο διορθώσεων, με τον αντιστοιχισμένο τύπο **Διόρθωση ώρας**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="31ee7-117">Οι καταχωρήσεις που επιλέξατε προστίθενται στο ημερολόγιο.</span><span class="sxs-lookup"><span data-stu-id="31ee7-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="31ee7-118">Στη σελίδα **Νέο ημερολόγιο** , εισαγάγετε μια **Περιγραφή** για το ημερολόγιο διορθώσεων κι, έπειτα, επιλέξτε την καρτέλα **Διορθώσεις καταχωρήσεων ώρας**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="31ee7-119">Στην ενότητα **Νέες τιμές για τις καταχωρήσεις ώρας** , ενημερώστε τα πεδία με τις σωστές πληροφορίες, όπου είναι απαραίτητο.</span><span class="sxs-lookup"><span data-stu-id="31ee7-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="31ee7-120">Για παράδειγμα, μπορείτε να αλλάξετε το έργο που έχει ανατεθεί ή τον πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="31ee7-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="31ee7-121">Επιλέξτε **Προεπισκόπηση**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-121">Select **Preview**.</span></span> <span data-ttu-id="31ee7-122">Στο παράθυρο διαλόγου, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="31ee7-123">Στην καρτέλα **Γραμμές ημερολογίου** , μπορείτε να προβάλετε μια λίστα των αρχικών πραγματικών τιμών που σχετίζονται με τις επιλεγμένες καταχωρήσεις ώρας που έχουν αντιστραφεί και τις διορθωμένους αντίστοιχες γραμμές που δημιουργήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="31ee7-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="31ee7-124">Εάν πρέπει να γίνουν πρόσθετες διορθώσεις, επαναλάβετε τα βήματα 5 και 6.</span><span class="sxs-lookup"><span data-stu-id="31ee7-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="31ee7-125">Όλες οι διορθωμένες πραγματικές τιμές θα έχουν τις ίδιες τιμές που επιλέξατε στην ενότητα **Νέες τιμές για καταχωρήσεις ώρας**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="31ee7-126">Εάν οι διορθώσεις εμφανίζονται όπως αναμενόταν, επιλέξτε **Επιβεβαίωση**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="31ee7-127">Στο παράθυρο διαλόγου, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="31ee7-128">Επιστρέψτε στην περιοχή **Πωλήσεις** , επιλέξτε **Έργα** κι, έπειτα, ανοίξτε το έργο για το οποίο μόλις ενημερώσατε τις καταχωρήσεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="31ee7-128">Return to the **Sales** area, select **Projects** , and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="31ee7-129">Στη σελίδα **Έργα** , στην καρτέλα **Πραγματικές τιμές** , προβάλετε τις αλλαγές που πραγματοποιήσατε.</span><span class="sxs-lookup"><span data-stu-id="31ee7-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="31ee7-130">Εάν η καρτέλα **Πραγματικές τιμές** δεν είναι ορατή, επιλέξτε **Σχετικά** > **Πραγματικές τιμές**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="31ee7-131">Στη λίστα **Πραγματική συσχετισμένη προβολή** , μπορείτε να δείτε ότι οι αρχικές καταχωρήσεις ώρας που αντιστράφηκαν παραμένουν στη λίστα, όπως και οι αντίστοιχες διορθωμένες καταχωρήσεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="31ee7-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="31ee7-132">Για παράδειγμα, στο ακόλουθο γραφικό, υπάρχουν δύο στοιχεία γραμμής με ποσότητα 8,00 που περιλαμβάνουν χρεώσεις που παρατίθενται στη στήλη "Ποσό".</span><span class="sxs-lookup"><span data-stu-id="31ee7-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="31ee7-133">Επιπλέον, υπάρχουν δύο στοιχεία γραμμής με ποσότητα - 8,00 που εμφανίζουν τα ποσά που πιστώνονται στη στήλη "Ποσό".</span><span class="sxs-lookup"><span data-stu-id="31ee7-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="31ee7-134">Αυτές οι διορθώσεις φέρνουν την ποσότητα στο μηδέν.</span><span class="sxs-lookup"><span data-stu-id="31ee7-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="31ee7-135">Σωστές εγκεκριμένες καταχωρήσεις εξόδων</span><span class="sxs-lookup"><span data-stu-id="31ee7-135">Correct approved expense entries</span></span>

<span data-ttu-id="31ee7-136">Ολοκληρώστε τα παρακάτω βήματα για να διορθώσετε μία ή περισσότερες καταχωρήσεις εξόδων.</span><span class="sxs-lookup"><span data-stu-id="31ee7-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="31ee7-137">Στην περιοχή **Πωλήσεις** , στο αριστερό παράθυρο περιήγησης, στην περιοχή **Συναλλαγές** , επιλέξτε **Εγκεκριμένα έξοδα**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-137">In the **Sales** area, in the left navigation pane, under **Transactions** , select **Approved Expenses**.</span></span>

2. <span data-ttu-id="31ee7-138">Στη λίστα **Εγκεκριμένα έξοδα** , επιλέξτε το έργο που θέλετε να διορθώσετε και, στη συνέχεια, επιλέξτε **Σωστές καταχωρήσεις**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="31ee7-139">Θα δημιουργηθεί αυτόματα ένα νέο ημερολόγιο διορθώσεων, με τον αντιστοιχισμένο τύπο **Διόρθωση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="31ee7-140">Στη σελίδα **Νέο ημερολόγιο** , καταχωρήστε μια **Περιγραφή** για τη διόρθωση και στην καρτέλα **Διόρθωση εξόδων** , στην ενότητα **Νέες τιμές για έξοδα** , επιλέξτε τα πεδία δεδομένων που θέλετε να διορθώσετε για τις επιλεγμένες γραμμές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="31ee7-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="31ee7-141">Για παράδειγμα, μπορείτε να αναθέσετε το έξοδο σε ένα άλλο **Έργο** ή να διορθώσετε την **Κατηγορία εξόδων** , την **Ημερομηνία εξόδων** ή τον **Πόρο με δυνατότητα κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-141">For example, you can assign the expense to another **Project** , or correct the **Expense Category** , **Expense Date** , or **Bookable Resource**.</span></span>

4. <span data-ttu-id="31ee7-142">Επιλέξτε **Προεπισκόπηση**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-142">Select **Preview**.</span></span> <span data-ttu-id="31ee7-143">Στο παράθυρο διαλόγου, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="31ee7-144">Επιβεβαιώστε τις διορθώσεις στην καρτέλα **Γραμμές ημερολογίου**. Μπορείτε να προβάλετε μια λίστα των αρχικών πραγματικών τιμών που σχετίζονται με τις επιλεγμένες καταχωρήσεις εξόδων που έχουν αντιστραφεί και τις διορθωμένους αντίστοιχες γραμμές που δημιουργήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="31ee7-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="31ee7-145">Εάν οι διορθωμένες τιμές είναι όπως αναμενόταν, επιλέξτε **Επιβεβαίωση**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="31ee7-146">Στο παράθυρο διαλόγου, επιλέξτε **OK.**</span><span class="sxs-lookup"><span data-stu-id="31ee7-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="31ee7-147">Εάν οι τιμές δεν εμφανίζονται όπως αναμενόταν, επιλέξτε **Άκυρο** για να επιστρέψετε στη λίστα **Εγκεκριμένα έξοδα**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="31ee7-148">Επαναλάβετε τα βήματα 2 έως 5.</span><span class="sxs-lookup"><span data-stu-id="31ee7-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="31ee7-149">Οι διορθωμένες πραγματικές τιμές θα έχουν τις ίδιες τιμές που επιλέξατε στην ενότητα **Νέες τιμές για έξοδα**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="31ee7-150">Αφού επιβεβαιώσετε το ημερολόγιο διορθώσεων, μεταβείτε ξανά στο έργο ή τα έργα που ενημερώσατε, για να προβάλετε τις αλλαγές σας.</span><span class="sxs-lookup"><span data-stu-id="31ee7-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="31ee7-151">Στη σελίδα έργου, στην καρτέλα **Πραγματικές τιμές** , εξετάστε την **Πραγματική συσχετισμένη προβολή**.</span><span class="sxs-lookup"><span data-stu-id="31ee7-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="31ee7-152">Οι αρχικές καταχωρήσεις και οι διορθωμένες καταχωρήσεις παρατίθενται.</span><span class="sxs-lookup"><span data-stu-id="31ee7-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="31ee7-153">Στο παρακάτω γραφικό εμφανίζονται τα αρχικά ποσά καταχώρησης εξόδων και τα αντίστοιχα διορθωμένα ποσά καταχώρησης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="31ee7-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 


