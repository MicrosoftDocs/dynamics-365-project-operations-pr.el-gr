---
title: Αρχική σελίδα διαστάσεων τιμολόγησης και κοστολόγησης
description: Αυτό το θέμα παρέχει μια επισκόπηση των διαστάσεων τιμολόγησης.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 137fee27dd2302d47ae12faccde1682cff43db93
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284133"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="ca5c6-103">Αρχική σελίδα διαστάσεων τιμολόγησης και κοστολόγησης</span><span class="sxs-lookup"><span data-stu-id="ca5c6-103">Pricing and costing dimensions home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ca5c6-104">Οι διαστάσεις που χρησιμοποιούνται για τον καθορισμό της τιμολόγησης εργασίας και της κοστολόγησης σε οργανισμούς που βασίζονται σε έργα, επηρεάζονται από τα ακόλουθα χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="ca5c6-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="ca5c6-105">Άτομα που κάνουν εργασίες παρόμοιες με την εμπειρία, το ρόλο ή τη γεωγραφία τους</span><span class="sxs-lookup"><span data-stu-id="ca5c6-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="ca5c6-106">Εργασίες που πρέπει να εκτελεστούν παρόμοια σε αναλογία με την πολυπλοκότητα ή την ώρα της ημέρας</span><span class="sxs-lookup"><span data-stu-id="ca5c6-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="ca5c6-107">Δεδομένης της τυπικής φύσης αυτών των χαρακτηριστικών των εργασιών και των ατόμων που απαιτούνται για την εκτέλεση της εργασίας, υπάρχουν δύο τύποι τιμών διαστάσεων τιμολόγησης που είναι διαθέσιμοι στο Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="ca5c6-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="ca5c6-108">**Σύνολα επιλογών** - Χαρακτηριστικά που είναι σταθερές απαριθμήσεις για ένα σύνολο τιμών.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="ca5c6-109">**Τιμές βασισμένες σε οντότητες** - Χαρακτηριστικά που μπορούν να έχουν ένα ποικιλόμορφο σύνολο τιμών που είναι πεπερασμένα, αλλά μπορούν να αλλάξουν με την πάροδο του χρόνου.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="ca5c6-110">Διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="ca5c6-110">Pricing dimensions</span></span>

<span data-ttu-id="ca5c6-111">Το PSA διαθέτει ένα προεπιλεγμένο σύνολο διαστάσεων τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="ca5c6-112">Μπορείτε να τις δείτε μεταβαίνοντας στο **Project Service** > **Παράμετροι**.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="ca5c6-113">Στην καρτέλα της παραμέτρου, στην καρτέλα **Διαστάσεις τιμολόγησης βάσει ποσού** επαληθεύστε ότι ο ρόλος **msdyn_resourcecategory** και η οργανωτική μονάδα πόρου **msdyn_organizationalunit** έχουν τα πεδία **Ισχύει για τις πωλήσεις** και **Ισχύει για το κόστος** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="ca5c6-114">Αυτό θα σας επιτρέψει να ορίσετε την τιμή και το κόστος για κάθε συνδυασμό ρόλου και οργανωτικής μονάδας.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Στιγμιότυπο οθόνης των παραμέτρων Project Service με επισήμανση "Ισχύει για πωλήσεις"](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="ca5c6-116">Εάν χρησιμοποιούσατε τα έτοιμα πεδία ρόλου και οργανωτικής μονάδας όπως οι διαστάσεις τιμολόγησης πριν από την έκδοση 3 του PSA, δεν θα υπάρξει καμία παρατηρήσιμη αλλαγή.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="ca5c6-117">Μπορείτε να συνεχίσετε να χρησιμοποιείτε το Project Service ως συνήθως.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="ca5c6-118">Εάν χρειάζεστε την τιμή ή το κόστος για τους πόρους σας χρησιμοποιώντας πρόσθετα χαρακτηριστικά, μπορείτε να δημιουργήσετε προσαρμοσμένα πεδία, οντότητες και διαστάσεις.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="ca5c6-119">Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα, ωστόσο λάβετε υπόψη ότι πρέπει να ολοκληρώσετε τις διαδικασίες με τη σειρά που παρατίθεται παρακάτω:</span><span class="sxs-lookup"><span data-stu-id="ca5c6-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="ca5c6-120">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="ca5c6-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="ca5c6-121">Προσθήκη προσαρμοσμένων πεδίων για τιμολόγηση οντοτήτων ρύθμισης παραμέτρων και συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="ca5c6-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="ca5c6-122">Ρύθμιση προσαρμοσμένων πεδίων ως διαστάσεις τιμολόγησης </span><span class="sxs-lookup"><span data-stu-id="ca5c6-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="ca5c6-123">Ενημέρωση χαρακτηριστικών προσθήκης για συμπερίληψη νέων διαστάσεων τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="ca5c6-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="ca5c6-124">Τιμολόγηση του χρόνου ανθρώπινου δυναμικού</span><span class="sxs-lookup"><span data-stu-id="ca5c6-124">Pricing human resource time</span></span>
<span data-ttu-id="ca5c6-125">Ο τρόπος με τον οποίο ένας οργανισμός τιμολογεί τον χρόνο του ανθρώπινου δυναμικού είναι συχνά μια σημαντική στρατηγική εκτίμηση που επηρεάζει άμεσα την κερδοφορία του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="ca5c6-126">Εργαστείτε με τις ομάδες οικονομικών και τους επικεφαλής πρακτικής όταν ο οργανισμός σας είναι έτοιμος να προσδιορίσει τον τρόπο με τον οποίο θέλει να ρυθμίσει τις τιμές χρέωσης και κόστους για τον χρόνο του ανθρώπινου δυναμικού.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="ca5c6-127">Άλλες εκτιμήσεις για την τιμολόγηση περιλαμβάνουν εάν θα επαναχρησιμοποιηθούν τα πεδία ή οι οντότητες που δεν είναι τώρα διαστάσεις τιμολόγησης αλλά εφαρμόζονται ως διάσταση τιμολόγησης για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="ca5c6-128">Τα πεδία όπως **Κατηγορία συναλλαγής** (**msdyn_transactioncategory**) και **Πόρος με δυνατότητα κράτησης** και (**bookableresource**) αποτελούν παραδείγματα διαστάσεων υποψηφίων.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="ca5c6-129">Λάβετε υπόψη σας εάν η διάσταση τιμολόγησης σας πρέπει να είναι πίνακας ή σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="ca5c6-130">Εάν προβλέπετε αλλαγές στις τιμές μιας διάστασης που θα υπερβαίνει τα 10 ή τα 12 και χρειάζεστε πρόσθετα χαρακτηριστικά σε αυτές τις τιμές, δημιουργήστε μια οντότητα και όχι ένα σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="ca5c6-131">Η διατήρηση ενός συνόλου επιλογών, όπως η προσθήκη ή η κατάργηση τιμών, απαιτεί έναν διαχειριστή ή προγραμματιστή, ενώ η προσθήκη νέων γραμμών σε έναν πίνακα μπορεί να γίνει από τους περισσότερους επιχειρηματικούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="ca5c6-132">Το παρακάτω παράδειγμα δείχνει τις χρεώσεις λογαριασμών που έχουν οριστεί με βάση το ρόλο και την οργανωτική μονάδα πόρων στην οποία ανήκει ο πόρος.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="ca5c6-133">Τα ποσοστά κόστους βασίζονται συνήθως στη ζώνη αποδοχών του υπαλλήλου και στη μονάδα οργανισμού στην οποία ανήκει.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="ca5c6-134">Σε αυτό το παράδειγμα, οι πίνακες ποσοστού χρέωσης και ποσοστού κόστους θα μοιάζουν με τους ακόλουθους.</span><span class="sxs-lookup"><span data-stu-id="ca5c6-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="ca5c6-135">**Δείγμα ποσοστών χρέωσης**</span><span class="sxs-lookup"><span data-stu-id="ca5c6-135">**Sample bill rates**</span></span>

| <span data-ttu-id="ca5c6-136">Ρόλος</span><span class="sxs-lookup"><span data-stu-id="ca5c6-136">Role</span></span>        | <span data-ttu-id="ca5c6-137">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-137">Org Unit</span></span>    |<span data-ttu-id="ca5c6-138">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-138">Unit</span></span>      |<span data-ttu-id="ca5c6-139">Τιμή</span><span class="sxs-lookup"><span data-stu-id="ca5c6-139">Price</span></span>      |<span data-ttu-id="ca5c6-140">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="ca5c6-141">Προγραμματιστής</span><span class="sxs-lookup"><span data-stu-id="ca5c6-141">Developer</span></span>   | <span data-ttu-id="ca5c6-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="ca5c6-142">Contoso US</span></span>  |<span data-ttu-id="ca5c6-143">Hour</span><span class="sxs-lookup"><span data-stu-id="ca5c6-143">Hour</span></span> | <span data-ttu-id="ca5c6-144">200</span><span class="sxs-lookup"><span data-stu-id="ca5c6-144">200</span></span>|<span data-ttu-id="ca5c6-145">USD</span><span class="sxs-lookup"><span data-stu-id="ca5c6-145">USD</span></span>     |
| <span data-ttu-id="ca5c6-146">Προγραμματιστής</span><span class="sxs-lookup"><span data-stu-id="ca5c6-146">Developer</span></span>   | <span data-ttu-id="ca5c6-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="ca5c6-147">Contoso India</span></span> |<span data-ttu-id="ca5c6-148">Hour</span><span class="sxs-lookup"><span data-stu-id="ca5c6-148">Hour</span></span>|   <span data-ttu-id="ca5c6-149">112</span><span class="sxs-lookup"><span data-stu-id="ca5c6-149">112</span></span>|<span data-ttu-id="ca5c6-150">USD</span><span class="sxs-lookup"><span data-stu-id="ca5c6-150">USD</span></span>     |


<span data-ttu-id="ca5c6-151">**Δείγμα ποσοστών κόστους**</span><span class="sxs-lookup"><span data-stu-id="ca5c6-151">**Sample cost rates**</span></span>

| <span data-ttu-id="ca5c6-152">Ζώνη αποδοχών</span><span class="sxs-lookup"><span data-stu-id="ca5c6-152">Salary Band</span></span>     | <span data-ttu-id="ca5c6-153">Οργανωτική μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-153">Org Unit</span></span>    |<span data-ttu-id="ca5c6-154">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-154">Unit</span></span>      |<span data-ttu-id="ca5c6-155">Τιμή</span><span class="sxs-lookup"><span data-stu-id="ca5c6-155">Price</span></span>      |<span data-ttu-id="ca5c6-156">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="ca5c6-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="ca5c6-157">My company_Band1</span><span class="sxs-lookup"><span data-stu-id="ca5c6-157">My company_Band1</span></span> | <span data-ttu-id="ca5c6-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="ca5c6-158">Contoso US</span></span>  |<span data-ttu-id="ca5c6-159">Hour</span><span class="sxs-lookup"><span data-stu-id="ca5c6-159">Hour</span></span> | <span data-ttu-id="ca5c6-160">145</span><span class="sxs-lookup"><span data-stu-id="ca5c6-160">145</span></span>|<span data-ttu-id="ca5c6-161">USD</span><span class="sxs-lookup"><span data-stu-id="ca5c6-161">USD</span></span>     |
| <span data-ttu-id="ca5c6-162">My company_Band2</span><span class="sxs-lookup"><span data-stu-id="ca5c6-162">My company_Band2</span></span> | <span data-ttu-id="ca5c6-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="ca5c6-163">Contoso India</span></span> |<span data-ttu-id="ca5c6-164">Hour</span><span class="sxs-lookup"><span data-stu-id="ca5c6-164">Hour</span></span>|   <span data-ttu-id="ca5c6-165">67</span><span class="sxs-lookup"><span data-stu-id="ca5c6-165">67</span></span>|<span data-ttu-id="ca5c6-166">USD</span><span class="sxs-lookup"><span data-stu-id="ca5c6-166">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]