---
title: Επισκόπηση του Project Service Automation
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη λύση ενοποίησης του Dynamics 365 Project Service Automation στο Dynamics 365 Finance.
author: ruhercul
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1e1a963bccefd1552aab6e42d3b2d1dc63a82e8f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077057"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="63430-103">Επισκόπηση του Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="63430-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="63430-104">Η λύση ενοποίησης του Project Service Automation στο Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Dynamics 365 Finance και Dynamics 365 Project Service Automation μέσω Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="63430-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="63430-105">Τα πρότυπα ενοποίησης που είναι διαθέσιμα με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιούν τη ροή των έργων, τις συμβάσεις έργου, τις γραμμές σύμβασης έργου, τα ορόσημα γραμμής σύμβασης έργου, τις εργασίες έργου, τις κατηγορίες των συναλλαγών εξόδων, τις εκτιμήσεις ωρών και τις εκτιμήσεις εξόδων από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="63430-106">Εάν χρησιμοποιείτε την έκδοση 7.3.0, θα πρέπει να εγκαταστήσετε το KB 4074835.</span><span class="sxs-lookup"><span data-stu-id="63430-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="63430-107">Στη συνέχεια, θα έχετε τη δυνατότητα να ενσωματώσετε έργα σταθερών τιμών.</span><span class="sxs-lookup"><span data-stu-id="63430-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="63430-108">Εάν χρησιμοποιείτε την έκδοση 7.3.0 και πραγματοποιείτε συναλλαγές αμοιβών πάνω από το Project Service Automation, πρέπει να εγκαταστήσετε το KB 4345320, προκειμένου να συμπεριλάβετε αυτές τις χρεώσεις στο τιμολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="63430-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="63430-109">Αν χρησιμοποιείτε την έκδοση 8.0, θα μπορείτε να χρησιμοποιείτε την ενοποίηση εργασιών έργου, τις κατηγορίες εξόδων, τις εκτιμήσεις ωρών, τις εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="63430-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="63430-110">Εάν χρησιμοποιείτε την έκδοση 8.0.1 ή νεότερη, θα μπορείτε να συγχρονίσετε πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="63430-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="63430-111">Για να μπορέσετε να ενσωματώσετε το Project Service Automation στο Finance, πρέπει να ρυθμίσετε τις παραμέτρους ενοποίησης του Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="63430-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="63430-112">Για περισσότερες πληροφορίες δείτε [Παράμετροι ενοποίησης του Project Service Automation](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="63430-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="63430-113">Αυτή η λύση ενοποίησης δίνει τη δυνατότητα άμεσου συγχρονισμού στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="63430-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="63430-114">Διατηρήστε τις συμβάσεις έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-115">Δημιουργήστε έργα στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-116">Διατηρήστε τις γραμμές σύμβασης έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-117">Διατηρήστε τα ορόσημα γραμμής σύμβασης έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-118">Διατηρήστε τις εργασίες έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-119">Διατηρήστε τις κατηγορίες συναλλαγών εξόδων στο Finance και συγχρονίστε τις απευθείας από το Finance στο Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="63430-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="63430-120">Δημιουργήστε ωριαίες εκτιμήσεις έργου στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-121">Δημιουργήστε εκτιμήσεις εξόδων έργου στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="63430-122">Δημιουργήστε χρόνο έργου, έξοδα και πραγματικές τιμές χρεώσεων στο Project Service Automation και δημιουργήστε συναλλαγές έργου στο ημερολόγιο συναλλαγών στο Project Service Automation, ώστε να είναι δυνατή η καταχώρησή τους στο Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="63430-123">Συγχρονισμός δεδομένων</span><span class="sxs-lookup"><span data-stu-id="63430-123">Data synchronization</span></span>

<span data-ttu-id="63430-124">Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα στα πλαίσια της ενοποίησης μεταξύ Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="63430-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="63430-125">Αυτήν τη στιγμή δεν είναι διαθέσιμα όλα τα πρότυπα.</span><span class="sxs-lookup"><span data-stu-id="63430-125">Not all templates are currently available.</span></span> <span data-ttu-id="63430-126">Τα πρότυπα θα διατεθούν μετά την ολοκλήρωσή τους.</span><span class="sxs-lookup"><span data-stu-id="63430-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="63430-127">[![Ενοποίηση του Project Service Automation με το Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="63430-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="63430-128">Απαιτήσεις συστήματος για το Finance</span><span class="sxs-lookup"><span data-stu-id="63430-128">System requirements for Finance</span></span>

<span data-ttu-id="63430-129">Για να χρησιμοποιήσετε τη λύση ενοποίησης του Project Service Automation με το Finance, πρέπει να εγκαταστήσετε το Enterprise Edition 7.3 με την ενημέρωση πλατφόρμας 12 ή μεταγενέστερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="63430-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="63430-130">Απαιτήσεις συστήματος για το Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="63430-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="63430-131">Για να χρησιμοποιήσετε τη λύση ενοποίησης του Project Service Automation με το Finance, πρέπει να εγκαταστήσετε τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="63430-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="63430-132">Έκδοση Dynamics 365 Project Service Automation 9.0.0.0 ή νεότερη</span><span class="sxs-lookup"><span data-stu-id="63430-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="63430-133">Λύση Prospect to cash για το Dynamics 365 Sales, έκδοση 1.14.0.0 (v14) ή νεότερη έκδοση</span><span class="sxs-lookup"><span data-stu-id="63430-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="63430-134">Λύση Project Service Automation σε Finance για την έκδοση Dynamics 365 Project Service Automation 1.0.0.0 ή μεταγενέστερη</span><span class="sxs-lookup"><span data-stu-id="63430-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="63430-135">Εγκατάσταση λύσης ενοποίησης του Project Service Automation με το Finance στην παρουσία Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="63430-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="63430-136">Πραγματοποιήστε λήψη της λύσης ενοποίησης του Project Service Automation με το Finance από το [Κέντρο λήψης της Microsoft](https://www.microsoft.com/download/details.aspx?id=57016) και ακολουθήστε τις οδηγίες που περιλαμβάνονται με τη λύση.</span><span class="sxs-lookup"><span data-stu-id="63430-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>
