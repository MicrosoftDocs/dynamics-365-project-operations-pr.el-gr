---
title: Τύποι σταδίου έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα στάδια έργου.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: ed725d8ea2f671c45a7a19bb017bbb08c41f42db
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008986"
---
# <a name="project-stage-types"></a><span data-ttu-id="91eae-103">Τύποι σταδίου έργου</span><span class="sxs-lookup"><span data-stu-id="91eae-103">Project stage types</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="91eae-104">Τα στάδια έργου σχεδιάζονται ώστε να αντικατοπτρίζουν την κατάσταση του έργου καθώς εξελίσσεται.</span><span class="sxs-lookup"><span data-stu-id="91eae-104">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="91eae-105">Οι προσαρμογές μπορούν να χρησιμοποιηθούν για την αυτόματη ενημέρωση των σταδίων με τις ροές επιχειρηματικών διαδικασίας, Power Automate ή με επεκτάσεις προσθήκης.</span><span class="sxs-lookup"><span data-stu-id="91eae-105">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="91eae-106">Τα ακόλουθα στάδια καθορίζονται στο προεπιλεγμένο BPF:</span><span class="sxs-lookup"><span data-stu-id="91eae-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="91eae-107">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="91eae-107">New</span></span>
- <span data-ttu-id="91eae-108">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="91eae-108">Quote</span></span>
- <span data-ttu-id="91eae-109">Πρόγραμμα</span><span class="sxs-lookup"><span data-stu-id="91eae-109">Plan</span></span>
- <span data-ttu-id="91eae-110">Παράδοση</span><span class="sxs-lookup"><span data-stu-id="91eae-110">Deliver</span></span>
- <span data-ttu-id="91eae-111">Ολοκληρώθηκε</span><span class="sxs-lookup"><span data-stu-id="91eae-111">Complete</span></span>
- <span data-ttu-id="91eae-112">Κλείσιμο</span><span class="sxs-lookup"><span data-stu-id="91eae-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="91eae-113">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="91eae-113">New</span></span>

<span data-ttu-id="91eae-114">Όταν δημιουργείτε ένα έργο, το στάδιο έργου έχει οριστεί στην επιλογή **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="91eae-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="91eae-115">Εάν το έργο δημιουργήθηκε από ένα πρότυπο, μπορεί να έχει δεδομένα χρονοδιαγράμματος, εκτίμησης και ομάδας.</span><span class="sxs-lookup"><span data-stu-id="91eae-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="91eae-116">Διαφορετικά, πρόκειται απλώς για ένα περίγραμμα του έργου και πρέπει να καταχωρηθούν τα υπόλοιπα στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="91eae-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="91eae-117">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="91eae-117">Quote</span></span>

<span data-ttu-id="91eae-118">Όταν συσχετίζετε ένα έργο σε μια προσφορά ή το δημιουργείτε από μια προσφορά, το στάδιο του έργου έχει οριστεί στην επιλογή **Προσφορά** και ενημερώνονται επίσης οι εκτιμώμενες ημερομηνίες έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="91eae-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="91eae-119">Ενώ το έργο βρίσκεται στο στάδιο της **Προσφοράς**, η καρτέλα **Πωλήσεις** στη σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="91eae-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="91eae-120">Πρόγραμμα</span><span class="sxs-lookup"><span data-stu-id="91eae-120">Plan</span></span>

<span data-ttu-id="91eae-121">Όταν κερδίζετε μια προσφορά που έχει συσχετιστεί με ένα έργο και το έργο μετακινείται στη φάση **Σύμβαση**, το στάδιο έργου ενημερώνεται σε **Πρόγραμμα**.</span><span class="sxs-lookup"><span data-stu-id="91eae-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="91eae-122">Ενώ το έργο βρίσκεται στο στάδιο **Πρόγραμμα**, η σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="91eae-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="91eae-123">Παράδοση</span><span class="sxs-lookup"><span data-stu-id="91eae-123">Deliver</span></span>

<span data-ttu-id="91eae-124">Όταν ολοκληρωθεί το σχέδιο έργου και είστε έτοιμοι να ξεκινήσετε το έργο, ο υπεύθυνος έργου θα πρέπει να ενημερώσει το στάδιο του έργου σε **Παράδοση** για να δείξει ότι το έργο έχει ξεκινήσει.</span><span class="sxs-lookup"><span data-stu-id="91eae-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="91eae-125">Ολοκληρώθηκε</span><span class="sxs-lookup"><span data-stu-id="91eae-125">Complete</span></span> 

<span data-ttu-id="91eae-126">Όταν ολοκληρωθεί η εργασία για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Ολοκληρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="91eae-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="91eae-127">Με την ενημέρωση του σταδίου του έργου σε **Ολοκληρώθηκε**, ο υπεύθυνος έργου δηλώνει ότι η εργασία έχει ολοκληρωθεί 100 τοις εκατό, αλλά ότι το έργο διατηρείται ανοιχτό έτσι ώστε να είναι δυνατή η καταγραφή τυχόν εκκρεμών καταχωρήσεων χρόνου ή εξόδων.</span><span class="sxs-lookup"><span data-stu-id="91eae-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="91eae-128">Κλείσιμο</span><span class="sxs-lookup"><span data-stu-id="91eae-128">Close</span></span>

<span data-ttu-id="91eae-129">Όταν καταγραφούν όλες οι συναλλαγές για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="91eae-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="91eae-130">Σε αυτό το σημείο, καμία συναλλαγή δεν μπορεί να καταγραφεί και το έργο έχει οριστεί ως "μόνο για ανάγνωση".</span><span class="sxs-lookup"><span data-stu-id="91eae-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]