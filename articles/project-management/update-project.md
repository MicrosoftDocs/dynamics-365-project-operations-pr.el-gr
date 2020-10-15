---
title: Ενημέρωση έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την ενημέρωση έργων Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897812"
---
# <a name="update-a-project"></a><span data-ttu-id="1f0af-103">Ενημέρωση έργου</span><span class="sxs-lookup"><span data-stu-id="1f0af-103">Update a project</span></span>

<span data-ttu-id="1f0af-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1f0af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1f0af-105">Παρακάτω εμφανίζεται μια σύνοψη των πεδίων που μπορούν να ενημερωθούν σε ένα έργο μετά τη δημιουργία του και τυχόν συνέπειες των ενημερώσεων.</span><span class="sxs-lookup"><span data-stu-id="1f0af-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="1f0af-106">Πεδία λεπτομερειών έργου</span><span class="sxs-lookup"><span data-stu-id="1f0af-106">Project detail fields</span></span>

- <span data-ttu-id="1f0af-107">**Όνομα**: Ο τίτλος του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="1f0af-108">**Περιγραφή**: Μια επισκόπηση του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="1f0af-109">**Πελάτης**: η εταιρεία στην οποία θα γίνει η παράδοση του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="1f0af-110">**Πρότυπο ημερολογίου**: οι ώρες εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="1f0af-111">Όταν γίνει αλλαγή του πεδίου, γίνεται εκ νέου υπολογισμός ολόκληρου του χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="1f0af-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="1f0af-112">**Νομισματική μονάδα**: Η νομισματική μονάδα για το έργο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="1f0af-113">Αυτό το πεδίο προκαθορίζεται από τις προεπιλογές με βάση τη νομισματική μονάδα που ορίζεται στη συμβαλλόμενη μονάδα.</span><span class="sxs-lookup"><span data-stu-id="1f0af-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="1f0af-114">Όταν ενημερωθεί η συμβαλλόμενη μονάδα, ενημερώνεται και το πεδίο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="1f0af-115">**Συμβαλλόμενη μονάδα**: Η οργανωτική μονάδα που εκπροσωπεί την ομάδα ή τη διαίρεση της εταιρείας η οποία είναι κατά κύριο λόγο υπεύθυνη για την επιτυχία της πώλησης και τη διαχείριση της παροχής της εργασίας και των υπηρεσιών στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="1f0af-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="1f0af-116">**Υπεύθυνος έργου**: το μέλος της ομάδας έργου που έχει την εξουσιοδότηση για την εξέταση και την έγκριση καταχωρήσεων και εξόδων χρόνου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="1f0af-117">Πεδία εκτίμησης</span><span class="sxs-lookup"><span data-stu-id="1f0af-117">Estimate fields</span></span>

- <span data-ttu-id="1f0af-118">**Εκτιμώμενη ημερομηνία έναρξης**: η ημερομηνία κατά την οποία θα ξεκινήσει το έργο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="1f0af-119">Όταν ενημερωθεί αυτό το πεδίο, οποιεσδήποτε εργασίες του έργου θα μετακινούνται αναλογικά με τη νέα ημερομηνία έναρξης.</span><span class="sxs-lookup"><span data-stu-id="1f0af-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="1f0af-120">**Ημερομηνία λήξης**: η ημερομηνία κατά την οποία έχει προγραμματιστεί η λήξη του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="1f0af-121">**Προσπάθεια**: η εκτιμώμενη προσπάθεια του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="1f0af-122">Όταν οι εργασίες προστίθενται στο έργο, αυτό το πεδίο δεν είναι πλέον επεξεργάσιμο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="1f0af-123">**Εκτιμώμενο κόστος εργασίας**: το εκτιμώμενο κόστος εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="1f0af-124">Όταν το κόστος εργασίας προστίθεται στο έργο, αυτό το πεδίο δεν είναι πλέον επεξεργάσιμο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="1f0af-125">**Εκτιμώμενα έξοδα**: τα εκτιμώμενα έξοδα του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="1f0af-126">Όταν δαπάνες προστίθενται στο έργο, αυτό το πεδίο δεν είναι πλέον επεξεργάσιμο.</span><span class="sxs-lookup"><span data-stu-id="1f0af-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="1f0af-127">Πραγματικά πεδία έργου</span><span class="sxs-lookup"><span data-stu-id="1f0af-127">Project actual fields</span></span>
- <span data-ttu-id="1f0af-128">**Πραγματική έναρξη**: η ημερομηνία έναρξης του έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="1f0af-129">**Πραγματικό τέλος**: Προς ενημέρωση κατά την ολοκλήρωση ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="1f0af-130">Πεδία κατάστασης έργου</span><span class="sxs-lookup"><span data-stu-id="1f0af-130">Project status fields</span></span>

- <span data-ttu-id="1f0af-131">**Συνολική κατάσταση έργου**: η συνολική εύρυθμη λειτουργία του έργου που παρέχεται από το διαχειριστή έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="1f0af-132">**Σχόλια**: μια περιγραφή σχετικά με την τρέχουσα κατάσταση του έργου που παρέχεται από τον υπεύθυνο έργου.</span><span class="sxs-lookup"><span data-stu-id="1f0af-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>

