---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 23, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 23, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: 87f89828aeff22d9b473539e294d5cf04d46a203
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150038"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="bba6b-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 23, V3</span><span class="sxs-lookup"><span data-stu-id="bba6b-103">Project Service Automation Update Release 23, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="bba6b-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="bba6b-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="bba6b-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="bba6b-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="bba6b-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="bba6b-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="bba6b-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="bba6b-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="bba6b-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="bba6b-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="bba6b-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 23.</span><span class="sxs-lookup"><span data-stu-id="bba6b-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="bba6b-110">Αυτή η έκδοση έχει αριθμό δομής V 3.10.34.30 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Αύγουστο του 2020.</span><span class="sxs-lookup"><span data-stu-id="bba6b-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="bba6b-111">Έκδοση κυκλοφορίας 23</span><span class="sxs-lookup"><span data-stu-id="bba6b-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="bba6b-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="bba6b-112">Bug fixes</span></span>

<span data-ttu-id="bba6b-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="bba6b-113">**Time and Expense**</span></span>

<span data-ttu-id="bba6b-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="bba6b-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="bba6b-115">Χειρισμός της υπόθεσης άκρου στη **Διαγραφή μέλους ομάδας έργου** για την παροχή μιας ουσιαστικής εξαίρεσης.</span><span class="sxs-lookup"><span data-stu-id="bba6b-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="bba6b-116">Η εισαγωγή ανάθεσης έχει ως αποτέλεσμα μια κενή οθόνη κατάργησης.</span><span class="sxs-lookup"><span data-stu-id="bba6b-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="bba6b-117">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="bba6b-117">**Resource Management**</span></span>

<span data-ttu-id="bba6b-118">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="bba6b-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba6b-119">Η **Κάρτα πόρων πλέγματος χρήσης πόρου** εμφανίζει εσφαλμένα δεδομένα όταν η κλίμακα χρόνου είναι περισσότερο από πέντε ημέρες.</span><span class="sxs-lookup"><span data-stu-id="bba6b-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="bba6b-120">Όταν οι πελάτες δημιουργούν έναν πόρο με δυνατότητα κράτησης, η προσθήκη αποτυγχάνει κατά διαστήματα για την αυτόματη προσθήκη του πόρου σε μια ομάδα Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="bba6b-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="bba6b-121">Η προβολή **συμψηφισμού** εμφανίζει λανθασμένα τις μη αυτόματες καμπύλες στην προβολή **Εβδομάδα** ή **Μήνα**.</span><span class="sxs-lookup"><span data-stu-id="bba6b-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="bba6b-122">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="bba6b-122">**Project Management**</span></span>

<span data-ttu-id="bba6b-123">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="bba6b-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba6b-124">Ο υπερβολικός αριθμός των οντοτήτων **RetrieveMultiple για ρυθμίσεις χρηστών** προκαλεί υποβαθμισμένη απόδοση για εγκρίσεις έργου και άλλες λειτουργίες.</span><span class="sxs-lookup"><span data-stu-id="bba6b-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="bba6b-125">Η αναζήτηση πόρου πλέγματος **Σχεδιασμού εργασιών** περιορίζεται μόνο σε πέντε μέλη ομάδας από την ομάδα έργου.</span><span class="sxs-lookup"><span data-stu-id="bba6b-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="bba6b-126">Η αναζήτηση πόρου πλέγματος **Σχεδιασμού εργασιών** δεν φιλτράρει τους ανενεργούς πόρους.</span><span class="sxs-lookup"><span data-stu-id="bba6b-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="bba6b-127">Η χειροκίνητη λειτουργία δεν λειτουργεί όπως αναμενόταν στη δομή ανάλυσης εργασίας σχεδιασμού έργου.</span><span class="sxs-lookup"><span data-stu-id="bba6b-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="bba6b-128">Το πλέγμα **Σχεδιασμού εργασιών** εμφανίζει **Κατηγορίες ανενεργών κινήσεων**.</span><span class="sxs-lookup"><span data-stu-id="bba6b-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="bba6b-129">Το πλέγμα **Ανάθεσης πόρου** στρογγυλοποιεί εσφαλμένα όταν μια εργασία έχει πολλές αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="bba6b-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="bba6b-130">Οι τιμές στρογγυλοποίησης διαφέρουν μεταξύ του προγραμματισμένου κόστους και του πραγματικού κόστους μιας μεμονωμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="bba6b-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="bba6b-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="bba6b-131">**Sales**</span></span>

<span data-ttu-id="bba6b-132">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="bba6b-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="bba6b-133">Το διπλό κλικ στην επιλογή **Λήψη όλων των κατηγοριών συναλλαγών** δημιουργεί πολλές γραμμές.</span><span class="sxs-lookup"><span data-stu-id="bba6b-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>
