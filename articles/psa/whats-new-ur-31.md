---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 31, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 31, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945535"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="0353d-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 31, V3</span><span class="sxs-lookup"><span data-stu-id="0353d-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="0353d-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="0353d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="0353d-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="0353d-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="0353d-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="0353d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="0353d-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="0353d-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="0353d-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="0353d-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="0353d-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 31.</span><span class="sxs-lookup"><span data-stu-id="0353d-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="0353d-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.52.77 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Μαΐου 2021.</span><span class="sxs-lookup"><span data-stu-id="0353d-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="0353d-111">Έκδοση κυκλοφορίας 31</span><span class="sxs-lookup"><span data-stu-id="0353d-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="0353d-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="0353d-112">Bug fixes</span></span>

<span data-ttu-id="0353d-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="0353d-113">**Time and Expense**</span></span>

<span data-ttu-id="0353d-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="0353d-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="0353d-115">Τα κουμπιά εντολής ελέγχου καταχώρησης χρόνου στη σελίδα **Πόρος με δυνατότητα κράτησης** ήταν μπερδεμένα.</span><span class="sxs-lookup"><span data-stu-id="0353d-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="0353d-116">Δημιουργήθηκε μια εξαίρεση αναφοράς null στο **Project.SetTrackingFields** κατά την έγκριση μιας καταχώρησης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="0353d-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="0353d-117">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="0353d-117">**Resource Management**</span></span>

<span data-ttu-id="0353d-118">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="0353d-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="0353d-119">Η ρύθμιση **δημιουργίας μέλους ομάδας** δεν εμφανίζει σωστά τη ρύθμιση μετα-δεδομένων ρύθμισης κράτησης για την **Προεπιλεγμένη κατάσταση δέσμευσης κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="0353d-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="0353d-120">Κατά την αναβάθμιση από PSA 1.X σε 3.X, η διεργασία αναβάθμισης αποτυγχάνει στο **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="0353d-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="0353d-121">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="0353d-121">**Sales**</span></span>

<span data-ttu-id="0353d-122">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="0353d-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="0353d-123">Τα πραγματικά έσοδα μετατρέπουν τα ποσά στη νομισματική μονάδα έργου στο πλέγμα παρακολούθησης.</span><span class="sxs-lookup"><span data-stu-id="0353d-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="0353d-124">Η προεπιλογή νομισματικής μονάδας χρησιμοποιείται κατά τη δημιουργία γραμμών χρονικού, γραμμών προσφοράς και γραμμών σύμβασης σε σενάρια όπου η βασική νομισματική μονάδα ενός οργανισμού διαφέρει από τη νομισματική μονάδα έργου.</span><span class="sxs-lookup"><span data-stu-id="0353d-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="0353d-125">Το ερώτημα **επικύρωσης ημερολογίου διόρθωσης σε εκκρεμότητα** δεν φιλτράρεται κατά έργο.</span><span class="sxs-lookup"><span data-stu-id="0353d-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="0353d-126">Οι υπόλοιπες πωλήσεις υπολογίζονται λανθασμένα σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="0353d-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="0353d-127">Οι προσφορές που βασίζονται σε μια επαφή αποτυγχάνουν όταν δημιουργούνται χωρίς τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="0353d-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="0353d-128">Δεν εμφανίζεται κανένα κουμπί αυξομείωσης επεξεργασίας όταν επιλέγετε **Επιβεβαίωση τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="0353d-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="0353d-129">Δεν εμφανίζεται κανένα κουμπί αυξομείωσης επεξεργασίας όταν επιλέγετε **Δημιουργία τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="0353d-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="0353d-130">Το κλείσιμο μιας προσφοράς ως χαμένης δεν ακυρώνει τις κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="0353d-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







