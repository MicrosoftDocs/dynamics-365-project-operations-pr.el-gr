---
title: Κατάργηση εγκατάστασης του Dynamics 365 Project Operations
description: Αυτό το θέμα παρέχει συνδέσεις σε πληροφορίες σχετικά με την κατάργηση της εγκατάστασης του Dynamics 365 Project Operations.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b87c9324b1c95c10ef1e18b0fbf4572bdbe76827
ms.sourcegitcommit: b8b7a59eee7d93638446e93726d270316e45ab3d
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/10/2021
ms.locfileid: "7783643"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Κατάργηση εγκατάστασης του Dynamics 365 Project Operations 

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Για να απεγκαταστήσετε το Dynamics 365 Project Operations, πρέπει να εκχωρήσετε τον ρόλο του Διαχειριστή.

1. Μεταβείτε στην επιλογή **Ρυθμίσεις** > **Λύσεις**.

    ![Σελίδα ρυθμίσεων.](./media/uninstall-proj-ops-solutions.png)
  
2. Καταργήστε τις λύσεις με την ακριβή σειρά με την οποία εμφανίζονται στον ακόλουθο πίνακα. 

    | Βήμα | Όνομα λύσης                                    | Σημείωμα                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1 | msdyn_ProjectServiceUpgrade_managed.cab            | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 2 | ProjectOperations_Anchor                           | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 3 | Dynamics365ProjectOperationsDualWriteEntityMaps    | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 5 | ProjectService                                     | Χωρίς πρόσθετες σημειώσεις.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | Χωρίς πρόσθετες σημειώσεις.                                                                         |
    | 7 | ProjectServiceCore                                 | Χωρίς πρόσθετες σημειώσεις.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 9 | FieldServiceCommon                                 | Απαιτείται για διπλή εγγραφή με το Dynamics 365 Finance ή το Dynamics 365 Supply Chain Management.   |
    | 10 | msdyn_AssetCommon                                  | Απαιτείται για διπλή εγγραφή με το Dynamics 365 Finance ή το Dynamics 365 Supply Chain Management.   |
    | 11 | msdyn_TESA_Anchor                                  | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 12 | msdyn_TESA_Patch                                   | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 13 | msdyn_TESA                                         | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 14 | ResourceSchedulingControls                         | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Απαιτείτια για Dynamics 365 Field Service.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 19 | Dynamics365Notes                                   | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 21 | DualWriteCore                                      | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 23 | Dynamics365AssetManagement                         | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 25 | Dynamics365FinanceExtended                         | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 26 | HCMCommon                                          | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 28 | Πάρτυ                                              | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 29 | Dynamics365Company                                 | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 30 | CurrencyExchangeRates                              | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
    | 31 | AssetCommon                                        | Εάν δεν βρεθεί, παραλείψτε αυτήν τη λύση.                                                            |
