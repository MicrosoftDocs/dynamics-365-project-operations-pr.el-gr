---
title: Παρακολούθηση της κατάστασης ενός έργου
description: Πώς γίνεται η παρακολούθηση της κατάστασης ενός έργου στο Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: e9c8b594d468016264d0b4d9745597a35f55e50e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149588"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="b5237-103">Παρακολούθηση της κατάστασης ενός έργου (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b5237-103">Track a project’s status (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b5237-104">Χρησιμοποιήστε το [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] για να παρακολουθήσετε την πρόοδο του έργου ενός πελάτη.</span><span class="sxs-lookup"><span data-stu-id="b5237-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="b5237-105">Καθώς εξελίσσεται η δέσμευση, τα στάδια του έργου ενημερώνονται, ώστε να αποτυπώνουν το στάδιο της δέσμευσης:</span><span class="sxs-lookup"><span data-stu-id="b5237-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="b5237-106">**Δημιουργία**</span><span class="sxs-lookup"><span data-stu-id="b5237-106">**New**</span></span>    | <span data-ttu-id="b5237-107">Όταν δημιουργείτε ένα έργο, το στάδιο έχει οριστεί στην επιλογή **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="b5237-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="b5237-108">Εάν δημιουργήσατε το έργο από ένα πρότυπο, στο στάδιο αυτό το έργο μπορεί να περιέχει ένα χρονοδιάγραμμα, εκτιμήσεις και τα δεδομένα της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="b5237-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="b5237-109">Διαφορετικά, θα αποτελεί την υπογράμμιση του έργου και πρέπει να εισαγάγετε με μη αυτόματο τρόπο τα υπόλοιπα στοιχεία του έργου.</span><span class="sxs-lookup"><span data-stu-id="b5237-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="b5237-110">**Προσφορά**</span><span class="sxs-lookup"><span data-stu-id="b5237-110">**Quote**</span></span>   |      <span data-ttu-id="b5237-111">Όταν συσχετίζετε ένα έργο με μια προσφορά ή το δημιουργείτε από μια προσφορά, το στάδιο του έργου έχει οριστεί στην επιλογή **Προσφορά** και ενημερώνονται επίσης οι εκτιμώμενες ημερομηνίες έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="b5237-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="b5237-112">Αν το έργο βρίσκεται στο στάδιο της προσφοράς, οι λεπτομέρειες σχετικά με την προσφορά εμφανίζονται στην καρτέλα **Sales** της σελίδας **Project**.</span><span class="sxs-lookup"><span data-stu-id="b5237-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="b5237-113">**Πρόγραμμα**</span><span class="sxs-lookup"><span data-stu-id="b5237-113">**Plan**</span></span>   |                                     <span data-ttu-id="b5237-114">Όταν κερδίζετε μια προσφορά που έχει συσχετιστεί με ένα έργο και όταν η δέσμευση εξελίσσεται στο στάδιο της σύμβασης, το στάδιο του έργου ενημερώνεται στην επιλογή **Πρόγραμμα**.</span><span class="sxs-lookup"><span data-stu-id="b5237-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="b5237-115">Οι λεπτομέρειες της σύμβασης εμφανίζονται στην καρτέλα **Sales** στη σελίδα **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="b5237-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="b5237-116">**Ολοκλήρωση**</span><span class="sxs-lookup"><span data-stu-id="b5237-116">**Complete**</span></span> |                    <span data-ttu-id="b5237-117">Όταν ολοκληρωθεί η εργασία του έργου, μπορείτε να ορίσετε το στάδιο στην επιλογή **Ολοκληρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="b5237-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="b5237-118">Κατά το στάδιο του έργου έχει οριστεί ως ολοκληρωμένο, είναι κατανοητό ότι η εργασία έχει ολοκληρωθεί κατά 100%, αλλά το έργο παραμένει ανοιχτό για να καταγραφούν τυχόν χρόνοι αναμονής ή εγγραφές εξόδων.</span><span class="sxs-lookup"><span data-stu-id="b5237-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="b5237-119">**Κλείσιμο**</span><span class="sxs-lookup"><span data-stu-id="b5237-119">**Close**</span></span>   |           <span data-ttu-id="b5237-120">Όταν έχουν καταγραφεί όλες οι συναλλαγές στο έργο και δεν αναμένετε να καταγραφούν άλλα, μπορείτε να ορίσετε με μη αυτόματο τρόπο το στάδιο στην επιλογή **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="b5237-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="b5237-121">Όταν το έργο έχει οριστεί στην επιλογή **Κλείσιμο**, δεν είναι δυνατή η καταγραφή άλλων συναλλαγών στο έργο και το έργο θα είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b5237-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="b5237-122">Για την παρακολούθηση της κατάστασης ενός έργου</span><span class="sxs-lookup"><span data-stu-id="b5237-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="b5237-123">Μεταβείτε στο μενού **Project Service > Έργα**.</span><span class="sxs-lookup"><span data-stu-id="b5237-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="b5237-124">Επιλέξτε το έργο στο οποίο θέλετε να εργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="b5237-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="b5237-125">Στη γραμμή στο επάνω μέρος της οθόνης, επιλέξτε το κάτω βέλος δίπλα από το όνομα του έργου και, στη συνέχεια, κάντε κλικ στο κουμπί **Παρακολούθηση έργου**.</span><span class="sxs-lookup"><span data-stu-id="b5237-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="b5237-126">Επιλέξτε **Παρακολούθηση προσπάθειας** ή **Παρακολούθηση κόστους** στην αναπτυσσόμενη λίστα πάνω από τη λίστα εργασιών.</span><span class="sxs-lookup"><span data-stu-id="b5237-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="b5237-127">Κάντε διπλό κλικ σε οποιαδήποτε εργασία για να την επεξεργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="b5237-127">Double-click any task to edit it.</span></span> <span data-ttu-id="b5237-128">Μπορείτε επίσης να μετακινήσετε ή να αλλάξετε το μέγεθος των γραμμών στο γράφημα Gantt, για να αλλάξετε την ώρα και την πρόοδο της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="b5237-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="b5237-129">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="b5237-129">See Also</span></span>  
 [<span data-ttu-id="b5237-130">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="b5237-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
