---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 24, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 24, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 3a37e71be2cce259d8aed0621d13393b6bbe4199
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126573"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="45289-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 24, V3</span><span class="sxs-lookup"><span data-stu-id="45289-103">Project Service Automation Update Release 24, V3</span></span>

<span data-ttu-id="45289-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="45289-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="45289-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="45289-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="45289-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="45289-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="45289-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="45289-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="45289-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="45289-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="45289-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 24.</span><span class="sxs-lookup"><span data-stu-id="45289-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="45289-110">Αυτή η έκδοση έχει αριθμό δομής V 3.10.42.43 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Οκτώβριο του 2020.</span><span class="sxs-lookup"><span data-stu-id="45289-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="45289-111">Έκδοση κυκλοφορίας 24</span><span class="sxs-lookup"><span data-stu-id="45289-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="45289-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="45289-112">Bug fixes</span></span>

<span data-ttu-id="45289-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="45289-113">**Sales**</span></span>

<span data-ttu-id="45289-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="45289-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="45289-115">Πρόβλημα κατά τη ρύθμιση του προεπιλεγμένου τιμοκαταλόγου προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="45289-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="45289-116">Οι επιδόσεις της Επιτυχούς προσφοράς είναι αργές λόγω του ενσωματωμένου τιμοκαταλόγου και του αντιγράφου των καρτελών τιμών ρόλου.</span><span class="sxs-lookup"><span data-stu-id="45289-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="45289-117">Η **Σύμβαση έργου/κέντρο πωλήσεων** > **Στοιχείο γραμμής προϊόντος/ποσότητα γραμμής παραγγελίας** στρογγυλοποιείται αυτόματα στον πλησιέστερο ακέραιο.</span><span class="sxs-lookup"><span data-stu-id="45289-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="45289-118">Προβιβασμός σε προνόμια συστήματος κατά την ανάγνωση των λιστών τιμών.</span><span class="sxs-lookup"><span data-stu-id="45289-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="45289-119">Αντιγράψτε τα πεδία διευθύνσεων πελατών **address1_freighttermscode** και **address1_shippingmethodcode** σε προσφορά/παραγγελία.</span><span class="sxs-lookup"><span data-stu-id="45289-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="45289-120">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="45289-120">**Time and Expense**</span></span>

<span data-ttu-id="45289-121">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="45289-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="45289-122">Το **Πλέγμα καταχώρησης ώρας** δεν υποστηρίζει συμπεριφορά ώρας **Μόνο ημερομηνία**.</span><span class="sxs-lookup"><span data-stu-id="45289-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="45289-123">Η **Καταχώρηση χρόνου** δεν ανανεώνεται αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="45289-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="45289-124">Απαιτείται μη αυτόματη ανανέωση.</span><span class="sxs-lookup"><span data-stu-id="45289-124">A manual refresh is required.</span></span>
- <span data-ttu-id="45289-125">Δεν είναι δυνατή η εισαγωγή των καταχωρήσεων ώρας από μια ανάθεση, όταν υπάρχει μια διακοπή (0 ώρες) στις αναθέσεις ενός πόρου.</span><span class="sxs-lookup"><span data-stu-id="45289-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="45289-126">Όταν δημιουργείτε μια καταχώρηση χρόνου, ορίστε την αρχή ίδια με την **msdyn_date**.</span><span class="sxs-lookup"><span data-stu-id="45289-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="45289-127">Ενεργοποιήστε εκ νέου την μαζική επεξεργασία για την καταχώρηση χρόνου.</span><span class="sxs-lookup"><span data-stu-id="45289-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="45289-128">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="45289-128">**Resource Management**</span></span>

<span data-ttu-id="45289-129">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="45289-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="45289-130">Η προσπάθεια ενημέρωσης της κατάστασης για μια διήμερη κράτηση χωρίς απαίτηση θα προκαλέσει μια εξαίρεση null-ref.</span><span class="sxs-lookup"><span data-stu-id="45289-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="45289-131">Σφάλμα κατά τη φόρτωση της **Προβολής συμψηφισμού**.</span><span class="sxs-lookup"><span data-stu-id="45289-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="45289-132">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="45289-132">**Project Management**</span></span>

<span data-ttu-id="45289-133">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="45289-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="45289-134">Στο **Χρονοδιάγραμμα έργου**, όταν αλλάζετε από το **Μη αυτόματο** στο **Αυτόματο**, η αυτόματη αποθήκευση δεν ολοκληρώνεται.</span><span class="sxs-lookup"><span data-stu-id="45289-134">In the **Project Schedule**, when changing from **Manual** to **Auto**, auto save is not completing.</span></span>
- <span data-ttu-id="45289-135">Το κόστος δαπανών δεν πρέπει να υπολογίζεται προς τη διακύμανση στο **Πλέγμα παρακολούθησης έργου**.</span><span class="sxs-lookup"><span data-stu-id="45289-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="45289-136">Ασυνεπής συμπεριφορά για στήλες **Ετικετών εκτιμήσεων** κατά τη διάρκεια της φόρτωσης σε σχέση με την αλλαγή του τύπου **Χρονικής φάσης**.</span><span class="sxs-lookup"><span data-stu-id="45289-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="45289-137">Το πραγματικό κόστος ενός έργου ενδέχεται να μην αντικατοπτρίζει τα σύνολα από τα **Πραγματικά στοιχεία**.</span><span class="sxs-lookup"><span data-stu-id="45289-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="45289-138">**Η εκτιμώμενη ημερομηνία λήξης** στην καρτέλα **Σύνοψης** δεν ταιριάζει με το **Χρονοδιάγραμμα WBS**.</span><span class="sxs-lookup"><span data-stu-id="45289-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="45289-139">Η **Ενημέρωση των πραγματικών ωρών** σε προεξοχή δεν λειτουργεί σωστά.</span><span class="sxs-lookup"><span data-stu-id="45289-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="45289-140">Ένας υπεύθυνος έργου εκτός του ριζικού καταλόγου **BU** δεν μπορεί να δημιουργήσει ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="45289-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="45289-141">Οι αλλαγές στην εργασία ή την κατηγορία στις **Εκτιμήσεις εξόδων** δεν διατηρούνται.</span><span class="sxs-lookup"><span data-stu-id="45289-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="45289-142">Το **Αντίγραφο της σύμβασης** αντιγράφει τα προγράμματα τιμολογίων και την κατάσταση εκτέλεσης.</span><span class="sxs-lookup"><span data-stu-id="45289-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="45289-143">Το κουμπί **Ανανέωση πραγματικών τιμών** υπολογίζει λανθασμένα τις εργασίες σύνοψης.</span><span class="sxs-lookup"><span data-stu-id="45289-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="45289-144">Πρόσθετο του Microsoft Project: Διόρθωση σφάλματος αναφοράς null εάν κάποιο μέλος της ομάδας έχει μια κενή μονάδα πόρων.</span><span class="sxs-lookup"><span data-stu-id="45289-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>

