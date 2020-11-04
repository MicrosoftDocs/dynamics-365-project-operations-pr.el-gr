---
title: Στάδια έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα στάδια του έργου που είναι διαθέσιμα στο Microsoft Dynamics Project Operations (Λειτουργίες έργου).
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 554ad63bc44cbe5a1fe91eb47fedbb74bbedd4b6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077043"
---
# <a name="project-stages"></a><span data-ttu-id="c2f5c-103">Στάδια έργου</span><span class="sxs-lookup"><span data-stu-id="c2f5c-103">Project stages</span></span>

<span data-ttu-id="c2f5c-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="c2f5c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c2f5c-105">Τα στάδια έργου σχεδιάζονται ώστε να αντικατοπτρίζουν την κατάσταση του έργου καθώς εξελίσσεται.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="c2f5c-106">Οι προσαρμογές μπορούν να χρησιμοποιηθούν για την αυτόματη ενημέρωση των σταδίων με τις ροές επιχειρηματικών διαδικασίας, Power Automate ή με επεκτάσεις προσθήκης.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="c2f5c-107">Τα ακόλουθα στάδια καθορίζονται στην προεπιλεγμένη ροή επιχειρηματικής διαδικασίας:</span><span class="sxs-lookup"><span data-stu-id="c2f5c-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="c2f5c-108">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="c2f5c-108">New</span></span>
- <span data-ttu-id="c2f5c-109">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="c2f5c-109">Quote</span></span>
- <span data-ttu-id="c2f5c-110">Πρόγραμμα</span><span class="sxs-lookup"><span data-stu-id="c2f5c-110">Plan</span></span>
- <span data-ttu-id="c2f5c-111">Παράδοση</span><span class="sxs-lookup"><span data-stu-id="c2f5c-111">Deliver</span></span>
- <span data-ttu-id="c2f5c-112">Ολοκλήρωση</span><span class="sxs-lookup"><span data-stu-id="c2f5c-112">Complete</span></span>
- <span data-ttu-id="c2f5c-113">Κλείσιμο </span><span class="sxs-lookup"><span data-stu-id="c2f5c-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="c2f5c-114">Δημιουργία</span><span class="sxs-lookup"><span data-stu-id="c2f5c-114">New</span></span>

<span data-ttu-id="c2f5c-115">Όταν δημιουργείτε ένα έργο, το στάδιο έργου έχει οριστεί στην επιλογή **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="c2f5c-116">Εάν το έργο δημιουργήθηκε από ένα πρότυπο, μπορεί να έχει δεδομένα χρονοδιαγράμματος, εκτίμησης και ομάδας.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="c2f5c-117">Διαφορετικά, πρόκειται για ένα περίγραμμα του έργου και πρέπει να καταχωρηθούν τα υπόλοιπα στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="c2f5c-118">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="c2f5c-118">Quote</span></span>

<span data-ttu-id="c2f5c-119">Όταν συσχετίζετε ένα έργο σε μια προσφορά ή το δημιουργείτε από μια προσφορά, το στάδιο του έργου έχει οριστεί στην επιλογή **Προσφορά** και ενημερώνονται επίσης οι εκτιμώμενες ημερομηνίες έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote** , and the estimated start and end dates are updated.</span></span> <span data-ttu-id="c2f5c-120">Ενώ το έργο βρίσκεται στο στάδιο της **Προσφοράς** , η καρτέλα **Πωλήσεις** στη σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="c2f5c-121">Πρόγραμμα</span><span class="sxs-lookup"><span data-stu-id="c2f5c-121">Plan</span></span>

<span data-ttu-id="c2f5c-122">Όταν κερδίζετε μια προσφορά που έχει συσχετιστεί με ένα έργο και το έργο μετακινείται στη φάση **Σύμβαση** , το στάδιο έργου ενημερώνεται σε **Πρόγραμμα**.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="c2f5c-123">Ενώ το έργο βρίσκεται στο στάδιο **Πρόγραμμα** , η σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="c2f5c-124">Παράδοση</span><span class="sxs-lookup"><span data-stu-id="c2f5c-124">Deliver</span></span>

<span data-ttu-id="c2f5c-125">Όταν ολοκληρωθεί το σχέδιο έργου και είστε έτοιμοι να ξεκινήσετε το έργο, ο υπεύθυνος έργου θα πρέπει να ενημερώσει το στάδιο του έργου σε **Παράδοση** για να δείξει ότι το έργο έχει ξεκινήσει.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="c2f5c-126">Ολοκληρώθηκε</span><span class="sxs-lookup"><span data-stu-id="c2f5c-126">Complete</span></span> 

<span data-ttu-id="c2f5c-127">Όταν ολοκληρωθεί η εργασία για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Ολοκληρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="c2f5c-128">Με την ενημέρωση του σταδίου του έργου σε **Ολοκληρώθηκε** , ο υπεύθυνος έργου δηλώνει ότι η εργασία έχει ολοκληρωθεί 100 τοις εκατό, αλλά ότι το έργο διατηρείται ανοιχτό έτσι ώστε να είναι δυνατή η καταγραφή τυχόν εκκρεμών καταχωρήσεων χρόνου ή εξόδων.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-128">By updating the project stage to **Complete** , the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="c2f5c-129">Κλείσιμο</span><span class="sxs-lookup"><span data-stu-id="c2f5c-129">Close</span></span>

<span data-ttu-id="c2f5c-130">Όταν καταγραφούν όλες οι συναλλαγές για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="c2f5c-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="c2f5c-131">Σε αυτό το σημείο, καμία συναλλαγή δεν μπορεί να καταγραφεί και το έργο έχει οριστεί ως "μόνο για ανάγνωση".</span><span class="sxs-lookup"><span data-stu-id="c2f5c-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

