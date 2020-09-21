---
title: Πειραματισμός με δεδομένα επίδειξης
description: Πώς μπορείτε να κάνετε λήψη και να πειραματιστείτε με τα δεδομένα επίδειξης για το Project Service Automation.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b195e5c8-63bc-4e90-914c-f29b8d565942
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 76dd5ff14cbafbfc5341885f0469a6e3e71dd66f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751629"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="1ef1c-103">Πειραματισμός με δεδομένα επίδειξης (Project Service)</span><span class="sxs-lookup"><span data-stu-id="1ef1c-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="1ef1c-104">Για να εξοικειωθείτε με τις δυνατότητες αυτοματοποίησης του Dynamics 365 Project Service Automation είναι χρήσιμο να έχετε ένα προκαθορισμένο περιβάλλον για να εξερευνήσετε.</span><span class="sxs-lookup"><span data-stu-id="1ef1c-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="1ef1c-105">Για το σκοπό αυτό, έχουμε δημιουργήσει ένα ξεχωριστό πακέτο εγκατάστασης δείγματος δεδομένων (επί του παρόντος μόνο στην αγγλική γλώσσα) ώστε να είναι πιο εύκολο να ενημερωθείτε σχετικά με αυτές τις λύσεις.</span><span class="sxs-lookup"><span data-stu-id="1ef1c-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="1ef1c-106">Το πακέτο εγκατάστασης είναι διαθέσιμο στο [Κέντρο λήψης της Microsoft](https://go.microsoft.com/fwlink/?linkid=859966).</span><span class="sxs-lookup"><span data-stu-id="1ef1c-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="1ef1c-107">Η εκτέλεση αυτού του Package Deployer εκτελεί τις ακόλουθες ενέργειες:</span><span class="sxs-lookup"><span data-stu-id="1ef1c-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="1ef1c-108">Δημιουργεί ή ορίζει τις παραμέτρους που καθοδηγούν τη συμπεριφορά του Project Service</span><span class="sxs-lookup"><span data-stu-id="1ef1c-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="1ef1c-109">Εισάγει δείγμα δεδομένων όπως πόροι με δυνατότητα κράτησης, ρόλοι, πωλήσεις και λίστες τιμών κόστους, οργανικές μονάδες, σχετικές καρτέλες επεξεργασίας πωλήσεων, παραγγελίες εργασίας και έργα</span><span class="sxs-lookup"><span data-stu-id="1ef1c-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="1ef1c-110">**Δεν υπάρχει τρόπος να καταργήσετε την εγκατάσταση των δεδομένων επίδειξης.**</span><span class="sxs-lookup"><span data-stu-id="1ef1c-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="1ef1c-111">Θα πρέπει να χρησιμοποιείτε αυτό το πακέτο μόνο σε συστήματα επίδειξης, αξιολόγησης, εκπαίδευσης ή δοκιμής.</span><span class="sxs-lookup"><span data-stu-id="1ef1c-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="1ef1c-112">Για περισσότερες πληροφορίες, δείτε αυτό το [ιστολόγιο](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span><span class="sxs-lookup"><span data-stu-id="1ef1c-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="1ef1c-113">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="1ef1c-113">See Also</span></span>  
 <span data-ttu-id="1ef1c-114">[Οδηγός διαχειριστή](../project-service/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1ef1c-114">[Administrator Guide](../project-service/admin-guide.md) </span></span>  
 <span data-ttu-id="1ef1c-115">[Οδηγός υπεύθυνου λογαριασμού](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1ef1c-115">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="1ef1c-116">[Οδηγός υπεύθυνου έργου](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1ef1c-116">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="1ef1c-117">[Οδηγός υπεύθυνου πόρων](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1ef1c-117">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="1ef1c-118">Οδηγός Χρόνου, Εξόδων και Συνεργασίας</span><span class="sxs-lookup"><span data-stu-id="1ef1c-118">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
