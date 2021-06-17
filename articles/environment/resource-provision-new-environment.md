---
title: Παροχή ενός νέου περιβάλλοντος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την παροχή ενός νέου περιβάλλοντος Project Operations.
author: sigitac
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d0712d9d5dfc6c35ccd07142ff5948f50e6a254c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995486"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="57dcc-103">Παροχή ενός νέου περιβάλλοντος</span><span class="sxs-lookup"><span data-stu-id="57dcc-103">Provision a new environment</span></span>

<span data-ttu-id="57dcc-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="57dcc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="57dcc-105">Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο προμήθειας ενός νέου περιβάλλοντος Dynamics 365 Project Operations για μη εφοδιασμένα σενάρια ή σενάρια βάσει πόρων.</span><span class="sxs-lookup"><span data-stu-id="57dcc-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="57dcc-106">Ενεργοποίηση αυτόματης παροχής Project Operations σε ένα έργο LCS</span><span class="sxs-lookup"><span data-stu-id="57dcc-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="57dcc-107">Χρησιμοποιήστε τα παρακάτω βήματα για να ενεργοποιήσετε την αυτοματοποιημένη ροή παροχής Project Operations για το έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="57dcc-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="57dcc-108">Μεταβείτε στο [LCS](https://lcs.dynamics.com/v2) και επιλέξτε το πλακίδιο **Διαχείριση δυνατοτήτων προεπισκόπησης**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="57dcc-109">Στη λίστα **Δυνατότητα προεπισκόπησης**, επιλέξτε **Δυνατότητα Project Operations** και **Η δυνατότητα προεπισκόπησης έχει ενεργοποιηθεί** για την ενεργοποίηση του Project Operations.</span><span class="sxs-lookup"><span data-stu-id="57dcc-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="57dcc-110">Αυτό το βήμα εκτελείται μόνο μία φορά ανά έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="57dcc-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="57dcc-111">Παροχή περιβάλλοντος Project Operations</span><span class="sxs-lookup"><span data-stu-id="57dcc-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="57dcc-112">Ανοίξτε ένα νέο Dynamics 365 Finance [περιβάλλον επίδειξης](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) ή μια ανάπτυξη [περιβάλλοντος προστατευμένης εκτέλεσης / παραγωγής](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="57dcc-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="57dcc-113">Περιηγηθείτε στον οδηγό **Παροχής περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="57dcc-114">Βεβαιωθείτε ότι η επιλεγμένη έκδοση της εφαρμογής είναι 10.0.13 ή μεταγενέστερη.</span><span class="sxs-lookup"><span data-stu-id="57dcc-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="57dcc-115">Για την παροχή του Project Operations, στην περιοχή **Ρυθμίσεις για προχωρημένους**, επιλέξτε **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="57dcc-116">Ενεργοποιήστε τη **Ρύθμιση Common Data Service** επιλέγοντας **Ναι** και, στη συνέχεια, καταχωρίστε πληροφορίες στα απαιτούμενα πεδία:</span><span class="sxs-lookup"><span data-stu-id="57dcc-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="57dcc-117">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="57dcc-117">Name</span></span>
  - <span data-ttu-id="57dcc-118">Περιοχή</span><span class="sxs-lookup"><span data-stu-id="57dcc-118">Region</span></span>
  - <span data-ttu-id="57dcc-119">Γλώσσα</span><span class="sxs-lookup"><span data-stu-id="57dcc-119">Language</span></span>
  - <span data-ttu-id="57dcc-120">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="57dcc-120">Currency</span></span>
 
5. <span data-ttu-id="57dcc-121">Στο πεδίο **Πρότυπο Common Data Service**, επιλέξτε **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="57dcc-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="57dcc-122">Επιλέξτε τον τύπο περιβάλλοντος για την ανάπτυξή σας.</span><span class="sxs-lookup"><span data-stu-id="57dcc-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="57dcc-123">Μια δοκιμαστική έκδοση με συνδρομή θα σας επιτρέψει να αναπτύξετε ένα περιβάλλον CDS για 30 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="57dcc-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Ρυθμίσεις ανάπτυξης](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="57dcc-125">Επιλέξτε **Συμφωνώ** για αποδοχή των όρων της υπηρεσίας και, στη συνέχεια, επιλέξτε **Τέλος** για να επιστρέψετε στις ρυθμίσεις ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="57dcc-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Συναίνεση ανάπτυξης](./media/2DeploymentConsent.png)

7. <span data-ttu-id="57dcc-127">Προαιρετικό - Εφαρμογή δεδομένων επίδειξης στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="57dcc-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="57dcc-128">Μεταβείτε στην επιλογή **Ρυθμίσεις για προχωρημένους**, επιλέξτε **Προσαρμογή ρύθμισης παραμέτρων βάσης δεδομένων SQL** και ορίστε το στοιχείο **Καθορισμός συνόλου δεδομένων για τη βάση δεδομένων εφαρμογών** σε **Επίδειξη**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="57dcc-129">Συμπληρώστε τα υπόλοιπα απαιτούμενα πεδία στον οδηγό και επιβεβαιώστε την ανάπτυξη.</span><span class="sxs-lookup"><span data-stu-id="57dcc-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="57dcc-130">Ο χρόνος για την παροχή του περιβάλλοντος ποικίλλει ανάλογα με τον τύπο του περιβάλλοντος.</span><span class="sxs-lookup"><span data-stu-id="57dcc-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="57dcc-131">Η παροχή μπορεί να διαρκέσει έως και έξι ώρες.</span><span class="sxs-lookup"><span data-stu-id="57dcc-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="57dcc-132">Αφού ολοκληρωθεί με επιτυχία η ανάπτυξη, το περιβάλλον θα εμφανίζεται ως **Αναπτυγμένο**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="57dcc-133">Για να επιβεβαιώσετε ότι το περιβάλλον έχει αναπτυχθεί με επιτυχία, επιλέξτε **Σύνδεση** και συνδεθείτε στο περιβάλλον για επιβεβαίωση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Λεπτομέρειες περιβάλλοντος ](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="57dcc-135">Εφαρμογή ενημερώσεων στο περιβάλλον Finance</span><span class="sxs-lookup"><span data-stu-id="57dcc-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="57dcc-136">Για το Project Operations απαιτείται ένα Finance περιβάλλον με έκδοση εφαρμογής **10.0.13 (10.0.569.20009)** ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="57dcc-137">Μπορεί να χρειαστεί να εφαρμόσετε ενημερωμένες εκδόσεις ποιότητας στο περιβάλλον Finance για να λάβετε αυτήν την έκδοση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="57dcc-138">Στο LCS, στη σελίδα **Λεπτομέρειες περιβάλλοντος**, στην ενότητα **Διαθέσιμες ενημερώσεις**, επιλέξτε **Προβολή ενημέρωσης**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Προβολή ενημερώσεων](./media/5ViewUpdates.png)

2. <span data-ttu-id="57dcc-140">Στη σελίδα **Δυαδικές ενημερώσεις**, επιλέξτε **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-140">On the **Binary updates** page, select **Save package.**</span></span>

![Αποθήκευση πακέτου](./media/6SavePackage.png)

3. <span data-ttu-id="57dcc-142">Επιλέξτε **Επιλογή όλων** και μετά **Αποθήκευση πακέτου**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-142">Click **Select all** and then select **Save package**.</span></span>

![Έλεγχος και αποθήκευση ενημερώσεων](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="57dcc-144">Καταχωρίστε ένα όνομα και μια περιγραφή του πακέτου και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="57dcc-145">Ανάλογα με τη σύνδεση στο Internet, αυτή η διαδικασία μπορεί να διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="57dcc-145">Depending on the internet connection, this process might take some time.</span></span>

![Αποστολή πακέτου στη βιβλιοθήκη παγίων στοιχείων](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="57dcc-147">Μετά την αποθήκευση του πακέτου, επιλέξτε **Τέλος** και αποθηκεύστε αυτό το πακέτο στη βιβλιοθήκη παγίων στοιχείων του έργου σας στο LCS.</span><span class="sxs-lookup"><span data-stu-id="57dcc-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="57dcc-148">Η αποθήκευση και η επικύρωση του πακέτου μπορεί να διαρκέσει ~ 15 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="57dcc-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="57dcc-149">Για να εφαρμόσετε την ενημέρωση, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος** στο LCS και επιλέξτε **Συντήρηση** > **Εφαρμογή ενημερώσεων**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Διατήρηση περιβαλλόντων](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="57dcc-151">Στη λίστα ενημερωμένων εκδόσεων, επιλέξτε το πακέτο που δημιουργήσατε και επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Εφαρμογή ενημερώσεων](./media/10ApplyUpdates.png)

<span data-ttu-id="57dcc-153">Η εξυπηρέτηση περιβάλλοντος θα διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="57dcc-153">Environment servicing will take some time.</span></span> <span data-ttu-id="57dcc-154">Αφού ολοκληρωθεί, το περιβάλλον θα επιστρέψει σε μια αναπτυγμένη κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-154">After it is complete, the environment will return to a deployed state.</span></span>

![Ανεπτυγμένο περιβάλλον](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="57dcc-156">Δημιουργία σύνδεσης διπλής εγγραφής</span><span class="sxs-lookup"><span data-stu-id="57dcc-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="57dcc-157">Στο έργο σας LCS, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="57dcc-158">Στην περιοχή **Πληροφορίες περιβάλλοντος Common Data Service**, επιλέξτε **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="57dcc-159">Αφού ολοκληρωθεί η σύνδεση, επιλέξτε ξανά **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="57dcc-160">Θα ανακατευθυνθείτε για διπλή εγγραφή στο Finance.</span><span class="sxs-lookup"><span data-stu-id="57dcc-160">You will be redirected to Dual Write in Finance.</span></span>

![Σύνδεση προς το CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="57dcc-162">Επιλέξτε **Εφαρμογή λύσης** για να αποκτήσετε πρόσβαση στις οντότητες που θα αντιστοιχιστούν στην ενοποίηση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Εφαρμογή λύσεων](./media/13ApplySolutions.png)

5. <span data-ttu-id="57dcc-164">Επιλέξτε και τις δύο λύσεις, τον **Χάρτη οντοτήτων διπλής γραφής Dynamics 365 Finance and Operations** και **Χάρτες οντοτήτων διπλής γραφής Dynamics 365 Project Operations** και, στη συνέχεια, επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Επιβεβαίωση λύσεων](./media/14ConfirmSolutions.png)

<span data-ttu-id="57dcc-166">Αφού εφαρμοστούν οι λύσεις, οι οντότητες διπλής εγγραφής εφαρμόζονται στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="57dcc-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Εφαρμογή λύσεων](./media/15ApplyingSolutions.png)

<span data-ttu-id="57dcc-168">Αφού εφαρμοστούν οι οντότητες, όλες οι διαθέσιμες αντιστοιχίσεις παρατίθενται στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="57dcc-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Αντιστοιχίσεις διπλής εγγραφής](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="57dcc-170">Ανανέωση των οντοτήτων δεδομένων μετά την ενημέρωση</span><span class="sxs-lookup"><span data-stu-id="57dcc-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="57dcc-171">Στο Finance, μεταβείτε στον χώρο εργασίας **Διαχείριση δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-171">In Finance, go to the **Data management** workspace.</span></span>

![Χώρος εργασίας διαχείρισης δεδομένων](./media/16DataManagement.png)

2. <span data-ttu-id="57dcc-173">Επιλέξτε το πλακίδιο **Παράμετροι πλαισίου**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-173">Select the **Framework parameters** tile.</span></span>

![Παράμετροι πλαισίου](./media/17FrameworkParameters.png)

3. <span data-ttu-id="57dcc-175">Στη σελίδα **Ρυθμίσεις οντότητας**, επιλέξτε **Ανανέωση λίστας οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Ανανέωση λίστας οντοτήτων](./media/18RefreshEntityList.png)

<span data-ttu-id="57dcc-177">Η ανανέωση θα διαρκέσει περίπου 20 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="57dcc-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="57dcc-178">Όταν ολοκληρωθεί, θα λάβετε μια ειδοποίηση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-178">You will receive an alert when it is complete.</span></span>

![Επιβεβαίωση ανανέωσης](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="57dcc-180">Ενημέρωση ρυθμίσεων ασφαλείας στο Project Operations στο Dataverse</span><span class="sxs-lookup"><span data-stu-id="57dcc-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="57dcc-181">Μεταβείτε στο Project Operations στο περιβάλλον Dataverse.</span><span class="sxs-lookup"><span data-stu-id="57dcc-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="57dcc-182">Επιλέξτε **Ρυθμίσεις** > **Ασφάλεια** > **Ρόλοι ασφαλείας**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="57dcc-183">Από τη σελίδα **Ρόλοι ασφαλείας**, επιλέξτε **χρήστης εφαρμογής διπλής εγγραφής** και επιλέξτε την καρτέλα **Προσαρμοσμένες οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="57dcc-184">Επαληθεύστε ότι ο ρόλος διαθέτει δικαιώματα **Ανάγνωση** και **Προσάρτηση σε**:</span><span class="sxs-lookup"><span data-stu-id="57dcc-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="57dcc-185">**Τύπος συναλλαγματικής ισοτιμίας**</span><span class="sxs-lookup"><span data-stu-id="57dcc-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="57dcc-186">**Γράφημα λογαριασμών**</span><span class="sxs-lookup"><span data-stu-id="57dcc-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="57dcc-187">**Οικονομικό ημερολόγιο**</span><span class="sxs-lookup"><span data-stu-id="57dcc-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="57dcc-188">**Καθολικό**</span><span class="sxs-lookup"><span data-stu-id="57dcc-188">**Ledger**</span></span>

5. <span data-ttu-id="57dcc-189">Μετά την ενημέρωση του ρόλου ασφαλείας, μεταβείτε στις **Ρυθμίσεις** > **Ασφάλεια** > **Ομάδες** και επιλέξτε την προεπιλεγμένη ομάδα στην προβολή ομάδας **Τοπικός επιχειρηματικός κάτοχος**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="57dcc-190">Επιλέξτε **Διαχείριση ρόλων** και επιβεβαιώστε ότι το προνόμιο ασφαλείας χρήστη της **εφαρμογής διπλής εγγραφής** εφαρμόζεται σε αυτήν την ομάδα.</span><span class="sxs-lookup"><span data-stu-id="57dcc-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="57dcc-191">Εκτέλεση αντιστοιχίσεων διπλής εγγραφής Project Operations</span><span class="sxs-lookup"><span data-stu-id="57dcc-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="57dcc-192">Στο έργο σας LCS, μεταβείτε στη σελίδα **Λεπτομέρειες περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="57dcc-193">Στην περιοχή **Πληροφορίες περιβάλλοντος Common Data Service**, επιλέξτε **Σύνδεση σε CD για εφαρμογές**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="57dcc-194">Αφού επιλέξετε τη σύνδεση, θα ανακατευθυνθείτε στη λίστα με τις οντότητες στις αντιστοιχίσεις.</span><span class="sxs-lookup"><span data-stu-id="57dcc-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="57dcc-195">Ξεκινήστε τις αντιστοιχίσεις όπως περιγράφεται στον ακόλουθο πίνακα.</span><span class="sxs-lookup"><span data-stu-id="57dcc-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="57dcc-196">Βεβαιωθείτε ότι έχετε ακολουθήσει την ακολουθία όπως εμφανίζεται στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="57dcc-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="57dcc-197">**Αντιστοίχιση οντότητας**</span><span class="sxs-lookup"><span data-stu-id="57dcc-197">**Entity Map**</span></span> | <span data-ttu-id="57dcc-198">**Ανανέωση οντότητας**</span><span class="sxs-lookup"><span data-stu-id="57dcc-198">**Refresh entity**</span></span> | <span data-ttu-id="57dcc-199">**Αρχικός συγχρονισμός**</span><span class="sxs-lookup"><span data-stu-id="57dcc-199">**Initial sync**</span></span> | <span data-ttu-id="57dcc-200">**Κύρια για αρχικό συγχρονισμό**</span><span class="sxs-lookup"><span data-stu-id="57dcc-200">**Master for initial sync**</span></span> | <span data-ttu-id="57dcc-201">**Προϋποθέσεις εκτέλεσης**</span><span class="sxs-lookup"><span data-stu-id="57dcc-201">**Run prerequisites**</span></span> | <span data-ttu-id="57dcc-202">**Προϋποθέσεις για αρχικό συγχρονισμό**</span><span class="sxs-lookup"><span data-stu-id="57dcc-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="57dcc-203">**Ρόλοι πόρων έργου για όλες τις εταιρείες (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="57dcc-204">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-204">No</span></span> | <span data-ttu-id="57dcc-205">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-205">Yes</span></span> | <span data-ttu-id="57dcc-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="57dcc-206">Common Data Service</span></span> | <span data-ttu-id="57dcc-207">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-207">No</span></span> | <span data-ttu-id="57dcc-208">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-208">N\A</span></span> |
| <span data-ttu-id="57dcc-209">**Νομικές οντότητες (cdm\_εταιρείες)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="57dcc-210">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-210">No</span></span> | <span data-ttu-id="57dcc-211">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-211">Yes</span></span> | <span data-ttu-id="57dcc-212">Εφαρμογές Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="57dcc-212">Finance and Operations apps</span></span> | <span data-ttu-id="57dcc-213">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-213">No</span></span> | <span data-ttu-id="57dcc-214">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-214">N\A</span></span> |
| <span data-ttu-id="57dcc-215">**Καθολικό (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="57dcc-216">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-216">No</span></span> | <span data-ttu-id="57dcc-217">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-217">Yes</span></span> | <span data-ttu-id="57dcc-218">Εφαρμογές Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="57dcc-218">Finance and Operations apps</span></span> | <span data-ttu-id="57dcc-219">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-219">Yes</span></span> | <span data-ttu-id="57dcc-220">Ναι, εφαρμογές Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="57dcc-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="57dcc-221">**Πραγματικές τιμές ενοποίησης Project Operations (msdyn\_πραγματικές τιμές)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="57dcc-222">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-222">No</span></span> | <span data-ttu-id="57dcc-223">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-223">No</span></span> | <span data-ttu-id="57dcc-224">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-224">N\A</span></span> | <span data-ttu-id="57dcc-225">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-225">Yes</span></span> | <span data-ttu-id="57dcc-226">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-226">No</span></span> |
| <span data-ttu-id="57dcc-227">**Γραμμές σύμβασης βάσει έργου (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="57dcc-228">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-228">No</span></span> | <span data-ttu-id="57dcc-229">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-229">No</span></span> | <span data-ttu-id="57dcc-230">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-230">N\A</span></span> | <span data-ttu-id="57dcc-231">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-231">No</span></span> | <span data-ttu-id="57dcc-232">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-232">No</span></span> |
| <span data-ttu-id="57dcc-233">**Οντότητα ενοποίησης για σχέσεις συναλλαγών έργου (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="57dcc-234">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-234">No</span></span> | <span data-ttu-id="57dcc-235">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-235">No</span></span> | <span data-ttu-id="57dcc-236">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-236">N\A</span></span> | <span data-ttu-id="57dcc-237">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-237">No</span></span> | <span data-ttu-id="57dcc-238">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-238">N\A</span></span> |
| <span data-ttu-id="57dcc-239">**Ορόσημα γραμμής σύμβασης ενοποίησης Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="57dcc-240">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-240">No</span></span> | <span data-ttu-id="57dcc-241">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-241">No</span></span> | <span data-ttu-id="57dcc-242">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-242">N\A</span></span> | <span data-ttu-id="57dcc-243">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-243">No</span></span> | <span data-ttu-id="57dcc-244">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-244">N\A</span></span> |
| <span data-ttu-id="57dcc-245">**Οντότητα ενοποίησης Project Operations για εκτιμήσεις δαπανών (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="57dcc-246">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-246">No</span></span> | <span data-ttu-id="57dcc-247">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-247">No</span></span> | <span data-ttu-id="57dcc-248">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-248">N\A</span></span> | <span data-ttu-id="57dcc-249">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-249">No</span></span> | <span data-ttu-id="57dcc-250">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-250">N\A</span></span> |
| <span data-ttu-id="57dcc-251">**Οντότητα εξαγωγής κατηγοριών δαπανών έργου ενοποίησης Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="57dcc-252">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-252">No</span></span> | <span data-ttu-id="57dcc-253">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-253">No</span></span> | <span data-ttu-id="57dcc-254">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-254">N\A</span></span> | <span data-ttu-id="57dcc-255">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-255">No</span></span> | <span data-ttu-id="57dcc-256">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-256">N\A</span></span> |
| <span data-ttu-id="57dcc-257">**Οντότητα εξαγωγής δαπανών έργου ενοποίησης Project Operations (msdyn\_έξοδα)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="57dcc-258">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-258">Yes</span></span> | <span data-ttu-id="57dcc-259">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-259">No</span></span> | <span data-ttu-id="57dcc-260">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-260">N\A</span></span> | <span data-ttu-id="57dcc-261">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-261">No</span></span> | <span data-ttu-id="57dcc-262">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-262">N\A</span></span> |
| <span data-ttu-id="57dcc-263">**Οντότητα ενοποίησης Project Operations για ωριαίες εκτιμήσεις (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="57dcc-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="57dcc-264">Ναι</span><span class="sxs-lookup"><span data-stu-id="57dcc-264">Yes</span></span> | <span data-ttu-id="57dcc-265">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-265">No</span></span> | <span data-ttu-id="57dcc-266">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-266">N\A</span></span> | <span data-ttu-id="57dcc-267">No</span><span class="sxs-lookup"><span data-stu-id="57dcc-267">No</span></span> | <span data-ttu-id="57dcc-268">Μη διαθέσιμο</span><span class="sxs-lookup"><span data-stu-id="57dcc-268">N\A</span></span> |


4. <span data-ttu-id="57dcc-269">Για να ανανεώσετε την οντότητα, επιλέξτε το όνομα της αντιστοίχισης και, στη συνέχεια, επιλέξτε **Ανανέωση οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Ανανέωση αντιστοίχισης](./media/20RefreshMapping.png)

5. <span data-ttu-id="57dcc-271">Μετά την ολοκλήρωση της ανανέωσης, εκτελέστε την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="57dcc-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="57dcc-272">Πριν ενεργοποιήσετε την επόμενη αντιστοίχιση, επαληθεύστε ότι η αντιστοίχιση στον πίνακα βρίσκεται σε κατάσταση **Εκτελείται**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="57dcc-273">Η εκτέλεση αντιστοιχίσεων με μεγαλύτερο αριθμό προϋποθέσεων ενδέχεται να διαρκέσει αρκετό χρόνο.</span><span class="sxs-lookup"><span data-stu-id="57dcc-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="57dcc-274">Για να εκτελεστεί μια αντιστοίχιση με προϋποθέσεις, ενεργοποιήστε την εναλλαγή **Εμφάνιση σχετικών αντιστοιχίσεων οντοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="57dcc-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="57dcc-275">Εάν ο πίνακας υποδεικνύει ότι οι **Προϋποθέσεις για αρχικό συγχρονισμό** είναι **Όχι**, βεβαιωθείτε ότι η σημαία **Αρχικός συγχρονισμός** είναι **Απενεργοποιημένη** σε όλες τις προαπαιτούμενες αντιστοιχίσεις πριν να τον πραγματοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="57dcc-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Εκτέλεση αντιστοίχισης](./media/21RunMap.png)

6. <span data-ttu-id="57dcc-277">Επικυρώστε όλες τις αντιστοιχίσεις που σχετίζονται με το έργο βρίσκονται σε κατάσταση "εκτέλεση".</span><span class="sxs-lookup"><span data-stu-id="57dcc-277">Validate all project related maps are in the running state.</span></span>

![Όλοι οι αντιστοιχίσεις που εκτελούνται](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="57dcc-279">Εφαρμογή δεδομένων ρύθμισης παραμέτρων στο CDS για Project Operations (προαιρετικό)</span><span class="sxs-lookup"><span data-stu-id="57dcc-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="57dcc-280">Εάν έχετε εφαρμόσει δεδομένα επίδειξης στο περιβάλλον Finance, ανατρέξτε στο θέμα [Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service για το Project Operations](resource-apply-pro-setup-config-data.md) για εφαρμογή δεδομένων επίδειξης σε περιβάλλον CDS.</span><span class="sxs-lookup"><span data-stu-id="57dcc-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="57dcc-281">Το περιβάλλον Project Operations έχει πλέον δοθεί και ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="57dcc-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]