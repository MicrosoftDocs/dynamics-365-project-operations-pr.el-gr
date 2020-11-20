---
title: Δημιουργία έργου
description: Πώς γίνεται η δημιουργία έργου στο Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/13/2020
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
ms.openlocfilehash: de26bb4c3fa0ee8abf6edf5494968d1d0403266a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133098"
---
# <a name="create-a-project-project-service"></a><span data-ttu-id="2349f-103">Δημιουργία έργου (Project Service)</span><span class="sxs-lookup"><span data-stu-id="2349f-103">Create a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="2349f-104">Δημιουργήστε ένα έργο χρησιμοποιώντας τις δυνατότητες [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στο [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)], όταν θέλετε να δημιουργήσετε μια ευκαιρία, προσφορά ή σύμβαση για υπηρεσίες που βασίζονται σε έργο.</span><span class="sxs-lookup"><span data-stu-id="2349f-104">Create a project using the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] when you want to create an opportunity, quote, or contract for project-based services.</span></span> <span data-ttu-id="2349f-105">Οι δυνατότητες [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] σας βοηθούν να διαχειριστείτε το έργο σας από την ευκαιρία έως την ολοκλήρωση.</span><span class="sxs-lookup"><span data-stu-id="2349f-105">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities help you manage your project from opportunity through completion.</span></span> <span data-ttu-id="2349f-106">Κατά τη δημιουργία ενός έργου, θα δημιουργήσετε επίσης μια δομή ανάλυσης εργασίας, η οποία επηρεάζει τις προσφορές σας, τις εκτιμήσεις κόστους και τη διαχείριση πόρων.</span><span class="sxs-lookup"><span data-stu-id="2349f-106">When you create a project, you’ll also create a work breakdown structure, which affects your quotes, cost estimates, and resource management.</span></span>  
  
1.  <span data-ttu-id="2349f-107">Μεταβείτε στο μενού **Project Service > Έργα**.</span><span class="sxs-lookup"><span data-stu-id="2349f-107">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="2349f-108">Επιλέξτε **Νέο έργο**.</span><span class="sxs-lookup"><span data-stu-id="2349f-108">Click **New Project**.</span></span>  
  
3.  <span data-ttu-id="2349f-109">Στην περιοχή **Σύνοψη**, πληκτρολογήστε ένα όνομα για το έργο σας και, στη συνέχεια, συμπληρώστε όσες λεπτομέρειες μπορείτε.</span><span class="sxs-lookup"><span data-stu-id="2349f-109">In the **Summary** area, enter a name for your project, and then fill in as many of the details as you can.</span></span> <span data-ttu-id="2349f-110">Τα στοιχεία που επισημαίνονται με κόκκινο αστερίσκο (\*) είναι υποχρεωτικά.</span><span class="sxs-lookup"><span data-stu-id="2349f-110">Items marked with a red asterisk (\*) are required.</span></span>  
  
4.  <span data-ttu-id="2349f-111">Επιλέξτε **Αποθήκευση**, για να δημιουργήσετε το έργο σας, έτσι ώστε να μπορείτε να συνεχίσετε να το επεξεργάζεστε.</span><span class="sxs-lookup"><span data-stu-id="2349f-111">Click **Save** to create your project so you can continue editing it.</span></span>  
  
<span data-ttu-id="2349f-112">Στη συνέχεια, θα δημιουργήσετε μια δομή ανάλυσης εργασίας για το έργο σας, ώστε να καθορίσετε τις εργασίες, το χρονισμό και τους ρόλους πόρων που απαιτούνται για το έργο.</span><span class="sxs-lookup"><span data-stu-id="2349f-112">Next, you’ll create a work breakdown structure for your project to define the tasks, timing, and resource roles needed for the project.</span></span>  

> [!NOTE]
> <span data-ttu-id="2349f-113">Κατά τον προγραμματισμό, το Project Service Automation σέβεται τη ζώνη ώρας του εφαρμοζόμενου προτύπου **Ώρας εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="2349f-113">When scheduling, Project Service Automation respects the time zone of the applied **Work Hour** template.</span></span> <span data-ttu-id="2349f-114">Ωστόσο, κατά την προβολή των εργασιών χρονοδιαγράμματος, οι ημερομηνίες έναρξης και λήξης μιας εργασίας θα εμφανίζονται στην ζώνη ώρας του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="2349f-114">However, when viewing the schedule tasks, the start and end dates of a task will be displayed in the user's time zone.</span></span> <span data-ttu-id="2349f-115">Αυτό ισχύει για άλλες προβολές με χρονική κλιμάκωση στη φόρμα **Έργου**.</span><span class="sxs-lookup"><span data-stu-id="2349f-115">This applies to other time-phased views in the **Project** form.</span></span> <span data-ttu-id="2349f-116">Εάν η ζώνη ώρας του χρήστη δεν αντιστοιχεί στη ζώνη ώρας του προτύπου ωρών εργασίας που έχει εφαρμοστεί στο έργο, θα εμφανιστεί μια προειδοποίηση που θα εξηγήσει τη διαφορά.</span><span class="sxs-lookup"><span data-stu-id="2349f-116">If the user's time zone does not match the time zone of the work hour template applied to the project, a warning which explains the difference will occur.</span></span> 
  
### <a name="see-also"></a><span data-ttu-id="2349f-117">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="2349f-117">See Also</span></span>  
 [<span data-ttu-id="2349f-118">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="2349f-118">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
