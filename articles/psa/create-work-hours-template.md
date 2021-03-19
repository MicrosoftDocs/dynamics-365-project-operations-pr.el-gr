---
title: Δημιουργία προτύπου ωρών εργασίας
description: Πώς γίνεται η δημιουργία ενός προτύπου ωρών εργασίας στο Project Service
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
ms.openlocfilehash: 5e859a58f86d8cd98fa429beeeb99cf397a207cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285033"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="212e0-103">Δημιουργήστε ένα πρότυπο ωρών εργασίας (Project Service)</span><span class="sxs-lookup"><span data-stu-id="212e0-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="212e0-104">Για να μπορείτε να δημιουργήσετε χρονοδιαγράμματα έργων, πρέπει να ορίσετε ένα ημερολόγιο έργου το οποίο θα καθορίζει τον αριθμό των ωρών εργασίας που θα εξυπηρετούνται ανά ημέρα στο χρονοδιάγραμμα, καθώς και κάθε διακοπή εργασιών επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="212e0-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="212e0-105">Αυτό μπορείτε να το κάνετε με ένα πρότυπο ωρών εργασίας, το οποίο περιέχει λεπτομέρειες σχετικά με τις ώρες εργασίας ανά ημέρα, τα ρεπό και τυχόν άλλες διακοπές εργασιών της επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="212e0-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="212e0-106">Όταν δημιουργείτε ένα έργο, μπορείτε να συσχετίσετε ένα πρότυπο εργασίας στο ημερολόγιο έργου, για να εφαρμόσετε το χρονοδιάγραμμα για το έργο.</span><span class="sxs-lookup"><span data-stu-id="212e0-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="212e0-107">Υπάρχουν δύο τρόποι για να δημιουργήσετε ένα πρότυπο ωρών εργασίας:</span><span class="sxs-lookup"><span data-stu-id="212e0-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="212e0-108">Δημιουργήστε ένα πρότυπο ωρών εργασίας με βάση το ημερολόγιο ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="212e0-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="212e0-109">Δημιουργήστε ένα νέο πρότυπο ωρών εργασίας.</span><span class="sxs-lookup"><span data-stu-id="212e0-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="212e0-110">Για να δημιουργήσετε ένα πρότυπο ωρών εργασίας βάσει ενός ημερολογίου πόρων</span><span class="sxs-lookup"><span data-stu-id="212e0-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="212e0-111">Μεταβείτε στο μενού **Project Service > Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="212e0-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="212e0-112">Επιλέξτε τον πόρο στον οποίο θέλετε να βασιστούν οι ώρες εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="212e0-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="212e0-113">Πατήστε **Αποθήκευση ημερολογίου ως**, εισαγάγετε το όνομα για το πρότυπο ωρών εργασίας και, στη συνέχεια, πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="212e0-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="212e0-114">Όταν ολοκληρώσετε τις αλλαγές των επιλογών, επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="212e0-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="212e0-115">Επιλέξτε το κουμπί **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="212e0-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="212e0-116">Για να δημιουργήσετε ένα νέο πρότυπο ωρών εργασίας</span><span class="sxs-lookup"><span data-stu-id="212e0-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="212e0-117">Μεταβείτε στο μενού **Project Service > Πρότυπα ωρών εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="212e0-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="212e0-118">Επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="212e0-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="212e0-119">Πληκτρολογήστε ένα όνομα για το πρότυπο ωρών εργασίας.</span><span class="sxs-lookup"><span data-stu-id="212e0-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="212e0-120">Επιλέξτε έναν πόρο επάνω στον οποίο θα βασίσετε τις ώρες εργασίας και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="212e0-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="212e0-121">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="212e0-121">See Also</span></span>  
 [<span data-ttu-id="212e0-122">Ρύθμιση πόρων</span><span class="sxs-lookup"><span data-stu-id="212e0-122">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]