---
title: Συγχρονισμός κατηγοριών εξόδων έργου μεταξύ του Finance and Operations και του Project Service Automation
description: Αυτό το θέμα περιγράφει τα πρότυπα και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδων έργου μεταξύ του Microsoft Dynamics 365 Finance και του Dynamics 365 Project Service Automation.
author: KimANelson
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
ms.assetid: 7dd914dc-1913-45eb-8a67-e897b00089fa
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 757fe1dbc804b986fc3334ebae7254a3f0491f59
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751624"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="87c6b-103">Συγχρονισμός κατηγοριών εξόδων έργου μεταξύ του Finance and Operations και του Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="87c6b-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="87c6b-104">Αυτό το θέμα περιγράφει τα πρότυπα και τις υποκείμενες εργασίες που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδων έργου μεταξύ του Dynamics 365 Finance και του Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="87c6b-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="87c6b-105">Η ενοποίηση εργασιών έργου, οι κατηγορίες εξόδων, οι εκτιμήσεις ωρών, οι εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών είναι διαθέσιμα στην έκδοση 8.0.</span><span class="sxs-lookup"><span data-stu-id="87c6b-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="87c6b-106">Η ενοποίηση πραγματικών στοιχείων είναι διαθέσιμη στην έκδοση 8.0.1 ή μεταγενέστερη.</span><span class="sxs-lookup"><span data-stu-id="87c6b-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="87c6b-107">Αν χρησιμοποιείτε το Enterprise edition 7.3.0, μετά την εγκατάσταση των KB 4132657 και KB 4132660, θα μπορείτε να χρησιμοποιήσετε τα πρότυπα για να ενσωματώσετε εργασίες έργου, κατηγορίες εξόδων, εκτιμήσεις ωρών, εκτιμήσεις εξόδων και πραγματικές τιμές και για να ρυθμίσετε τις παραμέτρους του κλειδώματος λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="87c6b-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="87c6b-108">Εάν πρέπει να επαναφέρετε τις λογιστικές κατανομές, συνιστάται επίσης η εγκατάσταση του KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="87c6b-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="87c6b-109">Ροή δεδομένων για το Project Service Automation και το Finance</span><span class="sxs-lookup"><span data-stu-id="87c6b-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="87c6b-110">Η λύση ενοποίησης Project Service Automation και Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="87c6b-111">Τα πρότυπα ενοποίησης που είναι διαθέσιμα με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιούν τη ροή των δεδομένων σχετικά με τις κατηγορίες συναλλαγών εξόδων έργου μεταξύ του Project Service Automation και του Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="87c6b-112">Εάν οι κατηγορίες εξόδων έργου έχουν δημιουργηθεί στο Finance, η ροή ενοποίησης είναι από το Finance στο Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="87c6b-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="87c6b-113">Στη συνέχεια, τα αναγνωριστικά ενοποίησης των κατηγοριών εξόδων έργου ενημερώνονται μέσω συγχρονισμού από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="87c6b-114">Εάν οι κατηγορίες εξόδων έργου έχουν δημιουργηθεί στο Project Service Automation, η ροή ενοποίησης είναι από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="87c6b-115">Οι κατηγορίες έργου πρέπει να ρυθμιστούν ήδη στο Finance πριν από το συγχρονισμό από το Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="87c6b-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="87c6b-116">Κατόπιν συγχρονίστε από το Finance στο Project Service Automation και μετά από το Project Service Automation στο Finance ξανά.</span><span class="sxs-lookup"><span data-stu-id="87c6b-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="87c6b-117">Με αυτόν τον τρόπο, μπορείτε να εγγυηθείτε ότι οι κατηγορίες είναι συνδεδεμένες και ότι δεν δημιουργούνται διπλότυπα.</span><span class="sxs-lookup"><span data-stu-id="87c6b-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="87c6b-118">Συνήθως, οι κατηγορίες εξόδων έργου καταχωρούνται στο Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="87c6b-119">Ωστόσο, εάν δεν υπάρχουν ή εάν έχουν ήδη δημιουργηθεί κατηγορίες εξόδων στο Project Service Automation, πρέπει πρώτα να πραγματοποιήσετε συγχρονισμό χρησιμοποιώντας το πρότυπο κατηγοριών συναλλαγών εξόδων έργου (PSA σε Fin και Ops).</span><span class="sxs-lookup"><span data-stu-id="87c6b-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="87c6b-120">Στη συνέχεια, πραγματοποιήστε συγχρονισμό χρησιμοποιώντας το πρότυπο κατηγοριών συναλλαγών εξόδων έργου (Fin and Ops σε PSA).</span><span class="sxs-lookup"><span data-stu-id="87c6b-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="87c6b-121">Στη συνέχεια, θα πρέπει να εκτελέσετε τον συγχρονισμό από το Project Service Automation στο Finance μια ακόμα φορά.</span><span class="sxs-lookup"><span data-stu-id="87c6b-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="87c6b-122">Εάν συγχρονίσετε πρώτα από το Project Service Automation, πρέπει να πληρούνται οι παρακάτω προϋποθέσεις στο Finance για την εκτέλεση του συγχρονισμού:</span><span class="sxs-lookup"><span data-stu-id="87c6b-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="87c6b-123">Η κοινόχρηστη κατηγορία που αντιστοιχεί στην κατηγορία έργου που έχει ρυθμιστεί στο Project Service Automation πρέπει να υπάρχει και πρέπει να είναι ενεργοποιημένη τόσο για το **Έργο** όσο και για το **Έξοδο**.</span><span class="sxs-lookup"><span data-stu-id="87c6b-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="87c6b-124">Για κάθε νομική οντότητα Finance με την οποία πρέπει να ενοποιηθεί, πρέπει να υπάρχουν οι ακόλουθες κατηγορίες έργου:</span><span class="sxs-lookup"><span data-stu-id="87c6b-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="87c6b-125">Η **Κατηγορία έργου** υπάρχει.</span><span class="sxs-lookup"><span data-stu-id="87c6b-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="87c6b-126">Η **Χρήση σε έξοδο** έχει ενεργοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="87c6b-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="87c6b-127">Το στοιχείο **Ενεργό στο ημερολόγιο** είναι ενεργοποιημένο.</span><span class="sxs-lookup"><span data-stu-id="87c6b-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="87c6b-128">Ο **Τύπος συναλλαγής** ορίστηκε σε **Έξοδο**.</span><span class="sxs-lookup"><span data-stu-id="87c6b-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="87c6b-129">Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα μεταξύ Project Service Automation και Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="87c6b-130">[![Ροή δεδομένων για την ενοποίηση του Project Service Automation με το Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="87c6b-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="87c6b-131">Συγχρονισμός κατηγορίας εξόδου έργου από το Finance στο Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="87c6b-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="87c6b-132">Πρότυπο και εργασία</span><span class="sxs-lookup"><span data-stu-id="87c6b-132">Template and task</span></span>

<span data-ttu-id="87c6b-133">Για να αποκτήσετε πρόσβαση στο πρότυπο, στο κέντρο διαχείρισης του Microsoft Power Apps, επιλέξτε **Έργα** και, στη συνέχεια, στην επάνω δεξιά γωνία, επιλέξτε **Νέο έργο** για να επιλέξετε δημόσια πρότυπα.</span><span class="sxs-lookup"><span data-stu-id="87c6b-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="87c6b-134">Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδου έργου από το Finance στο Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="87c6b-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="87c6b-135">**Όνομα του προτύπου στην ενοποίηση δεδομένων:** Κατηγορίες συναλλαγών εξόδου έργου (Fin και Ops σε PSA)</span><span class="sxs-lookup"><span data-stu-id="87c6b-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="87c6b-136">**Όνομα της εργασίας του έργου:** Κατηγορίες συγχρονισμού στο PSA</span><span class="sxs-lookup"><span data-stu-id="87c6b-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="87c6b-137">Σύνολο οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="87c6b-137">Entity set</span></span>

| <span data-ttu-id="87c6b-138">Οικονομικά</span><span class="sxs-lookup"><span data-stu-id="87c6b-138">Finance</span></span>                           | <span data-ttu-id="87c6b-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="87c6b-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="87c6b-140">Οντότητα ενοποίησης για κατηγορίες</span><span class="sxs-lookup"><span data-stu-id="87c6b-140">Integration entity for categories</span></span> | <span data-ttu-id="87c6b-141">Κατηγορίες συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="87c6b-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="87c6b-142">Ροή οντότητας</span><span class="sxs-lookup"><span data-stu-id="87c6b-142">Entity flow</span></span>

<span data-ttu-id="87c6b-143">Η διαχείριση των κατηγοριών εξόδων έργου γίνεται στο Finance και συγχρονίζονται με το Project Service Automation ως κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="87c6b-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="87c6b-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="87c6b-144">Power Query</span></span>

<span data-ttu-id="87c6b-145">Όταν εκτελείτε συγχρονισμό με το Project Service Automation, πρέπει να χρησιμοποιήσετε το Microsoft Power Query για Excel για να ορίσετε τον τύπο χρέωσης στην κατηγορία συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="87c6b-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="87c6b-146">Το πρότυπο "κατηγορίες συναλλαγών εξόδων έργου" (FIN και OPS σε PSA) παρέχει μια προεπιλεγμένη στήλη και αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="87c6b-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="87c6b-147">Εάν δημιουργήσετε το δικό σας πρότυπο, θα πρέπει να προσθέσετε μια στήλη υπό όρους στο Power Query.</span><span class="sxs-lookup"><span data-stu-id="87c6b-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="87c6b-148">Ακολουθήστε αυτά τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="87c6b-148">Follow these steps.</span></span>

1. <span data-ttu-id="87c6b-149">Κάντε κλικ στο βέλος για να ανοίξετε την αντιστοίχιση των κατηγοριών εξόδων έργου στο πρότυπο κατηγοριών συναλλαγών εξόδων έργου (FIN και OPS σε PSA).</span><span class="sxs-lookup"><span data-stu-id="87c6b-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="87c6b-150">Κάντε κλικ στη σύνδεση **Υποβολή ερωτημάτων και φιλτράρισμα για προχωρημένους** για να ανοίξετε το Power Query.</span><span class="sxs-lookup"><span data-stu-id="87c6b-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="87c6b-151">Επιλέξτε **Προσθήκη στήλης υπό όρους**.</span><span class="sxs-lookup"><span data-stu-id="87c6b-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="87c6b-152">Καταγράψτε ένα όνομα για τη νέα στήλη, για παράδειγμα, **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="87c6b-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="87c6b-153">Καταγράψτε την ακόλουθη συνθήκη: **Εάν το CATEGORYID δεν ισούται με null, τότε 19235001, διαφορετικά null**.</span><span class="sxs-lookup"><span data-stu-id="87c6b-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="87c6b-154">Επιλέξτε **OK** στη στήλη.</span><span class="sxs-lookup"><span data-stu-id="87c6b-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="87c6b-155">Βεβαιωθείτε ότι αντιστοιχίσατε αυτήν τη νέα στήλη στη σελίδα αντιστοίχισης.</span><span class="sxs-lookup"><span data-stu-id="87c6b-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="87c6b-156">Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="87c6b-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="87c6b-157">Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Finance στο Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="87c6b-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="87c6b-158">[![Αντιστοίχιση προτύπου](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="87c6b-158">[![Template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="87c6b-159">Συγχρονισμός κατηγορίας εξόδου έργου από το Project Service Automation στο Finance</span><span class="sxs-lookup"><span data-stu-id="87c6b-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="87c6b-160">Πρότυπο και εργασία</span><span class="sxs-lookup"><span data-stu-id="87c6b-160">Template and task</span></span>

<span data-ttu-id="87c6b-161">Το παρακάτω πρότυπο και η υποκείμενη εργασία που χρησιμοποιούνται για το συγχρονισμό των κατηγοριών εξόδου έργου από το Project Service Automation στο Finance:</span><span class="sxs-lookup"><span data-stu-id="87c6b-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="87c6b-162">**Όνομα του προτύπου στην ενοποίηση δεδομένων:** Κατηγορίες συναλλαγών εξόδου έργου (PSA σε Fin και Ops)</span><span class="sxs-lookup"><span data-stu-id="87c6b-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="87c6b-163">**Όνομα της εργασίας του έργου:** Κατηγορίες συγχρονισμού σε Fin Ops</span><span class="sxs-lookup"><span data-stu-id="87c6b-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="87c6b-164">Σύνολο οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="87c6b-164">Entity set</span></span>

| <span data-ttu-id="87c6b-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="87c6b-165">Project Service Automation</span></span> | <span data-ttu-id="87c6b-166">Οικονομικά</span><span class="sxs-lookup"><span data-stu-id="87c6b-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="87c6b-167">Κατηγορίες συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="87c6b-167">Transaction categories</span></span>     | <span data-ttu-id="87c6b-168">Οντότητα ενοποίησης για κατηγορίες</span><span class="sxs-lookup"><span data-stu-id="87c6b-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="87c6b-169">Ροή οντότητας</span><span class="sxs-lookup"><span data-stu-id="87c6b-169">Entity flow</span></span>

<span data-ttu-id="87c6b-170">Η διαχείριση των κατηγοριών εξόδων έργου γίνεται στο Finance και συγχρονίζονται με το Project Service Automation ως κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="87c6b-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="87c6b-171">Ο συγχρονισμός με ενημερώσεις του Finance ενημερώνει την κατηγορία έργου στο Finance με το αναγνωριστικό ενοποίησης από το Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="87c6b-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="87c6b-172">Αντιστοίχιση προτύπου στην ενοποίηση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="87c6b-172">Template mapping in Data integration</span></span>

<span data-ttu-id="87c6b-173">Η εικόνα που ακολουθεί δείχνει ένα παράδειγμα των αντιστοιχίσεων εργασιών προτύπου στην ενοποίηση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="87c6b-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="87c6b-174">Η αντιστοίχιση εμφανίζει τις πληροφορίες πεδίου που θα συγχρονιστούν από το Project Service Automation στο Finance.</span><span class="sxs-lookup"><span data-stu-id="87c6b-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="87c6b-175">[![Αντιστοίχιση προτύπου](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="87c6b-175">[![Template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
