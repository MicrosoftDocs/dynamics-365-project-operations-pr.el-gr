---
title: Δημιουργία προτύπου ωρών εργασίας
description: Πώς γίνεται η δημιουργία ενός προτύπου ωρών εργασίας στο Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: c34634817fc8e4c993261024a8b19d45052bf5e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076926"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="c8c3d-103">Δημιουργήστε ένα πρότυπο ωρών εργασίας (Project Service)</span><span class="sxs-lookup"><span data-stu-id="c8c3d-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="c8c3d-104">Για να μπορείτε να δημιουργήσετε χρονοδιαγράμματα έργων, πρέπει να ορίσετε ένα ημερολόγιο έργου το οποίο θα καθορίζει τον αριθμό των ωρών εργασίας που θα εξυπηρετούνται ανά ημέρα στο χρονοδιάγραμμα, καθώς και κάθε διακοπή εργασιών επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="c8c3d-105">Αυτό μπορείτε να το κάνετε με ένα πρότυπο ωρών εργασίας, το οποίο περιέχει λεπτομέρειες σχετικά με τις ώρες εργασίας ανά ημέρα, τα ρεπό και τυχόν άλλες διακοπές εργασιών της επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="c8c3d-106">Όταν δημιουργείτε ένα έργο, μπορείτε να συσχετίσετε ένα πρότυπο εργασίας στο ημερολόγιο έργου, για να εφαρμόσετε το χρονοδιάγραμμα για το έργο.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="c8c3d-107">Υπάρχουν δύο τρόποι για να δημιουργήσετε ένα πρότυπο ωρών εργασίας:</span><span class="sxs-lookup"><span data-stu-id="c8c3d-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="c8c3d-108">Δημιουργήστε ένα πρότυπο ωρών εργασίας με βάση το ημερολόγιο ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="c8c3d-109">Δημιουργήστε ένα νέο πρότυπο ωρών εργασίας.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="c8c3d-110">Για να δημιουργήσετε ένα πρότυπο ωρών εργασίας βάσει ενός ημερολογίου πόρων</span><span class="sxs-lookup"><span data-stu-id="c8c3d-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="c8c3d-111">Μεταβείτε στο μενού **Project Service > Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="c8c3d-112">Επιλέξτε τον πόρο στον οποίο θέλετε να βασιστούν οι ώρες εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="c8c3d-113">Πατήστε **Αποθήκευση ημερολογίου ως** , εισαγάγετε το όνομα για το πρότυπο ωρών εργασίας και, στη συνέχεια, πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-113">Click **Save Calendar As** , enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="c8c3d-114">Όταν ολοκληρώσετε τις αλλαγές των επιλογών, επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="c8c3d-115">Επιλέξτε το κουμπί **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="c8c3d-116">Για να δημιουργήσετε ένα νέο πρότυπο ωρών εργασίας</span><span class="sxs-lookup"><span data-stu-id="c8c3d-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="c8c3d-117">Μεταβείτε στο μενού **Project Service > Πρότυπα ωρών εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="c8c3d-118">Επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="c8c3d-119">Πληκτρολογήστε ένα όνομα για το πρότυπο ωρών εργασίας.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="c8c3d-120">Επιλέξτε έναν πόρο επάνω στον οποίο θα βασίσετε τις ώρες εργασίας και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="c8c3d-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="c8c3d-121">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="c8c3d-121">See Also</span></span>  
 [<span data-ttu-id="c8c3d-122">Ρύθμιση πόρων</span><span class="sxs-lookup"><span data-stu-id="c8c3d-122">Set up resources</span></span>](../psa/set-up-resources.md)
