---
title: Αναφορές εξόδων και πολλαπλοί υπεύθυνοι έγκρισης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις αναφορές εξόδων που απαιτούν έγκριση από περισσότερα από ένα άτομα.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 548673541cee5ce598721f94415c0444995c8325
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076919"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="95d9f-103">Αναφορές εξόδων και πολλαπλοί υπεύθυνοι έγκρισης</span><span class="sxs-lookup"><span data-stu-id="95d9f-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="95d9f-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="95d9f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="95d9f-105">Ανάλογα με τις πολιτικές έγκρισης εξόδων του οργανισμού σας, περισσότερα από ένα άτομα μπορεί να πρέπει να εγκρίνουν μια αναφορά εξόδων που έχει υποβληθεί.</span><span class="sxs-lookup"><span data-stu-id="95d9f-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="95d9f-106">Όταν ρυθμίζετε τη διεργασία ροής εργασιών για έγκριση αναφοράς εξόδων, μπορείτε να προσθέσετε στοιχεία ροής εργασίας που περιλαμβάνουν εργασίες ή βήματα για έναν ή περισσότερους υπεύθυνους έγκρισης αναφορών εξόδων.</span><span class="sxs-lookup"><span data-stu-id="95d9f-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="95d9f-107">Για παράδειγμα, μπορείτε να απαιτήσετε την έγκριση όλων των αναφορών εξόδων από δύο ξεχωριστά άτομα, τον προϊστάμενο του υπαλλήλου που υπέβαλε την αναφορά και τον συντονιστή πληρωτέων λογαριασμών.</span><span class="sxs-lookup"><span data-stu-id="95d9f-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="95d9f-108">Εάν αποφασίσετε να απαιτήσετε πολλούς υπεύθυνους έγκρισης αναφορών εξόδων, μπορείτε να προσθέσετε τα στοιχεία της ροής εργασιών με έναν από τους ακόλουθους τρόπους:</span><span class="sxs-lookup"><span data-stu-id="95d9f-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="95d9f-109">Να προσθέσετε ένα στοιχείο έγκρισης που έχει ένα βήμα.</span><span class="sxs-lookup"><span data-stu-id="95d9f-109">Add one approval element that has one step.</span></span> <span data-ttu-id="95d9f-110">Για παράδειγμα, το βήμα μπορεί να απαιτήσει μια αναφορά εξόδων να ανατεθεί σε μια ομάδα χρηστών και να εγκριθεί από το 50 τοις εκατό των μελών της ομάδας χρηστών.</span><span class="sxs-lookup"><span data-stu-id="95d9f-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="95d9f-111">Να προσθέσετε ένα στοιχείο έγκρισης που έχει πολλά βήματα.</span><span class="sxs-lookup"><span data-stu-id="95d9f-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="95d9f-112">Για παράδειγμα, το στοιχείο έγκρισης μπορεί να έχει τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="95d9f-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="95d9f-113">Ο προϊστάμενος του υπαλλήλου που υπέβαλε την αναφορά εξόδων, την εγκρίνει.</span><span class="sxs-lookup"><span data-stu-id="95d9f-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="95d9f-114">Ο υπάλληλος πληρωτέων λογαριασμών επιβεβαιώνει τις αποδείξεις και τα στοιχεία της αναφοράς εξόδων.</span><span class="sxs-lookup"><span data-stu-id="95d9f-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="95d9f-115">Ο κάτοχος του προϋπολογισμού εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="95d9f-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="95d9f-116">Προσθέστε πολλαπλά στοιχεία έγκρισης, καθένα από τα οποία έχει ένα βήμα.</span><span class="sxs-lookup"><span data-stu-id="95d9f-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="95d9f-117">Για παράδειγμα, μπορείτε να προσθέσετε ένα ξεχωριστό στοιχείο έγκρισης για κάθε ένα από τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="95d9f-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="95d9f-118">Ο προϊστάμενος του υπαλλήλου εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="95d9f-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="95d9f-119">Ο κάτοχος του προϋπολογισμού εγκρίνει την αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="95d9f-119">The budget owner approves the expense report.</span></span>
