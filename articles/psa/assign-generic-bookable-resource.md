---
title: Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια ομάδα εργασιών και έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κράτηση γενικών πόρων σε εργασίες και ομάδες έργου.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
ms.topic: article
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
ms.openlocfilehash: ca0999ae5413d824dd1384fe2262e5226695a5f8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076931"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="17a93-103">Ανάθεση γενικών πόρων με δυνατότητα κράτησης σε μια εργασία και δημιουργία απαιτήσεων πόρου</span><span class="sxs-lookup"><span data-stu-id="17a93-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="17a93-104">Εκτός από την κράτηση και την ανάθεση καθορισμένων ή πραγματικών πόρων στο έργο σας, μπορείτε να αναθέσετε γενικούς πόρους σε εργασίες έργου.</span><span class="sxs-lookup"><span data-stu-id="17a93-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="17a93-105">Οι πόροι αυτοί μπορούν να χρησιμεύσουν ως χαρακτήρες κράτησης θέσης για τους καθορισμένους πόρους μέχρι να είστε έτοιμοι να αντιστοιχίσετε καθορισμένους πόρους στο έργο σας.</span><span class="sxs-lookup"><span data-stu-id="17a93-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="17a93-106">Στο Project Service Automation (PSA), ανοίξτε τη σελίδα **Έργο** και στην καρτέλα **Χρονοδιάγραμμα** , καταγράψτε το όνομα θέσης του γενικού πόρου στο κελί **Πόρος** του χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="17a93-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="17a93-107">Εναλλακτικά, κάντε κλικ στο εικονίδιο **Πόρος** στο κελί για να ανοίξετε τον επιλογέα πόρων και, στη συνέχεια, καταγράψτε το όνομα του γενικού πόρου που θέλετε να δημιουργήσετε.</span><span class="sxs-lookup"><span data-stu-id="17a93-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![Δημιουργία και ανάθεση σε ένα γενικό μέλος της ομάδας](media/RM-how-to-9.png)

<span data-ttu-id="17a93-109">Με αυτήν την ενέργεια θα ανοίξει ο πίνακας **Γρήγορη δημιουργία: Μέλος ομάδας έργου**.</span><span class="sxs-lookup"><span data-stu-id="17a93-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="17a93-110">Καταγράψτε τον ρόλο και την οργανωτική μονάδα του γενικού έλους της ομάδας πόρων και μετά πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="17a93-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![Γρήγορη δημιουργία γενικού μέλους ομάδας](media/RM-how-to-10.png)

3. <span data-ttu-id="17a93-112">Αφού δημιουργήσετε το νέο γενικό μέλος της ομάδας πόρων, του ανατίθεται η εργασία.</span><span class="sxs-lookup"><span data-stu-id="17a93-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="17a93-113">Μπορείτε να συνεχίσετε να αναθέτετε αυτόν τον γενικό πόρο σε άλλες εργασίες του χρονοδιαγράμματος εργασιών.</span><span class="sxs-lookup"><span data-stu-id="17a93-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![Ανάθεση υπάρχοντος γενικού μέλους ομάδας σε εργασίες](media/RM-how-to-11.png)

4. <span data-ttu-id="17a93-115">Αφού αναθέσετε τον γενικό πόρο, μπορείτε να δημιουργήσετε μια απαίτηση πόρου και να την εκπληρώσετε με άμεση κράτηση ή υποβολή αιτήματος πόρου σε ένα διαχειριστή πόρων.</span><span class="sxs-lookup"><span data-stu-id="17a93-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![Δημιουργία μιας απαίτησης για ένα γενικό μέλος της ομάδας](media/RM-how-to-12.png)

<span data-ttu-id="17a93-117">Στο πλέγμα του μέλους ομάδας, εκτός από τη δυνατότητα χρήσης του επιλογέα πόρων όπως προαναφέρθηκε, μπορείτε να προσθέσετε γενικούς πόρους απευθείας.</span><span class="sxs-lookup"><span data-stu-id="17a93-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="17a93-118">Οι πόροι προστίθενται με μια απαίτηση πόρου η οποία βασίζεται στις ημερομηνίες έναρξης/λήξης και στη μέθοδο ανάθεσης που καθορίζεται στον πίνακα **Γρήγορη δημιουργία: Μέλος ομάδας έργου**.</span><span class="sxs-lookup"><span data-stu-id="17a93-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="17a93-119">Μπορείτε να δείτε μια διαφορά εάν προσθέσετε το γενικό μέλος ομάδας απευθείας και, στη συνέχεια, αναθέσετε περισσότερες εργασίες στο γενικό πόρο από όσες ώρες χρειάστηκαν να καλυφθούν.</span><span class="sxs-lookup"><span data-stu-id="17a93-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="17a93-120">Κάντε κλικ στη **Δημιουργία απαίτησης** για την αναδημιουργία της απαίτησης εξισορρόπησης των απαιτούμενων ωρών σε σχέση με τις αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="17a93-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="17a93-121">Μπορείτε επίσης να κάνετε κλικ στη σύνδεση **Απαίτηση πόρου** στο πλέγμα ομάδας για να ανοίξετε την απαίτηση και να προσθέσετε δεξιότητες, προτιμώμενους πόρους κτλ.</span><span class="sxs-lookup"><span data-stu-id="17a93-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![Απαίτηση πόρου](media/RM-how-to-13.png)

