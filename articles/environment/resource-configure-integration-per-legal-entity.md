---
title: Ρύθμιση παραμέτρων για την ενοποίηση του Project Operations ανά νομική οντότητα
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης της ενοποίησης ανά νομική οντότητα στο Project Operations.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e5a12de275a9f886434da45fbbed5140e3913d83
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000076"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="46ee5-103">Ρύθμιση παραμέτρων για την ενοποίηση του Project Operations ανά νομική οντότητα</span><span class="sxs-lookup"><span data-stu-id="46ee5-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="46ee5-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="46ee5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="46ee5-105">Αυτό το θέμα σάς καθοδηγεί στα βήματα που απαιτούνται για τη ρύθμιση παραμέτρων του Dynamics 365 Project Operations ανά νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="46ee5-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="46ee5-106">Ενεργοποίηση βασικών δυνατοτήτων στο Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="46ee5-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="46ee5-107">Ολοκληρώστε τα παρακάτω βήματα για να ενεργοποιήσετε τις απαιτούμενες δυνατότητες.</span><span class="sxs-lookup"><span data-stu-id="46ee5-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="46ee5-108">Στο Dynamics 365 Finance, μεταβείτε στον χώρο εργασίας **Διαχείριση δυνατοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="46ee5-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="46ee5-109">Στη **Λίστα δυνατοτήτων**, βρείτε και ενεργοποιήστε τις ακόλουθες δυνατότητες:</span><span class="sxs-lookup"><span data-stu-id="46ee5-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="46ee5-110">**Ενεργοποίηση πολλών γραμμών σύμβασης για ένα έργο**</span><span class="sxs-lookup"><span data-stu-id="46ee5-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="46ee5-111">**Ενεργοποίηση του Project Operations στο Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="46ee5-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="46ee5-112">Εάν δεν βλέπετε τις **Βασικές δυνατότητες**, επαληθεύστε ότι η έκδοση Finance ικανοποιεί την ελάχιστη απαίτηση έκδοσης (έκδοση εφαρμογής 10.0.13 με όλες τις ενημερώσεις ποιότητας που εφαρμόζονται ή μεταγενέστερη).</span><span class="sxs-lookup"><span data-stu-id="46ee5-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="46ee5-113">Επιλέξτε **Έλεγχος για ενημερώσεις** για να ανανεώσετε τη λίστα δυνατοτήτων.</span><span class="sxs-lookup"><span data-stu-id="46ee5-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="46ee5-114">Ορισμός το σενάριο ανάπτυξης του Project Operations για μια νομική οντότητα</span><span class="sxs-lookup"><span data-stu-id="46ee5-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="46ee5-115">Μπορείτε να ενεργοποιήσετε το Project Operations στο Dynamics 365 Customer Engagement σε ένα επίπεδο νομικής οντότητας.</span><span class="sxs-lookup"><span data-stu-id="46ee5-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="46ee5-116">Μπορείτε να έχετε μια νομική οντότητα που χρησιμοποιεί το Project Operations στο Dynamics 365 Customer Engagement για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.</span><span class="sxs-lookup"><span data-stu-id="46ee5-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="46ee5-117">Στο ίδιο περιβάλλον, μπορείτε να έχετε μια άλλη νομική οντότητα που χρησιμοποιεί το Project Operations για σενάρια εφοδιασμένα/παραγγελίας παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="46ee5-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="46ee5-118">Στο Dynamics 365 Finance, μεταβείτε στη **Διαχείριση έργου και λογιστική** > **Ρύθμιση** > **Παράμετροι καθολικής διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="46ee5-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="46ee5-119">Στη λίστα με τις διαθέσιμες νομικές οντότητες, επιλέξτε τις οντότητες όπου θα ενεργοποιηθούν πολλαπλές γραμμές σύμβασης και το Project Operations στις δυνατότητες του Dynamics 365 Customer Engagement.</span><span class="sxs-lookup"><span data-stu-id="46ee5-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="46ee5-120">Αφήστε μη επιλεγμένες νομικές οντότητες που θα χρησιμοποιούν το Project Operations για σενάρια εφοδιασμού/παραγγελίας παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="46ee5-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="46ee5-121">Μια νομική οντότητα μπορεί να επιλεγεί μόνο εάν δεν υπάρχουν ήδη υπάρχοντα έργα.</span><span class="sxs-lookup"><span data-stu-id="46ee5-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="46ee5-122">Ρύθμιση παραμέτρων διαχείρισης έργου και λογιστικής</span><span class="sxs-lookup"><span data-stu-id="46ee5-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="46ee5-123">Κάθε νομική οντότητα που χρησιμοποιεί το Project Operations στο Dynamics 365 Customer Engagement χρειάζεται ένα σύνολο προεπιλεγμένων παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="46ee5-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="46ee5-124">Αυτές οι παράμετροι ρυθμίζονται στην καρτέλα **Project Operations** στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="46ee5-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="46ee5-125">Οι παράμετροι είναι οι εξής:</span><span class="sxs-lookup"><span data-stu-id="46ee5-125">The parameters are:</span></span>

  - <span data-ttu-id="46ee5-126">**Προεπιλογές τύπου χρέωσης**: Το Project Operations χρησιμοποιεί ένα σταθερό σύνολο προεπιλογών τύπου χρέωσης, το οποίο πρέπει να αντιστοιχιστεί στις ιδιότητες γραμμής του Finance.</span><span class="sxs-lookup"><span data-stu-id="46ee5-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="46ee5-127">Δημιουργήστε μια καρτέλα για κάθε τύπο χρέωσης: **Δεν καθορίζεται**, **Χρεώσιμο**, **Μη χρεώσιμο**, **Δωρεάν** και **Μη διαθέσιμο**.</span><span class="sxs-lookup"><span data-stu-id="46ee5-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="46ee5-128">**Προεπιλογές κατηγορίας έργου**: Επιλέξτε τις προεπιλεγμένες κατηγορίες έργου που θα χρησιμοποιηθούν για κάθε τύπο συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="46ee5-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="46ee5-129">Αυτές οι προεπιλογές θα χρησιμοποιηθούν στο **Ημερολόγιο ενοποίησης Project Operations** και σε εκτιμήσεις όπου καμία κατηγορία συναλλαγής δεν έχει καθοριστεί για το πραγματικό έργο.</span><span class="sxs-lookup"><span data-stu-id="46ee5-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="46ee5-130">**Προβλέψεις**: Επιλέξτε το μοντέλο πρόβλεψης που θα χρησιμοποιηθεί για τις εκτιμήσεις χρόνου και εξόδων.</span><span class="sxs-lookup"><span data-stu-id="46ee5-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]