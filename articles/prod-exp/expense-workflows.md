---
title: Ρύθμιση ροών εργασιών διαχείρισης εξόδων
description: Μπορείτε να δημιουργήσετε μια διεργασία ροής εργασιών για την αναθεώρηση και την έγκριση εγγράφων ταξιδιών και εξόδων.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0af23ed2cf172e4c90de72f5db389c349303c039
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077070"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="0cd5b-103">Ρύθμιση ροών εργασιών διαχείρισης εξόδων</span><span class="sxs-lookup"><span data-stu-id="0cd5b-103">Set up Expense management workflows</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="0cd5b-104">Μπορείτε να δημιουργήσετε μια διεργασία ροής εργασιών που χρησιμοποιείται για την αναθεώρηση και την έγκριση εγγράφων ταξιδιών και εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="0cd5b-105">Τα έγγραφα για τα οποία μπορείτε να ορίσετε ροές εργασιών περιλαμβάνουν αναφορές εξόδων, αιτήσεις για ταξίδια και αιτήσεις προκαταβολής μετρητών.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="0cd5b-106">Μια ροή εργασιών αντιπροσωπεύει μια επιχειρηματική διεργασία.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-106">A workflow represents a business process.</span></span> <span data-ttu-id="0cd5b-107">Καθορίζει τον τρόπο με τον οποίο ένα έγγραφο ρέει μέσω του συστήματος και υποδεικνύει ποιος πρέπει να ολοκληρώσει μια εργασία ή να εγκρίνει ένα έγγραφο.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="0cd5b-108">Υπάρχουν πολλά πλεονεκτήματα από τη χρήση του συστήματος ροής εργασιών στον οργανισμό σας:</span><span class="sxs-lookup"><span data-stu-id="0cd5b-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="0cd5b-109">**Συνεπείς διεργασίες** - Μπορείτε να καθορίσετε τη διεργασία έγκρισης για συγκεκριμένα έγγραφα, όπως τις αιτήσεις αγορών και τις αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="0cd5b-110">Η χρήση του συστήματος ροής εργασιών σάς βοηθάει να διασφαλίσετε ότι η επεξεργασία και η έγκριση των εγγράφων γίνεται με συνεκτικό και αποτελεσματικό τρόπο.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="0cd5b-111">Διαφάνεια διεργασίας - Μπορείτε να παρακολουθήσετε την κατάσταση, το ιστορικό και τους δείκτες επιδόσεων μιας συγκεκριμένης παρουσίας ροής εργασιών.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="0cd5b-112">Με αυτόν τον τρόπο μπορείτε να καθορίσετε θα πρέπει να γίνουν αλλαγές στη ροή εργασιών για τη βελτίωση της αποτελεσματικότητας.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="0cd5b-113">Κεντρική λίστα εργασιών - Οι χρήστες μπορούν να προβάλουν μια κεντρική λίστα εργασιών για να προβάλουν τις εργασίες και τις εγκρίσεις της ροής εργασίας που τους έχουν ανατεθεί.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="0cd5b-114">**Οι τύποι των ροών εργασίας που μπορείτε να δημιουργήσετε**</span><span class="sxs-lookup"><span data-stu-id="0cd5b-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="0cd5b-115">Ο παρακάτω πίνακας εμφανίζει τους τύπους ροών εργασιών που μπορείτε να δημιουργήσετε στα **Έξοδα**.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="0cd5b-116"><strong>Τύπος</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="0cd5b-117"><strong>Χρησιμοποιήστε αυτόν τον τύπο για να</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="0cd5b-118"><strong>Κατάσταση εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="0cd5b-119">Δημιουργήστε ροές εργασιών έγκρισης για αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="0cd5b-120"><strong>Αυτόματη καταχώρηση αναφορών εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="0cd5b-121">Δημιουργήστε αυτόματες ροές εργασιών καταχώρησης για αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="0cd5b-122"><strong>Στοιχείο γραμμής εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="0cd5b-123">Δημιουργήστε ροές εργασιών έγκρισης για στοιχεία γραμμής σε αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="0cd5b-124"><strong>Αυτόματη καταχώρηση στοιχείων γραμμής εξόδων</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="0cd5b-125">Δημιουργήστε ροές εργασιών αυτόματης καταχώρησης για στοιχεία γραμμής σε αναφορές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="0cd5b-126"><strong>Ταξιδιωτική αναπλήρωση</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="0cd5b-127">Δημιουργήστε ροές εργασιών έγκρισης για τις αιτήματα ταξιδίων.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="0cd5b-128"><strong>Αίτημα προκαταβολής</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="0cd5b-129">Δημιουργήστε ροές εργασιών έγκρισης για αιτήσεις προκαταβολής μετρητών.</span><span class="sxs-lookup"><span data-stu-id="0cd5b-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="0cd5b-130"><strong>Επιστροφή φόρου ΦΠΑ</strong></span><span class="sxs-lookup"><span data-stu-id="0cd5b-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="0cd5b-131">Δημιουργήστε ροές εργασιών έγκρισης για την επιστροφή του φόρου προστιθέμενης αξίας (ΦΠΑ).</span><span class="sxs-lookup"><span data-stu-id="0cd5b-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |

