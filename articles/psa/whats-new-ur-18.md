---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 18, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 18, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: f7def50e77a83fd790b81b1b4fd36008ce293b0c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006646"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="01dc3-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 18, V3</span><span class="sxs-lookup"><span data-stu-id="01dc3-103">Project Service Automation Update Release 18, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="01dc3-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="01dc3-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="01dc3-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="01dc3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="01dc3-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="01dc3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="01dc3-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="01dc3-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="01dc3-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="01dc3-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="01dc3-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 18.</span><span class="sxs-lookup"><span data-stu-id="01dc3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="01dc3-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.8.12 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Απριλίου 2020.</span><span class="sxs-lookup"><span data-stu-id="01dc3-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="01dc3-111">Έκδοση κυκλοφορίας 18</span><span class="sxs-lookup"><span data-stu-id="01dc3-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="01dc3-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="01dc3-112">Bug fixes</span></span>

<span data-ttu-id="01dc3-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="01dc3-113">**Time and Expense**</span></span>

- <span data-ttu-id="01dc3-114">Διορθώθηκε: Οι ροές **Ανάκληση**, **Αίτημα** και **Ακύρωση έγκρισης** δημιουργούν εξαιρέσεις με ασαφή μηνύματα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="01dc3-114">Fixed: **Recall**, **Request**, and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="01dc3-115">Διορθώθηκε: Όταν η **Ακύρωση έγκρισης** αποτυγχάνει για μια δαπάνη, δεν δημιουργείτε ένα σχετικό σφάλμα εξαίρεσης.</span><span class="sxs-lookup"><span data-stu-id="01dc3-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="01dc3-116">Διορθώθηκε: Το πλέγμα χρονικής καταχώρησης χειρίζεται λανθασμένα τις μη εργάσιμες ημέρες στην Αυστραλία μετά την αλλαγή θερινής ώρας (DST) τον Οκτώβριο.</span><span class="sxs-lookup"><span data-stu-id="01dc3-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="01dc3-117">Διορθώθηκε: Η λανθασμένη λογική προεπιλογής αποτρέπει την υποβολή των εξόδων.</span><span class="sxs-lookup"><span data-stu-id="01dc3-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="01dc3-118">Διορθώθηκε: Όταν αποτυγχάνει η έγκριση χρονικής καταχώρησης, η έγκριση παραμένει σε κατάσταση **εκκρεμότητας**.</span><span class="sxs-lookup"><span data-stu-id="01dc3-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="01dc3-119">Διορθώθηκε: Σφάλματα SQL σε μαζικές εγκρίσεις (αδιέξοδο/χρονικό όριο).</span><span class="sxs-lookup"><span data-stu-id="01dc3-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="01dc3-120">Διορθώθηκε: Σημαντικά προβλήματα απόδοσης στην εμπειρία χρήστη προκαλούνταν από την ενημέρωση μελών της ομάδας κατά την έγκριση χρονικών καταχωρήσεων.</span><span class="sxs-lookup"><span data-stu-id="01dc3-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="01dc3-121">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="01dc3-121">**Project Management**</span></span>

- <span data-ttu-id="01dc3-122">Διόρθωση: Η ειδοποίηση ζώνης ώρας μετακινήθηκε από την προβολή **Εναρμόνισης** στην κύρια φόρμα του **Έργου**.</span><span class="sxs-lookup"><span data-stu-id="01dc3-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="01dc3-123">Διορθώθηκε: Το πρότυπο ημερολογίου δεν είναι σωστά προεπιλεγμένο όταν ανοίγει μια νέα φόρμα έργου.</span><span class="sxs-lookup"><span data-stu-id="01dc3-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="01dc3-124">Διορθώθηκε: Στα προγράμματα περιήγησης που βασίζονται στο Chromium, οι χρήστες δεν μπορούν να επιλέξουν εύκολα τις εργασίες προκατόχου για διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="01dc3-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="01dc3-125">Διορθώθηκε: Η δημιουργία ή η αντιγραφή **έργου από κενό πρότυπο** ανακτά μη σχετικές αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="01dc3-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="01dc3-126">Διορθώθηκε: Σε συγκεκριμένες υποθέσεις άκρων, η δημιουργία μιας νέας ανάθεσης από το πλέγμα εργασιών καταλήγει στη δημιουργία διπλότυπων καρτελών.</span><span class="sxs-lookup"><span data-stu-id="01dc3-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="01dc3-127">Διορθώθηκε: Στη μη αυτόματη λειτουργία, οι χρήστες δεν μπορούν να ενημερώσουν τις ημερομηνίες έναρξης εργασιών, ώστε να είναι μεταγενέστερες της τρέχουσας αποθηκευμένης ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="01dc3-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="01dc3-128">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="01dc3-128">**Resource Management**</span></span>

- <span data-ttu-id="01dc3-129">Διορθώθηκε: Η γραμμή μερικού αθροίσματος της προβολής **Εναρμόνισης** υπολογίζει εσφαλμένα τη διακύμανση κρατήσεων μετά την παράταση των κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="01dc3-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="01dc3-130">Διορθώθηκε: Η προβολή **Εναρμόνισης** εμφανίζει εσφαλμένα τις αναθέσεις πόρων όταν ο πόρος με δυνατότητα κράτησης έχει ένα ημερολόγιο που δεν ταιριάζει με το ημερολόγιο του έργου.</span><span class="sxs-lookup"><span data-stu-id="01dc3-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="01dc3-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="01dc3-131">**Sales**</span></span>

- <span data-ttu-id="01dc3-132">Διορθώθηκε: Όταν οι χρονικές καταχωρήσεις επανεγκρίνονται (**Έγκριση > Ακύρωση >** επανέγκριση), δημιουργείται μια διπλότυπη μη χρεώσιμη πραγματική τιμή.</span><span class="sxs-lookup"><span data-stu-id="01dc3-132">Fixed: When time entries are re-approved (**Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]