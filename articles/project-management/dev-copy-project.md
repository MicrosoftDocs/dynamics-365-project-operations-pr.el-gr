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
ms.openlocfilehash: 87696b41db20e9ec70270c850d9acfe05df8cd84
ms.sourcegitcommit: d5004acb6f1c257b30063c873896fdea92191e3b
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 01/22/2021
ms.locfileid: "5045009"
---
# <a name="develop-project-templates-with-copy-project"></a>Ανάπτυξη προτύπων έργου με την αντιγραφή έργου

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Το Dynamics 365 Project Operations υποστηρίζει τη δυνατότητα αντιγραφής ενός έργου και την επαναφορά οποιωνδήποτε αναθέσεων στους γενικούς πόρους που αντιπροσωπεύουν τον ρόλο. Οι πελάτες μπορούν να χρησιμοποιήσουν αυτήν τη λειτουργικότητα για τη δημιουργία βασικών προτύπων έργου.

Όταν επιλέγετε **Αντιγραφή έργου**, ενημερώνεται η κατάσταση του έργου προορισμού. Χρησιμοποιήστε την **Αιτιολογία κατάστασης** για να καθορίσετε το πότε ολοκληρώνεται η ενέργεια αντιγραφής. Αν επιλέξτε **Αντιγραφή έργου** ενημερώνεται επίσης η ημερομηνία έναρξης του έργου με την τρέχουσα ημερομηνία έναρξης, εάν δεν εντοπιστεί ημερομηνία-στόχος στην οντότητα έργου προορισμού.

## <a name="copy-project-custom-action"></a>Προσαρμοσμένη ενέργεια αντιγραφής έργου 

### <a name="name"></a>Ονομασία 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Παράμετροι εισόδου
Υπάρχουν τρεις παράμετροι καταχώρισης:

| Παράμετρος          | Τύπος   | Τιμές                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** ή **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Αναφορά οντότητας | Έργο προέλευσης |
| Στόχος             | Αναφορά οντότητας | Έργο-στόχος |


- **{"clearTeamsAndAssignments":true}**: Η προεπιλεγμένη συμπεριφορά για το Project for the Web και θα καταργηθούν όλες οι αναθέσεις και τα μέλη της ομάδας.
- **{"removeNamedResources":true}** Η προεπιλεγμένη συμπεριφορά για το Project Operations και θα γίνει επαναφορά των αναθέσεων σε γενικούς πόρους.

Για περισσότερες προεπιλογές όσον αφορά ενέργειες δείτε [Χρήση ενεργειών Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>Καθορισμός πεδίων προς αντιγραφή 
Όταν καλείται η ενέργεια, η **Αντιγραφή έργου** θα εξετάσει την προβολή έργου **Αντιγραφή στηλών έργου** για να προσδιορίσει ποια πεδία θα αντιγραφούν κατά την αντιγραφή του έργου.


### <a name="example"></a>Παράδειγμα
Το παρακάτω παράδειγμα δείχνει τον τρόπο κλήσης της προσαρμοσμένης ενέργειας **CopyProject** με την παράμετρο **removeNamedResources**.
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
