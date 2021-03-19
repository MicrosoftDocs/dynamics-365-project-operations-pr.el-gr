---
title: Ρύθμιση παραμέτρων κατηγοριών έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη ρύθμιση των παραμέτρων των κατηγοριών έργου.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b7adf61a82714a0148d9c8b1d2b2b37fd611c1cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287508"
---
# <a name="configure-project-categories"></a><span data-ttu-id="167cf-103">Ρύθμιση παραμέτρων κατηγοριών έργου</span><span class="sxs-lookup"><span data-stu-id="167cf-103">Configure project categories</span></span>

<span data-ttu-id="167cf-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="167cf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="167cf-105">Το Project Operations προσφέρει ισχυρές δυνατότητες για την κατηγοριοποίηση των εσόδων και των δαπανών σε έργα.</span><span class="sxs-lookup"><span data-stu-id="167cf-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="167cf-106">Οι κατηγορίες παρέχουν τη δυνατότητα αναφοράς και ανάλυσης συναλλαγών έργου, καθώς και τη δυνατότητα καταχώρησης στη γενική λογιστική.</span><span class="sxs-lookup"><span data-stu-id="167cf-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="167cf-107">Στο ακόλουθο διάγραμμα απεικονίζεται ο συσχετισμός ανάμεσα σε κατηγορίες συναλλαγών, κοινόχρηστες κατηγορίες και κατηγορίες έργων.</span><span class="sxs-lookup"><span data-stu-id="167cf-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="167cf-108">Οι κατηγορίες συναλλαγών είναι η βασική ομαδοποίηση για τις συναλλαγές έργου.</span><span class="sxs-lookup"><span data-stu-id="167cf-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="167cf-109">Στο πλαίσιο της εν λόγω ομαδοποίησης, υπάρχει ένα σύνολο κοινόχρηστων κατηγοριών που μπορεί να χρησιμοποιηθεί από κοινού σε όλες τις εφαρμογές και τις λειτουργικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="167cf-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="167cf-110">Ακόμα πιο αναλυτικά, οι κατηγορίες έργου είναι το πιο λεπτομερές επίπεδο κατηγοριών.</span><span class="sxs-lookup"><span data-stu-id="167cf-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="167cf-111">Οι κατηγορίες έργου αφορούν συγκεκριμένα τη νομική οντότητα, την ενότητα και την εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="167cf-111">Project categories are specific to legal entity, module, and application.</span></span>

![Η συσχέτιση ανάμεσα σε κατηγορίες συναλλαγών, κοινόχρηστες κατηγορίες και κατηγορίες έργων.](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="167cf-113">Κατηγορίες συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="167cf-113">Transaction categories</span></span>

<span data-ttu-id="167cf-114">Οι κατηγορίες συναλλαγών αντιπροσωπεύουν τη βασική ομαδοποίηση για τις συναλλαγές έργου και δεν είναι συγκεκριμένες για την εταιρεία ή για κάθε τύπο συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="167cf-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="167cf-115">Για παράδειγμα, η Contoso Robotics χρησιμοποιεί τις κατηγορίες συναλλαγών "Σχεδίαση", "Ταξίδια", "Εγκατάσταση" και "Εξυπηρέτηση" για να ομαδοποιήσει συναλλαγές έργου.</span><span class="sxs-lookup"><span data-stu-id="167cf-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="167cf-116">Οι κατηγορίες συναλλαγών καθορίζονται στη λειτουργική μονάδα του Project Operations.</span><span class="sxs-lookup"><span data-stu-id="167cf-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="167cf-117">Μεταβείτε στις **Ρυθμίσεις** \> **Κατηγορίες συναλλαγών** για να ανοίξετε τη φόρμα.</span><span class="sxs-lookup"><span data-stu-id="167cf-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="167cf-118">Δημιουργήστε μια νέα κατηγορία συναλλαγής είτε επιλέγοντας **Δημιουργία** είτε επιλέγοντας **Εισαγωγή από το Excel**.</span><span class="sxs-lookup"><span data-stu-id="167cf-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="167cf-119">Κοινόχρηστες κατηγορίες</span><span class="sxs-lookup"><span data-stu-id="167cf-119">Shared categories</span></span>

<span data-ttu-id="167cf-120">Το Dynamics 365 χρησιμοποιεί την έννοια των κοινόχρηστων κατηγοριών για την κατηγοριοποίηση των δαπανών σε διαφορετικές εφαρμογές, όπως οι Dynamics 365 Finance, Dynamics 365 Supply Chain και Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="167cf-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="167cf-121">Για κάθε κατηγορία συναλλαγής που δημιουργείται, το Project Operations δημιουργεί αυτόματα τέσσερις σχετικές κοινόχρηστες κατηγορίες: ώρες, δαπάνη, χρεώσεις και στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="167cf-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="167cf-122">Μπορείτε να εξετάσετε και να προσαρμόσετε τις κοινόχρηστες κατηγορίες μεταβαίνοντας στα στοιχεία **Διαχείριση έργου και λογιστική** \> **Ρύθμιση παραμέτρων** \> **Κατηγορίες** \> **Κοινόχρηστες κατηγορίες**.</span><span class="sxs-lookup"><span data-stu-id="167cf-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="167cf-123">Κατηγορίες έργου</span><span class="sxs-lookup"><span data-stu-id="167cf-123">Project categories</span></span>

<span data-ttu-id="167cf-124">Οι κατηγορίες έργου αντιπροσωπεύουν το πιο λεπτομερές επίπεδο ρύθμισης παραμέτρων κατηγορίας και πρέπει να ρυθμιστούν χωριστά και για κάθε εταιρεία από έναν λογιστή έργου.</span><span class="sxs-lookup"><span data-stu-id="167cf-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="167cf-125">Μεταβείτε στα στοιχεία **Διαχείριση έργου και λογιστική** \> **Ρύθμιση παραμέτρων** \> **Κατηγορίες** \> **Κατηγορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="167cf-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="167cf-126">Επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="167cf-126">Select **New**.</span></span>
3. <span data-ttu-id="167cf-127">Επιλέξτε το **Αναγνωριστικό κατηγορίας** της κοινόχρηστης κατηγορίας που δημιουργήσατε στην προηγούμενη ενότητα.</span><span class="sxs-lookup"><span data-stu-id="167cf-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="167cf-128">Το Project Operations επιτρέπει τη χρήση μόνο αυτών των κοινόχρηστων κατηγοριών που σχετίζονται με κατηγορίες συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="167cf-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="167cf-129">Επιλέξτε μια ομάδα κατηγοριών.</span><span class="sxs-lookup"><span data-stu-id="167cf-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="167cf-130">Ομάδες κατηγοριών</span><span class="sxs-lookup"><span data-stu-id="167cf-130">Category groups</span></span>

<span data-ttu-id="167cf-131">Οι ομάδες κατηγοριών χρησιμοποιούνται για την κοινοποίηση ιδιοτήτων, κυρίως για την καταχώρηση προφίλ, μεταξύ σχετικών κατηγοριών έργου.</span><span class="sxs-lookup"><span data-stu-id="167cf-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="167cf-132">Πρέπει να υπάρχει τουλάχιστον μία ομάδα κατηγοριών για κάθε τύπο συναλλαγής και σε κάθε κατηγορία έργου να έχει εκχωρηθεί μια ομάδα.</span><span class="sxs-lookup"><span data-stu-id="167cf-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="167cf-133">Οι προδιαγραφές καταχώρησης στο Project Operations ορίζονται από το προφίλ κόστους και τους κανόνες προφίλ εσόδων, τις κατηγορίες έργου και τις ομάδες κατηγοριών.</span><span class="sxs-lookup"><span data-stu-id="167cf-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="167cf-134">Μπορείτε να ορίσετε ομάδες κατηγοριών μεταβαίνοντας στα στοιχεία **Διαχείριση έργου και λογιστική** \> **Ρύθμιση παραμέτρων** \> **Κατηγορίες** \> **Ομάδες κατηγοριών**.</span><span class="sxs-lookup"><span data-stu-id="167cf-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]