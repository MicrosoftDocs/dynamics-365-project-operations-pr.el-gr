---
title: Ρύθμιση ροών εργασιών για Διαχείριση εξόδων
description: Μπορείτε να δημιουργήσετε μια διεργασία ροής εργασιών που χρησιμοποιείται για την αναθεώρηση και την έγκριση εγγράφων ταξιδιών και εξόδων.
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
ms.openlocfilehash: af6463b07e282ae1ff6aa7dc1a540ff7c8cc318a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127698"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="80d21-103">Ρύθμιση ροών εργασιών για Διαχείριση εξόδων</span><span class="sxs-lookup"><span data-stu-id="80d21-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="80d21-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="80d21-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="80d21-105">Μπορείτε να δημιουργήσετε μια διεργασία ροής εργασιών για την αναθεώρηση και την έγκριση εγγράφων ταξιδιών και εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="80d21-106">Μπορείτε να ορίσετε ροές εργασιών για αναφορές εξόδων, αιτήσεις για ταξίδια και αιτήσεις προκαταβολής μετρητών.</span><span class="sxs-lookup"><span data-stu-id="80d21-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="80d21-107">Μια ροή εργασιών αντιπροσωπεύει μια επιχειρηματική διεργασία και καθορίζει τον τρόπο με τον οποίο το έγγραφο ρέει μέσω του συστήματος.</span><span class="sxs-lookup"><span data-stu-id="80d21-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="80d21-108">Η ροή εργασιών υποδεικνύει επίσης ποιος πρέπει να ολοκληρώσει μια εργασία ή να εγκρίνει ένα έγγραφο.</span><span class="sxs-lookup"><span data-stu-id="80d21-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="80d21-109">Υπάρχουν πολλά πλεονεκτήματα από τη χρήση του συστήματος ροής εργασιών στον οργανισμό σας:</span><span class="sxs-lookup"><span data-stu-id="80d21-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="80d21-110">**Συνεπείς διεργασίες**: Μπορείτε να καθορίσετε τη διεργασία έγκρισης για συγκεκριμένα έγγραφα, όπως τις αιτήσεις αγορών και τις αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="80d21-111">Η χρήση του συστήματος ροής εργασιών σάς βοηθάει να διασφαλίσετε ότι η επεξεργασία και η έγκριση των εγγράφων γίνεται με συνεκτικό και αποτελεσματικό τρόπο.</span><span class="sxs-lookup"><span data-stu-id="80d21-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="80d21-112">**Διαφάνεια διεργασίας**: Μπορείτε να παρακολουθήσετε την κατάσταση, το ιστορικό και τους δείκτες επιδόσεων μιας συγκεκριμένης παρουσίας ροής εργασιών.</span><span class="sxs-lookup"><span data-stu-id="80d21-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="80d21-113">Με αυτόν τον τρόπο μπορείτε να καθορίσετε θα πρέπει να γίνουν αλλαγές στη ροή εργασιών για τη βελτίωση της αποτελεσματικότητας.</span><span class="sxs-lookup"><span data-stu-id="80d21-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="80d21-114">**Κεντρική λίστα εργασιών**: Οι χρήστες μπορούν να προβάλουν μια κεντρική λίστα εργασιών για να προβάλουν τις εργασίες και τις εγκρίσεις της ροής εργασίας που τους έχουν ανατεθεί.</span><span class="sxs-lookup"><span data-stu-id="80d21-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="80d21-115">Τύποι ροής εργασιών</span><span class="sxs-lookup"><span data-stu-id="80d21-115">Workflow types</span></span>

<span data-ttu-id="80d21-116">Ο παρακάτω πίνακας εμφανίζει τους τύπους ροών εργασιών που μπορείτε να δημιουργήσετε στη **Διαχείριση εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="80d21-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="80d21-117"><strong>Τύπος</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="80d21-118"><strong>Χρησιμοποιήστε αυτόν τον τύπο για να</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="80d21-119"><strong>Αυτόματη έγκριση αναφορών εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="80d21-120">Δημιουργήστε ροές εργασιών έγκρισης για αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="80d21-121"><strong>Αυτόματη καταχώρηση αναφορών εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="80d21-122">Δημιουργήστε αυτόματες ροές εργασιών καταχώρησης για αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="80d21-123"><strong>Στοιχείο γραμμής εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="80d21-124">Δημιουργήστε ροές εργασιών έγκρισης για στοιχεία γραμμής σε αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="80d21-125"><strong>Αυτόματη καταχώρηση στοιχείων γραμμής εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="80d21-126">Δημιουργήστε ροές εργασιών αυτόματης καταχώρησης για στοιχεία γραμμής σε αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="80d21-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="80d21-127"><strong>Ταξιδιωτική αναπλήρωση</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="80d21-128">Δημιουργήστε ροές εργασιών έγκρισης για τις αιτήματα ταξιδίων.</span><span class="sxs-lookup"><span data-stu-id="80d21-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="80d21-129"><strong>Αίτημα προκαταβολής</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="80d21-130">Δημιουργήστε ροές εργασιών έγκρισης για αιτήσεις προκαταβολής μετρητών.</span><span class="sxs-lookup"><span data-stu-id="80d21-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="80d21-131"><strong>Επιστροφή φόρου ΦΠΑ</strong></span><span class="sxs-lookup"><span data-stu-id="80d21-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="80d21-132">Δημιουργήστε ροές εργασιών έγκρισης για την επιστροφή του φόρου προστιθέμενης αξίας (ΦΠΑ).</span><span class="sxs-lookup"><span data-stu-id="80d21-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |
