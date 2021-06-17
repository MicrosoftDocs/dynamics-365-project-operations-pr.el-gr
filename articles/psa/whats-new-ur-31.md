---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 31, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 31, V3.
author: ruhercul
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
ms.openlocfilehash: 160187ba7b96547e85a7a4ec4bf84c86d8fd8257
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999131"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="52050-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 31, V3</span><span class="sxs-lookup"><span data-stu-id="52050-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="52050-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="52050-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="52050-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="52050-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="52050-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="52050-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="52050-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="52050-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="52050-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="52050-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="52050-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 31.</span><span class="sxs-lookup"><span data-stu-id="52050-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="52050-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.52.77 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Μαΐου 2021.</span><span class="sxs-lookup"><span data-stu-id="52050-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="52050-111">Έκδοση κυκλοφορίας 31</span><span class="sxs-lookup"><span data-stu-id="52050-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="52050-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="52050-112">Bug fixes</span></span>

<span data-ttu-id="52050-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="52050-113">**Time and Expense**</span></span>

<span data-ttu-id="52050-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="52050-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="52050-115">Τα κουμπιά εντολής ελέγχου καταχώρησης χρόνου στη σελίδα **Πόρος με δυνατότητα κράτησης** ήταν μπερδεμένα.</span><span class="sxs-lookup"><span data-stu-id="52050-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="52050-116">Δημιουργήθηκε μια εξαίρεση αναφοράς null στο **Project.SetTrackingFields** κατά την έγκριση μιας καταχώρησης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="52050-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="52050-117">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="52050-117">**Resource Management**</span></span>

<span data-ttu-id="52050-118">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="52050-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="52050-119">Η ρύθμιση **δημιουργίας μέλους ομάδας** δεν εμφανίζει σωστά τη ρύθμιση μετα-δεδομένων ρύθμισης κράτησης για την **Προεπιλεγμένη κατάσταση δέσμευσης κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="52050-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="52050-120">Κατά την αναβάθμιση από PSA 1.X σε 3.X, η διεργασία αναβάθμισης αποτυγχάνει στο **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="52050-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="52050-121">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="52050-121">**Sales**</span></span>

<span data-ttu-id="52050-122">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="52050-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="52050-123">Τα πραγματικά έσοδα μετατρέπουν τα ποσά στη νομισματική μονάδα έργου στο πλέγμα παρακολούθησης.</span><span class="sxs-lookup"><span data-stu-id="52050-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="52050-124">Η προεπιλογή νομισματικής μονάδας χρησιμοποιείται κατά τη δημιουργία γραμμών χρονικού, γραμμών προσφοράς και γραμμών σύμβασης σε σενάρια όπου η βασική νομισματική μονάδα ενός οργανισμού διαφέρει από τη νομισματική μονάδα έργου.</span><span class="sxs-lookup"><span data-stu-id="52050-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="52050-125">Το ερώτημα **επικύρωσης ημερολογίου διόρθωσης σε εκκρεμότητα** δεν φιλτράρεται κατά έργο.</span><span class="sxs-lookup"><span data-stu-id="52050-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="52050-126">Οι υπόλοιπες πωλήσεις υπολογίζονται λανθασμένα σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="52050-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="52050-127">Οι προσφορές που βασίζονται σε μια επαφή αποτυγχάνουν όταν δημιουργούνται χωρίς τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="52050-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="52050-128">Δεν εμφανίζεται κανένα κουμπί αυξομείωσης επεξεργασίας όταν επιλέγετε **Επιβεβαίωση τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="52050-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="52050-129">Δεν εμφανίζεται κανένα κουμπί αυξομείωσης επεξεργασίας όταν επιλέγετε **Δημιουργία τιμολογίου**.</span><span class="sxs-lookup"><span data-stu-id="52050-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="52050-130">Το κλείσιμο μιας προσφοράς ως χαμένης δεν ακυρώνει τις κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="52050-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







