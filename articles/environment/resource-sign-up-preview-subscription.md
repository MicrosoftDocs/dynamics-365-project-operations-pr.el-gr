---
title: Εγγραφή για συνδρομές προεπισκόπησης του Project Operations για σενάρια πόρων/ μη εφοδιασμένα
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εγγραφής και ανάπτυξης του Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334827"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="7096d-103">Εγγραφή για συνδρομές προεπισκόπησης του Project Operations για σενάρια πόρων/ μη εφοδιασμένα</span><span class="sxs-lookup"><span data-stu-id="7096d-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="7096d-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="7096d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="7096d-105">Αυτό θέμα εξηγεί τον τρόπο εγγραφής στη δοκιμαστική προσφορά και ανάπτυξης του περιβάλλοντος Project Operations για σενάρια που βασίζονται σε πόρους/μη εφοδιασμένα.</span><span class="sxs-lookup"><span data-stu-id="7096d-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7096d-106">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="7096d-106">Prerequisites</span></span>
- <span data-ttu-id="7096d-107">Ο χρήστης που αναπτύσσει την προεπισκόπηση πρέπει να έχει δικαιώματα καθολικού διαχειριστή μισθωτή Azure.</span><span class="sxs-lookup"><span data-stu-id="7096d-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="7096d-108">Μπορείτε να δημιουργήσετε έναν μισθωτή κατά τη διάρκεια της εξαργύρωσης της πρώτης προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="7096d-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="7096d-109">Η ανάπτυξη ενός περιβάλλοντος Finance απαιτεί μια έγκυρη συνδρομή Azure η οποία θα χρεώνεται ανά περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="7096d-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="7096d-110">Μπορείτε να χρησιμοποιήσετε την υφιστάμενη συνδρομή των οργανισμών σας ή να χρησιμοποιήσετε μια [δοκιμαστική έκδοση του Azure](https://azure.microsoft.com/en-us/free/) για να ξεκινήσετε.</span><span class="sxs-lookup"><span data-stu-id="7096d-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="7096d-111">Το περιβάλλον CDS θα παρέχεται δωρεάν για περιορισμένο χρονικό διάστημα 30 ημερών.</span><span class="sxs-lookup"><span data-stu-id="7096d-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7096d-112">Μόνο ένα άτομο, ο διαχειριστής μισθωτή, σε έναν οργανισμό πρέπει να εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="7096d-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="7096d-113">Εάν δεν είστε ο συνδρομητής σε αυτήν την έκδοση, περιμένετε έως ότου ολοκληρωθεί η εγγραφή του οργανισμού σας και λάβετε τα διαπιστευτήρια χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="7096d-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="7096d-114">Οι δοκιμαστικές εκδόσεις είναι μίας χρήσης στον μισθωτή.</span><span class="sxs-lookup"><span data-stu-id="7096d-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="7096d-115">Μπορείτε να εκτελέσετε μια δοκιμαστική έκδοση μόνο μία φορά.</span><span class="sxs-lookup"><span data-stu-id="7096d-115">You can only run a trial one time.</span></span> <span data-ttu-id="7096d-116">Συνιστούμε να δημιουργήσετε ένα νέο μισθωτή για τον σκοπό της δοκιμαστικής έκδοσης.</span><span class="sxs-lookup"><span data-stu-id="7096d-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="7096d-117">Dynamics 365 Project Operations (CE) - Προεπισκόπηση δοκιμαστικής έκδοσης</span><span class="sxs-lookup"><span data-stu-id="7096d-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="7096d-118">Πριν ξεκινήσετε, βεβαιωθείτε ότι έχετε συνδεθεί σε ένα πρόγραμμα περιήγησης με το λογαριασμό εργασίας χρήστη του μισθωτή όπου θέλετε να γίνει προεπισκόπηση του Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7096d-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="7096d-119">Εξαργυρώστε τον κωδικό πρώτης προσφοράς, **Dynamics 365 Project Operations** εδώ [Project Operations δοκιμαστική έκδοση](https://aka.ms/try-po).</span><span class="sxs-lookup"><span data-stu-id="7096d-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="7096d-120">Επιβεβαιώστε την παραγγελία σας.</span><span class="sxs-lookup"><span data-stu-id="7096d-120">Confirm your order.</span></span>

  <span data-ttu-id="7096d-121">Θα δείτε ότι η προσφορά επιβεβαίωσης έχει εξαργυρωθεί με επιτυχία.</span><span class="sxs-lookup"><span data-stu-id="7096d-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="7096d-122">Προεπισκόπηση δοκιμαστικής έκδοσης Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="7096d-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="7096d-123">Μεταβείτε [στη δοκιμαστική έκδοση του Dynamics 365 for Χρηματοοικονομικά](https://aka.ms/trypoche) και επαναλάβετε τα βήματα από την προηγούμενη ενότητα με την προσφορά, Εγγραφείτε στο Περιβάλλον που φιλοξενείται σε cloud.</span><span class="sxs-lookup"><span data-stu-id="7096d-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="7096d-124">Εκχώρηση αδειών χρήσης</span><span class="sxs-lookup"><span data-stu-id="7096d-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7096d-125">Θα χρειαστείτε πρόσβαση διαχειριστή στην πύλη του οργανισμού σας Microsoft 365 για να ολοκληρώσετε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="7096d-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="7096d-126">Μεταβείτε στο [Κέντρο διαχείρισης της Microsoft 365](https://portal.office.com/) για να αναθέσετε τις άδειες χρήσης στους χρήστες σας.</span><span class="sxs-lookup"><span data-stu-id="7096d-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="7096d-127">Στη σελίδα **Ενεργοί χρήστες**, επιλέξτε τους χρήστες στους οποίους θέλετε να αναθέσετε μια άδεια χρήσης.</span><span class="sxs-lookup"><span data-stu-id="7096d-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="7096d-128">Επαληθεύστε ότι η άδεια χρήσης **Dynamics 365 Project Operations** έχει επιλεγεί και επιλέξτε **Αποθήκευση αλλαγών**.</span><span class="sxs-lookup"><span data-stu-id="7096d-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="7096d-129">Η δοκιμαστική έκδοση του Finance δεν χρειάζεται να ανατεθεί σε χρήστη.</span><span class="sxs-lookup"><span data-stu-id="7096d-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="7096d-130">Έναρξη νέου έργου στο LCS</span><span class="sxs-lookup"><span data-stu-id="7096d-130">Start a new project in LCS</span></span>

<span data-ttu-id="7096d-131">Δημιουργήστε ένα νέο έργο LCS, όπως περιγράφεται στο θέμα, [Έναρξη νέου έργου στο LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="7096d-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="7096d-132">Προσθήκη μιας συνδρομής Azure σε ένα έργο LCS</span><span class="sxs-lookup"><span data-stu-id="7096d-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="7096d-133">Για να ολοκληρώσετε αυτήν την εργασία, ακολουθήστε τα βήματα που περιγράφονται στο θέμα, [Προσθήκη συνδρομής Azure σε έργο LCS](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="7096d-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="7096d-134">Ανάπτυξη του περιβάλλοντος επίδειξης Finance για σενάρια πόρων/μη εφοδιασμένα</span><span class="sxs-lookup"><span data-stu-id="7096d-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="7096d-135">Ακολουθήστε τις οδηγίες στο θέμα [Παροχή ενός νέου περιβάλλοντος](resource-provision-new-environment.md) για την ολοκλήρωση της ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="7096d-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="7096d-136">Χρησιμοποιήστε τον τύπο ανάπτυξης [περιβάλλον επίδειξης](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) για προεπισκόπηση.</span><span class="sxs-lookup"><span data-stu-id="7096d-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="7096d-137">Εγκατάσταση δεδομένων ρύθμισης παραμέτρων και διαμόρφωσης του CDS</span><span class="sxs-lookup"><span data-stu-id="7096d-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="7096d-138">Εγκαταστήστε τα δεδομένα ρύθμισης παραμέτρων και διαμόρφωσης του CDS, όπως περιγράφεται στο θέμα [Ρύθμιση και εφαρμογή δεδομένων στο Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="7096d-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="7096d-139">Ολοκληρώστε αυτό το βήμα μόνο μετά την ανάπτυξη του περιβάλλοντος επίδειξης Οικονομικών και όταν τα δεδομένα επίδειξης είναι έτοιμα.</span><span class="sxs-lookup"><span data-stu-id="7096d-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
