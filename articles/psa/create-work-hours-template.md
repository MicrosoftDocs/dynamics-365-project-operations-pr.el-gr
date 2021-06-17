---
title: Δημιουργία προτύπου ωρών εργασίας
description: Αυτό το θέμα περιγράφει πώς γίνεται η δημιουργία ενός προτύπου ωρών εργασίας στο Project Service.
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
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997196"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="18084-103">Δημιουργήστε ένα πρότυπο ωρών εργασίας (Project Service)</span><span class="sxs-lookup"><span data-stu-id="18084-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="18084-104">Για να δημιουργήσετε και να διαχειριστείτε ένα έργο, πρέπει να εφαρμόσετε ένα πρότυπο ημερολογίου στο έργο.</span><span class="sxs-lookup"><span data-stu-id="18084-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="18084-105">Το πρότυπο ημερολογίου καθορίζει τα ακόλουθα χαρακτηριστικά του έργου:</span><span class="sxs-lookup"><span data-stu-id="18084-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="18084-106">Ώρες εργασίας, συμπεριλαμβανομένων των ωρών έναρξης και λήξης</span><span class="sxs-lookup"><span data-stu-id="18084-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="18084-107">Εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="18084-107">Working days</span></span>
- <span data-ttu-id="18084-108">Εξαιρέσεις ημερολογίου, όπως για παράδειγμα, μη εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="18084-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="18084-109">Το πρότυπο ημερολογίου που εφαρμόζεται σε ένα έργο είναι ένα αντίγραφο του προτύπου ημερολογίου που ορίζεται στις ρυθμίσεις του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="18084-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="18084-110">Εάν αλλάξετε το πρότυπο ημερολογίου, αυτές οι αλλαγές δεν αναπαράγονται στις ώρες εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="18084-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="18084-111">Για να αλλάξετε τις ώρες εργασίας του έργου, πρέπει να εφαρμοστεί ένα νέο πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="18084-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="18084-112">Για να δημιουργήσετε ένα πρότυπο ημερολογίου για τον οργανισμό σας, υπάρχουν δύο βασικές απαιτήσεις:</span><span class="sxs-lookup"><span data-stu-id="18084-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="18084-113">Να καθορίσετε τις επιθυμητές ώρες εργασίας του προτύπου χρησιμοποιώντας έναν νέο ή υπάρχοντα πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="18084-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="18084-114">Να δημιουργήσετε ένα νέο πρότυπο ημερολογίου και συσχετίστε το πρότυπο με τον πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="18084-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="18084-115">**Ορισμός ωρών εργασίας του προτύπου**</span><span class="sxs-lookup"><span data-stu-id="18084-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="18084-116">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="18084-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="18084-117">Δημιουργήστε έναν νέο πόρο για αναφορά στο πρότυπο ημερολογίου ή επιλέξτε έναν υπάρχοντα πόρο.</span><span class="sxs-lookup"><span data-stu-id="18084-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="18084-118">Επιλέξτε την καρτέλα **Ώρες εργασίας** του πόρου και ολοκληρώστε τις οδηγίες στο στοιχείο [Ορισμός ωρών εργασίας για έναν πόρο](/dynamics365/field-service/set-work-hours-resource.md) για τη ρύθμιση των κανόνων ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="18084-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="18084-119">**Δημιουργήστε ένα νέο πρότυπο ημερολογίου**</span><span class="sxs-lookup"><span data-stu-id="18084-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="18084-120">Μεταβείτε στο **Ρυθμίσεις** \> **Πρότυπο ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="18084-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="18084-121">Επιλέξτε **Δημιουργία** και καταχωρήστε ένα όνομα, μια περιγραφή και έναν πόρο προτύπου.</span><span class="sxs-lookup"><span data-stu-id="18084-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="18084-122">Όταν γίνεται αναφορά ενός πόρου σε ένα πρότυπο ημερολογίου, ένα αντίγραφο του ημερολογίου του πόρου συσχετίζεται με το πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="18084-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="18084-123">Εάν αλλάξετε τις ώρες εργασίας της αλλαγής του αντιγραμμένου προτύπου, αυτές οι αλλαγές δεν αναπαράγονται στο πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="18084-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="18084-124">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="18084-124">See Also</span></span>  
 [<span data-ttu-id="18084-125">Ρύθμιση πόρων</span><span class="sxs-lookup"><span data-stu-id="18084-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
