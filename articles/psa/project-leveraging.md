---
title: Εκτιμήσεις πωλήσεων και έργων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο αξιοποίησης του χρονοδιαγράμματος και των εκτιμήσεων στη διαδικασία πωλήσεων.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: d8bb380519759659dc1b4151b62228a626ee7a26
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120678"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="34255-103">Εκτιμήσεις πωλήσεων και έργων</span><span class="sxs-lookup"><span data-stu-id="34255-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="34255-104">Κατά τη διάρκεια της διαδικασίας πωλήσεων, μπορείτε να δημιουργήσετε εκτιμήσεις πωλήσεων συνδέοντας ένα έργο με μια προσφορά πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="34255-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="34255-105">Με αυτόν τον τρόπο, η προσδιοριστική εκτίμηση μπορεί να πραγματοποιηθεί κατά τη διαδικασία πωλήσεων, προκειμένου να αξιοποιήσετε τις δυνατότητες προγραμματισμού και εκτίμησης του έργου.</span><span class="sxs-lookup"><span data-stu-id="34255-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="34255-106">Εάν η πώληση γίνει, το χρονοδιάγραμμα που χρησιμοποιήθηκε για λόγους εκτίμησης πωλήσεων μπορεί να χρησιμοποιηθεί ως βάση για περαιτέρω τελειοποίηση του σχεδίου έργου.</span><span class="sxs-lookup"><span data-stu-id="34255-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="34255-107">Σύνδεση ενός έργου με μια γραμμή προσφοράς</span><span class="sxs-lookup"><span data-stu-id="34255-107">Linking a project to a quote line</span></span>

<span data-ttu-id="34255-108">Όταν δημιουργείτε μια γραμμή προσφοράς βάσει έργου, μπορείτε να δημιουργήσετε ένα νέο έργο ή να συσχετίσετε ένα υπάρχον έργο pn στη σελίδα **Γραμμή προσφοράς**.</span><span class="sxs-lookup"><span data-stu-id="34255-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![Φόρμα γραμμής προσφοράς](media/project-8.png)
 
<span data-ttu-id="34255-110">Όταν δημιουργείτε ένα νέο έργο από τις λεπτομέρειες της γραμμής προσφοράς, μπορείτε να εκμεταλλευτείτε τα πρότυπα έργου.</span><span class="sxs-lookup"><span data-stu-id="34255-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="34255-111">Τα πρότυπα έργου είναι σχέδια μοντέλου που αντιπροσωπεύουν τυπικά σχέδια έργου και οικονομικές εκτιμήσεις που είναι συνηθισμένες σε έναν οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="34255-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="34255-112">Επίσης, μπορούν να αναπαριστούν αντίγραφα σχεδίων και προβλέψεων έργου από προηγούμενα έργα.</span><span class="sxs-lookup"><span data-stu-id="34255-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![Λεπτομέρειες γραμμής προσφοράς](media/project-9.png)
  
<span data-ttu-id="34255-114">Όταν δημιουργείτε το έργο από την προσφορά, το έργο συσχετίζεται αυτόματα με τη γραμμή της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="34255-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="34255-115">Στοιχεία των προβλέψεων σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="34255-115">Components of estimates in a project</span></span>

<span data-ttu-id="34255-116">Ένα χρονοδιάγραμμα σάς δίνει τη δυνατότητα να διαιρέσετε την εργασία σε εργασίες, να διατηρήσετε μια ιεραρχία εργασιών, να καθορίσετε τους πόρους που απαιτούνται για την ολοκλήρωση μιας εργασίας και να αναθέσετε μια εκτίμηση της προσπάθειας που απαιτείται για την ολοκλήρωση μιας εργασίας.</span><span class="sxs-lookup"><span data-stu-id="34255-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="34255-117">Μπορείτε να καθορίσετε τις προσπάθειες εργασίας και τις προβλέψεις χρονοδιαγράμματος χρησιμοποιώντας τα πεδία στην καρτέλα **Χρονοδιάγραμμα** της σελίδας **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="34255-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="34255-118">Επειδή ένας τιμοκατάλογος συσχετίζεται με το έργο, οι οικονομικές εκτιμήσεις υπολογίζονται με τη χρήση του κόστους και των τιμών πώλησης που καθορίζονται στον τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="34255-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="34255-119">Εισαγωγή εκτιμήσεων από ένα έργο σε μια προσφορά</span><span class="sxs-lookup"><span data-stu-id="34255-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="34255-120">Αφού καθορίσετε τις εκτιμήσεις του έργου, μπορείτε να τις εισαγάγετε στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="34255-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="34255-121">Στη σελίδα **Λεπτομέρειες γραμμής προσφοράς** επιλέξτε **Εισαγωγή από εκτιμήσεις** στην κορδέλα για να συνοψίσετε εκτιμήσεις έργου ανά τύπο συναλλαγής, ρόλο ή επίπεδο εργασίας.</span><span class="sxs-lookup"><span data-stu-id="34255-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
