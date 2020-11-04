---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 12, V3
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το τι νέο υπάρχει Project Service Automation, έκδοση ενημέρωσης 12, V3.
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
ms.openlocfilehash: 62c3a0c5cfbecb568faef570da309c20afd86de9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076877"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="9f8ab-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 12, V3</span><span class="sxs-lookup"><span data-stu-id="9f8ab-103">Project Service Automation Update Release 12, V3</span></span>
<span data-ttu-id="9f8ab-104">Είμαστε στην ευχάριστη θέση να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="9f8ab-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="9f8ab-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9f8ab-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9f8ab-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online και μεταβείτε στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="9f8ab-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9f8ab-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9f8ab-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 12.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="9f8ab-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.2.34 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Οκτώβριο του 2019.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="9f8ab-111">Έκδοση κυκλοφορίας 12</span><span class="sxs-lookup"><span data-stu-id="9f8ab-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9f8ab-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="9f8ab-112">Bug fixes</span></span>

- <span data-ttu-id="9f8ab-113">Χρόνος και έξοδα</span><span class="sxs-lookup"><span data-stu-id="9f8ab-113">Time and Expense</span></span>

    - <span data-ttu-id="9f8ab-114">Διορθώθηκε: Η ανταλλαγή μηνυμάτων για σφάλματα χρονικής καταχώρησης έχει ενημερωθεί με πιο σχετικό περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="9f8ab-115">Διορθώθηκε: Το πλέγμα και το χρονοδιάγραμμα χρονικής καταχώρησης ώρας εμφανίζουν σωστά την κατακόρυφη γραμμή κύλισης, όταν απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="9f8ab-116">Διορθώθηκε: Είναι δυνατή η έγκριση καταχωρήσεων χρόνου ή εξόδων που έχουν υποβληθεί.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="9f8ab-117">Διορθώθηκε: Η ακύρωση του μηνύματος του παραθύρου διαλόγου επιβεβαίωσης έγκρισης διορθώθηκε, για να αντικατοπτρίζει την κατάσταση της έγκρισης όταν αλλάζει **Εγκρίθηκε** σε **Υποβλήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="9f8ab-118">Διορθώθηκε: Τα πεδία **Τιμή** , **Μονάδα** και **Ποιότητα** είναι πλέον κλειδωμένα στην καρτέλα εξόδων μετά την έγκρισή της.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-118">Fixed: **Price** , **Unit** , and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="9f8ab-119">Διαχείριση έργων</span><span class="sxs-lookup"><span data-stu-id="9f8ab-119">Project Management</span></span>

    - <span data-ttu-id="9f8ab-120">Διορθώθηκε: Καταργήθηκε η ενέργεια **Νέο** στην κύρια φόρμα  **Μέλους ομάδας**.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="9f8ab-121">Διορθώθηκε: Οι αναθέσεις πόρων έχουν ενημερωθεί για να αιτιολογήσουν σφάλματα ανακριβούς στρογγυλοποίησης, τα οποία οδηγούν σε μετατόπιση της ημερομηνίας λήξης μιας εργασίας.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="9f8ab-122">Διορθώθηκε: Στο πλέγμα εργασιών, τα σχετικά σφάλματα από την πλευρά του διακομιστή θα εμφανίζονται στον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="9f8ab-123">Διορθώθηκε: Το όνομα του μέλους της ομάδας αποδίδεται πλέον στον επιλογέα ατόμων για εργασία αντί για το όνομα θέσης.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="9f8ab-124">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="9f8ab-124">Resource Management</span></span>

    - <span data-ttu-id="9f8ab-125">Διορθώθηκε: Οι λεπτομέρειες απαίτησης πόρου για έργα που δημιουργούνται από ένα πρότυπο χρησιμοποιούν πλέον το ημερολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="9f8ab-126">Διορθώθηκε: Οι δεξιότητες και οι ικανότητες ορίζονται πλέον από προεπιλογή από τα δεδομένα βασικού ρόλου στην απαίτηση πόρου που δημιουργείται για αυτόν τον ρόλο.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="9f8ab-127">Sales</span><span class="sxs-lookup"><span data-stu-id="9f8ab-127">Sales</span></span>

    - <span data-ttu-id="9f8ab-128">Διορθώθηκε: Διπλότυπα αναγνωριστικά αντικειμένου βρέθηκαν στην κύρια φόρμα **σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="9f8ab-129">Διορθώθηκε: Η λογική ενημερώθηκε για να είναι ορατή η καρτέλα **Ανάλυση προσφοράς** , ούτως ώστε να εμφανίζει τη ρύθμιση μετα-δεδομένων της καρτέλας.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="9f8ab-130">Διορθώθηκε: Η ημερομηνία λογιστικής στην πραγματική καρτέλα προέρχεται πλέον από την ημερομηνία της ημερομηνίας καταχώρησης χρόνου/εξόδων και όχι την ημερομηνία έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="9f8ab-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>
