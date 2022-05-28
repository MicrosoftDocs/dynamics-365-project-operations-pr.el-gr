---
title: Ανάπτυξη προτύπων έργου με την αντιγραφή έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προτύπων έργου χρησιμοποιώντας την προσαρμοσμένη ενέργεια αντιγραφής έργου.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 72aa2db7c717eeab85ada448c673bf702087baeb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590898"
---
# <a name="develop-project-templates-with-copy-project"></a>Ανάπτυξη προτύπων έργου με την αντιγραφή έργου

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Το Dynamics 365 Project Operations υποστηρίζει τη δυνατότητα αντιγραφής ενός έργου και την επαναφορά οποιωνδήποτε αναθέσεων στους γενικούς πόρους που αντιπροσωπεύουν τον ρόλο. Οι πελάτες μπορούν να χρησιμοποιήσουν αυτήν τη λειτουργικότητα για τη δημιουργία βασικών προτύπων έργου.

Όταν επιλέγετε **Αντιγραφή έργου**, ενημερώνεται η κατάσταση του έργου προορισμού. Χρησιμοποιήστε την **Αιτιολογία κατάστασης** για να καθορίσετε το πότε ολοκληρώνεται η ενέργεια αντιγραφής. Αν επιλέξτε **Αντιγραφή έργου** ενημερώνεται επίσης η ημερομηνία έναρξης του έργου με την τρέχουσα ημερομηνία έναρξης, εάν δεν εντοπιστεί ημερομηνία-στόχος στην οντότητα έργου προορισμού.

## <a name="copy-project-custom-action"></a>Προσαρμοσμένη ενέργεια αντιγραφής έργου

### <a name="name"></a>'Ονομα 

msdyn\_CopyProjectV3

### <a name="input-parameters"></a>Παράμετροι εισόδου

Υπάρχουν τρεις παράμετροι καταχώρισης:

- **ReplaceNamedResources** ή **ClearTeamsAndAssignments** – Ορίστε μόνο μία από τις επιλογές. Μην ορίσετε και τις δύο.

    - **\{"ReplaceNamedResources":true\}** – Η προεπιλεγμένη συμπεριφορά για το Project Operations. Οποιοιδήποτε πόροι με όνομα αντικαθίστανται με γενικούς πόρους.
    - **\{"ClearTeamsAndAssignments":true\}** – Η προεπιλεγμένη συμπεριφορά για το Project for the Web. Όλες οι αναθέσεις και τα μέλη ομάδας καταργούνται.

- **SourceProject** - Η αναφορά οντότητας του έργου προέλευσης από το οποίο θα αντιγραφούν. Αυτή η παράμετρος δεν μπορεί να είναι null.
- **Target** - Η αναφορά οντότητας του έργου στόχου στο οποίο θα αντιγραφούν. Αυτή η παράμετρος δεν μπορεί να είναι null.

Ο παρακάτω πίνακας παρέχει μια σύνοψη των τριών παραμέτρων.

| Παράμετρος                | Type             | Τιμή                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **True** ή **False** |
| ClearTeamsAndAssignments | Boolean          | **True** ή **False** |
| SourceProject            | Αναφορά οντότητας | Το έργο προέλευσης    |
| Στόχος                   | Αναφορά οντότητας | Το έργο προορισμός    |

Για περισσότερες προεπιλογές όσον αφορά ενέργειες δείτε [Χρήση ενεργειών Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>Επικυρώσεις

Οι ακόλουθες επικυρώσεις έχουν τελειώσει.

1. Η τιμή Null ελέγχει και ανακτά τα έργα προέλευσης και προορισμού για επιβεβαίωση της ύπαρξης και των δύο έργων στον οργανισμό.
2. Το σύστημα επικυρώνει ότι το έργο προορισμού είναι έγκυρο για αντιγραφή, με επαλήθευση των ακόλουθων συνθηκών:

    - Δεν υπάρχει προηγούμενη δραστηριότητα στο έργο (συμπεριλαμβανομένης της επιλογής της καρτέλας **Εργασίες**) και το έργο δημιουργήθηκε πρόσφατα.
    - Δεν υπάρχει προηγούμενο αντίγραφο, δεν ζητήθηκε εισαγωγή σε αυτό το έργο και το έργο δεν έχει κατάσταση **αποτυχία**.

3. Η λειτουργία δεν καλείται με χρήση του HTTP.

## <a name="specify-fields-to-copy"></a>Καθορισμός πεδίων προς αντιγραφή

Όταν καλείται η ενέργεια, η **Αντιγραφή έργου** θα εξετάσει την προβολή έργου **Αντιγραφή στηλών έργου** για να προσδιορίσει ποια πεδία θα αντιγραφούν κατά την αντιγραφή του έργου.

### <a name="example"></a>Παράδειγμα

Το παρακάτω παράδειγμα δείχνει τον τρόπο κλήσης της προσαρμοσμένης ενέργειας **CopyProjectV3** με την παράμετρο **removeNamedResources** να έχει οριστεί.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
