---
title: Συγχρονισμός εκτιμήσεων έργου απευθείας από το Project Service Automation στο Finance and Operations
description: Αυτό το θέμα περιγράφει τα πρότυπο και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό ωριαίων εκτιμήσεων έργου και εκτιμήσεων δαπανών έργου απευθείας από το Microsoft Dynamics 365 Project Service Automation στο Dynamics 365 Finance.
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
ms.openlocfilehash: 58e204b2c1238e00ffb16533cc82dad69fbf77a9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289459"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="5a789-103">Συγχρονισμός εκτιμήσεων έργου απευθείας από το Project Service Automation στο Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="5a789-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="5a789-104">Αυτό το θέμα περιγράφει τα πρότυπο και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό ωριαίων εκτιμήσεων έργου και εκτιμήσεων δαπανών έργου απευθείας από το Dynamics 365 Project Service Automation στο Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="5a789-105">Η ενοποίηση εργασιών έργου, οι κατηγορίες εξόδων, οι εκτιμήσεις ωρών, οι εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών είναι διαθέσιμα στην έκδοση 8.0.</span><span class="sxs-lookup"><span data-stu-id="5a789-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="5a789-106">Η ενοποίηση πραγματικών στοιχείων είναι διαθέσιμη στην έκδοση 8.0.1 ή μεταγενέστερη.</span><span class="sxs-lookup"><span data-stu-id="5a789-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="5a789-107">Ροή δεδομένων για το Project Service Automation στο Finance</span><span class="sxs-lookup"><span data-stu-id="5a789-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="5a789-108">Η λύση ενοποίησης Project Service Automation σε Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="5a789-109">Τα πρότυπα ενοποίησης που είναι διαθέσιμα με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιούν τη ροή των δεδομένων σχετικά με τις ωριαίες εκτιμήσεις έργου και τις εκτιμήσεις δαπανών έργου μεταξύ του Project Service Automation και του Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="5a789-110">Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα μεταξύ Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="5a789-111">[![Ροή δεδομένων για την ενοποίηση του Project Service Automation με το Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="5a789-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="5a789-112">Ωριαίες εκτιμήσεις έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="5a789-113">Πρότυπο και εργασίες</span><span class="sxs-lookup"><span data-stu-id="5a789-113">Template and tasks</span></span>

<span data-ttu-id="5a789-114">Για να αποκτήσετε πρόσβαση στα διαθέσιμα πρότυπα, στο κέντρο διαχείρισης του Microsoft Power Apps, επιλέξτε **Έργα** και, στη συνέχεια, στην επάνω δεξιά γωνία, επιλέξτε **Νέο έργο** για να επιλέξετε δημόσια πρότυπα.</span><span class="sxs-lookup"><span data-stu-id="5a789-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="5a789-115">Το παρακάτω πρότυπο και οι υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των ωριαίων εκτιμήσεων έργου απευθείας από το Project Service Automation στο Finance:</span><span class="sxs-lookup"><span data-stu-id="5a789-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="5a789-116">**Όνομα του προτύπου στην ενοποίηση δεδομένων:** Ωριαίες εκτιμήσεις έργου (PSA σε Fin και Ops)</span><span class="sxs-lookup"><span data-stu-id="5a789-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="5a789-117">**Όνομα των εργασιών στο έργο:**</span><span class="sxs-lookup"><span data-stu-id="5a789-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="5a789-118">Σχέσεις συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="5a789-118">Transaction relationships</span></span>
    - <span data-ttu-id="5a789-119">Εκτιμήσεις εξόδων</span><span class="sxs-lookup"><span data-stu-id="5a789-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="5a789-120">Σύνολο οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="5a789-120">Entity set</span></span>

| <span data-ttu-id="5a789-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a789-121">Project Service Automation</span></span> | <span data-ttu-id="5a789-122">Οικονομικά</span><span class="sxs-lookup"><span data-stu-id="5a789-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="5a789-123">Εργασίες έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-123">Project tasks</span></span>              | <span data-ttu-id="5a789-124">Οντότητα ενοποίησης για ωριαίες εκτιμήσεις έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="5a789-125">Ροή οντότητας</span><span class="sxs-lookup"><span data-stu-id="5a789-125">Entity flow</span></span>

<span data-ttu-id="5a789-126">Η διαχείριση των ωριαίων εκτιμήσεων έργου γίνεται στο Project Service Automation και συγχρονίζονται με το Finance ως προβλέψεις ωρών έργου.</span><span class="sxs-lookup"><span data-stu-id="5a789-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="5a789-127">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="5a789-127">Prerequisites</span></span>

<span data-ttu-id="5a789-128">Για να είναι δυνατός ο συγχρονισμός των εκτιμήσεων ωρών έργου, πρέπει να συγχρονίσετε έργα, εργασίες έργου και κατηγορίες εξόδων έργου.</span><span class="sxs-lookup"><span data-stu-id="5a789-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="5a789-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="5a789-129">Power Query</span></span>

<span data-ttu-id="5a789-130">Στο πρότυπο ωριαίων εκτιμήσεων έργου, πρέπει να χρησιμοποιήσετε το Microsoft Power Query για Excel για την ολοκλήρωση αυτών των εργασιών:</span><span class="sxs-lookup"><span data-stu-id="5a789-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="5a789-131">Ορίστε το αναγνωριστικό προεπιλεγμένου μοντέλου πρόβλεψης που θα χρησιμοποιηθεί όταν η ενοποίηση δημιουργεί νέες προβλέψεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="5a789-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="5a789-132">Φιλτράρετε τυχόν καρτέλες που αφορούν συγκεκριμένους πόρους στην εργασία που θα αποτύχει η ενοποίηση σε προβλέψεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="5a789-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="5a789-133">Φιλτράρετε όλες τις κενές γραμμές κατηγορίας συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="5a789-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="5a789-134">Εάν δεν ολοκληρωθεί αυτή η εργασία, αυτό μπορεί να οδηγήσει σε εσφαλμένες προβλέψεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="5a789-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="5a789-135">Ορίστε το αναγνωριστικό του προεπιλεγμένου μοντέλου πρόβλεψης</span><span class="sxs-lookup"><span data-stu-id="5a789-135">Set the default forecast model ID</span></span>

<span data-ttu-id="5a789-136">Για να ενημερώσετε το αναγνωριστικό του προεπιλεγμένου μοντέλου πρόβλεψης στο πρότυπο, κάντε κλικ στο βέλος **Αντιστοίχιση** για να ανοίξετε την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="5a789-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="5a789-137">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="5a789-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="5a789-138">Εάν χρησιμοποιείτε το προεπιλεγμένο πρότυπο εκτιμήσεων ωρών (PSA σε Fin και Ops), στο Power Query, επιλέξτε την τελευταία **Συνθήκη που έχει εισαχθεί** από τη λίστα **Εφαρμοσμένα βήματα**.</span><span class="sxs-lookup"><span data-stu-id="5a789-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="5a789-139">Στην καταχώριση **Συνάρτηση**, αντικαταστήστε το **O\_forecast** με το όνομα του αναγνωριστικού μοντέλου πρόβλεψης που θα πρέπει να χρησιμοποιηθεί με την ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="5a789-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="5a789-140">Το προεπιλεγμένο πρότυπο έχει ένα αναγνωριστικό μοντέλου πρόβλεψης από τα δεδομένα επίδειξης.</span><span class="sxs-lookup"><span data-stu-id="5a789-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="5a789-141">Εάν δημιουργείτε ένα νέο πρότυπο, πρέπει να προσθέσετε αυτήν τη στήλη.</span><span class="sxs-lookup"><span data-stu-id="5a789-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="5a789-142">Στο Power Query επιλέξτε **Προσθήκη στήλης υπό όρους** και καταχωρίστε ένα όνομα για τη νέα στήλη, για παράδειγμα, **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="5a789-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="5a789-143">Εισάγετε τη συνθήκη για τη στήλη, όπου, εάν η εργασία έργου είναι null, τότε \<enter the forecast model ID\>; else null.</span><span class="sxs-lookup"><span data-stu-id="5a789-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="5a789-144">Φιλτράρισμα καρτελών που αφορούν πόρους</span><span class="sxs-lookup"><span data-stu-id="5a789-144">Filter out resource-specific records</span></span>

<span data-ttu-id="5a789-145">Το πρότυπο "ώρες έργου" (PSA σε Fin και Ops) έχει ένα προεπιλεγμένο φίλτρο που καταργεί τυχόν καρτέλες που αφορούν πόρους.</span><span class="sxs-lookup"><span data-stu-id="5a789-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="5a789-146">Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτό το φίλτρο.</span><span class="sxs-lookup"><span data-stu-id="5a789-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="5a789-147">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** για να φιλτράρετε τη στήλη **msdyn\_islinetask** έτσι, ώστε να περιλαμβάνονται μόνο οι καρτέλες **Ψευδές**.</span><span class="sxs-lookup"><span data-stu-id="5a789-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="5a789-148">Φιλτράρετε τις κενές γραμμές κατηγορίας συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="5a789-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="5a789-149">Πρέπει να προσθέσετε ένα φίλτρο για να καταργήσετε τις κενές κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="5a789-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="5a789-150">Αυτή η εργασία απαιτείται, ανεξάρτητα από το εάν χρησιμοποιείτε το προεπιλεγμένο πρότυπο ή δημιουργείτε το δικό σας πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="5a789-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="5a789-151">Αυτό το φίλτρο καταργεί όλες τις συνοπτικές γραμμές από το Project Service Automation οι οποίες ενδέχεται να προκαλέσουν την εσφαλμένη πρόβλεψη της ώρας στο Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="5a789-152">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** για να φιλτράρετε τις κενές καρτέλες στη στήλη **msdyn\_transactioncategory\_value**.</span><span class="sxs-lookup"><span data-stu-id="5a789-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="5a789-153">Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="5a789-153">Template mapping in Data integration</span></span>

<span data-ttu-id="5a789-154">Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="5a789-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="5a789-155">Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="5a789-156">[![Αντιστοίχιση προτύπου εργασίας στην ενοποίηση δεδομένων](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="5a789-156">[![Template task mapping in data integration](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="5a789-157">Εκτιμήσεις εξόδων έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="5a789-158">Πρότυπο και εργασίες</span><span class="sxs-lookup"><span data-stu-id="5a789-158">Template and tasks</span></span>

<span data-ttu-id="5a789-159">Το παρακάτω πρότυπο και οι υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των εκτιμήσεων εξόδων έργου απευθείας από το Project Service Automation στο Finance:</span><span class="sxs-lookup"><span data-stu-id="5a789-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="5a789-160">**Όνομα του προτύπου στην ενοποίηση δεδομένων:** Εκτιμήσεις δαπανών έργου (PSA σε Fin και Ops)</span><span class="sxs-lookup"><span data-stu-id="5a789-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="5a789-161">**Όνομα των εργασιών στο έργο:**</span><span class="sxs-lookup"><span data-stu-id="5a789-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="5a789-162">Σχέσεις συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="5a789-162">Transaction relationships</span></span> 
    - <span data-ttu-id="5a789-163">Εκτιμήσεις εξόδων</span><span class="sxs-lookup"><span data-stu-id="5a789-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="5a789-164">Σύνολο οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="5a789-164">Entity set</span></span>

| <span data-ttu-id="5a789-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5a789-165">Project Service Automation</span></span> | <span data-ttu-id="5a789-166">Οικονομικά</span><span class="sxs-lookup"><span data-stu-id="5a789-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="5a789-167">Συνδέσεις συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="5a789-167">Transaction Connections</span></span>    | <span data-ttu-id="5a789-168">Οντότητα ενοποίησης για σχέσεις συναλλαγών έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="5a789-169">Γραμμές εκτιμήσεων</span><span class="sxs-lookup"><span data-stu-id="5a789-169">Estimate Lines</span></span>             | <span data-ttu-id="5a789-170">Οντότητα ενοποίησης για εκτιμήσεις δαπανών έργου</span><span class="sxs-lookup"><span data-stu-id="5a789-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="5a789-171">Ροή οντότητας</span><span class="sxs-lookup"><span data-stu-id="5a789-171">Entity flow</span></span>

<span data-ttu-id="5a789-172">Η διαχείριση των δαπανών έργου γίνεται στο Project Service Automation και συγχρονίζονται με το Finance ως προβλέψεις δαπανών έργου.</span><span class="sxs-lookup"><span data-stu-id="5a789-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="5a789-173">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="5a789-173">Prerequisites</span></span>

<span data-ttu-id="5a789-174">Για να είναι δυνατός ο συγχρονισμός των εκτιμήσεων δαπανών έργου, πρέπει να συγχρονίσετε έργα, εργασίες έργου και κατηγορίες εξόδων έργου.</span><span class="sxs-lookup"><span data-stu-id="5a789-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="5a789-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="5a789-175">Power Query</span></span>

<span data-ttu-id="5a789-176">Στο πρότυπο εκτιμήσεων εξόδων έργου, πρέπει να χρησιμοποιήσετε το Power Query για Excel για την ολοκλήρωση αυτών των εργασιών:</span><span class="sxs-lookup"><span data-stu-id="5a789-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="5a789-177">Φιλτράρετε το για να συμπεριλάβετε μόνο καρτέλες εξόδων για τις γραμμές εκτίμησης εξόδων.</span><span class="sxs-lookup"><span data-stu-id="5a789-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="5a789-178">Ορίστε το αναγνωριστικό προεπιλεγμένου μοντέλου πρόβλεψης που θα χρησιμοποιηθεί όταν η ενοποίηση δημιουργεί νέες προβλέψεις ώρας.</span><span class="sxs-lookup"><span data-stu-id="5a789-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="5a789-179">Μεταμορφώστε τους τύπους χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="5a789-179">Transform the billing types.</span></span>
- <span data-ttu-id="5a789-180">Μεταμορφώστε τους τύπους συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="5a789-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="5a789-181">Φιλτράρετε το για να συμπεριλάβετε μόνο γραμμές εκτίμησης εξόδων</span><span class="sxs-lookup"><span data-stu-id="5a789-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="5a789-182">Το πρότυπο εκτιμήσεων έργου (PSA σε Fin και Ops) έχει ένα προεπιλεγμένο φίλτρο που περιλαμβάνει μόνο γραμμές εξόδων στην ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="5a789-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="5a789-183">Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτό το φίλτρο.</span><span class="sxs-lookup"><span data-stu-id="5a789-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="5a789-184">Επιλέξτε την εργασία **Σχέσεις συναλλαγών** και, στη συνέχεια, κάντε κλικ στο βέλος **Αντιστοίχιση** για να ανοίξετε την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="5a789-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="5a789-185">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="5a789-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="5a789-186">Φιλτράρετε τη στήλη **msdyn\_transactiontype1** ώστε να περιλαμβάνει μόνο το **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="5a789-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="5a789-187">Ορίστε το αναγνωριστικό του προεπιλεγμένου μοντέλου πρόβλεψης</span><span class="sxs-lookup"><span data-stu-id="5a789-187">Set the default forecast model ID</span></span>

<span data-ttu-id="5a789-188">Για να ενημερώσετε το αναγνωριστικό του προεπιλεγμένου μοντέλου πρόβλεψης στο πρότυπο, επιλέξτε την εργασία **Εκτιμήσεις δαπανών** κάντε κλικ στο βέλος **Αντιστοίχιση** για να ανοίξετε την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="5a789-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="5a789-189">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="5a789-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="5a789-190">Εάν χρησιμοποιείτε το πρότυπο προεπιλεγμένων εκτιμήσεων δαπανών έργου (PSA σε Fin και Ops), στο Power Query, επιλέξτε πρώτα την τελευταία **Συνθήκη που έχει εισαχθεί** από την ενότητα **Εφαρμοσμένα βήματα**.</span><span class="sxs-lookup"><span data-stu-id="5a789-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="5a789-191">Στην καταχώριση **Συνάρτηση**, αντικαταστήστε το **O\_forecast** με το όνομα του αναγνωριστικού μοντέλου πρόβλεψης που θα πρέπει να χρησιμοποιηθεί με την ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="5a789-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="5a789-192">Το προεπιλεγμένο πρότυπο έχει ένα αναγνωριστικό μοντέλου πρόβλεψης από τα δεδομένα επίδειξης.</span><span class="sxs-lookup"><span data-stu-id="5a789-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="5a789-193">Εάν δημιουργείτε ένα νέο πρότυπο, πρέπει να προσθέσετε αυτήν τη στήλη.</span><span class="sxs-lookup"><span data-stu-id="5a789-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="5a789-194">Στο Power Query επιλέξτε **Προσθήκη στήλης υπό όρους** και καταχωρίστε ένα όνομα για τη νέα στήλη, για παράδειγμα, **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="5a789-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="5a789-195">Εισάγετε τη συνθήκη για τη στήλη, όπου, εάν το αναγνωριστικό γραμμής εκτίμησης είναι null, τότε \<enter the forecast model ID\>; else null.</span><span class="sxs-lookup"><span data-stu-id="5a789-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="5a789-196">Μεταμορφώστε τους τύπους χρέωσης</span><span class="sxs-lookup"><span data-stu-id="5a789-196">Transform the billing types</span></span>

<span data-ttu-id="5a789-197">Το πρότυπο εκτιμήσεων εξόδων έργου (PSA σε Fin και Ops) περιλαμβάνει μια στήλη υπό όρους που χρησιμοποιείται για τον μετασχηματισμό των τύπων χρέωσης που λαμβάνονται από το Project Service Automation κατά την ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="5a789-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="5a789-198">Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτήν τη στήλη υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="5a789-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="5a789-199">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** και, στη συνέχεια, επιλέξτε **Προσθήκη στήλης υπό όρους**.</span><span class="sxs-lookup"><span data-stu-id="5a789-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="5a789-200">Καταγράψτε ένα όνομα για τη νέα στήλη, για παράδειγμα, **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="5a789-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="5a789-201">Μετά πληκτρολογήστε την εξής συνθήκη:</span><span class="sxs-lookup"><span data-stu-id="5a789-201">Then enter the following condition:</span></span>

<span data-ttu-id="5a789-202">Εάν **msdyn\_billingtype** = 192350000, τότε **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="5a789-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="5a789-203">else if **msdyn\_billingtype** = 192350001, τότε **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="5a789-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="5a789-204">else if **msdyn\_billingtype** = 192350002, τότε **Δωρεάν**</span><span class="sxs-lookup"><span data-stu-id="5a789-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="5a789-205">else **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="5a789-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="5a789-206">Μεταμορφώστε τους τύπους συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="5a789-206">Transform the transaction types</span></span>

<span data-ttu-id="5a789-207">Το πρότυπο εκτιμήσεων εξόδων έργου (PSA σε Fin και Ops) περιλαμβάνει μια στήλη υπό όρους που χρησιμοποιείται για τον μετασχηματισμό των τύπων συναλλαγών που λαμβάνονται από το Project Service Automation κατά την ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="5a789-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="5a789-208">Εάν δημιουργήσετε το δικό σας πρότυπο, πρέπει να προσθέσετε αυτήν τη στήλη υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="5a789-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="5a789-209">Επιλέξτε τη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** και, στη συνέχεια, επιλέξτε **Προσθήκη στήλης υπό όρους**.</span><span class="sxs-lookup"><span data-stu-id="5a789-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="5a789-210">Καταγράψτε ένα όνομα για τη νέα στήλη, για παράδειγμα, **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="5a789-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="5a789-211">Μετά πληκτρολογήστε την εξής συνθήκη:</span><span class="sxs-lookup"><span data-stu-id="5a789-211">Then enter the following condition:</span></span>

<span data-ttu-id="5a789-212">Εάν **msdyn\_transactiontypecode** = 192350000, τότε **Κόστος**</span><span class="sxs-lookup"><span data-stu-id="5a789-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="5a789-213">else if **msdyn\_transactiontypecode** = 192350005, τότε **Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="5a789-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="5a789-214">else **null**</span><span class="sxs-lookup"><span data-stu-id="5a789-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="5a789-215">Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="5a789-215">Template mapping in Data integration</span></span>

<span data-ttu-id="5a789-216">Οι εικόνες που ακολουθούν δείχνουν παραδείγματα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="5a789-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="5a789-217">Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="5a789-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="5a789-218">[![Αντιστοίχιση προτύπου των συναλλαγών εκτίμησης εξόδων](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="5a789-218">[![Template mapping of expense estimate transactions](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="5a789-219">[![Αντιστοίχιση προτύπου των εκτιμήσεων εξόδων](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="5a789-219">[![Template mapping of expense estimates](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]