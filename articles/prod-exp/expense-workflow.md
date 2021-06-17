---
title: Ροή εργασίας διαχείρισης εξόδων
description: Αυτό το θέμα περιγράφει τον τρόπο με τον οποίο μπορείτε να χρησιμοποιήσετε το σύστημα ροής εργασίας στο Microsoft Dynamics 365 Finance, για να ρυθμίσετε μια διαδικασία αναθεώρησης για τις αναφορές εξόδων στη διαχείριση εξόδων.
author: ShylaThompson
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 51ac2712f62d5c5d85b21c0ea929517ccb893bca
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005206"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="af183-103">Ροή εργασίας διαχείρισης εξόδων</span><span class="sxs-lookup"><span data-stu-id="af183-103">Expense management workflow</span></span>

<span data-ttu-id="af183-104">Μπορείτε να χρησιμοποιήσετε το σύστημα ροής εργασίας για να ρυθμίσετε μια διαδικασία αναθεώρησης για τις αναφορές εξόδων στη διαχείριση εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="af183-105">Μπορείτε να δημιουργήσετε μια ροή εργασιών που χρησιμοποιεί τα ακόλουθα κριτήρια για να προσδιορίσει ποιος εγκρίνει τις αναφορές εξόδων:</span><span class="sxs-lookup"><span data-stu-id="af183-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="af183-106">Η ιεραρχία αναφοράς υπαλλήλων και τα προκαθορισμένα όρια έγκρισης</span><span class="sxs-lookup"><span data-stu-id="af183-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="af183-107">Έγκριση πολλαπλών επιπέδων που υποστηρίζει προσωρινούς υπεύθυνους έγκρισης και έναν τελικό υπεύθυνο έγκρισης</span><span class="sxs-lookup"><span data-stu-id="af183-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="af183-108">Οικονομικές διαστάσεις και υπευθυνότητα έργου</span><span class="sxs-lookup"><span data-stu-id="af183-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="af183-109">Ανάθεση σε συγκεκριμένους χρήστες ή ομάδες χρηστών</span><span class="sxs-lookup"><span data-stu-id="af183-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="af183-110">Είναι δυνατή η δημιουργία εγκρίσεων ροής εργασιών για αναφορές εξόδων, αιτήσεις ταξιδίων, προκαταβολές μετρητών και επιστροφή φόρου προστιθέμενης αξίας (ΦΠΑ).</span><span class="sxs-lookup"><span data-stu-id="af183-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="af183-111">**Παράδειγμα**</span><span class="sxs-lookup"><span data-stu-id="af183-111">**Example**</span></span>

<span data-ttu-id="af183-112">Η παρακάτω διεργασία αποτελεί παράδειγμα της ροής εργασιών διαχείρισης εξόδων για μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="af183-113">Ένας εργαζόμενος δημιουργεί και αποθηκεύει μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="af183-114">Ο υπάλληλος υποβάλλει την αναφορά εξόδων για έγκριση.</span><span class="sxs-lookup"><span data-stu-id="af183-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="af183-115">Ο υπεύθυνος έγκρισης προσδιορίζεται με βάση τους κανόνες που ορίστηκαν κατά τη ρύθμιση της ροής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="af183-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="af183-116">Ο υπεύθυνος έγκρισης λαμβάνει μια ειδοποίηση ότι μια αναφορά εξόδων είναι έτοιμη για έγκριση.</span><span class="sxs-lookup"><span data-stu-id="af183-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="af183-117">Ο υπεύθυνος έγκρισης εξετάζει την αναφορά εξόδων και επιβεβαιώνει ότι πληρούνται οι ακόλουθες συνθήκες:</span><span class="sxs-lookup"><span data-stu-id="af183-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="af183-118">Οι δαπάνες δεν παραβιάζουν καμία πολιτική δαπανών.</span><span class="sxs-lookup"><span data-stu-id="af183-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="af183-119">Εάν μια δαπάνη παραβιάσει μια πολιτική, ο υπεύθυνος έγκρισης επιβεβαιώνει ότι η αναφορά εξόδων περιλαμβάνει μια έγκυρη επιχειρηματική αιτιολόγηση.</span><span class="sxs-lookup"><span data-stu-id="af183-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="af183-120">Η ηλεκτρονική απόδειξη επισυνάπτεται στην αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="af183-121">Ο υπεύθυνος έγκρισης εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="af183-122">Η αναφορά εξόδων εκχωρείται στο συντονιστή πληρωτέων λογαριασμών για καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="af183-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="af183-123">Θα συμβεί ένα από τα παρακάτω βήματα, ανάλογα με το αν έχει ρυθμιστεί αυτόματη καταχώρηση:</span><span class="sxs-lookup"><span data-stu-id="af183-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="af183-124">Εάν έχει ρυθμιστεί η αυτόματη καταχώρηση, γίνεται επεξεργασία της αναφοράς εξόδων για πληρωμή και ενημερώνεται η κατάσταση της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="af183-125">Εάν η αυτόματη καταχώρηση δεν έχει ρυθμιστεί, ο συντονιστής πληρωτέων λογαριασμών επιβεβαιώνει ότι έχουν υποβληθεί όλες οι αρχικές αποδείξεις και ότι οι αποδείξεις ευθυγραμμίζονται με τα έξοδα της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="af183-126">Όλοι οι κωδικοί φόρων που καταχωρούνται στην αναφορά εξόδων πρέπει επίσης να επαληθευτούν ως σωστοί.</span><span class="sxs-lookup"><span data-stu-id="af183-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="af183-127">Μετά την επαλήθευση αυτών των απαιτήσεων, καταχωρείται η αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="af183-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="af183-128">Αφού καταχωρηθεί η αναφορά εξόδων, η πληρωμή έχει εγκριθεί για την αναφορά εξόδων και ο εργαζόμενος αποζημιώνεται.</span><span class="sxs-lookup"><span data-stu-id="af183-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]