---
title: Επισκόπηση λειτουργιών διαχείρισης πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη λειτουργία διαχείρισης πόρων στο Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 872f4f2878f474e16674932f23fe192c6a8de6eb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279453"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="8db71-103">Επισκόπηση λειτουργιών διαχείρισης πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-103">Resource management modes overview</span></span>

<span data-ttu-id="8db71-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="8db71-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="8db71-105">Το Dynamics 365 Project Operations υποστηρίζει δύο λειτουργίες για να εκτελέσετε τη συνολική ροή κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="8db71-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="8db71-106">Ο τρόπος διαχείρισης ορίζεται ως παράμετρος έργου και μπορεί να τροποποιηθεί εάν η επιχείρησή σας χρειάζεται αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="8db71-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="8db71-107">Κεντρικός τρόπος λειτουργίας</span><span class="sxs-lookup"><span data-stu-id="8db71-107">Central mode</span></span>
<span data-ttu-id="8db71-108">Για οργανισμούς που συγκεντρώνουν την ανάθεση για πόρους σε έργα, η κεντρική λειτουργία παρέχει έναν τρόπο ώστε οι διαχειριστές έργου να μπορούν να καθορίσουν τις απαιτήσεις πόρων σε επίπεδο έργου.</span><span class="sxs-lookup"><span data-stu-id="8db71-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="8db71-109">Η εκπλήρωση των απαιτήσεων πόρου ανατίθεται σε ένα διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="8db71-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="8db71-110">Οι διαχειριστές έργου μπορούν να αποδεχθούν ή να απορρίψουν πόρους που προτείνονται από τον διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="8db71-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Κεντρικός τρόπος λειτουργίας](./media/resource-management-central.png)

<span data-ttu-id="8db71-112">Για να διαχειριστείτε τους πόρους με την κεντρική λειτουργία, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="8db71-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="8db71-113">Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια εργασία και δημιουργία απαιτήσεων πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="8db71-114">Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="8db71-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="8db71-115">Υποβολή μιας αίτησης πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="8db71-116">Κάλυψη αιτήματος πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="8db71-117">Αποδοχή ή απόρριψη ενός πόρου έργου που προτείνεται από μια αίτηση πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="8db71-118">Υβριδική λειτουργία</span><span class="sxs-lookup"><span data-stu-id="8db71-118">Hybrid mode</span></span>
<span data-ttu-id="8db71-119">Για οργανισμούς που απαιτούν ευελιξία στην ανάθεση πόρων, η υβριδική λειτουργία παρέχει στους διαχειριστές έργου και στους διαχειριστές πόρων τη δυνατότητα να κάνουν κράτηση πόρων.</span><span class="sxs-lookup"><span data-stu-id="8db71-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Υβριδική λειτουργία](./media/resource-management-hybrid.png)

<span data-ttu-id="8db71-121">Εκτός από τη διεργασία κεντρικής λειτουργίας που υποστηρίζεται, ανατρέξτε στα παρακάτω θέματα για να διαχειριστείτε όλες τις άλλες υποστηριζόμενες ροές κρατήσεων στην υβριδική λειτουργία:</span><span class="sxs-lookup"><span data-stu-id="8db71-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="8db71-122">Κράτηση πόρου απευθείας σε έργο:</span><span class="sxs-lookup"><span data-stu-id="8db71-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="8db71-123">Κράτηση καθορισμένων πόρων με δυνατότητα κράτησης σε μια ομάδα έργου και ανάθεση εργασιών</span><span class="sxs-lookup"><span data-stu-id="8db71-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="8db71-124">Κράτηση πόρου από απαίτηση πόρου:</span><span class="sxs-lookup"><span data-stu-id="8db71-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="8db71-125">Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια εργασία και δημιουργία απαιτήσεων πόρου</span><span class="sxs-lookup"><span data-stu-id="8db71-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="8db71-126">Κράτηση καθορισμένων πόρων από απαιτήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="8db71-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]