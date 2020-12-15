---
title: Εγγραφή για συνδρομές προεπισκόπησης του Project Operations για σενάρια πόρων/ μη εφοδιασμένα
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εγγραφής και ανάπτυξης του Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a6dfa51f59119834230b7c9f8859a9d85eaae999
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642958"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="2a105-103">Εγγραφή για συνδρομές προεπισκόπησης του Project Operations για σενάρια πόρων/ μη εφοδιασμένα</span><span class="sxs-lookup"><span data-stu-id="2a105-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="2a105-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="2a105-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="2a105-105">Αυτό το θέμα επεξηγεί τον τρόπο εγγραφής στην προσφορά προεπισκόπησης/συνεργάτη και την ανάπτυξη του περιβάλλοντος Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.</span><span class="sxs-lookup"><span data-stu-id="2a105-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a105-106">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="2a105-106">Prerequisites</span></span>

- <span data-ttu-id="2a105-107">Θα λάβετε ένα μήνυμα ηλεκτρονικού ταχυδρομείου που θα σας προσκαλεί να συμμετάσχετε στην προεπισκόπηση.</span><span class="sxs-lookup"><span data-stu-id="2a105-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="2a105-108">Μπορείτε να ζητήσετε μια προεπισκόπηση στην [τοποθεσία Web του Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="2a105-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="2a105-109">Ο χρήστης που αναπτύσσει την προεπισκόπηση πρέπει να έχει δικαιώματα καθολικού διαχειριστή μισθωτή Azure.</span><span class="sxs-lookup"><span data-stu-id="2a105-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="2a105-110">Η ανάπτυξη ενός περιβάλλοντος Finance απαιτεί μια έγκυρη συνδρομή Azure η οποία θα χρεώνεται ανά περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="2a105-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="2a105-111">Μπορείτε να χρησιμοποιήσετε την υφιστάμενη συνδρομή των οργανισμών σας ή να χρησιμοποιήσετε μια [δοκιμαστική έκδοση του Azure](https://azure.microsoft.com/en-us/free/) για να ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="2a105-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="2a105-112">Το περιβάλλον CDS θα παρέχεται δωρεάν για περιορισμένο χρονικό διάστημα 30 ημερών.</span><span class="sxs-lookup"><span data-stu-id="2a105-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="2a105-113">Συνδρομή</span><span class="sxs-lookup"><span data-stu-id="2a105-113">Subscribe</span></span>

<span data-ttu-id="2a105-114">Όταν λάβετε μια έγκριση [αιτήματος προεπισκόπησης](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u), θα λάβετε τρεις προσφορές από τη Microsoft μέσω ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="2a105-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive three offers from Microsoft by email.</span></span> <span data-ttu-id="2a105-115">Αυτές οι προσφορές σάς δίνουν τη δυνατότητα να αναπτύξετε την προεπισκόπηση του Project Operations:</span><span class="sxs-lookup"><span data-stu-id="2a105-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="2a105-116">Dynamics 365 Project Operations (CRM) - Δοκιμή έκδοσης προεπισκόπησης</span><span class="sxs-lookup"><span data-stu-id="2a105-116">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span>
- <span data-ttu-id="2a105-117">Office 365 Project Operations - Προεπισκόπηση δοκιμαστικής έκδοσης</span><span class="sxs-lookup"><span data-stu-id="2a105-117">Office 365 Project Operations - Preview Trial</span></span>
- <span data-ttu-id="2a105-118">Dynamics 365 Finance - Προεπισκόπηση δοκιμαστικής έκδοσης</span><span class="sxs-lookup"><span data-stu-id="2a105-118">Dynamics 365 Finance - Preview Trial</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2a105-119">Μόνο ένα άτομο, ο διαχειριστής μισθωτή, σε έναν οργανισμό πρέπει να εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="2a105-119">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="2a105-120">Εάν δεν είστε ο συνδρομητής σε αυτήν την έκδοση, περιμένετε έως ότου ολοκληρωθεί η εγγραφή του οργανισμού σας και λάβετε τα διαπιστευτήρια χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="2a105-120">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations-crm---preview-trial"></a><span data-ttu-id="2a105-121">Dynamics 365 Project Operations (CRM) - Δοκιμή έκδοσης προεπισκόπησης</span><span class="sxs-lookup"><span data-stu-id="2a105-121">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span> 

<span data-ttu-id="2a105-122">Πριν ξεκινήσετε, βεβαιωθείτε ότι έχετε συνδεθεί σε ένα πρόγραμμα περιήγησης με το λογαριασμό εργασίας χρήστη του μισθωτή όπου θέλετε να γίνει προεπισκόπηση του Project Operations.</span><span class="sxs-lookup"><span data-stu-id="2a105-122">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="2a105-123">Εξαργυρώστε τον κωδικό πρώτης προσφοράς, **Dynamics 365 Project Operations (CRM) - Δοκιμή έκδοσης προεπισκόπησης** επικολλώντας τον στη διεύθυνση URL του προγράμματος περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="2a105-123">Redeem the first offer code, **Dynamics 365 Project Operations (CRM) - Preview Trial** by pasting it into the browser URL.</span></span>

![Εξαργύρωση προσφοράς](./media/16RedeemFirstOfferNew.png)

2. <span data-ttu-id="2a105-125">Επιβεβαιώστε την παραγγελία σας.</span><span class="sxs-lookup"><span data-stu-id="2a105-125">Confirm your order.</span></span>

![Επιβεβαιώστε την παραγγελία](./media/17ConfirmOrderNew.png)

<span data-ttu-id="2a105-127">Θα δείτε ότι η προσφορά επιβεβαίωσης έχει εξαργυρωθεί με επιτυχία.</span><span class="sxs-lookup"><span data-stu-id="2a105-127">You will see confirmation offer was successfully redeemed.</span></span>

![Επιβεβαίωση](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a><span data-ttu-id="2a105-129">Office 365 Project Operations - Προεπισκόπηση δοκιμαστικής έκδοσης</span><span class="sxs-lookup"><span data-stu-id="2a105-129">Office 365 Project Operations - Preview Trial</span></span>

<span data-ttu-id="2a105-130">Επαναλάβετε τα ίδια βήματα όπως και με τον κωδικό πρώτης προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2a105-130">Repeat the same steps as with the first offer code.</span></span> <span data-ttu-id="2a105-131">Βεβαιωθείτε ότι έχετε προσθέσει τον κωδικό δεύτερης προσφοράς χρησιμοποιώντας τον ίδιο λογαριασμό χρήστη που χρησιμοποιήθηκε με τον κωδικό πρώτης προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2a105-131">Make sure to add the second offer code using the same user account that was used with the first offer code.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="2a105-132">Προεπισκόπηση δοκιμαστικής έκδοσης Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="2a105-132">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="2a105-133">Επαναλάβετε τα ίδια βήματα με την τελευταία προσφορά από το μήνυμα ηλεκτρονικού ταχυδρομείου υποδοχής.</span><span class="sxs-lookup"><span data-stu-id="2a105-133">Repeat the same steps with the last offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="2a105-134">Εκχώρηση αδειών χρήσης</span><span class="sxs-lookup"><span data-stu-id="2a105-134">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2a105-135">Θα χρειαστείτε πρόσβαση διαχειριστή στην πύλη του οργανισμού σας Microsoft 365 για να ολοκληρώσετε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="2a105-135">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="2a105-136">Μεταβείτε στο [Κέντρο διαχείρισης της Microsoft 365](https://portal.office.com/) για να αναθέσετε τις άδειες χρήσης στους χρήστες σας.</span><span class="sxs-lookup"><span data-stu-id="2a105-136">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

![Αρχική σελίδα του κέντρου διαχείρισης](./media/14AdminPortal.png)

2. <span data-ttu-id="2a105-138">Στη σελίδα **Ενεργοί χρήστες**, επιλέξτε τους χρήστες στους οποίους θέλετε να αναθέσετε μια άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="2a105-138">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Εκχώρηση αδειών χρήσης](./media/15AssignLicenses.png)

3. <span data-ttu-id="2a105-140">Επαληθεύστε ότι η άδεια χρήσης του **Dynamics 365 Project Operations (CRM) έκδοση προεπισκόπησης** και του **Office 365** έχουν επιλεγεί και επιλέξτε **Αποθήκευση αλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="2a105-140">Verify that the **Dynamics 365 Project Operations (CRM) Preview** and **Office 365 Project Operations - Preview** license have been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="2a105-141">Η δοκιμαστική έκδοση του Finance δεν χρειάζεται να ανατεθεί σε χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2a105-141">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="2a105-142">Έναρξη νέου έργου στο LCS</span><span class="sxs-lookup"><span data-stu-id="2a105-142">Start a new project in LCS</span></span>

<span data-ttu-id="2a105-143">Δημιουργήστε ένα νέο έργο LCS, όπως περιγράφεται στο θέμα, [Έναρξη νέου έργου στο LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="2a105-143">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="2a105-144">Προσθήκη μιας συνδρομής Azure σε ένα έργο LCS</span><span class="sxs-lookup"><span data-stu-id="2a105-144">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="2a105-145">Για να ολοκληρώσετε αυτήν την εργασία, ακολουθήστε τα βήματα που περιγράφονται στο θέμα, [Προσθήκη συνδρομής Azure σε έργο LCS](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="2a105-145">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="2a105-146">Ανάπτυξη του περιβάλλοντος επίδειξης Finance για σενάρια πόρων/μη εφοδιασμένα</span><span class="sxs-lookup"><span data-stu-id="2a105-146">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="2a105-147">Ακολουθήστε τις οδηγίες στο θέμα [Παροχή ενός νέου περιβάλλοντος](resource-provision-new-environment.md) για την ολοκλήρωση της ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="2a105-147">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="2a105-148">Χρησιμοποιήστε τον τύπο ανάπτυξης [περιβάλλον επίδειξης](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) για προεπισκόπηση.</span><span class="sxs-lookup"><span data-stu-id="2a105-148">Use the [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="2a105-149">Εγκατάσταση δεδομένων ρύθμισης παραμέτρων και διαμόρφωσης του CDS</span><span class="sxs-lookup"><span data-stu-id="2a105-149">Install CDS setup and configuration data</span></span>

<span data-ttu-id="2a105-150">Εγκαταστήστε τα δεδομένα ρύθμισης παραμέτρων και διαμόρφωσης του CDS, όπως περιγράφεται στο θέμα [Ρύθμιση και εφαρμογή δεδομένων στο Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="2a105-150">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="2a105-151">Ολοκληρώστε αυτό το βήμα μόνο αφού αναπτυχθεί το περιβάλλον επίδειξης Finance και τα δεδομένα επίδειξης στο FO είναι έτοιμα.</span><span class="sxs-lookup"><span data-stu-id="2a105-151">Complete this step only after Finance demo environment is deployed and demo data in FO is ready.</span></span>
