---
title: Ενημέρωση του Project Operations στο περιβάλλον Finance
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ενημέρωσης του Project Operations στο περιβάλλον Dynamics 365 Finance.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 249b8dba17165da04596ec46a625131b9b4daeb5
ms.sourcegitcommit: f4fc6e3a81e8551da050e92f8fde85f8d7b52fbd
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/29/2020
ms.locfileid: "4816625"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="40029-103">Ενημέρωση του Project Operations στο περιβάλλον Finance</span><span class="sxs-lookup"><span data-stu-id="40029-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="40029-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="40029-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="40029-105">Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ενημέρωσης του Dynamics 365 Project Operations στο περιβάλλον Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="40029-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="40029-106">Υπάρχουν τρεις διαδικασίες που απαιτούνται για την ενημέρωση του Project Operations στην Ενημέρωση 5 (UR5):</span><span class="sxs-lookup"><span data-stu-id="40029-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="40029-107">Εισαγωγή του πακέτου στο έργο προεπισκόπησης</span><span class="sxs-lookup"><span data-stu-id="40029-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="40029-108">Εφαρμογή της ενημέρωσης</span><span class="sxs-lookup"><span data-stu-id="40029-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="40029-109">Ενημέρωση του περιβάλλοντός σας Dataverse</span><span class="sxs-lookup"><span data-stu-id="40029-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="40029-110">Εισαγωγή του πακέτου στο έργο σας LCS</span><span class="sxs-lookup"><span data-stu-id="40029-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="40029-111">Συνδεθείτε στο [Lifecycle Services (LCS)](https://lcs.dynamics.com/) ως κάτοχος έργου ή διαχειριστής περιβάλλοντος.</span><span class="sxs-lookup"><span data-stu-id="40029-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="40029-112">Από τη λίστα έργων, επιλέξτε το έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="40029-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="40029-113">Στη σελίδα **Έργο**, στην ομάδα **Περιβάλλοντα**, ανοίξτε το περιβάλλον που θέλετε να ενημερώσετε.</span><span class="sxs-lookup"><span data-stu-id="40029-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="40029-114">Επαληθεύστε ότι το περιβάλλον εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="40029-114">Verify that the environment is running.</span></span> <span data-ttu-id="40029-115">Εάν δεν ξεκινήσει, εκκινείστε το περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="40029-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="40029-116">Στην ενότητα **Νέα έκδοση**, κάτω από τις **Διαθέσιμες ενημερώσεις**, επιλέξτε **Προβολή ενημέρωσης** για την 10.0.15.</span><span class="sxs-lookup"><span data-stu-id="40029-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![Κουμπί προβολής ενημέρωσης](media/view-update.png)

6. <span data-ttu-id="40029-118">Στη σελίδα **Δυαδικές ενημερώσεις**, επιλέξτε **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="40029-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="40029-119">Στη σελίδα **Έλεγχος και αποθήκευση ενημερώσεων**, επιλέξτε **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="40029-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="40029-120">Στο παράθυρο **Αποθήκευση πακέτου σε βιβλιοθήκη πάγιων στοιχείων**, εισαγάγετε το όνομα του πακέτου και, στη συνέχεια, επιλέξτε **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="40029-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="40029-121">Όταν το LCS ολοκληρώσει την αποθήκευση του πακέτου, το κουμπί **Τέλος** είναι ενεργοποιημένο.</span><span class="sxs-lookup"><span data-stu-id="40029-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="40029-122">Επιλέξτε **Τέλος**.</span><span class="sxs-lookup"><span data-stu-id="40029-122">Select **Done**.</span></span> <span data-ttu-id="40029-123">Το LCS θα επαληθεύσει το πακέτο.</span><span class="sxs-lookup"><span data-stu-id="40029-123">LCS will verify the package.</span></span> <span data-ttu-id="40029-124">Η επαλήθευση μπορεί να διαρκέσει μερικά λεπτά ή έως και μία ώρα.</span><span class="sxs-lookup"><span data-stu-id="40029-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="40029-125">Εφαρμόστε την ενημέρωση πακέτου</span><span class="sxs-lookup"><span data-stu-id="40029-125">Apply the package update</span></span>

1. <span data-ttu-id="40029-126">Στο LCS, στη σελίδα **Λεπτομέρειες περιβάλλοντος**, επιλέξτε **Διατήρηση** > **Εφαρμογή ενημερώσεων**.</span><span class="sxs-lookup"><span data-stu-id="40029-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="40029-127">Από τη λίστα, επιλέξτε το πακέτο που αποθηκεύατε νωρίτερα και, στη συνέχεια, επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="40029-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="40029-128">Επιλέξτε **Ναι** για να επιβεβαιώσετε ότι θέλετε να αναπτύξετε το πακέτο.</span><span class="sxs-lookup"><span data-stu-id="40029-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![Παράθυρο διαλόγου "Επιβεβαίωση ανάπτυξης πακέτου"](media/confirm-package-deployment.png)

4. <span data-ttu-id="40029-130">Επιλέξτε **Ναι** για να επιβεβαιώσετε ότι θέλετε να ενημερώσετε την εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="40029-130">Select **Yes** to confirm that you want to update the application.</span></span>

![Παράθυρο διαλόγου "Επιβεβαίωση ενημέρωσης εφαρμογής"](media/confirm-application-update.png)

<span data-ttu-id="40029-132">Η ανάπτυξη και η ενημέρωση της εφαρμογής θα ξεκινήσουν.</span><span class="sxs-lookup"><span data-stu-id="40029-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="40029-133">Στη σελίδα **Λεπτομέρειες περιβάλλοντος**, στην επάνω δεξιά γωνία, η κατάσταση περιβάλλοντος θα ενημερωθεί σε **Εξυπηρέτηση**.</span><span class="sxs-lookup"><span data-stu-id="40029-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="40029-134">Σε περίπου δύο ώρες, η ενημέρωση θα ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="40029-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="40029-135">Οι πληροφορίες έκδοσης εφαρμογής θα ενημερώσουν το **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** και η κατάσταση περιβάλλοντος θα ενημερωθεί σε **Ανάπτυξη**.</span><span class="sxs-lookup"><span data-stu-id="40029-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="40029-136">Ενημερώστε το περιβάλλον Dataverse σας</span><span class="sxs-lookup"><span data-stu-id="40029-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="40029-137">Συνδεθείτε στο [κέντρο διαχείρισης του Power Platform](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="40029-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="40029-138">Στη λίστα, εντοπίστε και ανοίξτε το περιβάλλον που χρησιμοποιήσατε για να εγκαταστήσετε το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="40029-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="40029-139">Στη σελίδα **Περιβάλλοντα**, επιλέξτε **Πόροι** > **Εφαρμογές Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="40029-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="40029-140">Στη λίστα, εντοπίστε το **Microsoft Dynamics 365 Project Operations** και στη στήλη **Κατάσταση**, επιλέξτε **Διαθέσιμη ενημέρωση**.</span><span class="sxs-lookup"><span data-stu-id="40029-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="40029-141">Επιλέξτε το πλαίσιο ελέγχου **Συμφωνώ με τους όρους παροχής υπηρεσίας** και, στη συνέχεια, επιλέξτε **Ενημέρωση**.</span><span class="sxs-lookup"><span data-stu-id="40029-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="40029-142">Θα εγκατασταθεί η πιο πρόσφατη έκδοση της λύσης.</span><span class="sxs-lookup"><span data-stu-id="40029-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="40029-143">Αφού ολοκληρωθεί η εγκατάσταση, θα έχετε εγκαταστήσει την έκδοση 4.5.0.134.</span><span class="sxs-lookup"><span data-stu-id="40029-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="40029-144">Διαμόρφωση νέων δυνατοτήτων</span><span class="sxs-lookup"><span data-stu-id="40029-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="40029-145">Ενεργοποίηση αντιστοίχισης διπλής εγγραφής</span><span class="sxs-lookup"><span data-stu-id="40029-145">Enable dual-write mapping</span></span>

<span data-ttu-id="40029-146">Αφού ολοκληρώσετε την ενημέρωση στα περιβάλλοντα Finance και Dataverse, μπορείτε να ενεργοποιήσετε τις απαιτούμενες αντιστοιχίσεις διπλής εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="40029-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="40029-147">Ολοκληρώστε τις παρακάτω διαδικασίες για να ενεργοποιήσετε τις αντιστοιχίσεις διπλής εγγραφής:</span><span class="sxs-lookup"><span data-stu-id="40029-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="40029-148">Ενημέρωση ρυθμίσεων ασφαλείας στο περιβάλλον Customer Engagement</span><span class="sxs-lookup"><span data-stu-id="40029-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="40029-149">Ανανέωση οντοτήτων δεδομένων</span><span class="sxs-lookup"><span data-stu-id="40029-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="40029-150">Ενημέρωση και εκτέλεση των αντιστοιχίσεων διπλής εγγραφής</span><span class="sxs-lookup"><span data-stu-id="40029-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="40029-151">Ενημέρωση των ρυθμίσεων ασφαλείας στο Dataverse περιβάλλον</span><span class="sxs-lookup"><span data-stu-id="40029-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="40029-152">Οι παρακάτω ενημερώσεις των δικαιωμάτων ασφαλείας για οντότητες απαιτούνται ως μέρος της ενημέρωσης σε UR5.</span><span class="sxs-lookup"><span data-stu-id="40029-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="40029-153">Στο περιβάλλον Dataverse σας, μεταβείτε στις **Ρυθμίσεις** και στην ομάδα **Σύστημα**, επιλέξτε **Ασφάλεια**.</span><span class="sxs-lookup"><span data-stu-id="40029-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Ρυθμίσεις περιβάλλοντος Dataverse](media/Picture21.png)

2. <span data-ttu-id="40029-155">Επιλέξτε **Ρόλους ασφαλείας**.</span><span class="sxs-lookup"><span data-stu-id="40029-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="40029-156">Από τη λίστα ρόλων, επιλέξτε **χρήστης εφαρμογής διπλής εγγραφής** και επιλέξτε την καρτέλα **Προσαρμοσμένες οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="40029-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="40029-157">Επαληθεύστε ότι ο ρόλος διαθέτει δικαιώματα **Ανάγνωση** και **Προσάρτηση σε**:</span><span class="sxs-lookup"><span data-stu-id="40029-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="40029-158">**Τύπος συναλλαγματικής ισοτιμίας**</span><span class="sxs-lookup"><span data-stu-id="40029-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="40029-159">**Γράφημα λογαριασμών**</span><span class="sxs-lookup"><span data-stu-id="40029-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="40029-160">**Οικονομικό ημερολόγιο**</span><span class="sxs-lookup"><span data-stu-id="40029-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="40029-161">**Καθολικό**</span><span class="sxs-lookup"><span data-stu-id="40029-161">**Ledger**</span></span>

5. <span data-ttu-id="40029-162">Μετά την ενημέρωση του ρόλου ασφαλείας, μεταβείτε στην επιλογή **Ρυθμίσεις** > **Ασφάλεια** > **Ομάδες**.</span><span class="sxs-lookup"><span data-stu-id="40029-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="40029-163">Επαληθεύστε ότι ο ρόλος **χρήστης εφαρμογής διπλής εγγραφής** έχει εφαρμοστεί στην ομάδα.</span><span class="sxs-lookup"><span data-stu-id="40029-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="40029-164">Ανανέωση οντοτήτων δεδομένων από την ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="40029-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="40029-165">Στο περιβάλλον Finance, ανοίξτε τον χώρο εργασίας **Διαχείριση δεδομένων** και, στη συνέχεια, ανοίξτε τη σελίδα **Παράμετροι πλαισίου**.</span><span class="sxs-lookup"><span data-stu-id="40029-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="40029-166">Στην καρτέλα **Ρυθμίσεις οντότητας**, επιλέξτε **Ανανέωση λίστας οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="40029-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="40029-167">Επιλέξτε **Κλείσιμο** για επιβεβαίωση της ανανέωσης της οντότητας.</span><span class="sxs-lookup"><span data-stu-id="40029-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="40029-168">Αυτή η διαδικασία θα διαρκέσει περίπου 20 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="40029-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="40029-169">Θα ειδοποιηθείτε όταν ολοκληρωθεί η ανανέωση.</span><span class="sxs-lookup"><span data-stu-id="40029-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="40029-170">Ενημέρωση αντιστοιχίσεων διπλής εγγραφής</span><span class="sxs-lookup"><span data-stu-id="40029-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="40029-171">Στο χώρο εργασίας **Διαχείριση δεδομένων**, επιλέξτε **Διπλή εγγραφή**.</span><span class="sxs-lookup"><span data-stu-id="40029-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="40029-172">Επιλέξτε **Εφαρμογή λύσεων**, επιλέξτε και τις δύο λύσεις από τη λίστα και, στη συνέχεια, επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="40029-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="40029-173">Στη σελίδα **Διπλή εγγραφή** επιλέξτε τις παρακάτω αντιστοιχίσεις πίνακα και, στη συνέχεια, επιλέξτε **Διακοπή**.</span><span class="sxs-lookup"><span data-stu-id="40029-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="40029-174">**Πραγματικές τιμές ενοποίησης Project Operations (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="40029-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="40029-175">**Κατηγορίες δαπανών έργου ενοποίησης Project Operations (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="40029-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="40029-176">**Οντότητα εξαγωγής πραγματικών δαπανών έργου ενοποίησης Project Operations (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="40029-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="40029-177">Στη σελίδα **Έκδοση χάρτη πίνακα**, εφαρμόστε μια νέα έκδοση του χάρτη σε καθεμία από τις τρεις οντότητες.</span><span class="sxs-lookup"><span data-stu-id="40029-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="40029-178">Στη σελίδα **Διπλή εγγραφή** επιλέξτε εκτέλεση για επανεκκίνηση των αντιστοιχίσεων.</span><span class="sxs-lookup"><span data-stu-id="40029-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="40029-179">Από τη λίστα χαρτών, επιλέξτε την αντιστοίχιση **Καθολικό (msdyn_ledgers)** με όλες τις προϋποθέσεις και επιλέξτε το πλαίσιο ελέγχου **Αρχικός συγχρονισμός**.</span><span class="sxs-lookup"><span data-stu-id="40029-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="40029-180">Στο πεδίο **Κύρια για αρχικό συγχρονισμό**, επιλέξτε **Εφαρμογές Finance and Operations** και στη συνέχεια, επιλέξτε **Εκτέλεση**.</span><span class="sxs-lookup"><span data-stu-id="40029-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![Συγχρονισμός αντιστοίχισης καθολικού](media/DW6.png)
 
