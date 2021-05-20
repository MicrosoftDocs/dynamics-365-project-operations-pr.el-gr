---
title: Ανάπτυξη προτύπων έργου με την αντιγραφή έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προτύπων έργου χρησιμοποιώντας την προσαρμοσμένη ενέργεια αντιγραφής έργου.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949814"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="5b8a5-103">Ανάπτυξη προτύπων έργου με την αντιγραφή έργου</span><span class="sxs-lookup"><span data-stu-id="5b8a5-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="5b8a5-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="5b8a5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="5b8a5-105">Το Dynamics 365 Project Operations υποστηρίζει τη δυνατότητα αντιγραφής ενός έργου και την επαναφορά οποιωνδήποτε αναθέσεων στους γενικούς πόρους που αντιπροσωπεύουν τον ρόλο.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="5b8a5-106">Οι πελάτες μπορούν να χρησιμοποιήσουν αυτήν τη λειτουργικότητα για τη δημιουργία βασικών προτύπων έργου.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="5b8a5-107">Όταν επιλέγετε **Αντιγραφή έργου**, ενημερώνεται η κατάσταση του έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="5b8a5-108">Χρησιμοποιήστε την **Αιτιολογία κατάστασης** για να καθορίσετε το πότε ολοκληρώνεται η ενέργεια αντιγραφής.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="5b8a5-109">Αν επιλέξτε **Αντιγραφή έργου** ενημερώνεται επίσης η ημερομηνία έναρξης του έργου με την τρέχουσα ημερομηνία έναρξης, εάν δεν εντοπιστεί ημερομηνία-στόχος στην οντότητα έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="5b8a5-110">Προσαρμοσμένη ενέργεια αντιγραφής έργου</span><span class="sxs-lookup"><span data-stu-id="5b8a5-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="5b8a5-111">Ονομασία</span><span class="sxs-lookup"><span data-stu-id="5b8a5-111">Name</span></span> 

<span data-ttu-id="5b8a5-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="5b8a5-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="5b8a5-113">Παράμετροι εισόδου</span><span class="sxs-lookup"><span data-stu-id="5b8a5-113">Input parameters</span></span>
<span data-ttu-id="5b8a5-114">Υπάρχουν τρεις παράμετροι καταχώρισης:</span><span class="sxs-lookup"><span data-stu-id="5b8a5-114">There are three input parameters:</span></span>

| <span data-ttu-id="5b8a5-115">Παράμετρος</span><span class="sxs-lookup"><span data-stu-id="5b8a5-115">Parameter</span></span>          | <span data-ttu-id="5b8a5-116">Τύπος</span><span class="sxs-lookup"><span data-stu-id="5b8a5-116">Type</span></span>   | <span data-ttu-id="5b8a5-117">Τιμές</span><span class="sxs-lookup"><span data-stu-id="5b8a5-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="5b8a5-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="5b8a5-118">ProjectCopyOption</span></span>  | <span data-ttu-id="5b8a5-119">String</span><span class="sxs-lookup"><span data-stu-id="5b8a5-119">String</span></span> | <span data-ttu-id="5b8a5-120">**{"removeNamedResources":true}** ή **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="5b8a5-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="5b8a5-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="5b8a5-121">SourceProject</span></span>      | <span data-ttu-id="5b8a5-122">Αναφορά οντότητας</span><span class="sxs-lookup"><span data-stu-id="5b8a5-122">Entity Reference</span></span> | <span data-ttu-id="5b8a5-123">Έργο προέλευσης</span><span class="sxs-lookup"><span data-stu-id="5b8a5-123">Source Project</span></span> |
| <span data-ttu-id="5b8a5-124">Στόχος</span><span class="sxs-lookup"><span data-stu-id="5b8a5-124">Target</span></span>             | <span data-ttu-id="5b8a5-125">Αναφορά οντότητας</span><span class="sxs-lookup"><span data-stu-id="5b8a5-125">Entity Reference</span></span> | <span data-ttu-id="5b8a5-126">Έργο-στόχος</span><span class="sxs-lookup"><span data-stu-id="5b8a5-126">Target Project</span></span> |


- <span data-ttu-id="5b8a5-127">**{"clearTeamsAndAssignments":true}**: Η προεπιλεγμένη συμπεριφορά για το Project for the Web και θα καταργηθούν όλες οι αναθέσεις και τα μέλη της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="5b8a5-128">**{"removeNamedResources":true}** Η προεπιλεγμένη συμπεριφορά για το Project Operations και θα γίνει επαναφορά των αναθέσεων σε γενικούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="5b8a5-129">Για περισσότερες προεπιλογές όσον αφορά ενέργειες δείτε [Χρήση ενεργειών Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="5b8a5-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="5b8a5-130">Καθορισμός πεδίων προς αντιγραφή</span><span class="sxs-lookup"><span data-stu-id="5b8a5-130">Specify fields to copy</span></span> 
<span data-ttu-id="5b8a5-131">Όταν καλείται η ενέργεια, η **Αντιγραφή έργου** θα εξετάσει την προβολή έργου **Αντιγραφή στηλών έργου** για να προσδιορίσει ποια πεδία θα αντιγραφούν κατά την αντιγραφή του έργου.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="5b8a5-132">Παράδειγμα</span><span class="sxs-lookup"><span data-stu-id="5b8a5-132">Example</span></span>
<span data-ttu-id="5b8a5-133">Το παρακάτω παράδειγμα δείχνει τον τρόπο κλήσης της προσαρμοσμένης ενέργειας **CopyProject** με την παράμετρο **removeNamedResources**.</span><span class="sxs-lookup"><span data-stu-id="5b8a5-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]