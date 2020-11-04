---
title: Παροχή ενός νέου περιβάλλοντος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την παροχή ενός νέου περιβάλλοντος Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a43b947207b6d4276ef27ec996713bf3883e7906
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076803"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="56d08-103">Παροχή ενός νέου περιβάλλοντος</span><span class="sxs-lookup"><span data-stu-id="56d08-103">Provision a new environment</span></span>

<span data-ttu-id="56d08-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="56d08-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="56d08-105">Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο παροχής ενός νέου περιβάλλοντος Dynamics 365 Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.</span><span class="sxs-lookup"><span data-stu-id="56d08-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="56d08-106">Ενεργοποίηση αυτόματης παροχής Project Operations σε ένα έργο LCS</span><span class="sxs-lookup"><span data-stu-id="56d08-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="56d08-107">Χρησιμοποιήστε τα παρακάτω βήματα για να ενεργοποιήσετε την αυτοματοποιημένη ροή παροχής Project Operations για το έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="56d08-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="56d08-108">Μεταβείτε στο [LCS](https://lcs.dynamics.com/v2) και επιλέξτε το πλακίδιο **Διαχείριση δυνατοτήτων προεπισκόπησης**.</span><span class="sxs-lookup"><span data-stu-id="56d08-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="56d08-109">Στη λίστα **Δυνατότητα προεπισκόπησης** , επιλέξτε **Δυνατότητα Project Operations** και **Η δυνατότητα προεπισκόπησης έχει ενεργοποιηθεί** για την ενεργοποίηση του Project Operations.</span><span class="sxs-lookup"><span data-stu-id="56d08-109">In the **Preview feature** list, select **Project Operations Feature** , and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="56d08-110">Αυτό το βήμα εκτελείται μόνο μία φορά ανά έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="56d08-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="56d08-111">Παροχή περιβάλλοντος Project Operations</span><span class="sxs-lookup"><span data-stu-id="56d08-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="56d08-112">Ανοίξτε ένα νέο Dynamics 365 Finance [περιβάλλον επίδειξης](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) ή μια ανάπτυξη [περιβάλλοντος προστατευμένης εκτέλεσης / παραγωγής](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="56d08-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="56d08-113">Περιηγηθείτε στον οδηγό **Παροχής περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="56d08-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="56d08-114">Βεβαιωθείτε ότι η επιλεγμένη έκδοση της εφαρμογής είναι 10.0.13 ή μεταγενέστερη.</span><span class="sxs-lookup"><span data-stu-id="56d08-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="56d08-115">Για την παροχή του Project Operations, στην περιοχή **Ρυθμίσεις για προχωρημένους** , επιλέξτε **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="56d08-115">To provision Project Operations, under **Advance settings** , select **Common Data Service**.</span></span> 
4. <span data-ttu-id="56d08-116">Ενεργοποιήστε τη **Ρύθμιση Common Data Service** επιλέγοντας **Ναι** και, στη συνέχεια, καταχωρίστε πληροφορίες στα απαιτούμενα πεδία:</span><span class="sxs-lookup"><span data-stu-id="56d08-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="56d08-117">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="56d08-117">Name</span></span>
  - <span data-ttu-id="56d08-118">Περιοχή</span><span class="sxs-lookup"><span data-stu-id="56d08-118">Region</span></span>
  - <span data-ttu-id="56d08-119">Γλώσσα</span><span class="sxs-lookup"><span data-stu-id="56d08-119">Language</span></span>
  - <span data-ttu-id="56d08-120">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="56d08-120">Currency</span></span>
 
5. <span data-ttu-id="56d08-121">Στο πεδίο **Πρότυπο Common Data Service** , επιλέξτε **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="56d08-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="56d08-122">Επιλέξτε τον τύπο περιβάλλοντος για την ανάπτυξή σας.</span><span class="sxs-lookup"><span data-stu-id="56d08-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="56d08-123">Μια δοκιμαστική έκδοση με συνδρομή θα σας επιτρέψει να αναπτύξετε ένα περιβάλλον CDS για 30 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="56d08-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Ρυθμίσεις ανάπτυξης](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="56d08-125">Επιλέξτε **Συμφωνώ** για αποδοχή των όρων της υπηρεσίας και, στη συνέχεια, επιλέξτε **Τέλος** για να επιστρέψετε στις ρυθμίσεις ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="56d08-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Συναίνεση ανάπτυξης](./media/2DeploymentConsent.png)

7. <span data-ttu-id="56d08-127">Συμπληρώστε τα υπόλοιπα απαιτούμενα πεδία στον οδηγό και επιβεβαιώστε την ανάπτυξη.</span><span class="sxs-lookup"><span data-stu-id="56d08-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="56d08-128">Ο χρόνος παροχής περιβάλλοντος ποικίλλει ανάλογα με τον τύπο περιβάλλοντος.</span><span class="sxs-lookup"><span data-stu-id="56d08-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="56d08-129">Η παροχή μπορεί να διαρκέσει έως και έξι ώρες.</span><span class="sxs-lookup"><span data-stu-id="56d08-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="56d08-130">Αφού ολοκληρωθεί με επιτυχία η ανάπτυξη, το περιβάλλον θα εμφανίζεται ως **Αναπτυγμένο**.</span><span class="sxs-lookup"><span data-stu-id="56d08-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="56d08-131">Για να επιβεβαιώσετε ότι το περιβάλλον έχει αναπτυχθεί με επιτυχία, επιλέξτε το στοιχείο **Σύνδεση** και συνδεθείτε στο περιβάλλον για επιβεβαίωση.</span><span class="sxs-lookup"><span data-stu-id="56d08-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Λεπτομέρειες περιβάλλοντος ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="56d08-133">Εφαρμογή των δεδομένων επίδειξης Project Operations Finance (προαιρετικό βήμα)</span><span class="sxs-lookup"><span data-stu-id="56d08-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="56d08-134">Εφαρμόστε τα δεδομένα επίδειξης του Project Operations Finance σε έκδοση υπηρεσίας 10.0.13 του φιλοξενούμενου περιβάλλοντος όπως περιγράφεται σε [αυτό το άρθρο](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="56d08-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="56d08-135">Εφαρμογή ενημερώσεων στο περιβάλλον Finance</span><span class="sxs-lookup"><span data-stu-id="56d08-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="56d08-136">Για το Project Operations απαιτείται ένα Finance περιβάλλον με έκδοση εφαρμογής **10.0.13 (10.0.569.20009)** ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="56d08-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="56d08-137">Μπορεί να χρειαστεί να εφαρμόσετε ενημερωμένες εκδόσεις ποιότητας στο περιβάλλον Finance για να λάβετε αυτήν την έκδοση.</span><span class="sxs-lookup"><span data-stu-id="56d08-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="56d08-138">Στο LCS, στη σελίδα **Λεπτομέρειες περιβάλλοντος** , στην ενότητα **Διαθέσιμες ενημερώσεις** , επιλέξτε **Προβολή ενημέρωσης**.</span><span class="sxs-lookup"><span data-stu-id="56d08-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Προβολή ενημερώσεων](./media/5ViewUpdates.png)

2. <span data-ttu-id="56d08-140">Στη σελίδα **Δυαδικές ενημερώσεις** , επιλέξτε **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="56d08-140">On the **Binary updates** page, select **Save package.**</span></span>

![Αποθήκευση πακέτου](./media/6SavePackage.png)

3. <span data-ttu-id="56d08-142">Επιλέξτε **Επιλογή όλων** και μετά **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="56d08-142">Click **Select all** and then select **Save package**.</span></span>

![Έλεγχος και αποθήκευση ενημερώσεων](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="56d08-144">Καταχωρίστε ένα όνομα και μια περιγραφή του πακέτου και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="56d08-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="56d08-145">Ανάλογα με τη σύνδεση στο Internet, αυτή η διαδικασία μπορεί να διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="56d08-145">Depending on the internet connection, this process might take some time.</span></span>

![Αποστολή πακέτου στη βιβλιοθήκη παγίων στοιχείων](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="56d08-147">Μετά την αποθήκευση του πακέτου, επιλέξτε **Τέλος** και αποθηκεύστε αυτό το πακέτο στη βιβλιοθήκη παγίων στοιχείων του έργου σας στο LCS.</span><span class="sxs-lookup"><span data-stu-id="56d08-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="56d08-148">Η αποθήκευση και η επικύρωση του πακέτου μπορεί να διαρκέσει ~ 15 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="56d08-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="56d08-149">Για να εφαρμόσετε την ενημέρωση, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος** στο LCS και επιλέξτε **Συντήρηση** > **Εφαρμογή ενημερώσεων**.</span><span class="sxs-lookup"><span data-stu-id="56d08-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Διατήρηση περιβαλλόντων](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="56d08-151">Στη λίστα ενημερωμένων εκδόσεων, επιλέξτε το πακέτο που δημιουργήσατε και επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="56d08-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Εφαρμογή ενημερώσεων](./media/10ApplyUpdates.png)

<span data-ttu-id="56d08-153">Η εξυπηρέτηση περιβάλλοντος θα διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="56d08-153">Environment servicing will take some time.</span></span> <span data-ttu-id="56d08-154">Αφού ολοκληρωθεί, το περιβάλλον θα επιστρέψει σε μια αναπτυγμένη κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="56d08-154">After it is complete, the environment will return to a deployed state.</span></span>

![Ανεπτυγμένο περιβάλλον](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="56d08-156">Δημιουργία σύνδεσης διπλής εγγραφής</span><span class="sxs-lookup"><span data-stu-id="56d08-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="56d08-157">Στο έργο σας LCS, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="56d08-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="56d08-158">Στην περιοχή **Πληροφορίες περιβάλλοντος Common Data Service** , επιλέξτε **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="56d08-158">Under **Common Data Service Environment Information** , select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="56d08-159">Αφού ολοκληρωθεί η σύνδεση, επιλέξτε ξανά **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="56d08-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="56d08-160">Θα ανακατευθυνθείτε για διπλή εγγραφή στο Finance.</span><span class="sxs-lookup"><span data-stu-id="56d08-160">You will be redirected to Dual Write in Finance.</span></span>

![Σύνδεση προς το CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="56d08-162">Επιλέξτε **Εφαρμογή λύσης** για να αποκτήσετε πρόσβαση στις οντότητες που θα αντιστοιχιστούν στην ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="56d08-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Εφαρμογή λύσεων](./media/13ApplySolutions.png)

5. <span data-ttu-id="56d08-164">Επιλέξτε και τις δύο λύσεις, **Αντιστοίχιση οντότητας διπλής εγγραφής Dynamics 365 Finance and Operations** και **Αντιστοιχίσεις οντότητας διπλής εγγραφής Dynamics 365 Project Operations** και, στη συνέχεια, επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="56d08-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps** , and then select **Apply**.</span></span>

![Επιβεβαίωση λύσεων](./media/14ConfirmSolutions.png)

<span data-ttu-id="56d08-166">Αφού εφαρμοστούν οι λύσεις, οι οντότητες διπλής εγγραφής εφαρμόζονται στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="56d08-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Εφαρμογή λύσεων](./media/15ApplyingSolutions.png)

<span data-ttu-id="56d08-168">Αφού εφαρμοστούν οι οντότητες, όλες οι διαθέσιμες αντιστοιχίσεις παρατίθενται στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="56d08-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Αντιστοιχίσεις διπλής εγγραφής](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="56d08-170">Ανανέωση των οντοτήτων δεδομένων μετά την ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="56d08-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="56d08-171">Στο Finance, μεταβείτε στον χώρο εργασίας **Διαχείριση δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="56d08-171">In Finance, go to the **Data management** workspace.</span></span>

![Χώρος εργασίας διαχείρισης δεδομένων](./media/16DataManagement.png)

2. <span data-ttu-id="56d08-173">Επιλέξτε το πλακίδιο **Παράμετροι πλαισίου**.</span><span class="sxs-lookup"><span data-stu-id="56d08-173">Select the **Framework parameters** tile.</span></span>

![Παράμετροι πλαισίου](./media/17FrameworkParameters.png)

3. <span data-ttu-id="56d08-175">Στη σελίδα **Ρυθμίσεις οντότητας** , επιλέξτε **Ανανέωση λίστας οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="56d08-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Ανανέωση λίστας οντοτήτων](./media/18RefreshEntityList.png)

<span data-ttu-id="56d08-177">Η ανανέωση θα διαρκέσει περίπου 20 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="56d08-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="56d08-178">Όταν ολοκληρωθεί, θα λάβετε μια ειδοποίηση.</span><span class="sxs-lookup"><span data-stu-id="56d08-178">You will receive an alert when it is complete.</span></span>

![Επιβεβαίωση ανανέωσης](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="56d08-180">Εκτέλεση αντιστοιχίσεων διπλής εγγραφής Project Operations</span><span class="sxs-lookup"><span data-stu-id="56d08-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="56d08-181">Στο έργο σας LCS, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="56d08-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="56d08-182">Στην περιοχή **Πληροφορίες περιβάλλοντος Common Data Service** , επιλέξτε **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="56d08-182">Under **Common Data Service Environment Information** , select **Link to CDS for Apps.**</span></span> <span data-ttu-id="56d08-183">Αφού επιλέξετε τη σύνδεση, θα ανακατευθυνθείτε στη λίστα με τις οντότητες στις αντιστοιχίσεις.</span><span class="sxs-lookup"><span data-stu-id="56d08-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="56d08-184">Ξεκινήστε τις αντιστοιχίσεις όπως περιγράφεται στον ακόλουθο πίνακα.</span><span class="sxs-lookup"><span data-stu-id="56d08-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="56d08-185">Βεβαιωθείτε ότι έχετε ακολουθήσει την ακολουθία όπως εμφανίζεται στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="56d08-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="56d08-186">**Αντιστοίχιση οντότητας**</span><span class="sxs-lookup"><span data-stu-id="56d08-186">**Entity Map**</span></span> | <span data-ttu-id="56d08-187">**Ανανέωση οντότητας**</span><span class="sxs-lookup"><span data-stu-id="56d08-187">**Refresh entity**</span></span> | <span data-ttu-id="56d08-188">**Αρχικός συγχρονισμός**</span><span class="sxs-lookup"><span data-stu-id="56d08-188">**Initial sync**</span></span> | <span data-ttu-id="56d08-189">**Κύρια για αρχικό συγχρονισμό**</span><span class="sxs-lookup"><span data-stu-id="56d08-189">**Master for initial sync**</span></span> | <span data-ttu-id="56d08-190">**Προϋποθέσεις εκτέλεσης**</span><span class="sxs-lookup"><span data-stu-id="56d08-190">**Run prerequisites**</span></span> | <span data-ttu-id="56d08-191">**Προϋποθέσεις για αρχικό συγχρονισμό**</span><span class="sxs-lookup"><span data-stu-id="56d08-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="56d08-192">**Ρόλοι πόρων έργου για όλες τις εταιρείες (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="56d08-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="56d08-193">No</span><span class="sxs-lookup"><span data-stu-id="56d08-193">No</span></span> | <span data-ttu-id="56d08-194">Ναι</span><span class="sxs-lookup"><span data-stu-id="56d08-194">Yes</span></span> | <span data-ttu-id="56d08-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="56d08-195">Common Data Service</span></span> | <span data-ttu-id="56d08-196">No</span><span class="sxs-lookup"><span data-stu-id="56d08-196">No</span></span> | <span data-ttu-id="56d08-197">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-197">N\A</span></span> |
| <span data-ttu-id="56d08-198">**Νομικές οντότητες (cdm\_εταιρείες)**</span><span class="sxs-lookup"><span data-stu-id="56d08-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="56d08-199">No</span><span class="sxs-lookup"><span data-stu-id="56d08-199">No</span></span> | <span data-ttu-id="56d08-200">Ναι</span><span class="sxs-lookup"><span data-stu-id="56d08-200">Yes</span></span> | <span data-ttu-id="56d08-201">Εφαρμογές Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="56d08-201">Finance and Operations apps</span></span> | <span data-ttu-id="56d08-202">No</span><span class="sxs-lookup"><span data-stu-id="56d08-202">No</span></span> | <span data-ttu-id="56d08-203">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-203">N\A</span></span> |
| <span data-ttu-id="56d08-204">**Πραγματικές τιμές ενοποίησης Project Operations (msdyn\_πραγματικές τιμές)**</span><span class="sxs-lookup"><span data-stu-id="56d08-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="56d08-205">No</span><span class="sxs-lookup"><span data-stu-id="56d08-205">No</span></span> | <span data-ttu-id="56d08-206">No</span><span class="sxs-lookup"><span data-stu-id="56d08-206">No</span></span> | <span data-ttu-id="56d08-207">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-207">N\A</span></span> | <span data-ttu-id="56d08-208">Ναι</span><span class="sxs-lookup"><span data-stu-id="56d08-208">Yes</span></span> | <span data-ttu-id="56d08-209">No</span><span class="sxs-lookup"><span data-stu-id="56d08-209">No</span></span> |
| <span data-ttu-id="56d08-210">**Γραμμές σύμβασης βάσει έργου (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="56d08-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="56d08-211">No</span><span class="sxs-lookup"><span data-stu-id="56d08-211">No</span></span> | <span data-ttu-id="56d08-212">No</span><span class="sxs-lookup"><span data-stu-id="56d08-212">No</span></span> | <span data-ttu-id="56d08-213">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-213">N\A</span></span> | <span data-ttu-id="56d08-214">No</span><span class="sxs-lookup"><span data-stu-id="56d08-214">No</span></span> | <span data-ttu-id="56d08-215">No</span><span class="sxs-lookup"><span data-stu-id="56d08-215">No</span></span> |
| <span data-ttu-id="56d08-216">**Οντότητα ενοποίησης για σχέσεις συναλλαγών έργου (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="56d08-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="56d08-217">No</span><span class="sxs-lookup"><span data-stu-id="56d08-217">No</span></span> | <span data-ttu-id="56d08-218">No</span><span class="sxs-lookup"><span data-stu-id="56d08-218">No</span></span> | <span data-ttu-id="56d08-219">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-219">N\A</span></span> | <span data-ttu-id="56d08-220">No</span><span class="sxs-lookup"><span data-stu-id="56d08-220">No</span></span> | <span data-ttu-id="56d08-221">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-221">N\A</span></span> |
| <span data-ttu-id="56d08-222">**Ορόσημα γραμμής σύμβασης ενοποίησης Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="56d08-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="56d08-223">No</span><span class="sxs-lookup"><span data-stu-id="56d08-223">No</span></span> | <span data-ttu-id="56d08-224">No</span><span class="sxs-lookup"><span data-stu-id="56d08-224">No</span></span> | <span data-ttu-id="56d08-225">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-225">N\A</span></span> | <span data-ttu-id="56d08-226">No</span><span class="sxs-lookup"><span data-stu-id="56d08-226">No</span></span> | <span data-ttu-id="56d08-227">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-227">N\A</span></span> |
| <span data-ttu-id="56d08-228">**Οντότητα ενοποίησης Project Operations για εκτιμήσεις δαπανών (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="56d08-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="56d08-229">No</span><span class="sxs-lookup"><span data-stu-id="56d08-229">No</span></span> | <span data-ttu-id="56d08-230">No</span><span class="sxs-lookup"><span data-stu-id="56d08-230">No</span></span> | <span data-ttu-id="56d08-231">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-231">N\A</span></span> | <span data-ttu-id="56d08-232">No</span><span class="sxs-lookup"><span data-stu-id="56d08-232">No</span></span> | <span data-ttu-id="56d08-233">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-233">N\A</span></span> |
| <span data-ttu-id="56d08-234">**Οντότητα εξαγωγής κατηγοριών δαπανών έργου ενοποίησης Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="56d08-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="56d08-235">No</span><span class="sxs-lookup"><span data-stu-id="56d08-235">No</span></span> | <span data-ttu-id="56d08-236">No</span><span class="sxs-lookup"><span data-stu-id="56d08-236">No</span></span> | <span data-ttu-id="56d08-237">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-237">N\A</span></span> | <span data-ttu-id="56d08-238">No</span><span class="sxs-lookup"><span data-stu-id="56d08-238">No</span></span> | <span data-ttu-id="56d08-239">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-239">N\A</span></span> |
| <span data-ttu-id="56d08-240">**Οντότητα εξαγωγής δαπανών έργου ενοποίησης Project Operations (msdyn\_έξοδα)**</span><span class="sxs-lookup"><span data-stu-id="56d08-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="56d08-241">Ναι</span><span class="sxs-lookup"><span data-stu-id="56d08-241">Yes</span></span> | <span data-ttu-id="56d08-242">No</span><span class="sxs-lookup"><span data-stu-id="56d08-242">No</span></span> | <span data-ttu-id="56d08-243">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-243">N\A</span></span> | <span data-ttu-id="56d08-244">No</span><span class="sxs-lookup"><span data-stu-id="56d08-244">No</span></span> | <span data-ttu-id="56d08-245">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-245">N\A</span></span> |
| <span data-ttu-id="56d08-246">**Οντότητα ενοποίησης Project Operations για ωριαίες εκτιμήσεις (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="56d08-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="56d08-247">Ναι</span><span class="sxs-lookup"><span data-stu-id="56d08-247">Yes</span></span> | <span data-ttu-id="56d08-248">No</span><span class="sxs-lookup"><span data-stu-id="56d08-248">No</span></span> | <span data-ttu-id="56d08-249">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-249">N\A</span></span> | <span data-ttu-id="56d08-250">No</span><span class="sxs-lookup"><span data-stu-id="56d08-250">No</span></span> | <span data-ttu-id="56d08-251">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="56d08-251">N\A</span></span> |


4. <span data-ttu-id="56d08-252">Για να ανανεώσετε την οντότητα, επιλέξτε το όνομα της αντιστοίχισης και, στη συνέχεια, επιλέξτε **Ανανέωση οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="56d08-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Ανανέωση αντιστοίχισης](./media/20RefreshMapping.png)

5. <span data-ttu-id="56d08-254">Μετά την ολοκλήρωση της ανανέωσης, εκτελέστε την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="56d08-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="56d08-255">Πριν ενεργοποιήσετε την επόμενη αντιστοίχιση, επαληθεύστε ότι η αντιστοίχιση στον πίνακα βρίσκεται σε κατάσταση **Εκτελείται**.</span><span class="sxs-lookup"><span data-stu-id="56d08-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="56d08-256">Η εκτέλεση αντιστοιχίσεων με μεγαλύτερο αριθμό προϋποθέσεων ενδέχεται να διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="56d08-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="56d08-257">Για να εκτελεστεί μια αντιστοίχιση με προϋποθέσεις, ενεργοποιήστε την εναλλαγή **Εμφάνιση σχετικών αντιστοιχίσεων οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="56d08-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="56d08-258">Εάν ο πίνακας υποδεικνύει ότι οι **Προϋποθέσεις για αρχικό συγχρονισμό** είναι **Όχι** , βεβαιωθείτε ότι η σημαία **Αρχικός συγχρονισμός** είναι **Απενεργοποιημένη** σε όλες τις προαπαιτούμενες αντιστοιχίσεις πριν να τον πραγματοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="56d08-258">If the table indicates **Prerequisite initial sync** is **No** , verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Εκτέλεση αντιστοίχισης](./media/21RunMap.png)

6. <span data-ttu-id="56d08-260">Επικυρώστε όλες τις αντιστοιχίσεις που σχετίζονται με το έργο βρίσκονται σε κατάσταση "εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="56d08-260">Validate all project related maps are in the running state.</span></span>

![Όλοι οι αντιστοιχίσεις που εκτελούνται](./media/22AllMapsRunning.png)

<span data-ttu-id="56d08-262">Το περιβάλλον Project Operations έχει πλέον δοθεί και ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="56d08-262">Your Project Operations environment is now provisioned and configured.</span></span>
