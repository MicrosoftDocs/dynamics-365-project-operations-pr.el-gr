---
title: Πειραματισμός με δεδομένα επίδειξης
description: Πώς μπορείτε να κάνετε λήψη και να πειραματιστείτε με τα δεδομένα επίδειξης για το Project Service Automation.
author: JohnPBurrows
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
ms.openlocfilehash: 8835ce5907e3dcece5ee6f9a98594f29cf328bf3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6015376"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="589a7-103">Πειραματισμός με δεδομένα επίδειξης (Project Service)</span><span class="sxs-lookup"><span data-stu-id="589a7-103">Experiment with demo data (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="589a7-104">Για να εξοικειωθείτε με τις δυνατότητες αυτοματοποίησης του Dynamics 365 Project Service Automation είναι χρήσιμο να έχετε ένα προκαθορισμένο περιβάλλον για να εξερευνήσετε.</span><span class="sxs-lookup"><span data-stu-id="589a7-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="589a7-105">Για το σκοπό αυτό, έχουμε δημιουργήσει ένα ξεχωριστό πακέτο εγκατάστασης δείγματος δεδομένων (επί του παρόντος μόνο στην αγγλική γλώσσα) ώστε να είναι πιο εύκολο να ενημερωθείτε σχετικά με αυτές τις λύσεις.</span><span class="sxs-lookup"><span data-stu-id="589a7-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="589a7-106">Το πακέτο εγκατάστασης είναι διαθέσιμο στο [Κέντρο λήψης της Microsoft](https://go.microsoft.com/fwlink/?linkid=859966).</span><span class="sxs-lookup"><span data-stu-id="589a7-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="589a7-107">Η εκτέλεση αυτού του Package Deployer εκτελεί τις ακόλουθες ενέργειες:</span><span class="sxs-lookup"><span data-stu-id="589a7-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="589a7-108">Δημιουργεί ή ορίζει τις παραμέτρους που καθοδηγούν τη συμπεριφορά του Project Service</span><span class="sxs-lookup"><span data-stu-id="589a7-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="589a7-109">Εισάγει δείγμα δεδομένων όπως πόροι με δυνατότητα κράτησης, ρόλοι, πωλήσεις και λίστες τιμών κόστους, οργανικές μονάδες, σχετικές καρτέλες επεξεργασίας πωλήσεων, παραγγελίες εργασίας και έργα</span><span class="sxs-lookup"><span data-stu-id="589a7-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="589a7-110">**Δεν υπάρχει τρόπος να καταργήσετε την εγκατάσταση των δεδομένων επίδειξης.**</span><span class="sxs-lookup"><span data-stu-id="589a7-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="589a7-111">Θα πρέπει να χρησιμοποιείτε αυτό το πακέτο μόνο σε συστήματα επίδειξης, αξιολόγησης, εκπαίδευσης ή δοκιμής.</span><span class="sxs-lookup"><span data-stu-id="589a7-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="589a7-112">Για περισσότερες πληροφορίες, δείτε αυτό το [ιστολόγιο](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span><span class="sxs-lookup"><span data-stu-id="589a7-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="589a7-113">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="589a7-113">See Also</span></span>  
 <span data-ttu-id="589a7-114">[Οδηγός διαχειριστή](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="589a7-114">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="589a7-115">[Οδηγός υπεύθυνου λογαριασμού](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="589a7-115">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="589a7-116">[Οδηγός υπεύθυνου έργου](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="589a7-116">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="589a7-117">[Οδηγός υπεύθυνου πόρων](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="589a7-117">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="589a7-118">Οδηγός Χρόνου, Εξόδων και Συνεργασίας</span><span class="sxs-lookup"><span data-stu-id="589a7-118">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]