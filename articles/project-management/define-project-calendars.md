---
title: Καθορισμός ημερολογίων έργου
description: Αυτό θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εφαρμογής ενός προτύπου ημερολογίου σε ένα έργο, για την παρακολούθηση του χρονοδιαγράμματος του έργου.
author: ruhercul
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0d1a2c4bd2d4022bbf79afcef79170eb482e6418
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998996"
---
# <a name="define-project-calendars"></a><span data-ttu-id="a0ba5-103">Καθορισμός ημερολογίων έργου</span><span class="sxs-lookup"><span data-stu-id="a0ba5-103">Define project calendars</span></span>

<span data-ttu-id="a0ba5-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="a0ba5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a0ba5-105">Για να δημιουργήσετε και να διαχειριστείτε ένα έργο, πρέπει να εφαρμόσετε ένα πρότυπο ημερολογίου στο έργο.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="a0ba5-106">Το πρότυπο ημερολογίου καθορίζει τα ακόλουθα χαρακτηριστικά του έργου:</span><span class="sxs-lookup"><span data-stu-id="a0ba5-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="a0ba5-107">Ώρες εργασίας, συμπεριλαμβανομένων των ωρών έναρξης και λήξης</span><span class="sxs-lookup"><span data-stu-id="a0ba5-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="a0ba5-108">Εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="a0ba5-108">Working days</span></span>
- <span data-ttu-id="a0ba5-109">Εξαιρέσεις ημερολογίου, όπως για παράδειγμα, μη εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="a0ba5-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="a0ba5-110">Το πρότυπο ημερολογίου που εφαρμόζεται σε ένα έργο είναι ένα αντίγραφο του προτύπου ημερολογίου που ορίζεται στις ρυθμίσεις του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="a0ba5-111">Εάν αλλάξετε το πρότυπο ημερολογίου, αυτές οι αλλαγές δεν αναπαράγονται στις ώρες εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="a0ba5-112">Για να αλλάξετε τις ώρες εργασίας του έργου, πρέπει να εφαρμοστεί ένα νέο πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="a0ba5-113">Για να δημιουργήσετε ένα πρότυπο ημερολογίου για τον οργανισμό σας, υπάρχουν δύο βασικές απαιτήσεις:</span><span class="sxs-lookup"><span data-stu-id="a0ba5-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="a0ba5-114">Να καθορίσετε τις επιθυμητές ώρες εργασίας του προτύπου χρησιμοποιώντας έναν νέο ή υπάρχοντα πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="a0ba5-115">Να δημιουργήσετε ένα νέο πρότυπο ημερολογίου και συσχετίστε το πρότυπο με τον πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="a0ba5-116">**Ορισμός ωρών εργασίας του προτύπου**</span><span class="sxs-lookup"><span data-stu-id="a0ba5-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="a0ba5-117">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="a0ba5-118">Δημιουργήστε έναν νέο πόρο για αναφορά στο πρότυπο ημερολογίου ή επιλέξτε έναν υπάρχοντα πόρο.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="a0ba5-119">Επιλέξτε την καρτέλα **Ώρες εργασίας** του πόρου και ολοκληρώστε τις οδηγίες στο στοιχείο [Ορισμός ωρών εργασίας για έναν πόρο](/dynamics365/field-service/set-work-hours-resource.md) για τη ρύθμιση των κανόνων ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="a0ba5-120">**Δημιουργήστε ένα νέο πρότυπο ημερολογίου**</span><span class="sxs-lookup"><span data-stu-id="a0ba5-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="a0ba5-121">Μεταβείτε στο **Ρυθμίσεις** \> **Πρότυπο ημερολογίου**.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="a0ba5-122">Επιλέξτε **Δημιουργία** και καταχωρήστε ένα όνομα, μια περιγραφή και έναν πόρο προτύπου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="a0ba5-123">Όταν γίνεται αναφορά ενός πόρου σε ένα πρότυπο ημερολογίου, ένα αντίγραφο του ημερολογίου του πόρου συσχετίζεται με το πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="a0ba5-124">Εάν αλλάξετε τις ώρες εργασίας της αλλαγής του αντιγραμμένου προτύπου, αυτές οι αλλαγές δεν αναπαράγονται στο πρότυπο ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="a0ba5-125">Τώρα, μπορείτε να συσχετίσετε το πρότυπο εργασίας με ένα πρότυπο ημερολογίου έργου.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

