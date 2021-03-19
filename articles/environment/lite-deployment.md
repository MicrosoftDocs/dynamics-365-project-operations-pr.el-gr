---
title: Ανάπτυξη Project Operations - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εγκατάστασης της ελαφριάς ανάπτυξη του Project Operations - συμφωνία για προτιμολόγηση.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0af8067fc0673890a317ac6f4e62d74b7f4eebca
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290089"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="a85bf-103">Ανάπτυξη Project Operations - lite</span><span class="sxs-lookup"><span data-stu-id="a85bf-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="a85bf-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="a85bf-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="a85bf-105">Το Project Operations υποστηρίζει πολλαπλά μοντέλα ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="a85bf-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="a85bf-106">Για να προσδιορίσετε το μοντέλο καλύτερης ανάπτυξης, ανατρέξτε στο θέμα [Τύποι ανάπτυξης](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="a85bf-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="a85bf-107">Αυτή η ανάπτυξη, η ελαφριά ανάπτυξη – συμφωνία για προτιμολόγηση, έχει ως αποτέλεσμα μια **Common Data Service-μόνο ανάπτυξη του Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="a85bf-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="a85bf-108">Εγκατάσταση του Project Operations σε νέο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="a85bf-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="a85bf-109">Εγκατάσταση σε υπάρχον περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="a85bf-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="a85bf-110">Εγκατάσταση του Project Operations σε νέο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="a85bf-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="a85bf-111">Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, δημιουργήστε ένα νέο περιβάλλον CDS στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="a85bf-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="a85bf-112">Βεβαιωθείτε ότι η **Βάση δεδομένων CDS** και οι **Εφαρμογές Dynamics 365** έχουν ενεργοποιηθεί.</span><span class="sxs-lookup"><span data-stu-id="a85bf-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="a85bf-113">Για περισσότερες πληροφορίες σχετικά με τα περιβάλλοντα παροχής, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση περιβαλλόντων στο κέντρο διαχείρισης του Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a85bf-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="a85bf-114">Επιλέξτε **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a85bf-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="a85bf-115">Εγκατάσταση του Project Operations σε υφιστάμενο περιβάλλον CDS</span><span class="sxs-lookup"><span data-stu-id="a85bf-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="a85bf-116">Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, εντοπίστε το περιβάλλον στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com) στο οποίο θέλετε να εγκαταστήσετε το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a85bf-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="a85bf-117">Εγκαταστήστε το **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a85bf-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="a85bf-118">Για περισσότερες πληροφορίες, ανατρέξτε στη [Διαχείριση εφαρμογών Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="a85bf-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]