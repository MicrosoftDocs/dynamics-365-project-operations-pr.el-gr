---
title: Υποβολή αίτησης πόρου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την υποβολή αίτησης για έναν πόρο έργου.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077009"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="be33d-103">Υποβολή αίτησης πόρου</span><span class="sxs-lookup"><span data-stu-id="be33d-103">Submitting a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="be33d-104">Μπορείτε να υποβάλετε μια απαίτηση πόρου που έχει δημιουργηθεί ως αίτημα πόρου.</span><span class="sxs-lookup"><span data-stu-id="be33d-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="be33d-105">Στη συνέχεια, το αίτημα αποστέλλεται σε έναν υπεύθυνο διαχείρισης πόρων για ολοκλήρωση.</span><span class="sxs-lookup"><span data-stu-id="be33d-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="be33d-106">Στο Project Service Automation (PSA), στη σελίδα **Έργα** , επιλέξτε την καρτέλα **Ομάδα** για να προβάλετε μια λίστα με πόρους με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="be33d-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="be33d-107">Επιλέξτε τον γενικό πόρο που διαθέτει μια απαίτηση πόρου από τη λίστα και, μετά επιλέξτε **Υποβολή αίτησης**.</span><span class="sxs-lookup"><span data-stu-id="be33d-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Υποβολή αίτησης πόρου](media/RM-how-to-18.png)

<span data-ttu-id="be33d-109">Η κατάσταση αίτησης του γενικού μέλους ομάδας θα αλλάξει σε **Υποβλήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="be33d-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="be33d-110">Μετά την ολοκλήρωση της αίτησης από τον διαχειριστή πόρων, ο γενικός πόρος θα αντικατασταθεί από έναν καθορισμένο πόρο, εάν ο υπεύθυνος πόρου εκπληρώσει την αίτηση με την κράτηση ενός καθορισμένου πόρου.</span><span class="sxs-lookup"><span data-stu-id="be33d-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="be33d-111">Διαφορετικά, ο γενικός πόρος θα παραμείνει στην ομάδα και η κατάσταση αίτησης θα αλλάξει σε **Χρειάζεται έλεγχο** εάν ο διαχειριστής πόρων έχει προτείνει έναν καθορισμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="be33d-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review** , if the resource manager has proposed a named resource.</span></span>