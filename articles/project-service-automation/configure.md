---
title: Ρύθμιση παραμέτρων του Project Service Automation
description: Βήματα για τη ρύθμιση παραμέτρων του Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 56ba0b8d-808c-48d6-965f-abd74b49c2b4
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 52be4705e6ef983dcf421df5d1bfb5c6de8e9a30
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751579"
---
# <a name="configure-project-service"></a><span data-ttu-id="cfdf7-103">Ρύθμιση παραμέτρων του Project Service</span><span class="sxs-lookup"><span data-stu-id="cfdf7-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="cfdf7-104">Πριν χρησιμοποιήσετε τις δυνατότητες αυτοματοποίησης [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στο [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] για τη διαχείριση των λογαριασμών, των έργων και των πόρων σας, πρέπει να ολοκληρώσετε ορισμένα βήματα ρύθμισης παραμέτρων ώστε να διασφαλίσετε ότι η λύση [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] καλύπτει τις ανάγκες του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="cfdf7-105">Στα βήματα αυτά περιλαμβάνονται τα εξής:</span><span class="sxs-lookup"><span data-stu-id="cfdf7-105">These steps include:</span></span>  
  
-   <span data-ttu-id="cfdf7-106">[Ρύθμιση χρονικών μονάδων](../project-service/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-106">[Set up time units](../project-service/set-up-time-units.md).</span></span> <span data-ttu-id="cfdf7-107">Ρυθμίστε τις παραμέτρους των χρονικών μονάδων στον τιμοκατάλογο που θα χρησιμοποιήσετε ως βάση για τον προγραμματισμό και την τιμολόγηση των έργων σας.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="cfdf7-108">[Ορισμός νομισματικών μονάδων και συναλλαγματικών ισοτιμιών](../project-service/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-108">[Set up currencies and exchange rates](../project-service/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="cfdf7-109">Ορίστε τις νομισματικές μονάδες για χρήση για τα έργα σας.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="cfdf7-110">[Δημιουργία οργανωτικών μονάδων](../project-service/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-110">[Create organizational units](../project-service/create-organizational-units.md).</span></span> <span data-ttu-id="cfdf7-111">Ορίστε τις ομάδες που χρησιμοποιεί η εταιρεία σας για να χωρίσεις τις επιχειρηματικές της δραστηριότητες, κατά γεωγραφική θέση, επιχειρηματική λειτουργία ή άλλες λογικές διαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="cfdf7-112">[Ρύθμιση συχνοτήτων τιμολόγησης](../project-service/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-112">[Set up invoice frequencies](../project-service/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="cfdf7-113">Ορίστε χρονικές περιόδους που θέλετε να χρησιμοποιήσετε για την τιμολόγηση των πελατών σας.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="cfdf7-114">[Ρύθμιση παραμέτρων κατηγοριών συναλλαγών](../project-service/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-114">[Configure transaction categories](../project-service/configure-transaction-categories.md).</span></span> <span data-ttu-id="cfdf7-115">Ορίστε κατηγορίες συναλλαγών στις οποίες θα μπορούν οι σύμβουλοί σας να χρεώνουν τα τιμολογήσιμα και μη τιμολογήσιμα έξοδά τους.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="cfdf7-116">[Ρύθμιση παραμέτρων κατηγοριών εξόδων](../project-service/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-116">[Configure expense categories](../project-service/configure-expense-categories.md).</span></span> <span data-ttu-id="cfdf7-117">Ορίστε τις κατηγορίες στις οποίες θα μπορούν οι σύμβουλοί σας να χρεώνουν τα τιμολογήσιμα και μη τιμολογήσιμα έξοδά τους.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="cfdf7-118">[Δημιουργία στοιχείων καταλόγου προϊόντων](../project-service/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-118">[Create product catalog items](../project-service/create-product-catalog-items.md).</span></span> <span data-ttu-id="cfdf7-119">Προσθέστε τα προϊόντα που πουλάτε, όπως άδειες χρήσης λογισμικού, στον τιμοκατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="cfdf7-120">[Δημιουργία τιμοκαταλόγου](../project-service/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-120">[Create a price list](../project-service/create-price-list.md).</span></span> <span data-ttu-id="cfdf7-121">Ρυθμίστε τις παραμέτρους διαφορετικών τιμοκαταλόγων, ανάλογα με το πόσο θέλετε να χρεώνετε τους πελάτες σας για κάθε ρόλο που απαιτεί η εργασία τους.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="cfdf7-122">[Ρύθμιση πόρων](../project-service/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="cfdf7-122">[Set up resources](../project-service/set-up-resources.md).</span></span> <span data-ttu-id="cfdf7-123">Προσθέστε τις δεξιότητες, τις επάρκειες, τους ρόλους πόρων και άλλες πληροφορίες πόρων που θα χρειαστείτε για τα έργα σας.</span><span class="sxs-lookup"><span data-stu-id="cfdf7-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="cfdf7-124">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="cfdf7-124">See Also</span></span>  
 <span data-ttu-id="cfdf7-125">[Επισκόπηση του Project Service Automation](../project-service/overview.md) </span><span class="sxs-lookup"><span data-stu-id="cfdf7-125">[Overview of Project Service Automation](../project-service/overview.md) </span></span>  
 <span data-ttu-id="cfdf7-126">[Ρύθμιση παραμέτρων του Project Service Automation](../project-service/configure.md) </span><span class="sxs-lookup"><span data-stu-id="cfdf7-126">[Configure Project Service Automation](../project-service/configure.md) </span></span>  
 <span data-ttu-id="cfdf7-127">[Οδηγός υπεύθυνου λογαριασμού](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="cfdf7-127">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="cfdf7-128">[Οδηγός υπεύθυνου έργου](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="cfdf7-128">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="cfdf7-129">[Οδηγός υπεύθυνου πόρων](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="cfdf7-129">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="cfdf7-130">Οδηγός Χρόνου, Εξόδων και Συνεργασίας</span><span class="sxs-lookup"><span data-stu-id="cfdf7-130">Time, Expense, and Collaboration Guid</span></span>](../project-service/time-expense-collaboration-guide.md)
