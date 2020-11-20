---
title: Επισκόπηση διαστάσεων τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις διαστάσεις τιμολόγησης στο Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ec2e350e0e4c28ea1c9540d70c83fdf0a75dc408
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128463"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="20abc-103">Επισκόπηση διαστάσεων τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="20abc-103">Pricing dimensions overview</span></span>

<span data-ttu-id="20abc-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="20abc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="20abc-105">Οι διαστάσεις που χρησιμοποιούνται στο ανθρώπινο δυναμικό για τη ρύθμιση της τιμολόγησης και του κόστους υπάγονται σε δύο κατηγορίες:</span><span class="sxs-lookup"><span data-stu-id="20abc-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="20abc-106">Άνθρωποι</span><span class="sxs-lookup"><span data-stu-id="20abc-106">People</span></span>
- <span data-ttu-id="20abc-107">Προγραμματισμένη εργασία</span><span class="sxs-lookup"><span data-stu-id="20abc-107">Planned work</span></span>

<span data-ttu-id="20abc-108">Για αυτόν το λόγο, υπάρχουν δύο διαθέσιμοι τύποι τιμών διαστάσεων τιμολόγησης:</span><span class="sxs-lookup"><span data-stu-id="20abc-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="20abc-109">**Σύνολα επιλογών**: Διαστάσεις που είναι σταθερές απαριθμήσεις για ένα σύνολο τιμών.</span><span class="sxs-lookup"><span data-stu-id="20abc-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="20abc-110">**Τιμές βασισμένες σε οντότητες**: Διαστάσεις που μπορεί να είναι ένα ποικίλο σύνολο τιμών.</span><span class="sxs-lookup"><span data-stu-id="20abc-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="20abc-111">Διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="20abc-111">Pricing dimensions</span></span>

<span data-ttu-id="20abc-112">Το Dynamics 365 Project Operations παραδίδεται με ένα προεπιλεγμένο σύνολο διαστάσεων τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="20abc-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="20abc-113">Μπορείτε να τις δείτε αυτές τις διαστάσεις τιμολόγησης μεταβαίνοντας στο **Λειτουργίες έργου** > **Παράμετροι**.</span><span class="sxs-lookup"><span data-stu-id="20abc-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="20abc-114">Στην καρτέλα της παραμέτρου, στην καρτέλα **Διαστάσεις τιμολόγησης βάσει ποσού** επαληθεύστε ότι ο ρόλος **msdyn_resourcecategory** και η οργανωτική μονάδα πόρου **msdyn_organizationalunit** έχουν τα πεδία **Ισχύει για τις πωλήσεις** και **Ισχύει για το κόστος** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="20abc-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="20abc-115">Με ενεργοποιημένα αυτά τα πεδία, θα μπορείτε να ορίσετε την τιμή και το κόστος για κάθε συνδυασμό ρόλου και οργανωτικής μονάδας.</span><span class="sxs-lookup"><span data-stu-id="20abc-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="20abc-116">Εάν χρειάζεστε την τιμή ή το κόστος για τους πόρους σας χρησιμοποιώντας πρόσθετα χαρακτηριστικά, μπορείτε να δημιουργήσετε προσαρμοσμένα πεδία, οντότητες και διαστάσεις.</span><span class="sxs-lookup"><span data-stu-id="20abc-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="20abc-117">Τιμολόγηση του χρόνου ανθρώπινου δυναμικού</span><span class="sxs-lookup"><span data-stu-id="20abc-117">Pricing human resource time</span></span>
<span data-ttu-id="20abc-118">Ο τρόπος με τον οποίο ένας οργανισμός τιμολογεί τον χρόνο του ανθρώπινου δυναμικού είναι συχνά μια σημαντική στρατηγική εκτίμηση που επηρεάζει άμεσα την κερδοφορία του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="20abc-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="20abc-119">Εργαστείτε με τις ομάδες οικονομικών και τους επικεφαλής πρακτικής όταν ο οργανισμός σας είναι έτοιμος να προσδιορίσει τον τρόπο με τον οποίο θέλει να ρυθμίσει τις τιμές χρέωσης και κόστους για τον χρόνο του ανθρώπινου δυναμικού.</span><span class="sxs-lookup"><span data-stu-id="20abc-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="20abc-120">Άλλες εκτιμήσεις για την τιμολόγηση περιλαμβάνουν εάν θα επαναχρησιμοποιηθούν τα πεδία ή οι οντότητες που δεν είναι τώρα διαστάσεις τιμολόγησης αλλά εφαρμόζονται ως διάσταση τιμολόγησης για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="20abc-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="20abc-121">Τα πεδία όπως **Κατηγορία συναλλαγής** (**msdyn_transactioncategory**) και **Πόρος με δυνατότητα κράτησης** και (**bookableresource**) αποτελούν παραδείγματα διαστάσεων υποψηφίων.</span><span class="sxs-lookup"><span data-stu-id="20abc-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="20abc-122">Λάβετε υπόψη σας εάν η διάσταση τιμολόγησης σας πρέπει να είναι πίνακας ή σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="20abc-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="20abc-123">Εάν προβλέψετε αλλαγές στις τιμές μιας διάστασης που θα υπερβαίνει τα 10 ή τα 12 και χρειάζεστε πρόσθετα χαρακτηριστικά σε αυτές τις τιμές, θα μπορούσατε να δημιουργήσετε μια οντότητα και όχι ένα σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="20abc-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="20abc-124">Η διατήρηση ενός συνόλου επιλογών, όπως η προσθήκη ή η κατάργηση τιμών, απαιτεί έναν διαχειριστή ή προγραμματιστή, ενώ η προσθήκη νέων γραμμών σε έναν πίνακα μπορεί να γίνει από τους περισσότερους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="20abc-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="20abc-125">Το παρακάτω παράδειγμα δείχνει τις χρεώσεις λογαριασμών που έχουν οριστεί με βάση το ρόλο και την οργανωτική μονάδα πόρων στην οποία ανήκει ο πόρος.</span><span class="sxs-lookup"><span data-stu-id="20abc-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="20abc-126">Τα ποσοστά κόστους βασίζονται συνήθως στη ζώνη αποδοχών του υπαλλήλου και στη μονάδα οργανισμού στην οποία ανήκει.</span><span class="sxs-lookup"><span data-stu-id="20abc-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="20abc-127">Σε αυτό το παράδειγμα, οι πίνακες ποσοστού χρέωσης και ποσοστού κόστους θα μοιάζουν με τους ακόλουθους.</span><span class="sxs-lookup"><span data-stu-id="20abc-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="20abc-128">**Δείγμα ποσοστών χρέωσης**</span><span class="sxs-lookup"><span data-stu-id="20abc-128">**Sample bill rates**</span></span>

| <span data-ttu-id="20abc-129">Ρόλος</span><span class="sxs-lookup"><span data-stu-id="20abc-129">Role</span></span>        | <span data-ttu-id="20abc-130">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-130">Org Unit</span></span>    |<span data-ttu-id="20abc-131">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-131">Unit</span></span>      |<span data-ttu-id="20abc-132">Τιμή</span><span class="sxs-lookup"><span data-stu-id="20abc-132">Price</span></span>      |<span data-ttu-id="20abc-133">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="20abc-134">Προγραμματιστής</span><span class="sxs-lookup"><span data-stu-id="20abc-134">Developer</span></span>   | <span data-ttu-id="20abc-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="20abc-135">Contoso US</span></span>  |<span data-ttu-id="20abc-136">Hour</span><span class="sxs-lookup"><span data-stu-id="20abc-136">Hour</span></span> | <span data-ttu-id="20abc-137">200</span><span class="sxs-lookup"><span data-stu-id="20abc-137">200</span></span>|<span data-ttu-id="20abc-138">USD</span><span class="sxs-lookup"><span data-stu-id="20abc-138">USD</span></span>     |
| <span data-ttu-id="20abc-139">Προγραμματιστής</span><span class="sxs-lookup"><span data-stu-id="20abc-139">Developer</span></span>   | <span data-ttu-id="20abc-140">Contoso India</span><span class="sxs-lookup"><span data-stu-id="20abc-140">Contoso India</span></span> |<span data-ttu-id="20abc-141">Hour</span><span class="sxs-lookup"><span data-stu-id="20abc-141">Hour</span></span>|   <span data-ttu-id="20abc-142">112</span><span class="sxs-lookup"><span data-stu-id="20abc-142">112</span></span>|<span data-ttu-id="20abc-143">USD</span><span class="sxs-lookup"><span data-stu-id="20abc-143">USD</span></span>     |


<span data-ttu-id="20abc-144">**Δείγμα ποσοστών κόστους**</span><span class="sxs-lookup"><span data-stu-id="20abc-144">**Sample cost rates**</span></span>

| <span data-ttu-id="20abc-145">Ζώνη αποδοχών</span><span class="sxs-lookup"><span data-stu-id="20abc-145">Salary Band</span></span>     | <span data-ttu-id="20abc-146">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-146">Org Unit</span></span>    |<span data-ttu-id="20abc-147">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-147">Unit</span></span>      |<span data-ttu-id="20abc-148">Τιμή</span><span class="sxs-lookup"><span data-stu-id="20abc-148">Price</span></span>      |<span data-ttu-id="20abc-149">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="20abc-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="20abc-150">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="20abc-150">My company_Band1</span></span> | <span data-ttu-id="20abc-151">Contoso US</span><span class="sxs-lookup"><span data-stu-id="20abc-151">Contoso US</span></span>  |<span data-ttu-id="20abc-152">Hour</span><span class="sxs-lookup"><span data-stu-id="20abc-152">Hour</span></span> | <span data-ttu-id="20abc-153">145</span><span class="sxs-lookup"><span data-stu-id="20abc-153">145</span></span>|<span data-ttu-id="20abc-154">USD</span><span class="sxs-lookup"><span data-stu-id="20abc-154">USD</span></span>     |
| <span data-ttu-id="20abc-155">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="20abc-155">My company_Band2</span></span> | <span data-ttu-id="20abc-156">Contoso India</span><span class="sxs-lookup"><span data-stu-id="20abc-156">Contoso India</span></span> |<span data-ttu-id="20abc-157">Hour</span><span class="sxs-lookup"><span data-stu-id="20abc-157">Hour</span></span>|   <span data-ttu-id="20abc-158">67</span><span class="sxs-lookup"><span data-stu-id="20abc-158">67</span></span>|<span data-ttu-id="20abc-159">USD</span><span class="sxs-lookup"><span data-stu-id="20abc-159">USD</span></span>     |
