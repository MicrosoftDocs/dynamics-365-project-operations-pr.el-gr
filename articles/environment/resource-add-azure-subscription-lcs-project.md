---
title: Προσθήκη μιας συνδρομής Azure σε ένα έργο LCS
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο σύνδεσης της συνδρομής σας Azure σε ένα έργο LCS.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ad1ddd69cbb8db7780b8277a7ed7533d3ea3d053
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289909"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="ad76f-103">Προσθήκη μιας συνδρομής Azure σε ένα έργο LCS</span><span class="sxs-lookup"><span data-stu-id="ad76f-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="ad76f-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="ad76f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ad76f-105">Τα περιβάλλοντα που φιλοξενούνται στο cloud πρέπει να αναπτυχθούν με χρήση μιας υπάρχουσας συνδρομής Azure.</span><span class="sxs-lookup"><span data-stu-id="ad76f-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="ad76f-106">Αυτό το θέμα εξηγεί τον τρόπο σύνδεσης της υφιστάμενής σας συνδρομής Azure σε ένα έργο LCS.</span><span class="sxs-lookup"><span data-stu-id="ad76f-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="ad76f-107">Εκχώρηση συγκατάθεσης διαχειριστή</span><span class="sxs-lookup"><span data-stu-id="ad76f-107">Grant admin consent</span></span>

1. <span data-ttu-id="ad76f-108">Στο έργο σας LCS, στην ενότητα **Περιβάλλοντα**, επιλέξτε **Ρυθμίσεις Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Ρυθμίσεις του Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="ad76f-110">Στη σελίδα **Ρυθμίσεις έργου**, στην καρτέλα **Συνδέσεις Azure** επιλέξτε **Εξουσιοδότηση**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="ad76f-111">Με αυτόν τον τρόπο, επιτρέπεται η ανάπτυξη περιβαλλόντων σε αυτό το έργο.</span><span class="sxs-lookup"><span data-stu-id="ad76f-111">This allows environments to be deployed to this project.</span></span>

![Συνδέσεις Azure](./media/2AzureConnectors.png)

3. <span data-ttu-id="ad76f-113">Επιλέξτε **Εξουσιοδότηση** ξανά για να παράσχετε τη συγκατάθεση του διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="ad76f-113">Select **Authorize** again to provide admin consent.</span></span>

![Εκχώρηση συγκατάθεσης διαχειριστή](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="ad76f-115">Αποδεχτείτε το αίτημα για δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="ad76f-115">Accept the permissions request.</span></span>

![Αποδεχτείτε το αίτημα για δικαιώματα](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="ad76f-117">Η εξουσιοδότηση έχει πλέον ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="ad76f-117">The authorization is now complete.</span></span> 

![Επιτυχής εξουσιοδότηση](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="ad76f-119">Παροχή υπηρεσιών ανάπτυξης Dynamics για πρόσβαση στη συνδρομή σας Azure</span><span class="sxs-lookup"><span data-stu-id="ad76f-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="ad76f-120">Μεταβείτε στη [Χρέωση Microsoft Azure](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) και επιλέξτε τη συνδρομή σας.</span><span class="sxs-lookup"><span data-stu-id="ad76f-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="ad76f-121">Οι υπηρεσίες ανάπτυξης του Dynamics πρέπει να αποκτήσουν πρόσβαση σε αυτήν τη συνδρομή για να είναι δυνατή η ανάπτυξη περιβαλλόντων.</span><span class="sxs-lookup"><span data-stu-id="ad76f-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Πληροφορίες συνδρομής Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="ad76f-123">Επιλέξτε **Έλεγχος πρόσβασης (IAM)** στο παράθυρο περιήγησης και, στη συνέχεια, επιλέξτε **Προσθήκη ανάθεσης ρόλου**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="ad76f-124">Στο ρυθμιστικό στη δεξιά πλευρά, επιλέξτε **Ρόλος συμμετέχοντα** και στη λίστα που παρέχεται, βρείτε και επιλέξτε **Υπηρεσίες ανάπτυξης του Dynamics**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="ad76f-125">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-125">Select **Save**.</span></span>

![Πρόσβαση συνδρομής](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="ad76f-127">Προσθήκη μιας σύνδεσης συνδρομής στο έργο LCS</span><span class="sxs-lookup"><span data-stu-id="ad76f-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="ad76f-128">Στο έργο LCS, στη σελίδα **Ρυθμίσεις Microsoft Azure**, επιλέξτε **Προσθήκη** για να προσθέσετε μια νέα σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="ad76f-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="ad76f-129">Εισαγάγετε το αναγνωριστικό συνδρομής Azure σας.</span><span class="sxs-lookup"><span data-stu-id="ad76f-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="ad76f-130">Μπορείτε να βρείτε το αναγνωριστικό της συνδρομής σας Azure στην [Πύλη Azure](https://ms.portal.azure.com/), στην περιοχή **Ρυθμίσεις** στην κάτω αριστερή πλευρά της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="ad76f-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="ad76f-131">Στο πεδίο **Ρύθμιση παραμέτρων για χρήση του διαχειριστή πόρων Azure**, επιλέξτε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="ad76f-132">Βεβαιωθείτε ότι ο τομέας μισθωτών AAD της συνδρομής Azure ταιριάζει με τον τομέα που έχει τη συνδρομή Azure που χρησιμοποιείτε και επιλέξτε **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="ad76f-133">Στη σελίδα **Ρύθμιση παραμέτρων Microsoft Azure**, επιλέξτε **Επόμενο** για να επιβεβαιώσετε.</span><span class="sxs-lookup"><span data-stu-id="ad76f-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="ad76f-134">Εάν λάβετε ένα μήνυμα σφάλματος σε αυτήν την οθόνη, επιστρέψτε στην ενότητα [Παροχή πρόσβασης στις Υπηρεσίες Ανάπτυξης του Dynamics στη συνδρομή Azure](#provide) αυτού του θέματος και βεβαιωθείτε ότι έχετε ολοκληρώσει όλα τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="ad76f-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="ad76f-135">Πραγματοποιήστε λήψη του πιστοποιητικού διαχείρισης Azure σε έναν τοπικό φάκελο στον υπολογιστή σας και, στη συνέχεια, φορτώστε το στην πύλη διαχείρισης Azure μεταβαίνοντας στις **Ρυθμίσεις** > **Πιστοποιητικά διαχείρισης**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="ad76f-136">Αυτό το πιστοποιητικό θα δώσει τη δυνατότητα στο LCS να επικοινωνεί με το Azure για λογαριασμό σας.</span><span class="sxs-lookup"><span data-stu-id="ad76f-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="ad76f-137">Μπορείτε να παραλείψετε αυτό το βήμα εάν ο χρήστης σας έχει πρόσβαση στη συνδρομή.</span><span class="sxs-lookup"><span data-stu-id="ad76f-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="ad76f-138">Επιλέξτε **Επόμενο**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-138">Select  **Next**.</span></span>
8. <span data-ttu-id="ad76f-139">Επιλέξτε την περιοχή Azure όπου θα γίνει η ανάπτυξη και επιλέξτε ένα κέντρο δεδομένων που βρίσκεται κοντά στο σημείο όπου σχεδιάζετε να χρησιμοποιήσετε αυτό το σύστημα.</span><span class="sxs-lookup"><span data-stu-id="ad76f-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="ad76f-140">Επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="ad76f-140">Select  **Connect**.</span></span>

<span data-ttu-id="ad76f-141">Έχετε συνδέσει με επιτυχία τη συνδρομή σας Azure.</span><span class="sxs-lookup"><span data-stu-id="ad76f-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="ad76f-142">Τώρα, μπορείτε να αναπτύξετε Dynamics 365 Finance περιβάλλοντα που φιλοξενούνται από cloud.</span><span class="sxs-lookup"><span data-stu-id="ad76f-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]