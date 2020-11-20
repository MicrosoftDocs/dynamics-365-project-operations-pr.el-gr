---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 16, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 16, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 2c93d34b61001b7755d426539ac384641a7bc9da
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121578"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="db310-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 16, V3</span><span class="sxs-lookup"><span data-stu-id="db310-103">Project Service Automation Update Release 16, V3</span></span>

<span data-ttu-id="db310-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="db310-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="db310-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="db310-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="db310-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="db310-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="db310-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="db310-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="db310-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση μιας προτιμώμενης λύσης](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span><span class="sxs-lookup"><span data-stu-id="db310-108">For more information, see [Install, Update a Preferred Solution](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="db310-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το PSA V3, έκδοση ενημέρωσης 16.</span><span class="sxs-lookup"><span data-stu-id="db310-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="db310-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.6.34 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Ιανουάριο του 2020.</span><span class="sxs-lookup"><span data-stu-id="db310-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="db310-111">Έκδοση κυκλοφορίας 16</span><span class="sxs-lookup"><span data-stu-id="db310-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="db310-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="db310-112">Bug fixes</span></span>

-   <span data-ttu-id="db310-113">Χρόνος και έξοδα</span><span class="sxs-lookup"><span data-stu-id="db310-113">Time and Expense</span></span>

    -   <span data-ttu-id="db310-114">Διόρθωση: οι χρήστες που επιχειρούν να υποβάλουν διαγραμμένες καταχωρήσεις ώρας και εξόδων για εγκρίσεις, θα λάβουν πλέον σχετικά μηνύματα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="db310-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="db310-115">Διαχείριση έργων</span><span class="sxs-lookup"><span data-stu-id="db310-115">Project Management</span></span>

    -   <span data-ttu-id="db310-116">Διόρθωση: οι μονάδες νέου εφοδιασμού που καθορίζονται για τα μέλη της ομάδας σε πρότυπα τηρούνται με τα πρότυπα που εφαρμόζονται σε ένα νέο έργο.</span><span class="sxs-lookup"><span data-stu-id="db310-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="db310-117">Διόρθωση: βελτιωμένη διαχείριση της εκ νέου εκχώρησης της κυριότητας καρτέλας.</span><span class="sxs-lookup"><span data-stu-id="db310-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="db310-118">Διόρθωση: τα έργα που βρίσκονται σε διεργασία αντιγραφής δεν θα επιτρέπεται να αντιγραφούν μέχρι να ολοκληρωθούν όλες οι λειτουργίες αντιγραφής.</span><span class="sxs-lookup"><span data-stu-id="db310-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="db310-119">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="db310-119">Resource Management</span></span>

    -   <span data-ttu-id="db310-120">Διόρθωση: η επέκταση των κρατήσεων πλέον χειρίζεται τις σύντομες διάρκειες σωστά και δεν δημιουργεί πλέον ώρες μηδέν για τις εκτεταμένες κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="db310-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="db310-121">Διόρθωση: η προβολή συμφιλίωσης αποδίδει πλέον όταν η ζώνη ώρας του έργου είναι + 5:30 GMT και η ώρα του χρήστη μόνο είναι διαφορετική.</span><span class="sxs-lookup"><span data-stu-id="db310-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="db310-122">Sales</span><span class="sxs-lookup"><span data-stu-id="db310-122">Sales</span></span>

    -   <span data-ttu-id="db310-123">Διόρθωση: όταν ένα έργο που αντιστοιχίζεται σε μια γραμμή σύμβασης καταργηθεί και έχει αντιστοιχιστεί ένα νέο έργο, οι πραγματικές καρτέλες στο νέο έργο δεν αξιολογήθηκαν εκ νέου με βάση τους κανόνες χρέωσης και τιμολόγησης που καθορίζονται στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="db310-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="db310-124">Αυτό διορθώθηκε σε αυτήν την έκδοση.</span><span class="sxs-lookup"><span data-stu-id="db310-124">This has been fixed in this release.</span></span> <span data-ttu-id="db310-125">Η τιμολόγηση και οι πραγματικές καρτέλες στο πρόσφατα αντιστοιχισμένο έργο θα αντιστραφούν και θα δημιουργηθούν εκ νέου σωστά με βάση τους κανόνες τιμολόγησης και χρέωσης της γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="db310-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="db310-126">Οι πραγματικές καρτέλες του έργου που δεν έχει αντιστοιχιστεί θα αξιολογηθούν εκ νέου και θα δημιουργηθούν εκ νέου ως συνέπεια.</span><span class="sxs-lookup"><span data-stu-id="db310-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="db310-127">Διόρθωση: έχει προστεθεί πρόσθετη επικύρωση στο πεδίο **Ποσό** μιας γραμμής εκτίμησης, για να διασφαλιστεί ότι οι τιμές null δεν θα παραμείνουν σταθερές.</span><span class="sxs-lookup"><span data-stu-id="db310-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="db310-128">Διόρθωση: όταν οι πραγματικές τιμές ενημερωθούν σε ένα έργο, ένα κουμπί ανανέωσης έχει προστεθεί στην κύρια φόρμα του έργου ώστε να επιτρέπεται στους χρήστες ο εκ νέου συγχρονισμός των πραγματικών τιμών.</span><span class="sxs-lookup"><span data-stu-id="db310-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="db310-129">Διόρθωση: όταν οι χρήστες κάνουν αναβάθμιση από 2. X σε 3. X, θα επιτρέπονται έργα με τιμή NULL για το όνομα του έργου.</span><span class="sxs-lookup"><span data-stu-id="db310-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>

