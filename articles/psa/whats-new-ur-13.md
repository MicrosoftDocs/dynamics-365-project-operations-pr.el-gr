---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 13, V3
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το τι νέο υπάρχει Project Service Automation, έκδοση ενημέρωσης 13, V3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 435b70255dd0053a496362c9ced9e742cfcca843
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076876"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="e6c5b-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 13, V3</span><span class="sxs-lookup"><span data-stu-id="e6c5b-103">Project Service Automation Update Release 13, V3</span></span>
<span data-ttu-id="e6c5b-104">Είμαστε στην ευχάριστη θέση να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="e6c5b-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="e6c5b-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="e6c5b-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="e6c5b-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online και μεταβείτε στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="e6c5b-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="e6c5b-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="e6c5b-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 13.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="e6c5b-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.3.18 και είναι διαθέσιμη σύμφωνα με το παρακάτω χρονοδιάγραμμα:</span><span class="sxs-lookup"><span data-stu-id="e6c5b-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="e6c5b-111">**Γενική διαθεσιμότητα (αυτοενημέρωση):** Νοέμβριος 2019</span><span class="sxs-lookup"><span data-stu-id="e6c5b-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="e6c5b-112">**Αυτοενημέρωση:** Δεκέμβριος 2019</span><span class="sxs-lookup"><span data-stu-id="e6c5b-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="e6c5b-113">Έκδοση κυκλοφορίας 13</span><span class="sxs-lookup"><span data-stu-id="e6c5b-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="e6c5b-114">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="e6c5b-114">Bug fixes</span></span>

- <span data-ttu-id="e6c5b-115">Χρόνος και έξοδα</span><span class="sxs-lookup"><span data-stu-id="e6c5b-115">Time and Expense</span></span>

     - <span data-ttu-id="e6c5b-116">Διορθώθηκε: Η λειτουργικότητα αναζήτησης στη σελίδα **έγκρισης εξόδων** δεν λειτουργεί κατά την αναζήτηση με βάση τον σκοπό των εξόδων.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="e6c5b-117">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="e6c5b-117">Resource Management</span></span>

     - <span data-ttu-id="e6c5b-118">Διορθώθηκε: Οι αριθμοί που υπάρχουν στην εναρμόνιση έχουν ενημερωθεί ώστε να δικαιολογούνται σωστά.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="e6c5b-119">Διορθώθηκε: Οι πόροι με όνομα δεν είναι δυνατό να ανατεθούν σε εργασίες μέσω της καρτέλας **Χρονοδιάγραμμα**.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="e6c5b-120">Διαχείριση έργων</span><span class="sxs-lookup"><span data-stu-id="e6c5b-120">Project Management</span></span>

     - <span data-ttu-id="e6c5b-121">Διορθώθηκε: Μηδενική εξαίρεση αναφοράς κατά την ανάθεση σε ένα μέλος ομάδας όταν λείπου πληροφορίες ρύθμισης από το **TransactionType** για την **Μονάδα** και το **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="e6c5b-122">Sales</span><span class="sxs-lookup"><span data-stu-id="e6c5b-122">Sales</span></span>

     - <span data-ttu-id="e6c5b-123">Διορθώθηκε: Διπλότυπες καρτέλες τύπου συναλλαγής επιστρέφουν ένα σφάλμα κατά τη δημιουργία καρτελών τιμής ρόλου.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="e6c5b-124">Διορθώθηκε: Επιπλέον κουμπιά για **Νέα ευκαιρία** , **Προσφορά** , **Γραμμή παραγγελίας** και **Προσθήκη προϊόντος** εμφανίζονται στις εντολές για Ευκαιρίες, Προσφορές, Προϊόντα παραγγελίας και στο υποπλέγμα γραμμών βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="e6c5b-124">Fixed: Extra buttons for **New Opportunity** , **Quote** , **Order Line** , and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


