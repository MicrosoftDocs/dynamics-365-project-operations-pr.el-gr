---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 19, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 19, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: e116bcbb8e9d184b7b894709c893aaf1dadefc2f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126842"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="f8fd1-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 19, V3</span><span class="sxs-lookup"><span data-stu-id="f8fd1-103">Project Service Automation Update Release 19, V3</span></span>

<span data-ttu-id="f8fd1-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f8fd1-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f8fd1-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f8fd1-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="f8fd1-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f8fd1-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f8fd1-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το PSA V3, έκδοση ενημέρωσης 19.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="f8fd1-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.30.41 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Μαΐου 2020.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="f8fd1-111">Έκδοση κυκλοφορίας 19</span><span class="sxs-lookup"><span data-stu-id="f8fd1-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f8fd1-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="f8fd1-112">Bug fixes</span></span>

<span data-ttu-id="f8fd1-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="f8fd1-113">**Time and Expense**</span></span>

<span data-ttu-id="f8fd1-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="f8fd1-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="f8fd1-115">Τα σφάλματα που προέκυψαν από τις εισαγωγές χρονικών καταχωρήσεων δεν εμφανίζονται σωστά.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="f8fd1-116">Το πλέγμα χρονικής καταχώρησης δεν υποστηρίζει τη συμπεριφορά πεδίου **Μόνο ημερομηνία**.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="f8fd1-117">Οι πόροι έργου δεν είναι δυνατό να δημιουργήσουν ένα έξοδο με ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="f8fd1-118">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="f8fd1-118">**Project Management**</span></span>

<span data-ttu-id="f8fd1-119">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="f8fd1-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="f8fd1-120">Η θυγατρική εργασία δεύτερου επιπέδου προκαλεί μια λανθασμένη εκτίμηση προσπάθειας κατά τη διάρκεια του υπολογισμού ολοκλήρωσης (ΕΚΟ).</span><span class="sxs-lookup"><span data-stu-id="f8fd1-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="f8fd1-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="f8fd1-121">**Sales**</span></span>

<span data-ttu-id="f8fd1-122">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="f8fd1-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="f8fd1-123">Η ενέργεια **Επανάληψης υπολογισμού** δεν λειτουργεί με τις λεπτομέρειες γραμμής σύμβασης εξόδων ή τις λεπτομέρειες γραμμής προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="f8fd1-124">Η **Ενημέρωση τιμών** λείπει για τις εκτιμήσεις εξόδων.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="f8fd1-125">Οι πελάτες δεν μπορούν να επιλέξουν προσαρμοσμένες αιτιολογίες κατάστασης σύμβασης από τη σελίδα **Σύμβαση έργου**.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="f8fd1-126">Οι πελάτες αντιμετωπίζουν υποβαθμισμένη απόδοση κατά τη δημιουργία ενός προσαρμοσμένου τιμοκαταλόγου από μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="f8fd1-127">Οι πελάτες αντιμετωπίζουν ασυνέπεια με τις προεπιλογές **μονάδων** στις σελίδες **λεπτομερειών γραμμής προσφοράς** και **λεπτομερειών γραμμής σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="f8fd1-128">Η προσθήκη στοιχείων κατηγορία μη χρεώσιμης συναλλαγής σε μια χρεώσιμη γραμμή σύμβασης δεν θα σεβαστεί τον τύπο χρέωσης **μη χρεώσιμη** της κατηγορίας συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="f8fd1-129">Οι πελάτες δεν μπορούν να χρησιμοποιήσουν τους ρόλους και την κατηγορία που προστέθηκαν πρόσφατα στις συμβάσεις που δημιουργήθηκαν ήδη.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="f8fd1-130">Οι πελάτες βιώνουν την υποβαθμισμένη απόδοση μη αναγκαίας ανάκτησης στο PreValidateProjectTeamMemberUpdate.cs</span><span class="sxs-lookup"><span data-stu-id="f8fd1-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="f8fd1-131">Οι ρόλοι που έχουν ρυθμιστεί ως μη χρεώσιμοι στη λίστα **Κατηγορίες πόρων** πρέπει να προστεθούν στην καρτέλα **Χρεώσιμοι ρόλοι** ως **Μη χρεώσιμοι** στη γραμμή σύμβασης ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="f8fd1-132">Οι πελάτες ενδέχεται να αντιμετωπίσουν υποβαθμισμένη απόδοση κατά τη δημιουργία ενός έργου, επειδή το **GetBookableResourceIdFromUser** ανακτά όλες τις στήλες των πόρων με δυνατότητα κράτησης και όχι μόνο το κύριο αναγνωριστικό.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="f8fd1-133">Από την οντότητα **TransactionType** λείπει η προσθήκη ενημέρωσης προ-επικύρωσης για να αποτραπούν οι χρήστες από το να εισαγάγουν **Μονάδες** και **UnitGroups** που δεν είναι έγκυρα για τους τύπους συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="f8fd1-134">Το βήμα **Κατάργηση** δεν λειτουργεί για την εισαγωγή χρονικής καταχώρησης.</span><span class="sxs-lookup"><span data-stu-id="f8fd1-134">The **Remove** step does not work for time entry import.</span></span>
