---
title: Ρύθμιση παραμέτρων αυτοματοποιημένης δημιουργίας τιμολογίων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης παραμέτρων του συστήματος ώστε να δημιουργεί αυτόματα τιμολόγια.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898126"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="1d92c-103">Ρύθμιση παραμέτρων αυτοματοποιημένης δημιουργίας τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="1d92c-103">Configure automated invoice creation</span></span>

<span data-ttu-id="1d92c-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1d92c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1d92c-105">Ολοκληρώστε τα παρακάτω βήματα για να ρυθμίσετε τις παραμέτρους μιας αυτοματοποιημένης εκτέλεσης τιμολογίων στο Project Operations (Λειτουργίες έργου).</span><span class="sxs-lookup"><span data-stu-id="1d92c-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="1d92c-106">Μεταβείτε στις **Ρυθμίσεις** \> **Μαζικές εργασίες**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="1d92c-107">Δημιουργήστε μια μαζική εργασία και ονομάστε την **Δημιουργία τιμολογίων λειτουργιών έργου**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="1d92c-108">Το όνομα της μαζικής εργασίας πρέπει να περιλαμβάνει τον όρο "δημιουργία τιμολογίων".</span><span class="sxs-lookup"><span data-stu-id="1d92c-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="1d92c-109">Στο πεδίο **Τύπος εργασίας**, επιλέξτε **Κανένας**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="1d92c-110">Από προεπιλογή, οι επιλογές **Συχνότητα καθημερινά** και **Είναι ενεργό** έχουν οριστεί σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="1d92c-111">Επιλέξτε **Εκτέλεση ροής εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-111">Select **Run Workflow**.</span></span> <span data-ttu-id="1d92c-112">Στο παράθυρο διαλόγου **Αναζήτηση καρτέλας**, θα δείτε τρεις ροές εργασιών:</span><span class="sxs-lookup"><span data-stu-id="1d92c-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="1d92c-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="1d92c-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="1d92c-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="1d92c-114">ProcessRunner</span></span>
    - <span data-ttu-id="1d92c-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="1d92c-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="1d92c-116">Επιλέξτε **ProcessRunCaller** και μετά επιλέξτε **Προσθήκη**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="1d92c-117">Στο επόμενο παράθυρο διαλόγου, κάντε κλικ στο κουμπί **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="1d92c-118">Μια ροή εργασίας **Αναμονή** ακολουθείται από μια ροή εργασίας **Διαδικασία**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="1d92c-119">Μπορείτε επίσης να επιλέξετε **ProcessRunner** στο βήμα 5.</span><span class="sxs-lookup"><span data-stu-id="1d92c-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="1d92c-120">Στη συνέχεια, όταν επιλέξετε **OK**, μια ροή εργασιών **Διαδικασία** ακολουθείται από μια ροή εργασιών **Αναμονή**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="1d92c-121">Οι ροές εργασιών **ProcessRunCaller** και **ProcessRunner** δημιουργούν τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="1d92c-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="1d92c-122">Το **ProcessRunCaller** καλεί **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="1d92c-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="1d92c-123">Το **ProcessRunner** είναι η ροή εργασιών που δημιουργεί πράγματι τα τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="1d92c-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="1d92c-124">Διατρέχει όλες τις γραμμές σύμβασης για τις οποίες πρέπει να δημιουργηθούν τιμολόγια και δημιουργεί τιμολόγια για αυτές τις γραμμές.</span><span class="sxs-lookup"><span data-stu-id="1d92c-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="1d92c-125">Για να καθορίσετε τις γραμμές σύμβασης για τις οποίες πρέπει να δημιουργηθούν τιμολόγια, η εργασία εξετάζει τις ημερομηνίες εκτέλεσης του τιμολογίου για τις γραμμές της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="1d92c-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="1d92c-126">Εάν οι γραμμές σύμβασης που ανήκουν σε μία σύμβαση έχουν την ίδια ημερομηνία εκτέλεσης τιμολογίου, οι συναλλαγές συνδυάζονται σε ένα τιμολόγιο που έχει δύο γραμμές τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="1d92c-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="1d92c-127">Εάν δεν υπάρχουν συναλλαγές για τη δημιουργία τιμολογίων, η εργασία θα παραλείψει τη δημιουργία τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="1d92c-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="1d92c-128">Αφού ολοκληρωθεί η εκτέλεση του **ProcessRunner**, καλεί το **ProcessRunCaller**, παρέχει την ώρα λήξης και κλείνει.</span><span class="sxs-lookup"><span data-stu-id="1d92c-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="1d92c-129">Το **ProcessRunCaller** ξεκινά ένα χρονόμετρο που εκτελείται για 24 ώρες από την καθορισμένη ώρα λήξης.</span><span class="sxs-lookup"><span data-stu-id="1d92c-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="1d92c-130">Στο τέλος του χρονοδιακόπτη, το **ProcessRunCaller** έχει κλείσει.</span><span class="sxs-lookup"><span data-stu-id="1d92c-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="1d92c-131">Η μαζική εργασία διεργασίας για τη δημιουργία τιμολογίων είναι μια επαναλαμβανόμενη εργασία.</span><span class="sxs-lookup"><span data-stu-id="1d92c-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="1d92c-132">Εάν αυτή η μαζική διεργασία εκτελείται πολλές φορές, δημιουργούνται πολλές παρουσίες της εργασίας και προκαλούν σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="1d92c-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="1d92c-133">Επομένως, θα πρέπει να ξεκινήσετε τη μαζική διεργασία μόνο μία φορά και θα πρέπει να την επανεκκινήσετε μόνο εάν σταματήσει να εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="1d92c-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="1d92c-134">Η μαζική τιμολόγηση εκτελείται μόνο για γραμμές σύμβασης έργου που έχουν ρυθμιστεί από χρονοδιαγράμματα τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="1d92c-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="1d92c-135">Μια γραμμή σύμβασης με μέθοδο χρέωσης σταθερής τιμής πρέπει να έχει ρυθμισμένα ορόσημα.</span><span class="sxs-lookup"><span data-stu-id="1d92c-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="1d92c-136">Μια γραμμή σύμβασης έργου με μέθοδο χρέωσης χρόνου και υλικού θα πρέπει να έχει ρυθμιστεί ως χρονοδιάγραμμα τιμολογίου βάσει ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="1d92c-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="1d92c-137">Το ίδιο ισχύει και για τη γραμμή σύμβασης βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="1d92c-137">The same applies to a project-based contract line.</span></span>     
