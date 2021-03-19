---
title: Επιδόσεις χρονοδιαγράμματος πόρου έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο βελτίωσης των επιδόσεων του προγραμματισμού των πόρων για ένα μεγάλο αριθμό έργων.
author: Yowelle
manager: AnnBe
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 34c31570778f9b64c23387112cf56fa1139cd0fd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289009"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="2c7e8-103">Επιδόσεις χρονοδιαγράμματος πόρου έργου</span><span class="sxs-lookup"><span data-stu-id="2c7e8-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="2c7e8-104">Τα ζητήματα επιδόσεων που σχετίζονται με τον προγραμματισμό των πόρων μπορεί να προκύψουν όταν ο αριθμός των έργων φθάνει τις χιλιάδες.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="2c7e8-105">Για τη βελτίωση των επιδόσεων του προγραμματισμού των πόρων, διατίθεται μια δυνατότητα που επιτρέπει στους χρήστες να μειώνουν το χρόνο που απαιτείται για την εκκίνηση της φόρμας "Διαθεσιμότητα πόρου".</span><span class="sxs-lookup"><span data-stu-id="2c7e8-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="2c7e8-106">Συγκεκριμένα, καταργείται η διαδικασία συγχρονισμού συνάθροισης παραγωγικής ικανότητας πόρων και χρησιμοποιεί τον πίνακα **ResProjectResource** για να επιταχύνει την αναζήτηση πόρων.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="2c7e8-107">Λάβετε υπόψη σας ότι ο πίνακας **ResRollup** δεν θα χρησιμοποιηθεί πλέον.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2c7e8-108">Εάν υπάρχει μια εξάρτηση από τη διεργασία συγχρονισμού συνάθροισης παραγωγικής ικανότητας πόρων ή τον πίνακα **ResProjectResource**, μην χρησιμοποιήσετε αυτήν τη δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="2c7e8-109">Ενεργοποίηση της βελτίωσης των επιδόσεων του προγραμματισμού πόρων</span><span class="sxs-lookup"><span data-stu-id="2c7e8-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="2c7e8-110">Για να ενεργοποιήσετε τη βελτίωση των επιδόσεων του προγραμματισμού πόρων, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="2c7e8-111">Μεταβείτε στην επιλογή **Διαχείριση δυνατοτήτων** > **Όλες** και στη λίστα δυνατοτήτων, εντοπίστε την **Ενεργοποίηση δυνατότητας βελτίωσης επιδόσεων προγραμματισμού πόρων έργου**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="2c7e8-112">Επιλέξτε **Ενεργοποίηση τώρα**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="2c7e8-113">Εάν δεν μπορείτε να βρείτε τη δυνατότητα στη λίστα, επιλέξτε **Έλεγχος για ενημερώσεις** για να ανανεώσετε τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="2c7e8-114">Ανανεώστε το πρόγραμμα περιήγησής σας και, στη συνέχεια, μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** > **Περιοδικός** > **Πόροι έργου** > **Συγχρονισμός χωρητικότητας ημερολογίων πόρων σε όλες τις εταιρείες**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="2c7e8-115">Ορίστε το στοιχείο **Κατάργηση υπαρχουσών καρτελών παραγωγικής ικανότητας** σε **Ναι** για την κατάργηση προηγούμενων δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="2c7e8-116">Εάν θέλετε να δημιουργήσετε στοιχειώδη δεδομένα, ορίστε σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="2c7e8-117">Στο πεδίο **Κωδικός περιόδου**, επιλέξτε την περίοδο στην οποία πρέπει να δημιουργηθούν τα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="2c7e8-118">Εάν επιλέξετε έναν κωδικό περιόδου, δεν χρειάζεται να ορίσετε μια ημερομηνία έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="2c7e8-119">Εάν αφήσετε κενό το πεδίο **Κωδικός περιόδου**, επιλέξτε συγκεκριμένες ημερομηνίες έναρξης και λήξης για τη δημιουργία δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="2c7e8-120">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="2c7e8-121">Με αυτόν τον τρόπο θα διανεμηθούν γενικά δεδομένα στον πίνακα **ResCalendarCapacity** σε όλες τις εταιρείες του περιβάλλοντός σας, επομένως η μαζική εργασία θα πρέπει να εκτελεστεί μόνο σε μία νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="2c7e8-122">Τα δεδομένα σε αυτήν τη μαζική εργασία είναι απαραίτητα για τον υπολογισμό της παραγωγικής ικανότητας των πόρων μέσω του συσχετισμένου ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="2c7e8-123">Μεταβείτε στα στοιχεία **Διαχείριση έργου και λογιστική** > **Περιοδικός** > **Πόροι έργου** > **Συμπλήρωση πόρων έργου σε όλες τις εταιρείες** και, στη συνέχεια, επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="2c7e8-124">Αυτή είναι η δέσμη ενεργειών αναβάθμισης δεδομένων για γενικά δεδομένα στους πίνακες **ResProjectResource**, **ResProjectResource** και **ResEffectiveDateTimeRange**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="2c7e8-125">Οι τιμές για το πεδίο **PSAPRojSchedRole.RootActivity** επίσης ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="2c7e8-126">Εάν δεν εκτελεστεί αυτό το στοιχείο, θα εμφανιστεί μια προειδοποίηση όταν επιχειρήσετε να εκτελέσετε λειτουργίες προγραμματισμού πόρων.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="2c7e8-127">Απενεργοποίηση της βελτίωσης των επιδόσεων του προγραμματισμού πόρων</span><span class="sxs-lookup"><span data-stu-id="2c7e8-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="2c7e8-128">Μεταβείτε στην επιλογή **Διαχείριση δυνατοτήτων** > **Όλες** και αναζητήστε την **Ενεργοποίηση δυνατότητας βελτίωσης επιδόσεων προγραμματισμού πόρων έργου**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="2c7e8-129">Επιλέξτε τη δυνατότητα και, στη συνέχεια, επιλέξτε το κουμπί **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="2c7e8-130">Ανανεώστε το πρόγραμμα περιήγησης που χρησιμοποιείτε.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-130">Refresh your browser.</span></span>
4. <span data-ttu-id="2c7e8-131">Μεταβείτε στα στοιχεία **Διαχείριση έργου και λογιστική** > **Περιοδική** > **Συγχρονισμός παραγωγικής ικανότητας** > **Συγχρονισμός συναθροίσεων παραγωγικής ικανότητας πόρων**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="2c7e8-132">Στη σελίδα **Συγχρονισμός συναθροίσεων παραγωγικής ικανότητας**, ορίστε την **Κατάργηση υπαρχουσών καρτελών παραγωγικής ικανότητας** σε **Ναι** για να καταργηθούν τα προηγούμενα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="2c7e8-133">Εάν θέλετε να δημιουργήσετε στοιχειώδη δεδομένα, ορίστε σε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="2c7e8-134">Στο πεδίο **Κωδικός περιόδου**, επιλέξτε την περίοδο στην οποία πρέπει να δημιουργηθούν τα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="2c7e8-135">Εάν επιλέξετε έναν κωδικό περιόδου, δεν χρειάζεται να ορίσετε μια ημερομηνία έναρξης και λήξης.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="2c7e8-136">Εάν αφήσετε κενό το πεδίο **Κωδικός περιόδου**, επιλέξτε συγκεκριμένες ημερομηνίες έναρξης και λήξης για τη δημιουργία δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="2c7e8-137">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="2c7e8-138">Με αυτόν τον τρόπο θα διανεμηθούν γενικά δεδομένα στον πίνακα **ResRollup** σε όλες τις εταιρείες του περιβάλλοντός σας, επομένως η μαζική εργασία θα πρέπει να εκτελεστεί μόνο σε μία νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="2c7e8-139">Αυτή η μαζική εργασία απαιτείται για όλες τις προβολές **Διαθεσιμότητα πόρου**.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="2c7e8-140">Σε περίπτωση που δεν εκτελεστεί αυτή η μαζική εργασία, τα δεδομένα **ResRollup** θα δημιουργηθούν άμεσα κάτι που μπορεί να διαρκέσει πολύ.</span><span class="sxs-lookup"><span data-stu-id="2c7e8-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]