---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 14, V3
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το τι νέο υπάρχει Project Service Automation, έκδοση ενημέρωσης 14, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: 8754f8eace50f1fa5743c5611d94f8c86693ebc9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006871"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="fced8-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 14, V3</span><span class="sxs-lookup"><span data-stu-id="fced8-103">Project Service Automation Update Release 14, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fced8-104">Είμαστε στην ευχάριστη θέση να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="fced8-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="fced8-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="fced8-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="fced8-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="fced8-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="fced8-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online και μεταβείτε στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="fced8-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="fced8-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="fced8-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="fced8-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το PSA V3, έκδοση ενημέρωσης 14.</span><span class="sxs-lookup"><span data-stu-id="fced8-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="fced8-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.4.21 και είναι διαθέσιμη σύμφωνα με το παρακάτω χρονοδιάγραμμα:</span><span class="sxs-lookup"><span data-stu-id="fced8-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="fced8-111">**Γενική διαθεσιμότητα (αυτοενημέρωση):** Ιανουάριος 2020</span><span class="sxs-lookup"><span data-stu-id="fced8-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="fced8-112">**Αυτόματη ενημέρωση:** Φεβρουάριος 2020</span><span class="sxs-lookup"><span data-stu-id="fced8-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="fced8-113">Έκδοση κυκλοφορίας 14</span><span class="sxs-lookup"><span data-stu-id="fced8-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="fced8-114">Βελτιώσεις</span><span class="sxs-lookup"><span data-stu-id="fced8-114">Enhancements</span></span>

- <span data-ttu-id="fced8-115">Sales</span><span class="sxs-lookup"><span data-stu-id="fced8-115">Sales</span></span>

     - <span data-ttu-id="fced8-116">Οι τιμές προσαρμοσμένων πεδίων από τις **Λεπτομέρειες σειράς προσφοράς** αντιγράφονται στις **Λεπτομέρειες της γραμμής σύμβασης έργου** όταν μια προσφορά ενημερώνεται σε **Κλειστή ως κερδισμένη**.</span><span class="sxs-lookup"><span data-stu-id="fced8-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="fced8-117">Τα επιβεβαιωμένα έργα μπορούν να **κλείσουν ως χαμένα**.</span><span class="sxs-lookup"><span data-stu-id="fced8-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="fced8-118">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="fced8-118">Resource Management</span></span>

     - <span data-ttu-id="fced8-119">Κατά την επέκταση των κρατήσεων, θα εμφανιστεί στους χρήστες ένα παράθυρο διαλόγου επιβεβαίωσης για να συνοψίσουν τα αποτελέσματα της κράτησης και να παράσχουν μια σύνδεση για Διατήρηση κρατήσεων.</span><span class="sxs-lookup"><span data-stu-id="fced8-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="fced8-120">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="fced8-120">Bug fixes</span></span>

- <span data-ttu-id="fced8-121">Χρόνος και έξοδα</span><span class="sxs-lookup"><span data-stu-id="fced8-121">Time and Expense</span></span>

     - <span data-ttu-id="fced8-122">Διορθώθηκε: Βελτιώθηκε η εμπειρία χρήστη, όταν ο χρήστης δεν έχει επιλέξει καμία καταχώρηση προς διόρθωση.</span><span class="sxs-lookup"><span data-stu-id="fced8-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="fced8-123">Διαχείριση πόρων</span><span class="sxs-lookup"><span data-stu-id="fced8-123">Resource Management</span></span>

     - <span data-ttu-id="fced8-124">Διορθώθηκε: Η κράτηση ενός πόρου πολλές φορές υπερχειλίζει το όνομα του πόρου με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="fced8-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="fced8-125">Sales</span><span class="sxs-lookup"><span data-stu-id="fced8-125">Sales</span></span>

     - <span data-ttu-id="fced8-126">Διορθώθηκε: Η συνολική τιμή πώλησης δεν υπολογίζεται μέχρι ο χρήστης να εισαγάγει επίσης μια τιμή κόστους για τις εκτιμήσεις εξόδων σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="fced8-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="fced8-127">Διορθώθηκε: Το κλείσιμο μιας προσφοράς **Κερδισμένης** αποτυγχάνει εάν η συσχετισμένη σύμβαση έργου δεν βρίσκεται σε κατάσταση **προσχεδίου**.</span><span class="sxs-lookup"><span data-stu-id="fced8-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]