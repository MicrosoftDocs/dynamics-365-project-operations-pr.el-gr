---
title: Ρύθμιση πρόσθετων ρυθμίσεων παραμέτρων
description: Πώς γίνεται η ρύθμιση πρόσθετων ρυθμίσεων παραμέτρων στο Project Service
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5ce7ffd635b10689c8295d9349966450f11282d1
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129363"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="00cec-103">Ρύθμιση πρόσθετων ρυθμίσεων παραμέτρων (Project Service)</span><span class="sxs-lookup"><span data-stu-id="00cec-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="00cec-104">Αφού ρυθμίσετε τις παραμέτρους των στοιχείων στα προηγούμενα θέματα, πρέπει να ορίσετε πρόσθετες παραμέτρους έργων για τα έργα σας.</span><span class="sxs-lookup"><span data-stu-id="00cec-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="00cec-105">Κατά την αρχική εγκατάσταση του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], δημιουργήσατε μια ρύθμιση παραμέτρων για την πρώτη δημιουργία όλων των καρτελών που απαιτούνται για τη λειτουργία του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="00cec-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="00cec-106">Ήρθε η ώρα να επιστρέψετε και να ρυθμίσετε τις παραμέτρους πρόσθετων πεδίων για αυτές τις ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="00cec-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="00cec-107">Θα πρέπει να ρυθμίσετε τις παραμέτρους των παρακάτω ρυθμίσεων:</span><span class="sxs-lookup"><span data-stu-id="00cec-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="00cec-108">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="00cec-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="00cec-109">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="00cec-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="00cec-110">Πρότυπα ωρών εργασίας</span><span class="sxs-lookup"><span data-stu-id="00cec-110">Work hours template</span></span>  
  
-   <span data-ttu-id="00cec-111">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="00cec-111">Price list</span></span>  
 
<span data-ttu-id="00cec-112">Σε αυτό το βήμα, θα δηλώσετε επίσης τον τύπο της κατανομής πόρων που θέλετε:</span><span class="sxs-lookup"><span data-stu-id="00cec-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="00cec-113">**Κεντρική**.</span><span class="sxs-lookup"><span data-stu-id="00cec-113">**Central**.</span></span> <span data-ttu-id="00cec-114">Μόνο οι διαχειριστές πόρων μπορούν να εκχωρούν πόρους σε έργα.</span><span class="sxs-lookup"><span data-stu-id="00cec-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="00cec-115">**Υβριδική**.</span><span class="sxs-lookup"><span data-stu-id="00cec-115">**Hybrid**.</span></span> <span data-ttu-id="00cec-116">Οι διαχειριστές πόρων, οι διαχειριστές έργου και οι υπεύθυνοι διαχείρισης λογαριασμών μπορούν να εκχωρούν πόρους σε έργα.</span><span class="sxs-lookup"><span data-stu-id="00cec-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="00cec-117">Για να ορίσετε παραμέτρους έργων:</span><span class="sxs-lookup"><span data-stu-id="00cec-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="00cec-118">Μεταβείτε στο μενού **Project Service > Παράμετροι**.</span><span class="sxs-lookup"><span data-stu-id="00cec-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="00cec-119">Επιλέξτε τη ρύθμιση παραμέτρων που θέλετε να ρυθμίσετε (αυτές που δημιουργήσατε κατά την πρώτη εγκατάσταση του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]) ή κάντε κλικ στο κουμπί **Δημιουργία** για να δημιουργήσετε μια νέα.</span><span class="sxs-lookup"><span data-stu-id="00cec-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="00cec-120">Στην περιοχή **Γενικά**, ορίστε όλες τις επιλογές για τις παραμέτρους του έργου σας.</span><span class="sxs-lookup"><span data-stu-id="00cec-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="00cec-121">Στην περιοχή **Τιμοκατάλογος**, κάντε κλικ στο κουμπί **+** για να προσθέσετε έναν τιμοκατάλογο, επιλέξτε έναν τιμοκατάλογο στην αναπτυσσόμενη λίστα **Τιμοκατάλογος παραμέτρων έργου** και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="00cec-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="00cec-122">Επιλέξτε το κουμπί **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="00cec-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="00cec-123">Η καρτέλα της παραμέτρου έργου πρέπει να διατηρηθεί για να λειτουργεί σωστά το Project Service.</span><span class="sxs-lookup"><span data-stu-id="00cec-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="00cec-124">Αυτή η καρτέλα δεν πρέπει να διαγραφεί.</span><span class="sxs-lookup"><span data-stu-id="00cec-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="00cec-125">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="00cec-125">See Also</span></span>  
 [<span data-ttu-id="00cec-126">Ρύθμιση πόρων</span><span class="sxs-lookup"><span data-stu-id="00cec-126">Set up resources</span></span>](../psa/set-up-resources.md)
