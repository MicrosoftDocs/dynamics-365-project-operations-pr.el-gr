---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 33, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 33, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334542"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="817c4-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 33, V3</span><span class="sxs-lookup"><span data-stu-id="817c4-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="817c4-104">Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="817c4-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="817c4-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="817c4-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="817c4-106">Είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="817c4-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="817c4-107">Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="817c4-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="817c4-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="817c4-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="817c4-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 33.</span><span class="sxs-lookup"><span data-stu-id="817c4-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="817c4-110">Αυτή η έκδοση έχει αριθμό έκδοσης V3.10.54.98 και είναι γενικά διαθέσιμη μέσω μιας αυτο-ενημέρωσης τον Ιούλιο του 2021.</span><span class="sxs-lookup"><span data-stu-id="817c4-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="817c4-111">Έκδοση κυκλοφορίας 33</span><span class="sxs-lookup"><span data-stu-id="817c4-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="817c4-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="817c4-112">Bug fixes</span></span>

<span data-ttu-id="817c4-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="817c4-113">**Time and Expense**</span></span>

<span data-ttu-id="817c4-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="817c4-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="817c4-115">Δύο κλειδωμένα πεδία, **msdyn_description** και **msdyn_externaldescription** είναι επεξεργάσιμα μετά την υποβολή.</span><span class="sxs-lookup"><span data-stu-id="817c4-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="817c4-116">Δημιουργείται ένα μήνυμα σφάλματος εάν δημιουργηθεί μια δαπάνη η οποία δεν σχετίζεται με ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="817c4-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="817c4-117">Όταν δημιουργείται μια καταχώρηση χρόνου, ο ρόλος του πόρου μετατρέπεται από προεπιλογή σε ανενεργό ρόλο.</span><span class="sxs-lookup"><span data-stu-id="817c4-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="817c4-118">Οι γραμμές ημερολογίου που συσχετίζονται με μια δαπάνη που έχει ανακληθεί και διαγραφεί, δεν διαγράφονται.</span><span class="sxs-lookup"><span data-stu-id="817c4-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="817c4-119">Στην καταχώρηση **Φόρμα γρήγορης δημιουργίας καταχώρησης ώρας**, ενημερώστε την προβολή **Λίστα εργασιών έργου**, για να αλλάξετε την ημερομηνία που εμφανίζεται από προεπιλογή στην ημερομηνία έναρξης της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="817c4-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="817c4-120">Όταν δημιουργείτε μια καταχώρηση χρόνου από την καρτέλα **Σχετικά** του πόρου με δυνατότητα κράτησης, η καταχώρηση χρόνου δημιουργείται λανθασμένα για τον συνδεδεμένο χρήστη αντί για τον γονικό πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="817c4-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="817c4-121">Νέα πεδία προστίθενται στο παράθυρο διαλόγου **Μαζική έγκριση MDD**.</span><span class="sxs-lookup"><span data-stu-id="817c4-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="817c4-122">**Σχεδιασμός έργου**</span><span class="sxs-lookup"><span data-stu-id="817c4-122">**Project planning**</span></span>

<span data-ttu-id="817c4-123">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="817c4-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="817c4-124">Αργές επιδόσεις στη δημιουργία έργων, όταν τα πρότυπα ωρών εργασίας έργου εφαρμόζονται με σύνθετα ημερολόγια.</span><span class="sxs-lookup"><span data-stu-id="817c4-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="817c4-125">Όταν η ημερομηνία έναρξης είναι μεγαλύτερη από την ημερομηνία λήξης, εμφανίζεται ένα σφάλμα στο αντίγραφο προτύπου έργου λόγω διαφορών στο στοιχείο χρόνου κάθε πεδίου.</span><span class="sxs-lookup"><span data-stu-id="817c4-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="817c4-126">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="817c4-126">**Resource management**</span></span>

<span data-ttu-id="817c4-127">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="817c4-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="817c4-128">Μια εσφαλμένη παράμετρος χρησιμοποιείται στο ερώτημα χρήσης πόρου και η XML συντελεί σε εσφαλμένα αποτελέσματα φιλτραρίσματος στο πλέγμα **Χρήσης πόρου**.</span><span class="sxs-lookup"><span data-stu-id="817c4-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="817c4-129">Η επιβεβαίωση **Επέκταση κρατήσεων** εμφανίζει εσφαλμένη ημερομηνία λήξης για κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="817c4-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="817c4-130">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="817c4-130">**Sales**</span></span>

<span data-ttu-id="817c4-131">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="817c4-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="817c4-132">Παρουσιάζεται μήνυμα σφάλματος όταν δημιουργείται μια τιμή κατηγορίας με τιμές που λείπουν.</span><span class="sxs-lookup"><span data-stu-id="817c4-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="817c4-133">Παρουσιάζεται μήνυμα σφάλματος εάν δημιουργηθεί ένα ορόσημο γραμμής σύμβασης χωρίς γραμμή εντολής.</span><span class="sxs-lookup"><span data-stu-id="817c4-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
