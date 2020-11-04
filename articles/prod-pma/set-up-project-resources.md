---
title: Ρύθμιση πόρων έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη ρύθμιση ή τη ζήτηση πόρων έργου.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7eec8ad5d78019219b2e04ca75eeaa5a3c8a748f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077088"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="ac2db-103">Ρύθμιση πόρων έργου</span><span class="sxs-lookup"><span data-stu-id="ac2db-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="ac2db-104">Πρέπει να ρυθμίσετε τις παραμέτρους ενός ημερολογίου και να το συσχετίσετε με έναν υπάλληλο ή έναν εργαζόμενο.</span><span class="sxs-lookup"><span data-stu-id="ac2db-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="ac2db-105">Το ημερολόγιο χρησιμοποιείται για τον προγραμματισμό του έργου και του χρόνου εργασίας των πόρων που προορίζονται για το έργο.</span><span class="sxs-lookup"><span data-stu-id="ac2db-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="ac2db-106">Κατά τη διάρκεια της εγκατάστασης του ημερολογίου, οι υπεύθυνοι μπορούν να ορίσουν επίπεδα πόρων ως μέρος της βελτιστοποίησης πόρων.</span><span class="sxs-lookup"><span data-stu-id="ac2db-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="ac2db-107">Με βάση το χρονοδιάγραμμα του ημερολογίου, είναι δυνατή η τοποθέτηση περιορισμών σε πόρους.</span><span class="sxs-lookup"><span data-stu-id="ac2db-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="ac2db-108">Μπορείτε να δημιουργήσετε ένα ημερολόγιο στη σελίδα **Ημερολόγια**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="ac2db-109">Όταν ρυθμίζετε έναν εργαζόμενο ως πόρο έργου, μπορείτε να επιλέξετε από εργαζομένους που εργάζονται στην εταιρεία για την οποία δημιουργείτε πόρους.</span><span class="sxs-lookup"><span data-stu-id="ac2db-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="ac2db-110">Εναλλακτικά, μπορείτε να επιλέξετε εργαζομένους από άλλες εταιρείες στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="ac2db-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="ac2db-111">Οι εν λόγω εργαζόμενοι είναι γνωστοί ως διεταιρικοί πόροι.</span><span class="sxs-lookup"><span data-stu-id="ac2db-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="ac2db-112">Οι παρακάτω διαδικασίες εξηγούν τον τρόπο με τον οποίο μπορείτε να ρυθμίσετε έναν εργαζόμενο ως πόρο έργου στην εταιρεία σας και πώς να ρυθμίσετε έναν διεταιρικό πόρο έργου.</span><span class="sxs-lookup"><span data-stu-id="ac2db-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="ac2db-113">Ρύθμιση ενός εργαζομένου ως πόρο έργου</span><span class="sxs-lookup"><span data-stu-id="ac2db-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="ac2db-114">Στη σελίδα **Εργαζόμενοι** στη λίστα **Εργαζόμενοι** , επιλέξτε τον εργαζόμενο που προσθέτετε ως πόρο έργου και ανοίξτε την καρτέλα του εργαζομένου.</span><span class="sxs-lookup"><span data-stu-id="ac2db-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="ac2db-115">Στο τμήμα παραθύρου ενεργειών, επιλέξτε **Έργο** &gt; **Ρύθμιση** &gt; **Ρύθμιση παραμέτρων έργου**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="ac2db-116">Επιλέξτε ένα ημερολόγιο και, στη συνέχεια, κλείστε τη σελίδα.</span><span class="sxs-lookup"><span data-stu-id="ac2db-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="ac2db-117">Μπορείτε επίσης να καθορίσετε προεπιλεγμένα έργα για έναν πόρο ως τύπο προ-ανάθεσης.</span><span class="sxs-lookup"><span data-stu-id="ac2db-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="ac2db-118">Οι προ-αναθέσεις μπορούν να χρησιμοποιηθούν όταν ο διαχειριστής πόρων ή ο υπεύθυνος έργου γνωρίζει σε ποια έργα θα εργάζεται ο πόρος εκ των προτέρων.</span><span class="sxs-lookup"><span data-stu-id="ac2db-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="ac2db-119">Οι προ-αναθέσεις μπορούν επίσης να βασιστούν στις αιτήσεις ενός χορηγού έργου ή ενός πελάτη.</span><span class="sxs-lookup"><span data-stu-id="ac2db-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="ac2db-120">Για να προχωρήσετε σε ένα έργο, στη σελίδα **Ανάθεση έργων** , στην καρτέλα **Έργα** , στη λίστα **Υπόλοιπα έργα** , επιλέξτε το κατάλληλο έργο.</span><span class="sxs-lookup"><span data-stu-id="ac2db-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="ac2db-121">Ρύθμιση ενός διεταιρικού πόρου</span><span class="sxs-lookup"><span data-stu-id="ac2db-121">Set up an intercompany resource</span></span>

<span data-ttu-id="ac2db-122">Όταν ρυθμίζετε έναν εργαζόμενο ως διεταιρικό πόρο, πρέπει να ολοκληρώσετε τη ρύθμιση των παραμέτρων τόσο στην εταιρεία δανεισμού όσο και στη δανειζόμενη εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="ac2db-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="ac2db-123">Στην εταιρεία δανεισμού</span><span class="sxs-lookup"><span data-stu-id="ac2db-123">In the lending company</span></span>

1. <span data-ttu-id="ac2db-124">Στο Finance, επαληθεύστε ότι η εταιρεία δανεισμού έχει επιλεγεί και, στη συνέχεια, ολοκληρώστε τη διαδικασία στην προηγούμενη ενότητα, "Ρύθμιση ενός εργαζομένου ως πόρος έργου."</span><span class="sxs-lookup"><span data-stu-id="ac2db-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="ac2db-125">Στη σελίδα **Διετιαρική λογιστική** , επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="ac2db-126">Στο πεδίο **Αναγνωριστικό νομικής οντότητας** , επιλέξτε την εταιρεία δανεισμού.</span><span class="sxs-lookup"><span data-stu-id="ac2db-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="ac2db-127">Συμπληρώστε τα υπόλοιπα πεδία και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="ac2db-128">Στη σελίδα **Τιμή μεταφοράς** , επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="ac2db-129">Στο πεδίο **Δανειζόμενη νομική οντότητα** , επιλέξτε την κατάλληλη εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="ac2db-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="ac2db-130">Για να δανείσετε στη δανειζόμενη εταιρεία μόνο τον πόρο που δημιουργήσατε στην αρχή αυτής της ενότητας, στο πεδίο **Πόρος** , επιλέξτε το όνομα του πόρου που δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="ac2db-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="ac2db-131">Για να καταστήσετε διαθέσιμους όλους τους πόρους της εταιρείας δανεισμού στη δανειζόμενη εταιρεία, αφήστε το πεδίο **Πόρος** κενό.</span><span class="sxs-lookup"><span data-stu-id="ac2db-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="ac2db-132">Στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής** , στην καρτέλα **Διεταρικός** , ορίστε την επιλογή **Ενεργοποίηση προγραμματισμούκαι φύλλων κατανομής χρόνου διεταιρικών πόρων** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="ac2db-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="ac2db-133">Στη δανειζόμενη εταιρεία</span><span class="sxs-lookup"><span data-stu-id="ac2db-133">In the borrowing company</span></span>

- <span data-ttu-id="ac2db-134">Στη σελίδα **Λίστα πόρων** , στο φίλτρο αναζήτησης, καταγράψτε το όνομα του πόρου που δημιουργήσατε για την εταιρεία δανεισμού για να επαληθεύσετε ότι το όνομα περιλαμβάνεται στη λίστα πόρων για τη δανειζόμενη εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="ac2db-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="ac2db-135">Ζήτηση πόρων έργου</span><span class="sxs-lookup"><span data-stu-id="ac2db-135">Request project resources</span></span>
<span data-ttu-id="ac2db-136">Η λειτουργικότητα για τον προγραμματισμό πόρων έργου επιτρέπει σε όλους τους διαχειριστές πόρων να κατανείμουν ανθρώπινους πόρους σε δεσμεύσεις ή έργα.</span><span class="sxs-lookup"><span data-stu-id="ac2db-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="ac2db-137">Για να ενεργοποιήσετε αυτήν τη λειτουργικότητα, ολοκληρώστε τις παρακάτω εργασίες ή επαληθεύστε ότι έχουν ολοκληρωθεί:</span><span class="sxs-lookup"><span data-stu-id="ac2db-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="ac2db-138">Ρύθμιση ακολουθιών αριθμών.</span><span class="sxs-lookup"><span data-stu-id="ac2db-138">Set up number sequences.</span></span>
- <span data-ttu-id="ac2db-139">Ρύθμιση ροών εργασιών διαχείρισης έργου και λογιστικής.</span><span class="sxs-lookup"><span data-stu-id="ac2db-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="ac2db-140">Ενεργοποίηση ροών εργασιών αιτήσεων πόρων.</span><span class="sxs-lookup"><span data-stu-id="ac2db-140">Enable resource request workflows.</span></span>

<span data-ttu-id="ac2db-141">Μετά την ολοκλήρωση των προηγούμενων εργασιών, μπορείτε να ολοκληρώσετε τις παρακάτω εργασίες όπως εσείς απαιτείτε:</span><span class="sxs-lookup"><span data-stu-id="ac2db-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="ac2db-142">Δημιουργήστε μια αίτηση πόρου από έναν στελεχωμένο πόρο με προκαταρκτική κράτηση.</span><span class="sxs-lookup"><span data-stu-id="ac2db-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="ac2db-143">Παρακολούθηση αιτήσεων πόρων.</span><span class="sxs-lookup"><span data-stu-id="ac2db-143">Monitor resource requests.</span></span>
- <span data-ttu-id="ac2db-144">Κάλυψη αιτημάτων πόρων.</span><span class="sxs-lookup"><span data-stu-id="ac2db-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="ac2db-145">Αίτημα από πόρο στελεχωμένο από μια WBS.</span><span class="sxs-lookup"><span data-stu-id="ac2db-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="ac2db-146">Κάντε κράτηση πόρων σε ένα έργο χωρίς να απαιτείται η υποβολή αιτήματος για στελεχωμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="ac2db-146">Book resources to a project without having a request for a staffed resource.</span></span>
