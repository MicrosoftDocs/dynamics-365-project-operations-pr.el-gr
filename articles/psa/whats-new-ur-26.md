---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 26, V3
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643263"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="12c98-102">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 26, V3</span><span class="sxs-lookup"><span data-stu-id="12c98-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="12c98-103">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="12c98-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="12c98-104">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="12c98-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="12c98-105">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="12c98-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="12c98-106">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="12c98-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="12c98-107">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="12c98-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="12c98-108">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 26, V3.</span><span class="sxs-lookup"><span data-stu-id="12c98-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="12c98-109">Αυτή η έκδοση έχει αριθμό δομής V 3.10.44.59 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Δεκέμβριο 2020.</span><span class="sxs-lookup"><span data-stu-id="12c98-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="12c98-110">Έκδοση κυκλοφορίας 26</span><span class="sxs-lookup"><span data-stu-id="12c98-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="12c98-111">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="12c98-111">Bug fixes</span></span>

<span data-ttu-id="12c98-112">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="12c98-112">**Time and Expense**</span></span>

<span data-ttu-id="12c98-113">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="12c98-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="12c98-114">Οι χρήστες μπορούν να αλλάξουν την εργασία σε μια καταχώρηση ώρας που έχει εγκριθεί/υποβληθεί.</span><span class="sxs-lookup"><span data-stu-id="12c98-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="12c98-115">Εμφανίζεται το μήνυμα «Δεν έχει οριστεί αναφορά αντικειμένου» κατά την αποθήκευση της καταχώρησης ώρας.</span><span class="sxs-lookup"><span data-stu-id="12c98-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="12c98-116">Η εισαγωγή καταχώρησης ώρας από αναθέσεις πόρων δημιουργεί καταχωρήσεις ώρας με εσφαλμένες τιμές ημερομηνίας και ώρας.</span><span class="sxs-lookup"><span data-stu-id="12c98-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="12c98-117">Όταν εγκατασταθούν και το Project Service Automation και η εφαρμογή Field Service, το κουμπί **Νέο** εμφανίζεται δύο φορές στη γραμμή εντολών για καταχωρήσεις ώρας στην εφαρμογή Field Service.</span><span class="sxs-lookup"><span data-stu-id="12c98-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="12c98-118">Οι ενημερώσεις κελιών **Να επιτρέπεται η μονάδα** και **Ομάδα μονάδων** λειτουργούν πλέον στο πλέγμα **Εκτιμήσεις εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="12c98-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="12c98-119">Η φόρμα **Ενημέρωση επεξεργασίας καταχώρησης ώρας** περιλαμβάνει **Λωρίδα χρόνου**.</span><span class="sxs-lookup"><span data-stu-id="12c98-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="12c98-120">Η έγκριση ώρας για καταχωρήσεις ώρας εκτός έργου αποκλείει το σύστημα κατά την αναζήτηση ενός ρόλου υπεύθυνου έγκρισης έργου.</span><span class="sxs-lookup"><span data-stu-id="12c98-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="12c98-121">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="12c98-121">**Resource Management**</span></span>

<span data-ttu-id="12c98-122">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="12c98-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="12c98-123">Προστέθηκε επικύρωση στην προσθήκη **PostProjectCreate** για τον έλεγχο για μια κύρια απαίτηση πριν από τη δημιουργία μίας.</span><span class="sxs-lookup"><span data-stu-id="12c98-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="12c98-124">Η φόρμα γρήγορης δημιουεγίας **Μέλος ομάδας έργου** παρουσιάζει μια εξαίρεση αναφοράς null εάν τα πεδία καταργηθούν από τη φόρμα.</span><span class="sxs-lookup"><span data-stu-id="12c98-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="12c98-125">Η δημιουργία απαιτήσεων για 12 ώρες πάνω από 1 έτος θα αποτύχει.</span><span class="sxs-lookup"><span data-stu-id="12c98-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="12c98-126">Βελτιωμένη εξαίρεση αναφοράς null μηνύματος σφάλματος κατά τη διάρκεια της δημιουργίας απαίτησης πόρου.</span><span class="sxs-lookup"><span data-stu-id="12c98-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="12c98-127">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="12c98-127">**Project Management**</span></span>

<span data-ttu-id="12c98-128">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="12c98-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="12c98-129">Βελτιωμένη επικύρωση για την αντιμετώπιση της εξαίρεσης αναφοράς null που δημιουργείται στην προσθήκη **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="12c98-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="12c98-130">Τα έργα που δημοσιεύονται από το πρόσθετο Microsoft Project Desktop διαγράφουν τις μη αντιστοιχισμένες αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="12c98-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="12c98-131">Προστέθηκε νέα επικύρωση όταν η αναφορά έργου μιας εργασίας δεν είναι έγκυρη λόγω εξαίρεσης αναφοράς null στο πρόσθετο **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="12c98-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="12c98-132">Το πλέγμα μελών ομάδας δεν εμφανίζει διακριτές αναθέσεις στην καρτέλα μέλους ομάδας.</span><span class="sxs-lookup"><span data-stu-id="12c98-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="12c98-133">Προσθήκη νέων επικυρώσεων και μηνυμάτων σφάλματος λόγω εξαίρεσης αναφοράς null στο πρόσθετο **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="12c98-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="12c98-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="12c98-134">**Sales**</span></span>

<span data-ttu-id="12c98-135">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="12c98-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="12c98-136">Όταν επιλέγετε μια γραμμή βάσει έργου σε μια προσφορά ή μια σύμβαση, το κουμπί **Πρόταση** θα πρέπει να είναι ορατό μόνο όταν επιλέγετε μια γραμμή βασισμένη σε προϊόντα που σχετίζεται με ένα υπάρχον προϊόν.</span><span class="sxs-lookup"><span data-stu-id="12c98-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="12c98-137">Διαίρεση του προνομίου **Create_Product** από το προνόμιο **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="12c98-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="12c98-138">Η διαγραφή μιας γραμμής τιμολογίου προκαλεί αποτυχία αναφοράς null στο **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="12c98-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
