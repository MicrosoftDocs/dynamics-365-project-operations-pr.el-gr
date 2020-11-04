---
title: Συμβάσεις έργων
description: Αυτό το θέμα παρέχει παραδείγματα των συμβάσεων έργων που μπορείτε να δημιουργήσετε για διάφορους τύπους έργων και πηγών χρηματοδότησης και πώς μπορείτε να διαχειριστείτε τις συμβάσεις και να τιμολογήσετε τους πελάτες του έργου.
author: Yowelle
manager: AnnBe
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: b7d15523f1b22bb8813a47f9f822f12bc4162104
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077047"
---
# <a name="project-contracts"></a><span data-ttu-id="64150-103">Συμβάσεις έργων</span><span class="sxs-lookup"><span data-stu-id="64150-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="64150-104">Αυτό το άρθρο παρέχει παραδείγματα των συμβάσεων έργων που μπορείτε να δημιουργήσετε για διάφορους τύπους έργων και πηγών χρηματοδότησης και πώς μπορείτε να διαχειριστείτε τις συμβάσεις και να τιμολογήσετε τους πελάτες του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="64150-105">Ο τύπος του έργου που δημιουργείτε για μια σύμβαση έργου καθορίζει τη μέθοδο που χρησιμοποιείται για την τιμολόγηση των πελατών του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="64150-106">Μπορείτε να αλλάξετε μια σύμβαση έργου και το σχετικό έργο, αλλά δεν μπορείτε να αλλάξετε τον τύπο έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="64150-107">Χρησιμοποιώντας μια σύμβαση έργου, μπορείτε να τιμολογήσετε ταυτόχρονα ένα ή περισσότερα έργα.</span><span class="sxs-lookup"><span data-stu-id="64150-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="64150-108">Επίσης, η σύμβαση έργου συμβάλλει στη διασφάλιση μιας συνεπούς διαδικασίας τιμολόγησης για κάθε δευτερεύον έργο σε μια δομή έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="64150-109">Κάθε έργο που θα τιμολογηθεί πρέπει να συσχετιστεί με μια σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="64150-110">Οι ρυθμίσεις για μια σύμβαση έργου εφαρμόζονται σε όλα τα έργα και τα δευτερεύοντα έργα που σχετίζονται με τη συγκεκριμένη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="64150-111">Μια σύμβαση έργου μπορεί να καθορίσει μία ή περισσότερες πηγές χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="64150-112">Για αυτόν το λόγο, μπορείτε να διαιρέσετε τη χρέωση ανάμεσα σε πολλούς χρηματοδότες, να ορίσετε όρια χρηματοδότησης έτσι ώστε οι προελεύσεις χρηματοδότησης να μην χρεώνονται περισσότερο από ένα συγκεκριμένο ποσό και να ρυθμίσετε τις παραμέτρους των κανόνων χρηματοδότησης για τη χρέωση των δαπανών.</span><span class="sxs-lookup"><span data-stu-id="64150-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="64150-113">Χρηματοδότηση συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="64150-113">Funding for project contracts</span></span>
<span data-ttu-id="64150-114">Ορισμένες συμβάσεις έργου ορίζουν ότι πολλαπλά μέρη μοιράζονται την ευθύνη για τη χρηματοδότηση του κόστους του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="64150-115">Ακολουθούν μερικά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="64150-115">Here are some examples:</span></span>

-   <span data-ttu-id="64150-116">Ένας μεγάλος πελάτης που έχει πολλαπλά τμήματα απαιτεί τη διαίρεση μιας χρηματοδότησης έργου με διαίρεση.</span><span class="sxs-lookup"><span data-stu-id="64150-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="64150-117">Η εταιρεία σας συμμερίζεται το κόστος ενός μεγάλου έργου με εξωτερικό οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="64150-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="64150-118">Ένα οδικό έργο συγχρηματοδοτείται από δύο δήμους.</span><span class="sxs-lookup"><span data-stu-id="64150-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="64150-119">Ένα έργο κατασκευής γέφυρας χρηματοδοτείται από μια κρατική επιδότηση και μια ιδιωτική εταιρεία.</span><span class="sxs-lookup"><span data-stu-id="64150-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="64150-120">Στο Dynamics 365 Finance, μπορείτε να διαιρέσετε τη χρέωση για μια μεμονωμένη συναλλαγή ή ένα σύνολο έργου μεταξύ πολλών πελατών, επιχορηγήσεων ή οργανισμών.</span><span class="sxs-lookup"><span data-stu-id="64150-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="64150-121">Σε έργα που έχουν πολλαπλούς χρηματοδότες, όλα τα μέρη που συνεισφέρουν στη χρηματοδότηση ενός προηγμένου χρηματοδοτικού έργου ονομάζονται πηγές χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="64150-122">Αφού ένας πελάτης, ένας οργανισμός ή μια επιδότηση ορίζεται ως προέλευση χρηματοδότησης, μπορεί να ανατεθεί σε έναν ή περισσότερους κανόνες χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="64150-123">Οι κανόνες χρηματοδότησης περιέχουν τα κριτήρια που καθορίζουν τον τρόπο με τον οποίο οι χρεώσεις εκχωρούνται στις διάφορες πηγές χρηματοδότησης ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="64150-124">Επειδή τα στοιχεία που έχουν απομείνει, όπως αυτά που εμφανίζονται στις αιτήσεις αγοράς και τις παραγγελίες αγοράς, δεν είναι δυνατό να διαχωριστούν, το ποσό του κόστους δεν μπορεί να χωριστεί μεταξύ πολλών προελεύσεων χρηματοδότησης κατά τη στιγμή της διανομής.</span><span class="sxs-lookup"><span data-stu-id="64150-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="64150-125">Επομένως, η τιμή προέλευσης χρηματοδότησης παραμένει 0 (μηδέν) έως ότου καταχωρηθεί το ζήτημα αποθέματος.</span><span class="sxs-lookup"><span data-stu-id="64150-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="64150-126">Όταν καταχωρείται το ζήτημα του αποθέματος, το ποσό του κόστους κατανέμεται σύμφωνα με τους κανόνες διανομής λογαριασμών του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="64150-127">Ακολουθούν ορισμένα βήματα που μπορείτε να ακολουθήσετε για να διευκολύνετε τη διαίρεση της χρέωσης μεταξύ πολλών προελεύσεων χρηματοδότησης:</span><span class="sxs-lookup"><span data-stu-id="64150-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="64150-128">Καθορίστε ότι όλες οι συναλλαγές που έχουν καταχωρηθεί για ένα έργο χρησιμοποιούν την ίδια νομισματική μονάδα πωλήσεων με τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="64150-129">Καθορίστε όρια χρηματοδότησης, έτσι ώστε μια προέλευση χρηματοδότησης να μην τιμολογείται περισσότερο από ένα καθορισμένο ποσό προς ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="64150-130">Ρυθμίστε τις παραμέτρους των κανόνων χρηματοδότησης και των ορίων χρηματοδότησης για κάθε εργαζόμενο, στοιχείο, κατηγορία, ομάδα κατηγοριών και τύπο συναλλαγής (ή για όλους τους τύπους συναλλαγών).</span><span class="sxs-lookup"><span data-stu-id="64150-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="64150-131">Επιλέξτε προαιρετικές ημερομηνίες έναρξης και λήξης για να καθορίσετε την περίοδο κατά την οποία θα είναι έγκυρος κάθε κανόνας χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="64150-132">Καθορίστε το ποσοστό για το οποίο είναι υπεύθυνη κάθε προέλευση χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="64150-133">Καθορίστε ποια προέλευση χρηματοδότησης είναι υπεύθυνη για τη στρογγυλοποίηση διαφορών που προκαλούνται από υπολογισμούς εκχώρησης χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="64150-134">Ρυθμίστε κανόνες που καθορίζουν τον τρόπο τιμολόγησης του κόστους έργου σε εξωτερικούς πελάτες και χρεώνεται σε εσωτερικούς οργανισμούς.</span><span class="sxs-lookup"><span data-stu-id="64150-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="64150-135">Καταγράψτε τις συναλλαγές σε ένα λογαριασμό χρηματοδότησης που βρίσκεται σε αναμονή μέχρι να αποκτηθεί πρόσθετη χρηματοδότηση ή μέχρι να αποφασίσετε να επιβαρυνθείτε εσωτερικά με το κόστος.</span><span class="sxs-lookup"><span data-stu-id="64150-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="64150-136">Για να καθοριστεί ποια ομάδα φόρων θα συσχετιστεί με μια συναλλαγή, γίνεται αναζήτηση του έργου για μια ανάθεση ομάδας φόρων.</span><span class="sxs-lookup"><span data-stu-id="64150-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="64150-137">Σε περίπτωση που δεν έχει γίνει καμία ανάθεση σε ομάδα φόρων σε επίπεδο έργου, γίνεται αναζήτηση της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="64150-138">Παράδειγμα: πολλαπλές πηγές χρηματοδότησης (απλή)</span><span class="sxs-lookup"><span data-stu-id="64150-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="64150-139">Στον ακόλουθο πίνακα παρουσιάζονται τα σενάρια για τη διαχείριση της ανάθεσης κονδυλίων μεταξύ πολλών προελεύσεων χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="64150-140">Τα σενάρια αυτά βασίζονται στις εξής υποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="64150-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="64150-141">Οι ρυθμίσεις προτεραιότητας υπολογίζονται στη διανομή των κονδυλίων προτού εφαρμοστούν άλλα κριτήρια κανόνων χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="64150-142">Δεν έχει καθοριστεί εύρος ημερομηνιών για τον καθορισμό της περιόδου d όταν ο κανόνας χρηματοδότησης είναι έγκυρος.</span><span class="sxs-lookup"><span data-stu-id="64150-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="64150-143"><strong>Σενάριο</strong></span><span class="sxs-lookup"><span data-stu-id="64150-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="64150-144"><strong>Προέλευση χρηματοδότησης</strong></span><span class="sxs-lookup"><span data-stu-id="64150-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="64150-145"><strong>Ποσοστό εκχώρησης</strong></span><span class="sxs-lookup"><span data-stu-id="64150-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="64150-146"><strong>Προτεραιότητα ανάθεσης</strong></span><span class="sxs-lookup"><span data-stu-id="64150-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64150-147">Θέλετε να αναθέσετε το κόστος σε μια πηγή χρηματοδότησης έως ότου εξαντληθούν τα κεφάλαιά της, να κατανείμετε το κόστος σε μια δεύτερη πηγή χρηματοδότησης έως ότου εξαντληθούν τα κεφάλαιά της και, τέλος, να κατανείμετε το υπόλοιπο κόστος σε μια τρίτη πηγή χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-148">Προέλευση　χρηματοδότησης　1</span><span class="sxs-lookup"><span data-stu-id="64150-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="64150-149">Προέλευση　χρηματοδότησης　2</span><span class="sxs-lookup"><span data-stu-id="64150-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="64150-150">Προέλευση　χρηματοδότησης　3</span><span class="sxs-lookup"><span data-stu-id="64150-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-151">100%</span><span class="sxs-lookup"><span data-stu-id="64150-151">100%</span></span></li>
<li><span data-ttu-id="64150-152">100%</span><span class="sxs-lookup"><span data-stu-id="64150-152">100%</span></span></li>
<li><span data-ttu-id="64150-153">100%</span><span class="sxs-lookup"><span data-stu-id="64150-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-154">1</span><span class="sxs-lookup"><span data-stu-id="64150-154">1</span></span></li>
<li><span data-ttu-id="64150-155">2</span><span class="sxs-lookup"><span data-stu-id="64150-155">2</span></span></li>
<li><span data-ttu-id="64150-156">3</span><span class="sxs-lookup"><span data-stu-id="64150-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="64150-157">Θέλετε να δεσμεύσετε το 75 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το 25 τοις εκατό σε μια δεύτερη προέλευση χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="64150-158">Όταν κάποια από αυτές τις πηγές χρηματοδότησης έχει εξαντληθεί, θέλετε να πληρώσετε τα υπόλοιπα έξοδα από μια τρίτη πηγή χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-159">Προέλευση　χρηματοδότησης　1</span><span class="sxs-lookup"><span data-stu-id="64150-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="64150-160">Προέλευση　χρηματοδότησης　2</span><span class="sxs-lookup"><span data-stu-id="64150-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="64150-161">Προέλευση　χρηματοδότησης　3</span><span class="sxs-lookup"><span data-stu-id="64150-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-162">75%</span><span class="sxs-lookup"><span data-stu-id="64150-162">75%</span></span></li>
<li><span data-ttu-id="64150-163">25%</span><span class="sxs-lookup"><span data-stu-id="64150-163">25%</span></span></li>
<li><span data-ttu-id="64150-164">100%</span><span class="sxs-lookup"><span data-stu-id="64150-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-165">1</span><span class="sxs-lookup"><span data-stu-id="64150-165">1</span></span></li>
<li><span data-ttu-id="64150-166">1</span><span class="sxs-lookup"><span data-stu-id="64150-166">1</span></span></li>
<li><span data-ttu-id="64150-167">2</span><span class="sxs-lookup"><span data-stu-id="64150-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64150-168">Θέλετε να δεσμεύσετε το 75 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το 25 τοις εκατό σε μια δεύτερη προέλευση χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="64150-169">Όταν κάποια από αυτές τις πηγές χρηματοδότησης έχει εξαντληθεί, θέλετε να διαχωρίσετε τα υπόλοιπα έξοδα μεταξύ μιας τρίτης πηγής χρηματοδότησης και μιας τέταρτης πηγής χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-170">Προέλευση　χρηματοδότησης　1</span><span class="sxs-lookup"><span data-stu-id="64150-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="64150-171">Προέλευση　χρηματοδότησης　2</span><span class="sxs-lookup"><span data-stu-id="64150-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="64150-172">Προέλευση　χρηματοδότησης　3</span><span class="sxs-lookup"><span data-stu-id="64150-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="64150-173">Προέλευση　χρηματοδότησης　4</span><span class="sxs-lookup"><span data-stu-id="64150-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-174">75%</span><span class="sxs-lookup"><span data-stu-id="64150-174">75%</span></span></li>
<li><span data-ttu-id="64150-175">25%</span><span class="sxs-lookup"><span data-stu-id="64150-175">25%</span></span></li>
<li><span data-ttu-id="64150-176">50%</span><span class="sxs-lookup"><span data-stu-id="64150-176">50%</span></span></li>
<li><span data-ttu-id="64150-177">50%</span><span class="sxs-lookup"><span data-stu-id="64150-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-178">1</span><span class="sxs-lookup"><span data-stu-id="64150-178">1</span></span></li>
<li><span data-ttu-id="64150-179">1</span><span class="sxs-lookup"><span data-stu-id="64150-179">1</span></span></li>
<li><span data-ttu-id="64150-180">2</span><span class="sxs-lookup"><span data-stu-id="64150-180">2</span></span></li>
<li><span data-ttu-id="64150-181">2</span><span class="sxs-lookup"><span data-stu-id="64150-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="64150-182">Θέλετε να δεσμεύσετε το πρώτο 25 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το υπόλοιπο σε μια δεύτερη προέλευση χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-183">Προέλευση　χρηματοδότησης　1</span><span class="sxs-lookup"><span data-stu-id="64150-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="64150-184">Προέλευση　χρηματοδότησης　2</span><span class="sxs-lookup"><span data-stu-id="64150-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-185">25%</span><span class="sxs-lookup"><span data-stu-id="64150-185">25%</span></span></li>
<li><span data-ttu-id="64150-186">100%</span><span class="sxs-lookup"><span data-stu-id="64150-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="64150-187">1</span><span class="sxs-lookup"><span data-stu-id="64150-187">1</span></span></li>
<li><span data-ttu-id="64150-188">2</span><span class="sxs-lookup"><span data-stu-id="64150-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="64150-189">Παράδειγμα: πολλαπλές πηγές χρηματοδότησης (σύνθετη)</span><span class="sxs-lookup"><span data-stu-id="64150-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="64150-190">Έχετε τρεις πηγές χρηματοδότησης που θέλετε να χρησιμοποιήσετε με την ακόλουθη σειρά:</span><span class="sxs-lookup"><span data-stu-id="64150-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="64150-191">Χρησιμοποιήστε την πηγή χρηματοδότησης 2 και την πηγή χρηματοδότησης 3 εξίσου, έως ότου εξαντληθεί η πηγή χρηματοδότησης 2.</span><span class="sxs-lookup"><span data-stu-id="64150-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="64150-192">Συνεχίστε να χρησιμοποιείτε την πηγή χρηματοδότησης 3 έως ότου εξαντληθεί.</span><span class="sxs-lookup"><span data-stu-id="64150-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="64150-193">Χρησιμοποιήστε την πηγή χρηματοδότησης 1 μόλις εξαντληθεί η πηγή χρηματοδότησης 3.</span><span class="sxs-lookup"><span data-stu-id="64150-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="64150-194">Για να πετύχετε αυτόν τον στόχο, πρώτα πρέπει να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="64150-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="64150-195">Καθορισμός ορίων χρηματοδότησης για την πηγή χρηματοδότησης 2 και την πηγή χρηματοδότησης 3, για τα αντίστοιχα ποσά.</span><span class="sxs-lookup"><span data-stu-id="64150-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="64150-196">Δημιουργήσετε τους παρακάτω κανόνες χρηματοδότησης:</span><span class="sxs-lookup"><span data-stu-id="64150-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="64150-197">Κανόνας 1 (προτεραιότητα 1): Εκχώρηση του 50 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 2 και του 50 τοις εκατό στην πηγή χρηματοδότησης 3.</span><span class="sxs-lookup"><span data-stu-id="64150-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="64150-198">Κανόνας 2 (προτεραιότητα 2): Εκχώρηση του 100 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 3.</span><span class="sxs-lookup"><span data-stu-id="64150-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="64150-199">Κανόνας 3 (προτεραιότητα 3): Εκχώρηση του 100 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 1.</span><span class="sxs-lookup"><span data-stu-id="64150-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="64150-200">Αυτή η ρύθμιση λειτουργεί επειδή οι συναλλαγές ελέγχονται με βάση τους κανόνες και τα όρια για να καθοριστεί εάν κάποιο από αυτά ισχύει για τη συναλλαγή.</span><span class="sxs-lookup"><span data-stu-id="64150-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="64150-201">Εάν δεν ισχύουν συγκεκριμένοι κανόνες ή όρια για τη συναλλαγή, ισχύει ο κανόνας "Όλες οι συναλλαγές".</span><span class="sxs-lookup"><span data-stu-id="64150-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="64150-202">Ο κανόνας "Όλες οι συναλλαγές" ταιριάζει με όλες τις συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="64150-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="64150-203">Εάν βρεθεί ένας κανόνας που αντιστοιχεί σε μια συναλλαγή, εφαρμόζεται πρώτα το ποσοστό που έχει εκχωρηθεί σε αυτόν τον κανόνα, αλλά μόνο αφού ελεγχθούν οι αντιστοιχίσεις με βάση τα όρια που έχουν οριστεί.</span><span class="sxs-lookup"><span data-stu-id="64150-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="64150-204">Εάν έχει τηρηθεί ένα όριο και εξαντληθούν τα κεφάλαια μιας πηγής χρηματοδότησης, ο κανόνας χρηματοδότησης που σχετίζεται με το όριο χρηματοδότησης δεν λαμβάνεται υπόψη και το πρόγραμμα ελέγχει για τον επόμενο κανόνα που ισχύει.</span><span class="sxs-lookup"><span data-stu-id="64150-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="64150-205">Σε ορισμένες περιπτώσεις, μόνο ένα μέρος μιας συναλλαγής μπορεί να εκχωρηθεί με βάση έναν κανόνα.</span><span class="sxs-lookup"><span data-stu-id="64150-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="64150-206">Αυτό μπορεί να συμβαίνει επειδή ένα όριο επιτυγχάνεται όταν η συναλλαγή έχει εκχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="64150-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="64150-207">Σε αυτήν την περίπτωση, μόνο ένα συγκεκριμένο ποσό εκχωρείται σύμφωνα με τον εν λόγω κανόνα, όπως το 50 τοις εκατό σε κάθε πηγή χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="64150-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="64150-208">Αυτή είναι η υπόθεση στον κανόνα 1, η οποία περιγράφεται παραπάνω σε αυτήν την ενότητα.</span><span class="sxs-lookup"><span data-stu-id="64150-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="64150-209">Το υπόλοιπο εκχωρείται σύμφωνα με τον επόμενο κανόνα στην ακολουθία.</span><span class="sxs-lookup"><span data-stu-id="64150-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="64150-210">Ο παρακάτω πίνακας εξετάζει αυτό το σενάριο με περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="64150-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="64150-211"><strong>Εστίαση</strong></span><span class="sxs-lookup"><span data-stu-id="64150-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="64150-212"><strong>Λεπτομέρειες</strong></span><span class="sxs-lookup"><span data-stu-id="64150-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64150-213">Κανόνες χρηματοδότησης</span><span class="sxs-lookup"><span data-stu-id="64150-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-214">Κανόνας 1 (προτεραιότητα 1): όλες οι συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="64150-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="64150-215">Καταχωρήστε την πηγή χρηματοδότησης 2 στο 50% και την πηγή χρηματοδότηση 3 στο 50%.</span><span class="sxs-lookup"><span data-stu-id="64150-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="64150-216">Κανόνας 2 (προτεραιότητα 2): όλες οι συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="64150-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="64150-217">Καταχωρήστε την πηγή χρηματοδότησης 3 στο 100%.</span><span class="sxs-lookup"><span data-stu-id="64150-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="64150-218">Κανόνας 3 (προτεραιότητα 2): όλες οι συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="64150-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="64150-219">Καταχωρήστε την πηγή χρηματοδότησης 1 στο 100%.</span><span class="sxs-lookup"><span data-stu-id="64150-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="64150-220">Όρια χρηματοδότησης</span><span class="sxs-lookup"><span data-stu-id="64150-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-221">Όριο πηγής χρηματοδότησης 1 = 10,000.00</span><span class="sxs-lookup"><span data-stu-id="64150-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="64150-222">Όριο πηγής χρηματοδότησης 2 = 500.00</span><span class="sxs-lookup"><span data-stu-id="64150-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="64150-223">Όριο πηγής χρηματοδότησης 3 = 750.00</span><span class="sxs-lookup"><span data-stu-id="64150-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64150-224">Συναλλαγή 1</span><span class="sxs-lookup"><span data-stu-id="64150-224">Transaction 1</span></span></td>
<td><span data-ttu-id="64150-225"><strong>Ποσό συναλλαγής:</strong> 100.00<strong>Χρηματοδότηση:</strong> Η συναλλαγή καταβάλλεται μόνο σύμφωνα με τον κανόνα 1, επειδή η συναλλαγή πληρώνεται πλήρως μετά την εφαρμογή του κανόνα 1.</span><span class="sxs-lookup"><span data-stu-id="64150-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="64150-226">Η συναλλαγή χρηματοδοτείται ισόποσα μεταξύ της πηγής χρηματοδότησης 2 και της πηγής χρηματοδότησης 3.</span><span class="sxs-lookup"><span data-stu-id="64150-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="64150-227">Πηγή χρηματοδότησης 2: 50.00</span><span class="sxs-lookup"><span data-stu-id="64150-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="64150-228">Πηγή χρηματοδότησης 3: 50.00</span><span class="sxs-lookup"><span data-stu-id="64150-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="64150-229">Συναλλαγή 2</span><span class="sxs-lookup"><span data-stu-id="64150-229">Transaction 2</span></span></td>
<td><span data-ttu-id="64150-230"><strong>Ποσό συναλλαγής:</strong> 5.000.00<strong>Χρηματοδότηση:</strong> Η συναλλαγή καταβάλλεται σύμφωνα με τους τρεις κανόνες.</span><span class="sxs-lookup"><span data-stu-id="64150-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="64150-231"><strong>Κανόνας 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="64150-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="64150-232">Πηγή χρηματοδότησης 2: 450.00</span><span class="sxs-lookup"><span data-stu-id="64150-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="64150-233">Πηγή χρηματοδότησης 3: 450.00</span><span class="sxs-lookup"><span data-stu-id="64150-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="64150-234">
<strong>Κανόνας 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="64150-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="64150-235">Πηγή χρηματοδότησης 3: 250.00 (= 750.00 – 50.00 – 450.00)</span><span class="sxs-lookup"><span data-stu-id="64150-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="64150-236">
<strong>Κανόνας 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="64150-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="64150-237">Πηγή χρηματοδότησης 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span><span class="sxs-lookup"><span data-stu-id="64150-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64150-238">Σύνολο κονδυλίων που διανέμονται για κάθε πηγή χρηματοδότησης</span><span class="sxs-lookup"><span data-stu-id="64150-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="64150-239">Πηγή χρηματοδότησης 1: 3,850.00</span><span class="sxs-lookup"><span data-stu-id="64150-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="64150-240">Πηγή χρηματοδότησης 2: 500.00</span><span class="sxs-lookup"><span data-stu-id="64150-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="64150-241">Πηγή χρηματοδότησης 3: 750.00</span><span class="sxs-lookup"><span data-stu-id="64150-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="64150-242">Κανόνες χρέωσης</span><span class="sxs-lookup"><span data-stu-id="64150-242">Billing rules</span></span>
<span data-ttu-id="64150-243">Όταν διαπραγματεύεστε μια σύμβαση έργου με έναν πελάτη, καθορίζετε τον τρόπο και το χρόνο με τον οποίο μπορείτε να τιμολογήσετε τον πελάτη για την εργασία σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="64150-244">Μετά τη ρύθμιση της σύμβασης έργου και του έργου, μπορείτε να ορίσετε κανόνες χρέωσης για το έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="64150-245">Οι κανόνες χρέωσης βασίζονται στους όρους έργου που καθορίζονται στη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="64150-246">Οι κανόνες χρέωσης που μπορείτε να δημιουργήσετε εξαρτώνται από τους όρους της σύμβασης έργου και τον τύπο έργου, για παράδειγμα, ο χρόνος και το υλικό ή η σταθερή τιμή, τα οποία συσχετίζετε με τον κανόνα χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="64150-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="64150-247">Μπορείτε να δημιουργήσετε περισσότερους από έναν κανόνες χρέωσης για μια σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="64150-248">Μπορείτε, επίσης, να αναθέσετε έναν κανόνα χρέωσης σε πολλαπλά έργα που σχετίζονται με την ίδια σύμβαση έργου και με παρόμοιους όρους χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="64150-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="64150-249">Μπορείτε να ορίσετε τους ακόλουθους τύπους κανόνων χρέωσης:</span><span class="sxs-lookup"><span data-stu-id="64150-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="64150-250">**Μονάδα παράδοσης** – Τιμολογήστε έναν πελάτη όταν ολοκληρώνετε μια μονάδα παράδοσης.</span><span class="sxs-lookup"><span data-stu-id="64150-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="64150-251">Μπορείτε να ορίσετε τις μονάδες παράδοσης στη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="64150-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="64150-252">**Πρόοδος** – Τιμολογήστε έναν πελάτη όταν ολοκληρώνετε ένα καθορισμένο ποσοστό του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="64150-253">Μπορείτε να ορίσετε έναν κανόνα χρέωσης για τον αυτόματο υπολογισμό του ποσοστού της εργασίας που έχει ολοκληρωθεί ή μπορείτε να υπολογίσετε με μη αυτόματο τρόπο το ποσοστό της εργασίας που έχει ολοκληρωθεί και το ποσό τιμολόγησης του πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="64150-254">**Ορόσημο** – Τιμολογήστε έναν πελάτη για το πλήρες ποσό ενός ορόσημου έργου όταν επιτυγχάνεται το ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="64150-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="64150-255">**Χρέωση** – Τιμολογήστε έναν πελάτη για τις υπηρεσίες σας συν ένα τέλος διαχείρισης, το οποίο κατά κανόνα αποτελεί ένα ποσοστό του κόστους των υπηρεσιών.</span><span class="sxs-lookup"><span data-stu-id="64150-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="64150-256">**Χρόνος και υλικό** – Τιμολογήστε έναν πελάτη για την αξία του χρόνου και των υλικών που χρησιμοποιούνται σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="64150-257">Για όλους τους τύπους κανόνων χρέωσης, μπορείτε να καθορίσετε ένα ποσοστό διατήρησης που αφαιρείται από τα τιμολόγια πελατών, έως ότου ένα έργο φθάσει σε ένα συμφωνημένο στάδιο.</span><span class="sxs-lookup"><span data-stu-id="64150-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="64150-258">Το ποσοστό διατήρησης της πληρωμής καθορίζεται στη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="64150-259">Το ποσό υπολογίζεται με βάση και αφαιρείται από τη συνολική αξία των γραμμών σε ένα τιμολόγιο πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="64150-260">Για τους κανόνες χρέωσης **Χρόνος και υλικό** και **Πρόοδος** μπορείτε να αναθέσετε κατηγορίες με χρέωση.</span><span class="sxs-lookup"><span data-stu-id="64150-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="64150-261">Οι τιμολογημένες κατηγορίες δηλώνουν τις συναλλαγές που θα πρέπει να συμπεριληφθούν στα τιμολόγια πελατών.</span><span class="sxs-lookup"><span data-stu-id="64150-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="64150-262">Όταν είστε έτοιμοι να τιμολογήσετε τον πελάτη, το ποσό τιμολόγησης για το έργο υπολογίζεται με βάση τους κανόνες χρέωσης και δημιουργείται μια πρόταση για το τιμολόγιο του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="64150-263">Οι παρακάτω ενότητες παρέχουν παραδείγματα που δείχνουν τον τρόπο ρύθμισης και διαχείρισης των κανόνων χρέωσης για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="64150-264">Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται στον αριθμό των μονάδων που παραδόθηκαν</span><span class="sxs-lookup"><span data-stu-id="64150-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="64150-265">Ο οργανισμός σας συνάπτει συμφωνία για την παροχή συνολικά πέντε εκπαιδευτικών σεμιναρίων στους υπαλλήλους ενός πελάτη με κόστος 10.000 ανά εκπαιδευτική συνεδρία.</span><span class="sxs-lookup"><span data-stu-id="64150-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="64150-266">Τιμολογήστε τον πελάτη μετά από εκπαιδευτική συνεδρία.</span><span class="sxs-lookup"><span data-stu-id="64150-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="64150-267">Όταν ρυθμίζετε τους κανόνες χρέωσης για τη σύμβαση, χρησιμοποιείτε τις παρακάτω τιμές:</span><span class="sxs-lookup"><span data-stu-id="64150-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="64150-268">Η μονάδα παραλαβής είναι μία εκπαιδευτική συνεδρία.</span><span class="sxs-lookup"><span data-stu-id="64150-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="64150-269">Η τιμή μονάδας είναι 10.000 ανά εκπαιδευτική συνεδρία.</span><span class="sxs-lookup"><span data-stu-id="64150-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="64150-270">Ο συνολικός αριθμός των μονάδων είναι πέντε εκπαιδευτικά σεμινάρια.</span><span class="sxs-lookup"><span data-stu-id="64150-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="64150-271">Όταν ολοκληρώσετε μια εκπαιδευτική συνεδρία, μπορείτε να δημιουργήσετε ένα τιμολόγιο για 10.000, για την πρώτη μονάδα που παρεδόθη και να στείλετε το τιμολόγιο στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="64150-272">Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε ένα καθορισμένο ποσοστό ολοκλήρωσης έργου (μη αυτόματος υπολογισμός)</span><span class="sxs-lookup"><span data-stu-id="64150-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="64150-273">Ο οργανισμός σας, μια εταιρεία συμβούλων λογισμικού, συνάπτει μια συμφωνία με έναν πελάτη για να αναπτύξει ένα μέρος ενός προϊόντος που αναπτύσσει ο πελάτης.</span><span class="sxs-lookup"><span data-stu-id="64150-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="64150-274">Ο οργανισμός σας συμφωνεί να παραδώσει τον κώδικα λογισμικού για μια περίοδο έξι μηνών.</span><span class="sxs-lookup"><span data-stu-id="64150-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="64150-275">Ο πελάτης συμφωνεί να καταβάλει στον οργανισμό σας συνολικά 100.000 για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="64150-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="64150-276">Μπορείτε να δημιουργήσετε έναν κανόνα χρέωσης για την τιμολόγηση του πελάτη με βάση το ποσοστό της εργασίας που ολοκληρώνεται στο έργο, όπως καθορίζεται στη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="64150-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="64150-277">Στο τέλος του πρώτου μήνα, θα συναντήσετε τον πελάτη για να καθορίσετε το ποσοστό της εργασίας που έχει ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="64150-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="64150-278">Μετά την αναθεώρηση του έργου από εσάς και τον πελάτη, αποφασίζετε ότι το έργο είναι 15 τοις εκατό ολοκληρωμένο.</span><span class="sxs-lookup"><span data-stu-id="64150-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="64150-279">Μπορείτε να δημιουργήσετε ένα τιμολόγιο για 15.000 (15 τοις εκατό των 100.000) και να το στείλετε στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="64150-280">Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε ένα καθορισμένο ποσοστό ολοκλήρωσης έργου (αυτόματος υπολογισμός)</span><span class="sxs-lookup"><span data-stu-id="64150-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="64150-281">Ο οργανισμός σας, μια εταιρεία ανάπτυξης λογισμικού, συμφωνεί να αναπτύξει ένα πακέτο λογιστικής μισθοδοσίας για έναν πελάτη για τα 30.000.</span><span class="sxs-lookup"><span data-stu-id="64150-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="64150-282">Ο πελάτης συμφωνεί να πληρώσει τον οργανισμό σας με βάση το ποσοστό της εργασίας που ολοκληρώθηκε.</span><span class="sxs-lookup"><span data-stu-id="64150-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="64150-283">Εκτιμάτε ότι το κόστος του έργου είναι 20.000.</span><span class="sxs-lookup"><span data-stu-id="64150-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="64150-284">Η σύμβαση έργου προσδιορίζει τις κατηγορίες εργασιών που χρησιμοποιείτε στη διαδικασία χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="64150-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="64150-285">Μπορείτε να ορίσετε κανόνες χρέωσης που υπολογίζουν αυτόματα τα ποσά τιμολόγησης για το ποσοστό της εργασίας που ολοκληρώνεται για κάθε κατηγορία.</span><span class="sxs-lookup"><span data-stu-id="64150-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="64150-286">Μπορείτε να δημιουργήσετε έναν προϋπολογισμό για κάθε κατηγορία:</span><span class="sxs-lookup"><span data-stu-id="64150-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="64150-287">**Ανάπτυξη** – Κόστος 15.000 και έσοδα 20.000</span><span class="sxs-lookup"><span data-stu-id="64150-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="64150-288">**Εγκατάσταση** – Κόστος 5.000 και έσοδα 10.000</span><span class="sxs-lookup"><span data-stu-id="64150-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="64150-289">Όταν δημιουργείτε ένα τιμολόγιο πελάτη για πρώτη φορά, το ποσό τιμολογίου υπολογίζεται αυτόματα με βάση τις εξής πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="64150-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="64150-290">Μετά από ένα μήνα, ο εργαζόμενος του έργου υποβάλλει ένα φύλλο κατανομής χρόνου για το έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="64150-291">Το κόστος των ωρών εργασίας του εργαζομένου είναι 5.000 για την ανάπτυξη και 1.000 για την εγκατάσταση.</span><span class="sxs-lookup"><span data-stu-id="64150-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="64150-292">Η εργασία ανάπτυξης είναι 33 τοις εκατό ολοκληρωμένη (5.000 πραγματικό κόστος/15.000 κόστος προϋπολογισμού) και η εργασία εγκατάστασης είναι 20 τοις εκατό ολοκληρωμένη (1.000 πραγματικό κόστος/5.000 κόστος προϋπολογισμού).</span><span class="sxs-lookup"><span data-stu-id="64150-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="64150-293">Το ποσό τιμολογίου 8.667 υπολογίζεται αυτόματα (33 τοις εκατό των 20.000 + 20 τοις εκατό των 10.000).</span><span class="sxs-lookup"><span data-stu-id="64150-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="64150-294">Μπορείτε να δημιουργήσετε ένα τιμολόγιο για 8.667 και να το στείλετε στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="64150-295">Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε συμφωνηθέντα ορόσημα</span><span class="sxs-lookup"><span data-stu-id="64150-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="64150-296">Ο οργανισμός σας, μια εταιρεία συμβούλων επιχειρήσεων, συμφωνεί να διεξάγει έρευνα αγοράς για ένα καταναλωτικό προϊόν, το οποίο προτίθεται να πωλήσει ο πελάτης.</span><span class="sxs-lookup"><span data-stu-id="64150-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="64150-297">Ο πελάτης συμφωνεί να χρησιμοποιήσει τις υπηρεσίες σας για μια περίοδο τριών μηνών, αρχής γενομένης από το Μάρτιο και συμφωνεί να καταβάλει στον οργανισμό σας 50.000.</span><span class="sxs-lookup"><span data-stu-id="64150-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="64150-298">Το έργο έχει τρία ορόσημα:</span><span class="sxs-lookup"><span data-stu-id="64150-298">The project has three milestones:</span></span>

-   <span data-ttu-id="64150-299">Ορόσημο 1: Συλλέξτε καταναλωτικά δεδομένα – 31 Μαρτίου</span><span class="sxs-lookup"><span data-stu-id="64150-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="64150-300">Ορόσημο 2: Ανάλυση καταναλωτικών δεδομένων-30 Απριλίου</span><span class="sxs-lookup"><span data-stu-id="64150-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="64150-301">Ορόσημο 3: Παρουσιάστε μια πρόταση βιωσιμότητας προϊόντος – 31 Μαΐου</span><span class="sxs-lookup"><span data-stu-id="64150-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="64150-302">Ο πελάτης συμφωνεί να καταβάλει στον οργανισμό σας 10.000 για το πρώτο ορόσημο, 20.000 για το δεύτερο ορόσημο και 20.000 για το τρίτο ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="64150-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="64150-303">Όταν ρυθμίζετε τη σύμβαση έργου, συμφωνείτε με την τιμολόγηση του πελάτη με βάση το ορόσημο που έχει ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="64150-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="64150-304">Η ρύθμιση κανόνων χρέωσης περιλαμβάνει τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="64150-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="64150-305">Καθορίστε τα ορόσημα του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-305">Define the project milestones.</span></span>
-   <span data-ttu-id="64150-306">Καθορίστε το ποσό τιμολόγησης του πελάτη όταν ολοκληρωθεί κάθε ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="64150-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="64150-307">Όταν το πρώτο ορόσημο ολοκληρωθεί στις 31 Μαρτίου, μαρκάρετε το ορόσημο ως ολοκληρωμένο και, στη συνέχεια, δημιουργήστε ένα τιμολόγιο για το 10.000 και στείλτε το στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64150-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="64150-308">Δεν μπορείτε να δημιουργήσετε ένα τιμολόγιο για ένα ορόσημο, μέχρι να έχετε επισημάνει το ορόσημο ως ολοκληρωμένο.</span><span class="sxs-lookup"><span data-stu-id="64150-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="64150-309">Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε υπηρεσίες συν ένα τέλος διαχείρισης</span><span class="sxs-lookup"><span data-stu-id="64150-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="64150-310">Ο οργανισμός σας, μια εταιρεία συμβούλων επιχειρήσεων, συμφωνεί να διεξάγει έρευνα αγοράς για την αξιολόγηση της βιωσιμότητας ενός προϊόντος που αναπτύσσει ο πελάτης, μια εταιρεία λιανικής πώλησης.</span><span class="sxs-lookup"><span data-stu-id="64150-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="64150-311">Οι όροι της σύμβασης ορίζουν ότι θα παράσχετε τις υπηρεσίες των τριών κορυφαίων συμβούλων διαχείρισης, οι οποίοι θα διεξάγουν την έρευνα σε βάση χρόνου και ύλης.</span><span class="sxs-lookup"><span data-stu-id="64150-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="64150-312">Ο πελάτης συμφωνεί να καταβάλει 100 ανά ώρα, συν ένα 10 τοις εκατό τέλος διαχείρισης για τις ώρες παροχής συμβουλών που χρεώνονται στο έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="64150-313">Όταν ρυθμίζετε τη σύμβαση έργου, δημιουργήστε έναν κανόνα χρέωσης για να προσθέσετε μια αμοιβή διαχείρισης 10 τοις εκατό στις ώρες παροχής συμβουλών που χρεώνονται στο έργο.</span><span class="sxs-lookup"><span data-stu-id="64150-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="64150-314">Όταν δημιουργείτε ένα τιμολόγιο για τον πελάτη, ο πελάτης χρεώνεται μια χρέωση διαχείρισης 10% συν το κόστος των ωρών διαβούλευσης.</span><span class="sxs-lookup"><span data-stu-id="64150-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="64150-315">Για παράδειγμα, εάν οι τρεις σύμβουλοι εργάστηκαν συνολικά 200 ώρες στο έργο, δημιουργείται ένα τιμολόγιο για τα 22.000 με βάση τον ακόλουθο υπολογισμό:</span><span class="sxs-lookup"><span data-stu-id="64150-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="64150-316">200 ώρες στις 100 ανά ώρα = 20.000</span><span class="sxs-lookup"><span data-stu-id="64150-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="64150-317">έξοδα διαχείρισης 10% = 2.000</span><span class="sxs-lookup"><span data-stu-id="64150-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="64150-318">Συνολικό ποσό τιμολογίου = 22.000</span><span class="sxs-lookup"><span data-stu-id="64150-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="64150-319">Εάν οι αμοιβές φορολογούνται από έναν πελάτη και επιλέξετε μια ομάδα φόρου πωλήσεων στη σύμβαση έργου, η ομάδα φόρου πωλήσεων καταχωρείται αυτόματα σε έναν κανόνα χρέωσης για χρεώσεις.</span><span class="sxs-lookup"><span data-stu-id="64150-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="64150-320">Παράδειγμα: Δημιουργία κανόνα χρέωσης για την τιμή του χρόνου και του υλικού</span><span class="sxs-lookup"><span data-stu-id="64150-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="64150-321">Ο οργανισμός σας, μια εταιρεία συμβούλων λογισμικού, συμφωνεί να παράσχει πέντε τεχνικούς συμβούλους για να εργαστούν σε ένα πρόγραμμα ανάπτυξης λογισμικού για έναν πελάτη για τους επόμενους έξι μήνες.</span><span class="sxs-lookup"><span data-stu-id="64150-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="64150-322">Ο πελάτης συμφωνεί να καταβάλει 150 για κάθε ώρα συμβουλευτικής, συν το κόστος των προμηθειών γραφείου.</span><span class="sxs-lookup"><span data-stu-id="64150-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="64150-323">Ο οργανισμός σας στέλνει ένα τιμολόγιο στον πελάτη στο τέλος κάθε μήνα.</span><span class="sxs-lookup"><span data-stu-id="64150-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="64150-324">Όταν ρυθμίζετε τη σύμβαση έργου, συμφωνείτε με την τιμολόγηση του πελάτη κάθε μήνα για το χρόνο και το υλικό του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="64150-325">Μπορείτε να δημιουργήσετε έναν κανόνα χρέωσης, ο οποίος περιλαμβάνει τις εξής πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="64150-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="64150-326">Η περίοδος σύμβασης είναι έξι μήνες.</span><span class="sxs-lookup"><span data-stu-id="64150-326">The contract period is six months.</span></span>
-   <span data-ttu-id="64150-327">Ο χρόνος παροχής συμβουλών υπολογίζεται με συντελεστή 150 ανά ώρα.</span><span class="sxs-lookup"><span data-stu-id="64150-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="64150-328">Τα αναλώσιμα γραφείου τιμολογούνται με χρέωση και το συνολικό κόστος για το έργο δεν πρέπει να υπερβαίνει τα 10.000.</span><span class="sxs-lookup"><span data-stu-id="64150-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="64150-329">Μπορείτε να δημιουργήσετε ένα τιμολόγιο πελάτη στο τέλος κάθε ημερολογιακού μήνα κατά τη διάρκεια του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="64150-330">Κατά τη διάρκεια του πρώτου μήνα, καταγράφονται συνολικά 800 ώρες από τους συμβούλους του έργου.</span><span class="sxs-lookup"><span data-stu-id="64150-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="64150-331">Το κόστος των προμηθειών γραφείου που χρεώνεται στο έργο είναι 2.000.</span><span class="sxs-lookup"><span data-stu-id="64150-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="64150-332">Επομένως, στο τέλος του μήνα, δημιουργείτε ένα τιμολόγιο για 122.000, το οποίο υπολογίζεται ως 800 ώρες με 150 ανά ώρα, συν 2.000 για τα αναλώσιμα γραφείου.</span><span class="sxs-lookup"><span data-stu-id="64150-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>



