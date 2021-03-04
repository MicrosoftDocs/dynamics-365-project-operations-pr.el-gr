---
title: Παροχή εκτιμήσεων εργασίας για ένα έργο κατά τη διάρκεια της διαδικασίας πώλησης
description: Πώς γίνεται η παροχή εκτιμήσεων εργασίας για ένα έργο κατά τη διάρκεια της διαδικασίας πωλήσεων στο Project Service
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
ms.openlocfilehash: e9382127b2ce0b157d681fc77d67200ba9c5e59d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147968"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="7c0c9-103">Παροχή εκτιμήσεων εργασίας για ένα έργο, κατά τη διάρκεια της διαδικασίας πώλησης (Project Service)</span><span class="sxs-lookup"><span data-stu-id="7c0c9-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="7c0c9-104">Κατά τη διάρκεια της διαδικασίας πώλησης, μπορείτε να επεξεργαστείτε εκτιμήσεις πωλήσεων από το μηδέν έως τις γραμμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> <span data-ttu-id="7c0c9-105">Οι δυνατότητες [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στο [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] παρέχουν έναν πιο επιστημονικό και καθοριστικό τρόπο για να προκύπτουν εκτιμήσεις πωλήσεων με ανάλυση των στοιχείων εργασίας και συσχέτιση σχετικών χαρακτηριστικών που συμβάλλουν με τις εκτιμήσεις για το έργο στη δομή ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="7c0c9-106">Μόλις κερδίσετε την πώληση, μπορείτε να χρησιμοποιήσετε τη συσχετισμένη δομή ανάλυσης εργασίας στο σχέδιο του έργου σας, ανάλογα με τις ανάγκες, για την επιτυχή ολοκλήρωση του έργου σας.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="7c0c9-107">Σύνδεση ενός έργου με μια γραμμή προσφοράς</span><span class="sxs-lookup"><span data-stu-id="7c0c9-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="7c0c9-108">Κατά τη δημιουργία μιας γραμμής προσφοράς με βάση ένα έργο, μπορείτε να δημιουργήσετε ένα νέο έργο από τη γραμμή της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="7c0c9-109">Μπορείτε να χρησιμοποιήσετε, στη συνέχεια, πρότυπα έργου, τα οποία είτε είναι ήδη ρυθμισμένα τυπικά σχέδια έργων και οικονομικές εκτιμήσεις που είναι κοινές για τον οργανισμό σας ή αντίγραφο του σχεδίου του έργου σας και εκτιμήσεις από προηγούμενα έργα.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="7c0c9-110">Όταν δημιουργείτε ένα έργο, επιλέγοντας ένα πρότυπο έργου παρέχει μια βάση για να περιορίσετε το σχέδιο, τις εκτιμήσεις και τις απαιτήσεις ρόλων του έργου.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="7c0c9-111">Με τη δημιουργία του έργου σας από την προσφορά, το έργο συσχετίζεται αυτόματα με τη γραμμή της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="7c0c9-112">Στοιχεία εκτίμησης έργου</span><span class="sxs-lookup"><span data-stu-id="7c0c9-112">Project estimate components</span></span>  
 <span data-ttu-id="7c0c9-113">Η δομή ανάλυσης εργασίας σε ένα έργο παρέχει έναν τρόπο για να αναλύετε εργασίες, να διατηρείτε μια ιεραρχία των εργασιών και να αντιστοιχίζετε μια εκτίμηση της απαιτούμενης προσπάθειας για την ολοκλήρωση κάθε εργασίας.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="7c0c9-114">Μπορείτε επίσης να συσχετίσετε ρόλους σε μια εργασία για να υποδείξετε μια εκτίμηση του τύπου του απαιτούμενου πόρου για την ολοκλήρωση μιας εργασίας και ενός χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="7c0c9-115">Η δομή ανάλυσης εργασίας σάς βοηθάει να προσδιορίσετε τις εκτιμήσεις προσπάθειας εργασίας και χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="7c0c9-116">Από προεπιλογή, το έργο χρησιμοποιεί προεπιλεγμένους τιμοκαταλόγους που ορίσατε προηγουμένως.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="7c0c9-117">Οι τιμές κόστους και πώλησης που ορίζονται στους τιμοκαταλόγους σάς βοηθάνε να προσδιορίσετε τις οικονομικές εκτιμήσεις για την ανάλυση της εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="7c0c9-118">Εάν το έργο σας έχει συσχετιστεί με μια προσφορά και η προσφορά έχει διαφορετικό τιμοκατάλογο από την προεπιλεγμένη, ο τιμοκατάλογος της προσφοράς χρησιμοποιείται για οικονομικές εκτιμήσεις.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="7c0c9-119">Εισαγωγή εκτιμήσεων από ένα έργο σε μια προσφορά</span><span class="sxs-lookup"><span data-stu-id="7c0c9-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="7c0c9-120">Εφόσον έχετε εκτιμήσεις έργου στο έργο, μπορείτε να εισαγάγετε τις εκτιμήσεις αυτές στη γραμμή προσφοράς:</span><span class="sxs-lookup"><span data-stu-id="7c0c9-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="7c0c9-121">Στην περιοχή **Λεπτομέρειες γραμμής προσφοράς**, κάντε κλικ στο κουμπί **Εισαγωγή από εκτιμήσεις**.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-121">In **Quote Line Details**, click **Import from estimates**.</span></span> 

-   <span data-ttu-id="7c0c9-122">Επιλέξτε εάν θα εισαγάγετε εκτιμήσεις έργων, οι οποίες θα συνοψίζονται ανά τύπο συναλλαγής, ρόλο ή επίπεδο κόμβου δομής ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="7c0c9-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="7c0c9-123">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="7c0c9-123">See Also</span></span>  
 [<span data-ttu-id="7c0c9-124">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="7c0c9-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
