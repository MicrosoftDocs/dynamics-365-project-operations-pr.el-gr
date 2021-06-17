---
title: Δημιουργία προτύπου έργου
description: Πώς γίνεται η δημιουργία προτύπου έργου στο Project Service
author: ruhercul
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
ms.openlocfilehash: 148bf1d42b640ff7b58b13bb0c30c7e583d803c8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997241"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="149aa-103">Δημιουργία προτύπου έργου (Project Service)</span><span class="sxs-lookup"><span data-stu-id="149aa-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="149aa-104">Τα πρότυπα έργου σάς εξοικονομούν χρόνο αν η εταιρεία σας υποβάλλει συχνά προσφορές για παρόμοιους τύπους έργων.</span><span class="sxs-lookup"><span data-stu-id="149aa-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="149aa-105">Παρέχουν ένα τυπικό σύνολο ρόλων και τις εκτιμώμενες ώρες για έναν τύπο έργου.</span><span class="sxs-lookup"><span data-stu-id="149aa-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="149aa-106">Οι διαχειριστές λογαριασμών και οι διαχειριστές έργων μπορούν να δημιουργήσουν έργα που βασίζονται σε ένα πρότυπο έργου ή μπορούν να αντιγράψουν το πρότυπο και να κάνουν ένα δικό τους.</span><span class="sxs-lookup"><span data-stu-id="149aa-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="149aa-107">Στοιχεία προτύπου έργου</span><span class="sxs-lookup"><span data-stu-id="149aa-107">Components of project template</span></span>
 <span data-ttu-id="149aa-108">Ένα πρότυπο έργου αποτελείται από τρία στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="149aa-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="149aa-109">**Δομή ανάλυσης εργασίας**: Μια δομή ανάλυσης εργασίας σε ένα πρότυπο έργου έχει το ίδιο σύνολο στοιχείων όπως και το έργο.</span><span class="sxs-lookup"><span data-stu-id="149aa-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="149aa-110">Μπορείτε να δημιουργήσετε μια ιεραρχία εργασιών, να συσχετίσετε ρόλους σε εργασία, να ορίσετε χαρακτηριστικά χρονοδιαγράμματος, να ορίσετε εξαρτήσεις και να προβάλλετε όλα τα δεδομένα σε Gantt.</span><span class="sxs-lookup"><span data-stu-id="149aa-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="149aa-111">Η δομή ανάλυσης εργασίας σε πρότυπα έργου υποστηρίζει επίσης λειτουργίες εργασίας για κάθε εργασία.</span><span class="sxs-lookup"><span data-stu-id="149aa-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="149aa-112">Δεν υπάρχει διαφορά μεταξύ ενός προτύπου έργου και ενός έργου κατά τη δημιουργία χρονοδιαγράμματος εργασίας.</span><span class="sxs-lookup"><span data-stu-id="149aa-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="149aa-113">**Εκτιμήσεις έργου**: Οι εκτιμήσεις έργου σε πρότυπα λειτουργούν με τον ίδιο τρόπο όπως και στα έργα, με τη διαφορά ότι οι τιμοκατάλογοι για προεπιλεγμένες επιλογές του κόστους και των τιμών πώλησης είναι πάντα το προεπιλεγμένο κόστος και οι τιμοκατάλογοι πωλήσεων που ορίζονται στις παραμέτρους [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="149aa-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="149aa-114">Οι υπόλοιπες λειτουργίες είναι οι ίδιες με αυτές σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="149aa-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="149aa-115">**Σχηματισμός ομάδας έργου**: Κατά τον σχηματισμό μιας ομάδας έργου για ένα πρότυπο έργου, δεν μπορείτε να κάνετε κράτηση ενός πόρου με όνομα σε ένα πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="149aa-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="149aa-116">Μπορείτε να χρησιμοποιήσετε τη **Δημιουργία ομάδας έργου** στη δομή ανάλυσης εργασίας για να δημιουργήσετε ένα σύνολο γενικών πόρων.</span><span class="sxs-lookup"><span data-stu-id="149aa-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="149aa-117">Μπορείτε επίσης να καθορίσετε τις απαιτούμενες ικανότητες και πιστοποιήσεις κατάρτισης για γενικούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="149aa-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="149aa-118">Δεν μπορείτε να αντικαταστήσετε έναν γενικό πόρο με έναν πόρο με δυνατότητα κράτησης σε πρότυπα έργου.</span><span class="sxs-lookup"><span data-stu-id="149aa-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="149aa-119">Δημιουργία έργου από πρότυπο</span><span class="sxs-lookup"><span data-stu-id="149aa-119">Create a project from a template</span></span>  
 <span data-ttu-id="149aa-120">Μπορείτε να δημιουργήσετε ένα έργο από ένα πρότυπο με τους παρακάτω τρόπους:</span><span class="sxs-lookup"><span data-stu-id="149aa-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="149aa-121">Όταν δημιουργείτε ένα έργο από την προσφορά, μπορείτε να επιλέξετε ένα πρότυπο έργου στη φόρμα γρήγορης δημιουργίας έργου.</span><span class="sxs-lookup"><span data-stu-id="149aa-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="149aa-122">Κατά τη δημιουργία ενός έργου, κάνοντας κλικ στο κουμπί **Νέο έργο**, εμφανίζεται η φόρμα του έργου πριν να αποθηκεύσετε την εγγραφή.</span><span class="sxs-lookup"><span data-stu-id="149aa-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="149aa-123">Από εδώ, μπορείτε να κάνετε κλικ στο πεδίο **Επιλέξτε ένα πρότυπο** για να επιλέξετε κάποιο από τη λίστα των προκαθορισμένων προτύπων έργου στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="149aa-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="149aa-124">Κάντε κλικ στο κουμπί **Δημιουργία έργου από πρότυπο** στη σελίδα **Πρότυπο έργου** για να δημιουργήσετε ένα έργο από το πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="149aa-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="149aa-125">Αντιγραφή στοιχείων προτύπου σε έργο</span><span class="sxs-lookup"><span data-stu-id="149aa-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="149aa-126">Όταν αντιγράφετε στοιχεία ενός προτύπου σε ένα έργο, υπάρχουν μερικά πράγματα που πρέπει να γνωρίζετε.</span><span class="sxs-lookup"><span data-stu-id="149aa-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="149aa-127">**Αντιγραφή δομής ανάλυσης εργασίας**: Κατά την αντιγραφή της δομής ανάλυσης εργασίας από ένα πρότυπο έργου, εάν το έργο έχει ένα ημερολόγιο έργου διαφορετικό από το πρότυπο, θα εφαρμοστούν οι ώρες εργασίας από το ημερολόγιο του έργου στο χρονοδιάγραμμα εργασιών.</span><span class="sxs-lookup"><span data-stu-id="149aa-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="149aa-128">Έτσι ρυθμίζεται το χρονοδιάγραμμα για το εφεδρικό ημερολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="149aa-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="149aa-129">Ομοίως, η πρώτη εργασία στη δομή ανάλυσης εργασίας λαμβάνει την ημερομηνία έναρξης του έργου, ώστε να ενημερώνεται το υπόλοιπο του χρονοδιαγράμματος εργασιών ιεραρχίας, με βάση τη διάρκεια και τις εξαρτήσεις που καθορίζονται στη δομή ανάλυσης εργασίας του προτύπου.</span><span class="sxs-lookup"><span data-stu-id="149aa-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="149aa-130">**Αντιγραφή εκτιμήσεων έργου**: Κατά την αντιγραφή σε γραμμές εκτίμησης έργου, οι τιμοκατάλογοι ενημερώνονται με βάση τη μονάδα-κάτοχο του έργου για το κόστος τιμοκαταλόγου και τον πελάτη για τη λίστα τιμών πώλησης.</span><span class="sxs-lookup"><span data-stu-id="149aa-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="149aa-131">Το κόστος μονάδας και οι τιμές πώλησης καθορίζονται από αυτούς τους τιμοκαταλόγους σε έργα που σχετίζονται με μια οντότητα πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="149aa-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="149aa-132">**Αντιγραφή ομάδας έργου**: Κατά την αντιγραφή της ομάδας έργου από το πρότυπο σε ένα έργο, οι γενικοί πόροι αντιγράφονται, μαζί με τις ικανότητες και τις πιστοποιήσεις κατάρτισης που ορίζονται στο πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="149aa-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="149aa-133">Οι αναθέσεις γενικών πόρων διατηρούνται επίσης σύμφωνα με το πρότυπο έργου.</span><span class="sxs-lookup"><span data-stu-id="149aa-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="149aa-134">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="149aa-134">See Also</span></span>  
 [<span data-ttu-id="149aa-135">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="149aa-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]