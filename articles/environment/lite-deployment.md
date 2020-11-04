---
title: Ανάπτυξη Project Operations Lite - συμφωνία για προτιμολόγηση
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εγκατάστασης της ελαφριάς ανάπτυξη του Project Operations - συμφωνία για προτιμολόγηση.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e938876d459b3f6dfedd90e57e3042cda96bffb7
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076780"
---
# <a name="deploy-project-operations-lite-deployment--deal-to-proforma-invoicing"></a><span data-ttu-id="7d94d-103">Ανάπτυξη Project Operations Lite - συμφωνία για προτιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="7d94d-103">Deploy Project Operations Lite deployment – deal to proforma invoicing</span></span>

<span data-ttu-id="7d94d-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="7d94d-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7d94d-105">Το Project Operations υποστηρίζει πολλαπλά μοντέλα ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="7d94d-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="7d94d-106">Για να προσδιορίσετε το μοντέλο καλύτερης ανάπτυξης, ανατρέξτε στο θέμα [Τύποι ανάπτυξης](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="7d94d-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="7d94d-107">Αυτή η ανάπτυξη, η ελαφριά ανάπτυξη – συμφωνία για προτιμολόγηση, έχει ως αποτέλεσμα μια **Common Data Service-μόνο ανάπτυξη του Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="7d94d-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="7d94d-108">Εγκατάσταση του Project Operations σε νέο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="7d94d-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="7d94d-109">Εγκατάσταση σε υπάρχον περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="7d94d-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="7d94d-110">Εγκατάσταση του Project Operations σε νέο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="7d94d-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="7d94d-111">Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, δημιουργήστε ένα νέο περιβάλλον CDS στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="7d94d-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="7d94d-112">Βεβαιωθείτε ότι η **Βάση δεδομένων CDS** και οι **Εφαρμογές Dynamics 365** έχουν ενεργοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="7d94d-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="7d94d-113">Για περισσότερες πληροφορίες σχετικά με τα περιβάλλοντα παροχής, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση περιβαλλόντων στο κέντρο διαχείρισης του Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7d94d-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="7d94d-114">Επιλέξτε **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7d94d-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="7d94d-115">Εγκατάσταση του Project Operations σε υφιστάμενο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="7d94d-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="7d94d-116">Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, εντοπίστε το περιβάλλον στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com) στο οποίο θέλετε να εγκαταστήσετε το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7d94d-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="7d94d-117">Εγκαταστήστε το **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7d94d-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="7d94d-118">Για περισσότερες πληροφορίες, ανατρέξτε στη [Διαχείριση εφαρμογών Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="7d94d-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


