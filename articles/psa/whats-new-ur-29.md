---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 29, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 29, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 711255ab66f84fe46d0f16fa72e5a10fe0360394
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "5499671"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="3c32b-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 29, V3</span><span class="sxs-lookup"><span data-stu-id="3c32b-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="3c32b-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="3c32b-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="3c32b-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="3c32b-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="3c32b-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="3c32b-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="3c32b-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="3c32b-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="3c32b-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="3c32b-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="3c32b-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 29.</span><span class="sxs-lookup"><span data-stu-id="3c32b-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="3c32b-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.45.98 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Φεβρουάριο 2021.</span><span class="sxs-lookup"><span data-stu-id="3c32b-110">This version has a build number of V3.10.45.98 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="3c32b-111">Έκδοση κυκλοφορίας 29</span><span class="sxs-lookup"><span data-stu-id="3c32b-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="3c32b-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="3c32b-112">Bug fixes</span></span>

<span data-ttu-id="3c32b-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="3c32b-113">**Time and Expense**</span></span>

<span data-ttu-id="3c32b-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="3c32b-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="3c32b-115">Οι χρήστες δεν μπορούν να δουν τις ώρες εργασίας που καταγράφονται σε μη εργάσιμες ημέρες στο πλέγμα καταχώρησης χρόνου.</span><span class="sxs-lookup"><span data-stu-id="3c32b-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="3c32b-116">Η επεξεργασία των εγκεκριμένων καταχωρήσεων δαπανών μπορεί να γίνει στο πλέγμα.</span><span class="sxs-lookup"><span data-stu-id="3c32b-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="3c32b-117">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="3c32b-117">**Project Management**</span></span>

<span data-ttu-id="3c32b-118">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="3c32b-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="3c32b-119">Η λογική επικύρωσης που λείπει για να διασφαλιστεί ότι οι ώρες προσπάθειας ανάθεσης πόρου δεν μπορούν να είναι αρνητικές.</span><span class="sxs-lookup"><span data-stu-id="3c32b-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="3c32b-120">Η προσαρμοσμένη ενέργεια, **AssignResourcesForTask** ενημερώνει όλα τα πεδία αντί μόνο τα αλλαγμένα πεδία.</span><span class="sxs-lookup"><span data-stu-id="3c32b-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="3c32b-121">Όταν αντιγράφετε ένα έργο σε ένα περιβάλλον με προσθήκες ή ροές εργασίας που είναι καταχωρημένες στο συμβάν **CreateProject**, το χαρακτηριστικό **msdyn_bulkgenerationstatus** δεν ενημερώνεται εάν το **CopyWBSToProject** αποτύχει.</span><span class="sxs-lookup"><span data-stu-id="3c32b-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="3c32b-122">Όταν αναπτύσσετε το ημερολόγιο έργου, οι ημέρες εργασίας δεν ταξινομούνται σε αύξουσα σειρά, με αποτέλεσμα ορισμένες ενημερώσεις εργασιών έργου να αποτυγχάνουν.</span><span class="sxs-lookup"><span data-stu-id="3c32b-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="3c32b-123">Η αλλαγή του Διαχειριστή έργου σε ένα υπάρχον έργο ενεργοποιεί τη λογική προεπιλογής της οργανωτικής μονάδας.</span><span class="sxs-lookup"><span data-stu-id="3c32b-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="3c32b-124">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="3c32b-124">**Sales**</span></span>

<span data-ttu-id="3c32b-125">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="3c32b-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="3c32b-126">Η καρτέλα **Επιδόσεις σύμβασης** στη σελίδα **Σύμβαση** αποτυγχάνει αθόρυβα κατά την προετοιμασία, όταν δεν υπάρχουν γραμμές σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="3c32b-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>
