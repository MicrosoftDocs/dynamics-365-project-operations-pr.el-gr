---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 32, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 32, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129666"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="58c43-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 32, V3</span><span class="sxs-lookup"><span data-stu-id="58c43-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="58c43-104">Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="58c43-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="58c43-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="58c43-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="58c43-106">Είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="58c43-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="58c43-107">Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="58c43-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="58c43-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="58c43-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="58c43-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 32.</span><span class="sxs-lookup"><span data-stu-id="58c43-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="58c43-110">Αυτή η έκδοση έχει έναν αριθμό έκδοσης V3.10.53.108 και είναι γενικά διαθέσιμη μέσω μιας αυτο-ενημέρωσης τον Ιούνη του 2021.</span><span class="sxs-lookup"><span data-stu-id="58c43-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="58c43-111">Έκδοση κυκλοφορίας 32</span><span class="sxs-lookup"><span data-stu-id="58c43-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="58c43-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="58c43-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="58c43-113">Γενικός</span><span class="sxs-lookup"><span data-stu-id="58c43-113">General</span></span>

- <span data-ttu-id="58c43-114">Όταν μια μείζονα αναβάθμιση αποτύχει, θα πρέπει να αποκλειστούν μόνο τα κύρια σημεία καταχώρησης εφαρμογής, για να διασφαλιστεί ότι οι κοινόχρηστες οντότητες θα εξακολουθούν να είναι προσβάσιμες.</span><span class="sxs-lookup"><span data-stu-id="58c43-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="58c43-115">Χρόνος και έξοδα</span><span class="sxs-lookup"><span data-stu-id="58c43-115">Time and Expense</span></span>

<span data-ttu-id="58c43-116">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="58c43-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="58c43-117">Το **TimeEntriesImportFromResourceAssignment** δεν διατηρεί τις ώρες έναρξης και λήξης του τμήματος περιγράμματος ανάθεσης πόρων.</span><span class="sxs-lookup"><span data-stu-id="58c43-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="58c43-118">Όταν επιλέγετε **Άνοιγμα καταχώρησης** στο πλέγμα **Καταχώρηση χρόνου**, ενδέχεται να μην μπορείτε να επιλέξετε άλλες φόρμες.</span><span class="sxs-lookup"><span data-stu-id="58c43-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="58c43-119">Ενώ εισάγετε αναθέσεις σε χρονικές καταχωρήσεις, το ερώτημα κώδικα του προγράμματος-πελάτη θα μπορούσε να δημιουργήσει μια μεγάλη διεύθυνση URL που αποτυγχάνει το ερώτημα.</span><span class="sxs-lookup"><span data-stu-id="58c43-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="58c43-120">Στο πλέγμα **Καταχώρηση χρόνου**, μετά τη διαγραφή μιας τιμής από ένα κελί, η εστίαση δεν παραμένει στο πλέγμα.</span><span class="sxs-lookup"><span data-stu-id="58c43-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="58c43-121">Το κουμπί **Απόρριψη** έχει καταργηθεί από την προβολή **Επεξεργασία εγκρίσεων** για τις σύγχρονες εγκρίσεις.</span><span class="sxs-lookup"><span data-stu-id="58c43-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="58c43-122">Η σταθερότητα και οι επιδόσεις της μαζικής έγκρισης καταχώρησης χρόνου επηρεάζονται από αδιέξοδα και αποτυχία κατάλληλου χειρισμού προσαρμογών που σχετίζονται με την οντότητα **Καταχώρηση χρόνου**.</span><span class="sxs-lookup"><span data-stu-id="58c43-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="58c43-123">Σχεδιασμός έργου</span><span class="sxs-lookup"><span data-stu-id="58c43-123">Project Planning</span></span>

- <span data-ttu-id="58c43-124">Δημιουργείται μια εξαίρεση αναφοράς null όταν ενημερώνετε ένα έργο που έχει μια τιμή null στο πεδίο **Μονάδα σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="58c43-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="58c43-125">**Η ανανέωση των συνόλων έργου** υπολογίζει λανθασμένα το υπόλοιπο κόστος και τις υπόλοιπες πωλήσεις σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="58c43-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="58c43-126">Οι πλεονάζοντες υπολογισμοί τιμολόγησης επηρεάζουν την απόδοση που σχετίζεται με ενημερώσεις σε καμπύλες εκχώρησης πόρων.</span><span class="sxs-lookup"><span data-stu-id="58c43-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="58c43-127">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="58c43-127">Resource Management</span></span>

<span data-ttu-id="58c43-128">Το παρακάτω ζήτημα έχει διορθωθεί:</span><span class="sxs-lookup"><span data-stu-id="58c43-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="58c43-129">Όταν η χωρητικότητα ημερολογίου ενός πόρου με δυνατότητα κράτησης είναι μεγαλύτερη από 1, το Project Service Automation αναγνωρίζει λανθασμένα τη χωρητικότητα ως 0 (μηδέν).</span><span class="sxs-lookup"><span data-stu-id="58c43-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="58c43-130">Επομένως, προκύπτει ένας ατέρμονος βρόχος στην προβολή χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="58c43-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="58c43-131">Πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="58c43-131">Sales</span></span>

<span data-ttu-id="58c43-132">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="58c43-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="58c43-133">Όταν δημιουργείται μια γραμμή ημερολογίου που έχει προσαρμοσμένο τύπο συναλλαγής, προκύπτει η ακόλουθη εξαίρεση αναφοράς null: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitServiceTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="58c43-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="58c43-134">Οι ρόλοι και οι κατηγορίες που απενεργοποιούνται πριν να αντιγράψετε μια προσφορά δεν πρέπει να προστίθενται σε χρεώσιμους ρόλους και κατηγορίες της προσφοράς που μόλις αντιγράψατε.</span><span class="sxs-lookup"><span data-stu-id="58c43-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="58c43-135">Η ημερομηνία εγγράφου και η ημερομηνία λογιστικής δεν είναι στοιχισμένες με την ημερομηνία έναρξης που παρέχεται σε μια λεπτομέρεια γραμμής τιμολογίου που δημιουργείται απευθείας σε ένα προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="58c43-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="58c43-136">Οι εξαιρέσεις αναφοράς Null δημιουργούνται σε σενάρια που σχετίζονται με την απενεργοποίηση ρόλων και κατηγοριών πριν από την αντιγραφή μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="58c43-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="58c43-137">Η ενέργεια **Ενημέρωση τιμών** στη σελίδα **Έργα** δεν ενημερώνει τις εκτιμήσεις των δαπανών και τις εκτιμήσεις των υλικών.</span><span class="sxs-lookup"><span data-stu-id="58c43-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
