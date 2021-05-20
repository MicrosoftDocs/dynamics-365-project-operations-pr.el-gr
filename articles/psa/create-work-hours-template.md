---
title: Δημιουργία προτύπου ωρών εργασίας
description: Αυτό το θέμα περιγράφει πώς γίνεται η δημιουργία ενός προτύπου ωρών εργασίας στο Project Service.
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
ms.openlocfilehash: 525f601ad6fee902cb6d5c128b596cc2d33f30c4
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981255"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="a4595-103">Δημιουργήστε ένα πρότυπο ωρών εργασίας (Project Service)</span><span class="sxs-lookup"><span data-stu-id="a4595-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a4595-104">Για να δημιουργήσετε και να διαχειριστείτε ένα έργο, πρέπει να εφαρμόσετε ένα πρότυπο ημερολογίου στο έργο.</span><span class="sxs-lookup"><span data-stu-id="a4595-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="a4595-105">Το πρότυπο ημερολογίου καθορίζει τα ακόλουθα χαρακτηριστικά του έργου:</span><span class="sxs-lookup"><span data-stu-id="a4595-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="a4595-106">Ώρες εργασίας, συμπεριλαμβανομένων των ωρών έναρξης και λήξης</span><span class="sxs-lookup"><span data-stu-id="a4595-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="a4595-107">Εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="a4595-107">Working days</span></span>
- <span data-ttu-id="a4595-108">Εξαιρέσεις ημερολογίου, όπως για παράδειγμα, μη εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="a4595-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="a4595-109">Το πρότυπο ημερολογίου που εφαρμόζεται σε ένα έργο είναι ένα αντίγραφο του προτύπου ημερολογίου που ορίζεται στις ρυθμίσεις του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="a4595-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="a4595-110">Εάν αλλάξετε το πρότυπο ημερολογίου, αυτές οι αλλαγές δεν αναπαράγονται στις ώρες εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="a4595-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="a4595-111">Για να αλλάξετε τις ώρες εργασίας του έργου, πρέπει να εφαρμοστεί ένα νέο πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="a4595-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="a4595-112">Για να δημιουργήσετε ένα πρότυπο ημερολογίου για τον οργανισμό σας, υπάρχουν δύο βασικές απαιτήσεις:</span><span class="sxs-lookup"><span data-stu-id="a4595-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="a4595-113">Να καθορίσετε τις επιθυμητές ώρες εργασίας του προτύπου χρησιμοποιώντας έναν νέο ή υπάρχοντα πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="a4595-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="a4595-114">Να δημιουργήσετε ένα νέο πρότυπο ημερολογίου και συσχετίστε το πρότυπο με τον πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="a4595-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="a4595-115">**Ορισμός ωρών εργασίας του προτύπου**</span><span class="sxs-lookup"><span data-stu-id="a4595-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="a4595-116">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="a4595-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="a4595-117">Δημιουργήστε έναν νέο πόρο για αναφορά στο πρότυπο ημερολογίου ή επιλέξτε έναν υπάρχοντα πόρο.</span><span class="sxs-lookup"><span data-stu-id="a4595-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="a4595-118">Επιλέξτε την καρτέλα **Ώρες εργασίας** του πόρου και ολοκληρώστε τις οδηγίες στο στοιχείο [Ορισμός ωρών εργασίας για έναν πόρο](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) για τη ρύθμιση των κανόνων ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a4595-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="a4595-119">**Δημιουργήστε ένα νέο πρότυπο ημερολογίου**</span><span class="sxs-lookup"><span data-stu-id="a4595-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="a4595-120">Μεταβείτε στο **Ρυθμίσεις** \> **Πρότυπο ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="a4595-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="a4595-121">Επιλέξτε **Δημιουργία** και καταχωρήστε ένα όνομα, μια περιγραφή και έναν πόρο προτύπου.</span><span class="sxs-lookup"><span data-stu-id="a4595-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="a4595-122">Όταν γίνεται αναφορά ενός πόρου σε ένα πρότυπο ημερολογίου, ένα αντίγραφο του ημερολογίου του πόρου συσχετίζεται με το πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a4595-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="a4595-123">Εάν αλλάξετε τις ώρες εργασίας της αλλαγής του αντιγραμμένου προτύπου, αυτές οι αλλαγές δεν αναπαράγονται στο πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a4595-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="a4595-124">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="a4595-124">See Also</span></span>  
 [<span data-ttu-id="a4595-125">Ρύθμιση πόρων</span><span class="sxs-lookup"><span data-stu-id="a4595-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
