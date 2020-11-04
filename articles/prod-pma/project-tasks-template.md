---
title: Συγχρονισμός εργασιών έργου απευθείας από το Project Service Automation στο Finance and Operations
description: Αυτό το θέμα περιγράφει το πρότυπο και την υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Microsoft Dynamics 365 Project Service Automation στο Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 0383607a07def6c21562bf4b0893fe3ce3db6a04
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076898"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="39b4b-103">Συγχρονισμός εργασιών έργου απευθείας από το Project Service Automation στο Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="39b4b-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="39b4b-104">Αυτό το θέμα περιγράφει το πρότυπο και την υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Dynamics 365 Project Service Automation στο Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="39b4b-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="39b4b-105">Η ενοποίηση εργασιών έργου, οι κατηγορίες εξόδων, οι εκτιμήσεις ωρών, οι εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών είναι διαθέσιμα στην έκδοση 8.0.</span><span class="sxs-lookup"><span data-stu-id="39b4b-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="39b4b-106">Αν χρησιμοποιείτε το Enterprise edition 7.3.0, μετά την εγκατάσταση των KB 4132657 και KB 4132660, θα μπορείτε να χρησιμοποιήσετε τα πρότυπα για να ενσωματώσετε εργασίες έργου, κατηγορίες εξόδων, εκτιμήσεις ωρών, εκτιμήσεις εξόδων και πραγματικές τιμές και για να ρυθμίσετε τις παραμέτρους του κλειδώματος λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="39b4b-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="39b4b-107">Εάν πρέπει να επαναφέρετε τις λογιστικές κατανομές, συνιστάται επίσης η εγκατάσταση του KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="39b4b-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="39b4b-108">Η ενοποίηση πραγματικών στοιχείων είναι διαθέσιμη στην έκδοση 8.0.1 ή μεταγενέστερη.</span><span class="sxs-lookup"><span data-stu-id="39b4b-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="39b4b-109">Ροή δεδομένων για το Project Service Automation στο Finance</span><span class="sxs-lookup"><span data-stu-id="39b4b-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="39b4b-110">Η λύση ενοποίησης Project Service Automation σε Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="39b4b-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="39b4b-111">Το πρότυπο ενοποίησης που είναι διαθέσιμο με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιεί τη ροή των δεδομένων σχετικά με τις εργασίες του έργου από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="39b4b-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="39b4b-112">Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα μεταξύ Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="39b4b-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="39b4b-113">[![Ροή δεδομένων για την ενοποίηση του Project Service Automation με το Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="39b4b-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="39b4b-114">Πρότυπο και εργασία</span><span class="sxs-lookup"><span data-stu-id="39b4b-114">Template and task</span></span>

<span data-ttu-id="39b4b-115">Για να αποκτήσετε πρόσβαση στο πρότυπο, στο κέντρο διαχείρισης του Microsoft Power Apps, επιλέξτε **Έργα** και, στη συνέχεια, στην επάνω δεξιά γωνία, επιλέξτε **Νέο έργο** για να επιλέξετε δημόσια πρότυπα.</span><span class="sxs-lookup"><span data-stu-id="39b4b-115">To access the template, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="39b4b-116">Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των εργασιών έργου απευθείας από το Project Service Automation στο Finance:</span><span class="sxs-lookup"><span data-stu-id="39b4b-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="39b4b-117">**Όνομα του προτύπου στην ενοποίηση δεδομένων:** Εργασίες έργου (PSA σε Fin και Ops)</span><span class="sxs-lookup"><span data-stu-id="39b4b-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="39b4b-118">**Όνομα της εργασίας στο έργο:** Εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="39b4b-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="39b4b-119">Για να είναι δυνατός ο συγχρονισμός των εργασιών έργου, πρέπει να συγχρονίσετε τις συμβάσεις και τα έργα του έργου.</span><span class="sxs-lookup"><span data-stu-id="39b4b-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="39b4b-120">Σύνολο οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="39b4b-120">Entity set</span></span>

| <span data-ttu-id="39b4b-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="39b4b-121">Project Service Automation</span></span> | <span data-ttu-id="39b4b-122">Οικονομικά</span><span class="sxs-lookup"><span data-stu-id="39b4b-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="39b4b-123">Εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="39b4b-123">Project Tasks</span></span>              | <span data-ttu-id="39b4b-124">Οντότητα ενοποίησης για εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="39b4b-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="39b4b-125">Ροή οντότητας</span><span class="sxs-lookup"><span data-stu-id="39b4b-125">Entity flow</span></span>

<span data-ttu-id="39b4b-126">Η διαχείριση των εργασιών έργου γίνεται στο Project Service Automation και συγχρονίζονται με το Finance ως δραστηριότητες έργου.</span><span class="sxs-lookup"><span data-stu-id="39b4b-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="39b4b-127">Προϋποθέσεις και ρύθμιση αντιστοίχισης</span><span class="sxs-lookup"><span data-stu-id="39b4b-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="39b4b-128">Για να είναι δυνατός ο συγχρονισμός των εργασιών έργου, πρέπει να συγχρονίσετε τις συμβάσεις και τα έργα του έργου.</span><span class="sxs-lookup"><span data-stu-id="39b4b-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="39b4b-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="39b4b-129">Power Query</span></span>

<span data-ttu-id="39b4b-130">Πρέπει να χρησιμοποιήσετε το Microsoft Power Query για Excel για να φιλτράρετε τα δεδομένα, εάν πληρούνται αυτές οι προϋποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="39b4b-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="39b4b-131">Διαθέτετε καρτέλες συγκεκριμένων πόρων σε μια εργασία έργου.</span><span class="sxs-lookup"><span data-stu-id="39b4b-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="39b4b-132">Εάν πρέπει να χρησιμοποιήσετε το Power Query, ακολουθήστε την παρακάτω οδηγία:</span><span class="sxs-lookup"><span data-stu-id="39b4b-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="39b4b-133">Το πρότυπο Εργασίες έργου (PSA σε Fin και Ops) έχει ένα προεπιλεγμένο φίλτρο που αποκλείει καρτέλες που αφορούν πόρους από μια εργασία έργου, ορίζοντας το φίλτρο στο **IsLineTask** σε **Ψευδές**.</span><span class="sxs-lookup"><span data-stu-id="39b4b-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="39b4b-134">Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτό το φίλτρο.</span><span class="sxs-lookup"><span data-stu-id="39b4b-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="39b4b-135">Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="39b4b-135">Template mapping in Data integration</span></span>

<span data-ttu-id="39b4b-136">Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="39b4b-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="39b4b-137">Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="39b4b-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="39b4b-138">[![Αντιστοίχιση προτύπου](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="39b4b-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>
