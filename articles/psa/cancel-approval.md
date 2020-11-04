---
title: Ακύρωση προηγούμενων εγκεκριμένων καταχωρήσεων χρόνου και εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ακύρωσης μιας εγκεκριμένης μιας συναλλαγής χρόνου και δαπάνης έργου.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0ea816040570cc8f6ddf3c5ec8a74ac092fc68b2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077091"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="bf3b3-103">Ακύρωση προηγούμενων εγκεκριμένων καταχωρήσεων χρόνου ή εξόδων</span><span class="sxs-lookup"><span data-stu-id="bf3b3-103">Cancel previously approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="bf3b3-104">Στην πιο πρόσφατη έκδοση του Dynamics 365 Project Service Automation, οι υπεύθυνοι έγκρισης μπορούν να ακυρώσουν τις καταχωρήσεις χρόνου ή εξόδων που εγκρίθηκαν προηγουμένως.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="bf3b3-105">Ακύρωση προηγούμενης εγκεκριμένης καταχώρισης χρόνου ή εξόδων</span><span class="sxs-lookup"><span data-stu-id="bf3b3-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="bf3b3-106">Ακολουθήστε τα παρακάτω βήματα για να ακυρώσετε μια ήδη εγκεκριμένη καταχώρηση ώρας ή εξόδων.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="bf3b3-107">Μεταβείτε στα στοιχεία **Έργα** \> **Οι εργασίες μου** \> **Εγκρίσεις**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="bf3b3-108">Στη σελίδα λίστας **Εγκρίσεις** , αλλάξτε την προβολή σε **Οι προηγούμενες εγκρίσεις μου**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="bf3b3-109">Εμφανίζεται μια λίστα με τις καταχωρήσεις χρόνου και εξόδων που εγκρίνατε ήδη.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="bf3b3-110">Επιλέξτε μία ή περισσότερες καταχωρήσεις και, στη συνέχεια, επιλέξτε **Ακύρωση έγκρισης**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="bf3b3-111">Εμφανίζεται ένα μήνυμα προειδοποίησης.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-111">You receive a warning message.</span></span>
4. <span data-ttu-id="bf3b3-112">Για να ακυρώσετε την έγκριση πατήστε **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="bf3b3-113">Κατανόηση της επίπτωσης της ακύρωσης μιας έγκρισης καταχώρισης χρόνου ή εξόδων</span><span class="sxs-lookup"><span data-stu-id="bf3b3-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="bf3b3-114">Όταν ακυρώνεται μια έγκριση, υπάρχει τόσο επιχειρησιακή επίπτωση όσο και οικονομικός αντίκτυπος.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="bf3b3-115">Επιχειρησιακή επίπτωση</span><span class="sxs-lookup"><span data-stu-id="bf3b3-115">Operational impact</span></span>

<span data-ttu-id="bf3b3-116">Από την πλευρά της λειτουργίας, όταν μια έγκριση ακυρώνεται, γίνεται επαναφορά της κατάστασης της καρτέλας σε **Προσχέδιο** και η έγκριση δεν εμφανίζεται πλέον στην προβολή **Οι προηγούμενες εγκρίσεις μου**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft** , and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="bf3b3-117">Αντίθετα, η ακυρωμένη έγκριση εμφανίζεται είτε στην προβολή **Καταχωρίσεις ώρας προς έγκριση** ή στην προβολή **Καταχωρίσεις εξόδων προς έγκριση** ανάλογα με το αν ήταν μια καταχώρηση χρόνου ή μια καταχώρηση εξόδων.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="bf3b3-118">Επιπλέον, η κατάσταση της σχετικής καταχώρισης ώρας ή εξόδων αλλάζει σε **Υποβλήθηκε** ", έτσι ώστε η σχετική καταχώριση να είναι συνεπής με εγκρίσεις σε κατάσταση **Προσχέδιο**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-118">Additionally, the status of the related time or expense entry is changed to **Submitted** , so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="bf3b3-119">Ως υπεύθυνος έγκρισης, μπορείτε να επεξεργαστείτε ορισμένα από τα πεδία μιας έγκρισης με κατάσταση **Προσχέδιο**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="bf3b3-120">Αυτά τα πεδία περιλαμβάνουν **Τύπος χρέωσης** και **Τύπος χρέωσης για καταχωρίσεις ώρας**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="bf3b3-121">Αφού κάνετε τις αλλαγές, μπορείτε να εγκρίνετε εκ νέου την καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="bf3b3-122">Εναλλακτικά, μπορείτε να απορρίψετε την καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="bf3b3-123">Εάν απορρίψετε την έγκριση μιας καταχώρησης χρόνου, η κατάσταση της εγγραφής αλλάζει σε **Επιστράφηκε**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="bf3b3-124">Εάν απορρίψετε την έγκριση μιας καταχώρησης εξόδων, η κατάσταση της εγγραφής αλλάζει σε **Απορρίφθηκε**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="bf3b3-125">Λειτουργικά, τόσο οι επιστρεφόμενες όσο και οι καταχωρίσεις που απορρίφθηκαν συμμορφώνονται με μια καταχώριση σε κατάσταση **Προσχέδιο**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="bf3b3-126">Ένα μέλος της ομάδας έργου μπορεί είτε να κάνει οποιεσδήποτε απαιτούμενες αλλαγές στην καταχώρηση και, στη συνέχεια, να την υποβάλει εκ νέου για έγκριση, είτε να διαγράψει την καταχώρηση εξ ολοκλήρου.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="bf3b3-127">Οικονομικές επιπτώσεις</span><span class="sxs-lookup"><span data-stu-id="bf3b3-127">Financial impact</span></span>

<span data-ttu-id="bf3b3-128">Ένα έργο επηρεάζεται επίσης οικονομικά όταν ακυρώνεται μια έγκριση.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="bf3b3-129">Πρώτα, τα αντίστοιχα πραγματικά στοιχεία για το κόστος και τις πωλήσεις ενημερώνονται με τον ακόλουθο τρόπο:</span><span class="sxs-lookup"><span data-stu-id="bf3b3-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="bf3b3-130">Η κατάσταση προσαρμογής ορίζεται σε **Προσαρμόστηκε**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="bf3b3-131">Η κατάσταση τιμολόγησης ορίστηκε σε **Ακυρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="bf3b3-132">Στη συνέχεια, δημιουργούνται αντίστροφες καταχωρήσεις στον πίνακα πραγματικών τιμών.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="bf3b3-133">Για να δημιουργήσετε αντίστροφες καταχωρήσεις, το σύστημα αντιγράφει τις τιμές των πεδίων από τις αρχικές πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="bf3b3-134">Οι μόνες τιμές που δεν αντιγράφονται είναι οι τιμές ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="bf3b3-135">Αυτές οι τιμές αντιστρέφονται αντί για αυτό.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-135">These values are reversed instead.</span></span> <span data-ttu-id="bf3b3-136">Τα αντίστροφα πραγματικά στοιχεία δημιουργούνται τόσο για το **Κόστος** όσο και τις **Μη τιμολογημένες πωλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="bf3b3-137">Το πεδίο **Κατάσταση προσαρμογής** στις αντίστροφες πραγματικές τιμές έχει οριστεί σε **Μη προσαρμόσιμο** και το πεδίο κατάστασης τιμολόγησης έχει οριστεί σε **Ακυρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable** , and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="bf3b3-138">Αφού γίνουν αυτές οι αλλαγές, οι καταγεγραμμένες δαπάνες του έργου και η λίστα εκκρεμοτήτων εσόδων δεν θα αντιπροσωπεύουν πλέον τα ποσά που αντιπροσωπεύουν αυτές οι πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="bf3b3-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>
