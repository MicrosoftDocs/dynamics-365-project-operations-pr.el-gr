---
title: Πολλοί υπεύθυνοι έγκρισης αναφορικά με την αναφορά εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις αναφορές εξόδων που απαιτούν έγκριση από πολλά άτομα.
author: saraschi2
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: c745dda957fab5acc464b9d1c774fcdc783cde40
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005251"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="ad153-103">Πολλοί υπεύθυνοι έγκρισης αναφορικά με την αναφορά εξόδων</span><span class="sxs-lookup"><span data-stu-id="ad153-103">Multiple approvers on an expense report</span></span>

<span data-ttu-id="ad153-104">Ανάλογα με τις πολιτικές έγκρισης εξόδων του οργανισμού σας, περισσότερα από ένα άτομα μπορεί να πρέπει να εγκρίνουν μια αναφορά εξόδων που έχει υποβληθεί από έναν εργαζόμενο.</span><span class="sxs-lookup"><span data-stu-id="ad153-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="ad153-105">Όταν ρυθμίζετε τη διεργασία ροής εργασιών για έγκριση αναφοράς εξόδων, μπορείτε να προσθέσετε στοιχεία ροής εργασίας που περιλαμβάνουν εργασίες ή βήματα για έναν ή περισσότερους υπεύθυνους έγκρισης αναφορών εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ad153-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="ad153-106">Για παράδειγμα, μπορείτε να απαιτήσετε την έγκριση όλων των αναφορών εξόδων πρώτα από τον προϊστάμενο του υπαλλήλου που υπέβαλε την αναφορά και μετά από τον συντονιστή πληρωτέων λογαριασμών.</span><span class="sxs-lookup"><span data-stu-id="ad153-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="ad153-107">Εάν αποφασίσετε να απαιτήσετε πολλούς υπεύθυνους έγκρισης αναφορών εξόδων, μπορείτε να προσθέσετε τα στοιχεία της ροής εργασιών με έναν από τους ακόλουθους τρόπους:</span><span class="sxs-lookup"><span data-stu-id="ad153-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="ad153-108">Να προσθέσετε ένα στοιχείο έγκρισης που έχει ένα βήμα.</span><span class="sxs-lookup"><span data-stu-id="ad153-108">Add one approval element that has one step.</span></span> <span data-ttu-id="ad153-109">Για παράδειγμα, το βήμα μπορεί να απαιτήσει μια αναφορά εξόδων να ανατεθεί σε μια ομάδα χρηστών και να εγκριθεί από το 50 τοις εκατό των μελών της ομάδας χρηστών.</span><span class="sxs-lookup"><span data-stu-id="ad153-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="ad153-110">Να προσθέσετε ένα στοιχείο έγκρισης που έχει πολλά βήματα.</span><span class="sxs-lookup"><span data-stu-id="ad153-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="ad153-111">Για παράδειγμα, το στοιχείο έγκρισης μπορεί να έχει τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="ad153-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="ad153-112">Ο προϊστάμενος του υπαλλήλου που υπέβαλε την αναφορά εξόδων, την εγκρίνει.</span><span class="sxs-lookup"><span data-stu-id="ad153-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="ad153-113">Ο υπάλληλος πληρωτέων λογαριασμών επιβεβαιώνει τις αποδείξεις και τα στοιχεία της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ad153-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="ad153-114">Ο κάτοχος του προϋπολογισμού εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ad153-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="ad153-115">Προσθέστε πολλαπλά στοιχεία έγκρισης, καθένα από τα οποία έχει ένα βήμα.</span><span class="sxs-lookup"><span data-stu-id="ad153-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="ad153-116">Για παράδειγμα, μπορείτε να προσθέσετε ένα ξεχωριστό στοιχείο έγκρισης για κάθε ένα από τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="ad153-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="ad153-117">Ο προϊστάμενος του υπαλλήλου εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ad153-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="ad153-118">Ο κάτοχος του προϋπολογισμού εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="ad153-118">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]