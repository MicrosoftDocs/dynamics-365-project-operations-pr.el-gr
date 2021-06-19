---
title: Υποβολή μιας αίτησης πόρου
description: Μπορείτε να υποβάλετε μια απαίτηση πόρου που έχει δημιουργηθεί ως αίτημα πόρου. Στη συνέχεια, το αίτημα αποστέλλεται σε έναν υπεύθυνο διαχείρισης πόρων για ολοκλήρωση.
author: ruhercul
ms.date: 10/04/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6ac0044a27d1e506c9c62c477014017fd0ca06cb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014026"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="b1ba0-104">Υποβολή μιας αίτησης πόρου</span><span class="sxs-lookup"><span data-stu-id="b1ba0-104">Submit a resource request</span></span>

<span data-ttu-id="b1ba0-105">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="b1ba0-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b1ba0-106">Μπορείτε να υποβάλετε μια απαίτηση πόρου που έχει δημιουργηθεί ως αίτημα πόρου.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="b1ba0-107">Στη συνέχεια, το αίτημα αποστέλλεται σε έναν υπεύθυνο διαχείρισης πόρων για ολοκλήρωση.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="b1ba0-108">Στο Dynamics 365 Project Operations, στη σελίδα **Έργα**, επιλέξτε την καρτέλα **Ομάδα** για να προβάλετε μια λίστα με πόρους με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="b1ba0-109">Επιλέξτε τον γενικό πόρο που διαθέτει μια απαίτηση πόρου από τη λίστα και, μετά επιλέξτε **Υποβολή αίτησης**.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="b1ba0-110">Η κατάσταση αίτησης του γενικού μέλους ομάδας θα αλλάξει σε **Υποβλήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="b1ba0-111">Μετά την ολοκλήρωση της αίτησης, ο γενικός πόρος θα αντικατασταθεί από έναν καθορισμένο πόρο, εάν ο υπεύθυνος πόρου εκπληρώσει την αίτηση με την κράτηση ενός καθορισμένου πόρου.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="b1ba0-112">Διαφορετικά, αν ο υπεύθυνος πόρου προτείνει έναν καθορισμένο πόρο, τότε ο γενικός πόρος θα παραμείνει στην ομάδα και η κατάσταση αίτησης θα αλλάξει σε **Χρειάζεται έλεγχο**.</span><span class="sxs-lookup"><span data-stu-id="b1ba0-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]