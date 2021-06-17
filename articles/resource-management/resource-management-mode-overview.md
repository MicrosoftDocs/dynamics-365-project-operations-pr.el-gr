---
title: Επισκόπηση λειτουργιών διαχείρισης πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη λειτουργία διαχείρισης πόρων στο Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94db65a2ddbdc6a7226c70907bcce4c45b4a3923
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000886"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="9dff8-103">Επισκόπηση λειτουργιών διαχείρισης πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-103">Resource management modes overview</span></span>

<span data-ttu-id="9dff8-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="9dff8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9dff8-105">Το Dynamics 365 Project Operations υποστηρίζει δύο λειτουργίες για να εκτελέσετε τη συνολική ροή κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="9dff8-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="9dff8-106">Ο τρόπος διαχείρισης ορίζεται ως παράμετρος έργου και μπορεί να τροποποιηθεί εάν η επιχείρησή σας χρειάζεται αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="9dff8-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="9dff8-107">Κεντρικός τρόπος λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="9dff8-107">Central mode</span></span>
<span data-ttu-id="9dff8-108">Για οργανισμούς που συγκεντρώνουν την ανάθεση για πόρους σε έργα, η κεντρική λειτουργία παρέχει έναν τρόπο ώστε οι διαχειριστές έργου να μπορούν να καθορίσουν τις απαιτήσεις πόρων σε επίπεδο έργου.</span><span class="sxs-lookup"><span data-stu-id="9dff8-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="9dff8-109">Η εκπλήρωση των απαιτήσεων πόρου ανατίθεται σε ένα διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="9dff8-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="9dff8-110">Οι διαχειριστές έργου μπορούν να αποδεχθούν ή να απορρίψουν πόρους που προτείνονται από τον διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="9dff8-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Κεντρικός τρόπος λειτουργίας](./media/resource-management-central.png)

<span data-ttu-id="9dff8-112">Για να διαχειριστείτε τους πόρους με την κεντρική λειτουργία, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="9dff8-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="9dff8-113">Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια εργασία και δημιουργία απαιτήσεων πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9dff8-114">Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="9dff8-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="9dff8-115">Υποβολή μιας αίτησης πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="9dff8-116">Κάλυψη αιτήματος πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="9dff8-117">Αποδοχή ή απόρριψη ενός πόρου έργου που προτείνεται από μια αίτηση πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="9dff8-118">Υβριδική λειτουργία</span><span class="sxs-lookup"><span data-stu-id="9dff8-118">Hybrid mode</span></span>
<span data-ttu-id="9dff8-119">Για οργανισμούς που απαιτούν ευελιξία στην ανάθεση πόρων, η υβριδική λειτουργία παρέχει στους διαχειριστές έργου και στους διαχειριστές πόρων τη δυνατότητα να κάνουν κράτηση πόρων.</span><span class="sxs-lookup"><span data-stu-id="9dff8-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Υβριδική λειτουργία](./media/resource-management-hybrid.png)

<span data-ttu-id="9dff8-121">Εκτός από τη διεργασία κεντρικής λειτουργίας που υποστηρίζεται, ανατρέξτε στα παρακάτω θέματα για να διαχειριστείτε όλες τις άλλες υποστηριζόμενες ροές κρατήσεων στην υβριδική λειτουργία:</span><span class="sxs-lookup"><span data-stu-id="9dff8-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="9dff8-122">Κράτηση πόρου απευθείας σε έργο:</span><span class="sxs-lookup"><span data-stu-id="9dff8-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="9dff8-123">Κράτηση καθορισμένων πόρων με δυνατότητα κράτησης σε μια ομάδα έργου και ανάθεση εργασιών</span><span class="sxs-lookup"><span data-stu-id="9dff8-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="9dff8-124">Κράτηση πόρου από απαίτηση πόρου:</span><span class="sxs-lookup"><span data-stu-id="9dff8-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="9dff8-125">Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια εργασία και δημιουργία απαιτήσεων πόρου</span><span class="sxs-lookup"><span data-stu-id="9dff8-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9dff8-126">Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="9dff8-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]