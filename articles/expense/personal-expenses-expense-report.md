---
title: Εργασία με προσωπικά έξοδα σε μια αναφορά εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εργασίας με προσωπικές δαπάνες που προκύπτουν από τους υπαλλήλους ενώ ταξιδεύουν για επαγγελματικούς σκοπούς.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025684"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="52f2b-103">Εργασία με προσωπικά έξοδα σε μια αναφορά εξόδων</span><span class="sxs-lookup"><span data-stu-id="52f2b-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="52f2b-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="52f2b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="52f2b-105">Κατά τη διάρκεια των επαγγελματικών ταξιδιών, ένας υπάλληλος ενδέχεται να χρεώσει προσωπικές δαπάνες στην εταιρική πιστωτική κάρτα του.</span><span class="sxs-lookup"><span data-stu-id="52f2b-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="52f2b-106">Αν δεν έχει οριστεί διαδικασία για τον χειρισμό των προσωπικών δαπανών, η διαδικασία έγκρισης της αναφοράς δαπανών ενδέχεται να προκαλέσει αναστάτωση όταν ένας υπάλληλος υποβάλλει την αναλυτική αναφορά δαπανών του.</span><span class="sxs-lookup"><span data-stu-id="52f2b-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="52f2b-107">Μπορείτε να χρησιμοποιήσετε δύο μεθόδους για να εργαστείτε με τις προσωπικές δαπάνες ενός υπαλλήλου:</span><span class="sxs-lookup"><span data-stu-id="52f2b-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="52f2b-108">**Πληρωμή από υπάλληλο**: Ο οργανισμός σας δεν πληρώνει προσωπικά έξοδα που εμφανίζονται στο λογαριασμό για την εταιρική πιστωτική κάρτα.</span><span class="sxs-lookup"><span data-stu-id="52f2b-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="52f2b-109">Αντ' αυτού, ο υπάλληλος πληρώνει απευθείας τον προμηθευτή πιστωτικής κάρτας για τις δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="52f2b-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="52f2b-110">**Πληρώθηκε από την εταιρεία**: Ο οργανισμός σας πληρώνει τον πλήρη λογαριασμό για την εταιρική πιστωτική κάρτα και, στη συνέχεια, χρεώνει το λογαριασμό του εργαζόμενου για τις προσωπικές δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="52f2b-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="52f2b-111">Μπορείτε να επιλέξετε τη μέθοδο που χρησιμοποιεί ο οργανισμός σας στη σελίδα **Παράμετροι διαχείρισης εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="52f2b-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="52f2b-112">Ενεργοποίηση της συνάρτησης διαίρεσης δαπανών όταν το πεδίο προσωπικού ποσού έχει καθορισμένη τιμή</span><span class="sxs-lookup"><span data-stu-id="52f2b-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="52f2b-113">Η δυνατότητα, **Ενεργοποίηση της συνάρτησης διαίρεσης δαπανών όταν το πεδίο προσωπικού ποσού έχει τιμή που καθορίζεται** εφαρμόζεται μόνο σε αναφορές δαπανών που έχουν εγκριθεί με χρήση ροής εργασιών επιπέδου γραμμής.</span><span class="sxs-lookup"><span data-stu-id="52f2b-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="52f2b-114">Οι αναφορές εγκρίνονται από την επιλογή **Επεξεργασία αναφορών δαπανών** > **Αναφορές δαπανών που έχουν ανατεθεί σε εμένα** > **Άνοιγμα αναφοράς δαπανών**.</span><span class="sxs-lookup"><span data-stu-id="52f2b-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="52f2b-115">Για να ενεργοποιήσετε αυτήν τη δυνατότητα, μεταβείτε στο **Χώροι εργασίας** > **Διαχείριση δυνατοτήτων**, επιλέξτε **Ενεργοποίηση της συνάρτησης διαίρεσης δαπανών, όταν το πεδίο προσωπικού ποσού έχει καθορισμένη τιμή** και, στη συνέχεια, επιλέξτε **Ενεργοποίηση τώρα**.</span><span class="sxs-lookup"><span data-stu-id="52f2b-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="52f2b-116">Όταν είναι ενεργοποιημένη η δυνατότητα, οι γραμμές δαπανών που χρησιμοποιούν αυτήν τη λειτουργικότητα δημιουργούν δύο γραμμές όταν υποβάλλεται η αναφορά.</span><span class="sxs-lookup"><span data-stu-id="52f2b-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="52f2b-117">Δημιουργούνται δύο γραμμές έτσι, ώστε ο υπεύθυνος έγκρισης να μπορεί να εγκρίνει κάθε γραμμή ξεχωριστά.</span><span class="sxs-lookup"><span data-stu-id="52f2b-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
