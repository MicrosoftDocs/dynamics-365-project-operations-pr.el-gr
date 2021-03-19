---
title: Υποβολή μιας αίτησης πόρου
description: Μπορείτε να υποβάλετε μια απαίτηση πόρου που έχει δημιουργηθεί ως αίτημα πόρου. Στη συνέχεια, το αίτημα αποστέλλεται σε έναν υπεύθυνο διαχείρισης πόρων για ολοκλήρωση.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc97af1ec90e60417c502eb329a85004e769e05b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279138"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="1c069-104">Υποβολή μιας αίτησης πόρου</span><span class="sxs-lookup"><span data-stu-id="1c069-104">Submit a resource request</span></span>

<span data-ttu-id="1c069-105">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1c069-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1c069-106">Μπορείτε να υποβάλετε μια απαίτηση πόρου που έχει δημιουργηθεί ως αίτημα πόρου.</span><span class="sxs-lookup"><span data-stu-id="1c069-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="1c069-107">Στη συνέχεια, το αίτημα αποστέλλεται σε έναν υπεύθυνο διαχείρισης πόρων για ολοκλήρωση.</span><span class="sxs-lookup"><span data-stu-id="1c069-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="1c069-108">Στο Dynamics 365 Project Operations, στη σελίδα **Έργα**, επιλέξτε την καρτέλα **Ομάδα** για να προβάλετε μια λίστα με πόρους με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="1c069-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="1c069-109">Επιλέξτε τον γενικό πόρο που διαθέτει μια απαίτηση πόρου από τη λίστα και, μετά επιλέξτε **Υποβολή αίτησης**.</span><span class="sxs-lookup"><span data-stu-id="1c069-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="1c069-110">Η κατάσταση αίτησης του γενικού μέλους ομάδας θα αλλάξει σε **Υποβλήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1c069-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="1c069-111">Μετά την ολοκλήρωση της αίτησης, ο γενικός πόρος θα αντικατασταθεί από έναν καθορισμένο πόρο, εάν ο υπεύθυνος πόρου εκπληρώσει την αίτηση με την κράτηση ενός καθορισμένου πόρου.</span><span class="sxs-lookup"><span data-stu-id="1c069-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="1c069-112">Διαφορετικά, αν ο υπεύθυνος πόρου προτείνει έναν καθορισμένο πόρο, τότε ο γενικός πόρος θα παραμείνει στην ομάδα και η κατάσταση αίτησης θα αλλάξει σε **Χρειάζεται έλεγχο**.</span><span class="sxs-lookup"><span data-stu-id="1c069-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]