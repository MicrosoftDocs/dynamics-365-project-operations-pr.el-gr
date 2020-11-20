---
title: Γιατί η τιμή είναι μηδέν κατά προεπιλογή στις πραγματικές δαπάνες κόστους;
description: Αντιμετώπιση του ζητήματος της τιμής που είναι μηδέν κατά προεπιλογή στις πραγματικές δαπάνες κόστους.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122118"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="1209a-103">Γιατί η τιμή είναι μηδέν κατά προεπιλογή στις πραγματικές δαπάνες κόστους;</span><span class="sxs-lookup"><span data-stu-id="1209a-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1209a-104">Αυτές οι συνήθεις ερωτήσεις εφαρμόζονται σε πραγματικές δαπάνες όπου η κλάση συναλλαγής έχει οριστεί σε δαπάνες και ο τύπος συναλλαγής είναι Κόστος.</span><span class="sxs-lookup"><span data-stu-id="1209a-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="1209a-105">Αντιμετώπιση προβλημάτων χρεώσεων σε πραγματικές δαπάνες</span><span class="sxs-lookup"><span data-stu-id="1209a-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="1209a-106">Μεταβείτε στη σχετική εγγραφή δαπανών και βεβαιωθείτε ότι υπάρχει ένα ποσό στο πεδίο εγγραφής δαπανών.</span><span class="sxs-lookup"><span data-stu-id="1209a-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="1209a-107">Εάν η αρχική εγγραφή δαπανών δεν έχει συμπληρωμένο το πεδίο "Ποσό", τότε έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="1209a-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="1209a-108">Για να επιλύσετε αυτό το πρόβλημα, δημιουργήστε ξανά την εγγραφή δαπανών με έναν έγκυρο αριθμό και εγκρίνετέ την.</span><span class="sxs-lookup"><span data-stu-id="1209a-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
