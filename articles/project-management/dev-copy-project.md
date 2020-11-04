---
title: Ανάπτυξη προτύπων έργου με την αντιγραφή έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προτύπων έργου χρησιμοποιώντας την προσαρμοσμένη ενέργεια αντιγραφής έργου.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076856"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="2868a-103">Ανάπτυξη προτύπων έργου με την αντιγραφή έργου</span><span class="sxs-lookup"><span data-stu-id="2868a-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="2868a-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="2868a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2868a-105">Το Dynamics 365 Project Operations υποστηρίζει τη δυνατότητα αντιγραφής ενός έργου και την επαναφορά οποιωνδήποτε αναθέσεων στους γενικούς πόρους που αντιπροσωπεύουν το ρόλο.</span><span class="sxs-lookup"><span data-stu-id="2868a-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="2868a-106">Οι πελάτες μπορούν να χρησιμοποιήσουν αυτήν τη λειτουργικότητα για τη δημιουργία βασικών προτύπων έργου.</span><span class="sxs-lookup"><span data-stu-id="2868a-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="2868a-107">Όταν επιλέγετε **Αντιγραφή έργου** , ενημερώνεται η κατάσταση του έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="2868a-107">When you select **Copy Project** , the status of the target project is updated.</span></span> <span data-ttu-id="2868a-108">Χρησιμοποιήστε την **Αιτιολογία κατάστασης** για να καθορίσετε το πότε ολοκληρώνεται η ενέργεια αντιγραφής.</span><span class="sxs-lookup"><span data-stu-id="2868a-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="2868a-109">Αν επιλέξτε **Αντιγραφή έργου** ενημερώνεται επίσης η ημερομηνία έναρξης του έργου με την τρέχουσα ημερομηνία έναρξης, εάν δεν εντοπιστεί ημερομηνία-στόχος στην οντότητα έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="2868a-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="2868a-110">Προσαρμοσμένη ενέργεια αντιγραφής έργου</span><span class="sxs-lookup"><span data-stu-id="2868a-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="2868a-111">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="2868a-111">Name</span></span> 

<span data-ttu-id="2868a-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="2868a-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="2868a-113">Παράμετροι εισόδου</span><span class="sxs-lookup"><span data-stu-id="2868a-113">Input parameters</span></span>
<span data-ttu-id="2868a-114">Υπάρχουν τρεις παράμετροι καταχώρισης:</span><span class="sxs-lookup"><span data-stu-id="2868a-114">There are three input parameters:</span></span>

| <span data-ttu-id="2868a-115">Παράμετρος</span><span class="sxs-lookup"><span data-stu-id="2868a-115">Parameter</span></span>          | <span data-ttu-id="2868a-116">Τύπος</span><span class="sxs-lookup"><span data-stu-id="2868a-116">Type</span></span>   | <span data-ttu-id="2868a-117">Τιμές</span><span class="sxs-lookup"><span data-stu-id="2868a-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="2868a-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="2868a-118">ProjectCopyOption</span></span>  | <span data-ttu-id="2868a-119">String</span><span class="sxs-lookup"><span data-stu-id="2868a-119">String</span></span> | <span data-ttu-id="2868a-120">**{"removeNamedResources":true}** ή **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="2868a-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="2868a-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="2868a-121">SourceProject</span></span>      | <span data-ttu-id="2868a-122">Αναφορά οντότητας</span><span class="sxs-lookup"><span data-stu-id="2868a-122">Entity Reference</span></span> | <span data-ttu-id="2868a-123">Έργο προέλευσης</span><span class="sxs-lookup"><span data-stu-id="2868a-123">Source Project</span></span> |
| <span data-ttu-id="2868a-124">Στόχος</span><span class="sxs-lookup"><span data-stu-id="2868a-124">Target</span></span>             | <span data-ttu-id="2868a-125">Αναφορά οντότητας</span><span class="sxs-lookup"><span data-stu-id="2868a-125">Entity Reference</span></span> | <span data-ttu-id="2868a-126">Έργο-στόχος</span><span class="sxs-lookup"><span data-stu-id="2868a-126">Target Project</span></span> |


- <span data-ttu-id="2868a-127">**{"clearTeamsAndAssignments":true}** : Η προεπιλεγμένη συμπεριφορά για το Project for the Web και θα καταργηθούν όλες οι αναθέσεις και τα μέλη της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="2868a-127">**{"clearTeamsAndAssignments":true}** : Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="2868a-128">**{"removeNamedResources":true}** Η προεπιλεγμένη συμπεριφορά για το Project Operations και θα γίνει επαναφορά των αναθέσεων σε γενικούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="2868a-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="2868a-129">Για περισσότερες προεπιλογές όσον αφορά ενέργειες δείτε [Χρήση ενεργειών Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="2868a-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="2868a-130">Καθορισμός πεδίων προς αντιγραφή</span><span class="sxs-lookup"><span data-stu-id="2868a-130">Specify fields to copy</span></span> 
<span data-ttu-id="2868a-131">Όταν καλείται η ενέργεια, η **Αντιγραφή έργου** θα εξετάσει την προβολή έργου **Αντιγραφή στηλών έργου** για να προσδιορίσει ποια πεδία θα αντιγραφούν κατά την αντιγραφή του έργου.</span><span class="sxs-lookup"><span data-stu-id="2868a-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>