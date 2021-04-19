---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 30, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 30, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 1169ee13c42e982cb30a40d92df660f8933786a9
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852855"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="d5b29-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 30, V3</span><span class="sxs-lookup"><span data-stu-id="d5b29-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d5b29-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="d5b29-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="d5b29-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="d5b29-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d5b29-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="d5b29-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d5b29-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="d5b29-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="d5b29-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="d5b29-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d5b29-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 30.</span><span class="sxs-lookup"><span data-stu-id="d5b29-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="d5b29-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.51.61 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Απριλίου 2021.</span><span class="sxs-lookup"><span data-stu-id="d5b29-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="d5b29-111">Έκδοση κυκλοφορίας 30</span><span class="sxs-lookup"><span data-stu-id="d5b29-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="d5b29-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="d5b29-112">Bug fixes</span></span>

<span data-ttu-id="d5b29-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="d5b29-113">**Time and Expense**</span></span>

<span data-ttu-id="d5b29-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="d5b29-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="d5b29-115">Παρουσιάζεται σφάλμα κατά τη δημιουργία και την αποθήκευση μιας καταχώρησης χρόνου στη σελίδα **Γρήγορη δημιουργία** εάν καταργηθεί το πεδίο **Ρόλος**.</span><span class="sxs-lookup"><span data-stu-id="d5b29-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="d5b29-116">Το φίλτρο εγγραφής χρόνου εφαρμόζει εσφαλμένο τελεστή φίλτρου.</span><span class="sxs-lookup"><span data-stu-id="d5b29-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="d5b29-117">Τα αντίγραφα φύλλων χρόνου δεν εμφανίζονται αυτόματα, όταν επιλέγετε **Αντιγραφή εβδομάδας** στο στοιχείο ελέγχου εγγραφής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="d5b29-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="d5b29-118">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="d5b29-118">**Resource Management**</span></span>

<span data-ttu-id="d5b29-119">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="d5b29-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="d5b29-120">Όταν επεκτείνετε μια κράτηση, η κατάσταση κράτησης που έχει εκχωρηθεί στην οριστική κράτηση είναι εσφαλμένη.</span><span class="sxs-lookup"><span data-stu-id="d5b29-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="d5b29-121">Η επέκταση μιας κράτησης σέβεται την κατάσταση κράτησης που ορίζεται ως **Δεσμευμένη** στα μετα-δεδομένα εγκατάστασης της κράτησης.</span><span class="sxs-lookup"><span data-stu-id="d5b29-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="d5b29-122">Όταν δεν καθορίζεται έγκυρη κατάσταση κράτησης, το μήνυμα σφάλματος δεν είναι σωστά μεταφρασμένο.</span><span class="sxs-lookup"><span data-stu-id="d5b29-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="d5b29-123">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="d5b29-123">**Project Management**</span></span>

<span data-ttu-id="d5b29-124">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="d5b29-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="d5b29-125">Τα έργα δεν είναι δυνατό να δημιουργηθούν σε μία νομισματική μονάδα και να συμπεριλάβουν σχετικές εργασίες σε άλλη νομισματική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="d5b29-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="d5b29-126">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="d5b29-126">**Sales**</span></span>

<span data-ttu-id="d5b29-127">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="d5b29-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="d5b29-128">Όταν αντιγράφεται ένας τιμοκατάλογος, οι τιμές δεν ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="d5b29-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="d5b29-129">Το κλείσιμο μιας προσφοράς ως κερδισμένης αποτυγχάνει όταν η λεπτομέρεια κόστους έχει μια τιμή για την προέλευση.</span><span class="sxs-lookup"><span data-stu-id="d5b29-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="d5b29-130">Στην οντότητα **Εργασία έργου**, το **Εκτιμώμενο κόστος** έχει μετονομαστεί σε **Προγραμματισμένο κόστος (Βάση)**.</span><span class="sxs-lookup"><span data-stu-id="d5b29-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="d5b29-131">Όταν δημιουργούνται ή διαγράφονται τιμολόγια, δημιουργείται μια εξαίρεση αναφοράς null.</span><span class="sxs-lookup"><span data-stu-id="d5b29-131">A null reference exception is generated when invoices are created or deleted.</span></span>
