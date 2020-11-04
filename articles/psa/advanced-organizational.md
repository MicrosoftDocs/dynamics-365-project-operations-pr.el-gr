---
title: Οργανικές μονάδες
description: Αυτό το θέμα παρέχει συνδέσεις σε πληροφορίες σχετικά με τις οργανικές μονάδες στο Dynamics 365 Project Service Automation.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/04/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 454d9a4c4d139f493adf4604f8ba40a0211f0eec
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077028"
---
# <a name="organizational-units"></a><span data-ttu-id="c858f-103">Οργανικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="c858f-103">Organizational units</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="c858f-104">Στο Dynamics 365 Project Service Automation μια οργανωτική μονάδα είναι μια διακριτή ομάδα ή διαίρεση σε μια εταιρεία επαγγελματικής εξυπηρέτησης που χρησιμοποιεί χρεώσιμους πόρους που έχουν χρεώσεις κόστους.</span><span class="sxs-lookup"><span data-stu-id="c858f-104">Dynamics 365 Project Service Automation, an organizational unit is a distinct group or division in a professional services company that employs billable resources that have cost rates.</span></span>

<span data-ttu-id="c858f-105">Για εταιρείες επαγγελματικής εξυπηρέτησης που χρησιμοποιούν τεχνικούς πόρους σε διάφορες περιοχές πρακτικής ή επιχειρηματικές γραμμές, το κόστος για την πλήρωση ενός ρόλου σε μια περιοχή πρακτικής άσκησης ή μια επιχειρηματική γραμμή μπορεί να διαφέρει από το κόστος για την πλήρωση ενός ρόλου σε μια άλλη περιοχή πρακτικής ή επιχειρηματικής γραμμής.</span><span class="sxs-lookup"><span data-stu-id="c858f-105">For professional services companies that employ technical resources in various practice areas or business lines, the cost to fill a role in one practice area or business line might differ from the cost to fill a role in another practice area or business line.</span></span> <span data-ttu-id="c858f-106">Οι οργανικές βοηθούν σε αυτό το σενάριο, παρέχοντας έναν τρόπο για να ομαδοποιήσετε ένα σύνολο χρεώσιμων ρόλων σε ένα τμήμα μιας εταιρείας που έχει μια διακριτή δομή κόστους για αυτούς τους ρόλους.</span><span class="sxs-lookup"><span data-stu-id="c858f-106">The concept  organizational units helps in this scenario by providing a way to group a set of billable roles in a division of a company that has a distinct cost structure for these roles.</span></span>

## <a name="key-attributes-and-associations-of-organizational-units"></a><span data-ttu-id="c858f-107">Βασικά χαρακτηριστικά και συσχετισμοί οργανικών μονάδων</span><span class="sxs-lookup"><span data-stu-id="c858f-107">Key attributes and associations of organizational units</span></span>

<span data-ttu-id="c858f-108">Στο PSA, μια οργανική μονάδα στο PSA έχει ένα συγκεκριμένο νόμισμα και συγκεκριμένους τιμοκαταλόγους κόστους.</span><span class="sxs-lookup"><span data-stu-id="c858f-108">In PSA, an organizational unit in PSA has a specific currency and specific cost price lists.</span></span>

<span data-ttu-id="c858f-109">Η νομισματική μονάδα μιας οργανικής μονάδας είναι η κύρια νομισματική μονάδα που χρησιμοποιείται για την παρακολούθηση του κόστους.</span><span class="sxs-lookup"><span data-stu-id="c858f-109">The currency of an organizational unit is the primary currency that is used to track costs.</span></span>

<span data-ttu-id="c858f-110">Ένας ή περισσότεροι τιμοκατάλογοι κόστους μπορούν να επισυναφθούν με κάθε οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-110">One or more cost price lists can be attached to each organizational unit.</span></span> <span data-ttu-id="c858f-111">Το PSA θέτει τους ακόλουθους περιορισμούς στους τιμοκαταλόγους που μπορούν να επισυναφθούν σε μια οργανωτική μονάδα:</span><span class="sxs-lookup"><span data-stu-id="c858f-111">PSA puts the following limitations on the price lists that can be attached to an organizational unit:</span></span>

- <span data-ttu-id="c858f-112">Οι τιμοκατάλογοι πρέπει να είναι στη νομισματική μονάδα της οργανωτικής μονάδας</span><span class="sxs-lookup"><span data-stu-id="c858f-112">Price lists must be in the currency of the organizational unit</span></span>
- <span data-ttu-id="c858f-113">Οι τιμοκατάλογοι πρέπει να είναι τιμοκατάλογοι κόστους</span><span class="sxs-lookup"><span data-stu-id="c858f-113">Price lists must be of cost price lists</span></span>

<span data-ttu-id="c858f-114">Επιπλέον, υπάρχει ένα χαρακτηριστικό για την οργανωτική μονάδα στην οντότητα "Πόρος".</span><span class="sxs-lookup"><span data-stu-id="c858f-114">In addition, there is an attribute for the organizational unit on the Resource entity.</span></span> <span data-ttu-id="c858f-115">Κάθε πόρος μπορεί να αντιστοιχιστεί μόνο σε μία οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-115">Each resource can be assigned to one organizational unit.</span></span>

## <a name="roles-of-organizational-units"></a><span data-ttu-id="c858f-116">Ρόλοι οργανικών μονάδων</span><span class="sxs-lookup"><span data-stu-id="c858f-116">Roles of organizational units</span></span>

<span data-ttu-id="c858f-117">Η οργανωτική μονάδα παίζει δύο ρόλους στο PSA:</span><span class="sxs-lookup"><span data-stu-id="c858f-117">The organizational unit plays two roles in PSA:</span></span>

- <span data-ttu-id="c858f-118">**Αναθέτουσα μονάδα** – Η οργανωτική μονάδα που εκπροσωπεί την ομάδα ή τη διαίρεση της εταιρείας η οποία είναι κατά κύριο λόγο υπεύθυνη για την επιτυχία της πώλησης και τη διαχείριση της παροχής της εργασίας και των υπηρεσιών στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="c858f-118">**Contracting unit** – The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> <span data-ttu-id="c858f-119">Η αναθέτουσα μονάδα προσδιορίζεται από το πεδίο **Οργανική μονάδα** στην ενότητα κεφαλίδας των σελίδων **Ευκαιρία** , **Προσφορά** , **Σύμβαση έργου** και **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="c858f-119">The contracting unit is identified by the **Contracting Unit** field in the header section of the **Opportunity** , **Quote** , **Project Contract** , and **Project** pages.</span></span>
- <span data-ttu-id="c858f-120">**Μονάδα πόρων** - Η οργανωτική μονάδα στην οποία ανήκει ή έχει ανατεθεί ένας πόρος.</span><span class="sxs-lookup"><span data-stu-id="c858f-120">**Resourcing unit** – The organizational unit that a resource belongs to or is assigned to.</span></span> <span data-ttu-id="c858f-121">Αυτή η οργανωτική μονάδα μπορεί να παρέχει τους πόρους της για ορισμένους ρόλους στις δηλώσεις εργασίας (SOW) και τα έργα που ανήκουν στην αναθέτουσα μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-121">This organizational unit can provide its resources for some roles on statements of work (SOWs) and projects that are owned by the contracting unit.</span></span>

> ![Αναθέτουσες μονάδες και μονάδες πόρων](media/advanced-1.png)

## <a name="organizational-unit-faqs"></a><span data-ttu-id="c858f-123">Συνήθεις ερωτήσεις για την οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="c858f-123">Organizational unit FAQs</span></span>

<span data-ttu-id="c858f-124">Εδώ θα βρείτε ορισμένες από τις πιο συνήθεις ερωτήσεις σχετικά με τις οργανικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-124">Here are some of the most frequently asked questions about organizational units.</span></span>

### <a name="how-is-the-organizational-unit-entity-in-psa-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a><span data-ttu-id="c858f-125">Πώς είναι η οντότητα οργανωτικής μονάδας στο PSA που σχετίζεται με την οντότητα "οργανισμός" η οποία υπάρχει ήδη στο Dynamics 365;</span><span class="sxs-lookup"><span data-stu-id="c858f-125">How is the Organizational Unit entity in PSA related to the Organization entity that already exists in Dynamics 365?</span></span>

<span data-ttu-id="c858f-126">Η οργανωτική μονάδα στο Microsoft Dynamics 365 αντιπροσωπεύει το όνομα μιας παρουσίας καθολικού Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c858f-126">The Organization entity in Microsoft Dynamics 365 represents the name of a global Dynamics 365 instance.</span></span> <span data-ttu-id="c858f-127">Αυτό το όνομα είναι συνήθως το όνομα της καθολικής επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="c858f-127">This name is usually the name of the global enterprise.</span></span>

<span data-ttu-id="c858f-128">Η οντότητα "οργανωτική μονάδα" αντιπροσωπεύει μια ομάδα ή ένα τμήμα της καθολικής επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="c858f-128">The Organizational Unit entity represents a group or division in the global enterprise.</span></span> <span data-ttu-id="c858f-129">Αυτή η ομάδα ή η διεύθυνση έχει ένα σύνολο ρόλων και έναν τιμοκατάλογο για αυτούς τους ρόλους και αυτοί οι ρόλοι και ο τιμοκατάλογος διαφέρουν από τους ρόλους και τον τιμοκατάλογο άλλων ομάδων ή τμημάτων της επιχείρησης.</span><span class="sxs-lookup"><span data-stu-id="c858f-129">This group or division has a set of roles and a cost price list for those roles, and those roles and price list differ from the roles and price list of other groups or divisions in the enterprise.</span></span>

<span data-ttu-id="c858f-130">Όταν το PSA είναι εγκατεστημένο, δημιουργείται μια προεπιλεγμένη οργανωτική μονάδα με βάση τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="c858f-130">When PSA is installed, a default organizational unit is created based on the organization.</span></span> <span data-ttu-id="c858f-131">Όλοι οι υπάρχοντες πόροι αντιστοιχίζονται στην προεπιλεγμένη οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-131">All existing resources are assigned to the default organizational unit.</span></span> <span data-ttu-id="c858f-132">Εάν εισαχθούν νέοι χρήστες ή πόροι της υπηρεσίας καταλόγου Active Directory στο Dynamics 365, η διεργασία εισαγωγής χρήστη τους αντιστοιχίζει την προεπιλεγμένη οργανωτική μονάδα στο PSA.</span><span class="sxs-lookup"><span data-stu-id="c858f-132">If any new Active Directory users or resources are imported into Dynamics 365, the user import process assigns them to the default organizational unit in PSA.</span></span>
 
### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a><span data-ttu-id="c858f-133">Πώς η οργανωτική μονάδα είναι διαφορετική από την οντότητα "επιχειρηματική μονάδα";</span><span class="sxs-lookup"><span data-stu-id="c858f-133">How does the organizational unit entity differ from the business unit entity?</span></span>

<span data-ttu-id="c858f-134">Στο Dynamics 365, η οντότητα επιχειρηματικής μονάδας είναι μια κατασκευή ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="c858f-134">In Dynamics 365, the Business Unit entity is a security construct.</span></span> <span data-ttu-id="c858f-135">Η συσχέτιση ενός χρήστη με μια επιχειρηματική μονάδα καθορίζει τις οντότητες και τις καρτέλες οντοτήτων στις οποίες έχει πρόσβαση ο χρήστης.</span><span class="sxs-lookup"><span data-stu-id="c858f-135">The association of a user with a business unit determines the entities and entity records that the user has access to.</span></span> <span data-ttu-id="c858f-136">Προσδιορίζει επίσης τα δικαιώματα (δημιουργία, ανάγνωση, εγγραφή, διαγραφή, προσάρτηση, προσάρτηση σε, ανάθεση ή κοινή χρήση) που έχει ο χρήστης για αυτές τις καρτέλες οντότητας.</span><span class="sxs-lookup"><span data-stu-id="c858f-136">It also determines the permissions (Create, Read, Write, Delete, Append, Append To, Assign, or Share) that the user has for those entity records.</span></span>

<span data-ttu-id="c858f-137">Η οντότητα "οργανωτική μονάδα" αντιπροσωπεύει μια ομάδα ή μια ομάδα εταιρειών με διακριτούς συντελεστές κόστους για τους υπαλλήλους που της έχουν ανατεθεί.</span><span class="sxs-lookup"><span data-stu-id="c858f-137">The Organizational Unit entity represents a company group or division that has distinct cost rates for employees that are assigned to it.</span></span> <span data-ttu-id="c858f-138">Η συσχέτιση ενός πόρου με μια οργανική μονάδα προσδιορίζει το κόστος του πόρου σε μια δέσμευση έργου.</span><span class="sxs-lookup"><span data-stu-id="c858f-138">The association of a resource with an organizational unit determines the resource's cost to a project engagement.</span></span>

<span data-ttu-id="c858f-139">Όταν υλοποιείτε το Dynamics 365, βελτιστοποιήστε την εξουσιοδότηση ασφαλείας για την ιεραρχία των επιχειρηματικών μονάδων και την εκχώρηση χρηστών σε επιχειρηματικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-139">When you implement Dynamics 365, optimize security authorization for the hierarchy of business units and the assignment of users to business units.</span></span> <span data-ttu-id="c858f-140">Αναθέστε σε όλους τους χρήστες που πρέπει να έχουν πρόσβαση συνήθως στο ίδιο σύνολο καρτελών την ίδια επιχειρηματική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-140">Assign all users who must typically access the same set of records to the same business unit.</span></span> <span data-ttu-id="c858f-141">Η οργανωτική μονάδα δεν επηρεάζει την εξουσιοδότηση ασφαλείας ή την πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="c858f-141">The organizational unit has no effect on security authorization or access.</span></span>

#### <a name="example-of-organizational-units-and-business-units"></a><span data-ttu-id="c858f-142">Παράδειγμα οργανωτικών μονάδων και επιχειρηματικών μονάδων</span><span class="sxs-lookup"><span data-stu-id="c858f-142">Example of organizational units and business units</span></span>

<span data-ttu-id="c858f-143">Η Contoso, Ltd. έχει μια ακμάζουσα τεχνολογική πρακτική της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c858f-143">Contoso, Ltd. has a thriving Microsoft technology practice.</span></span> <span data-ttu-id="c858f-144">Ο Φίλιππος και η Κατερίνα είναι\# προγραμματιστές, αλλά η Κατερίνα είναι στις Ηνωμένες Πολιτείες, ενώ ο Φίλιππος είναι στην Ινδία.</span><span class="sxs-lookup"><span data-stu-id="c858f-144">Prakash and Tricia are both C\# developers, but Tricia is in the United States, whereas Prakash is in India.</span></span> <span data-ttu-id="c858f-145">Οι περισσότερες από τις δεσμεύσεις του έργου απαιτούν πόρους από την Contoso India και την Contoso US, ενώ ο Φίλιππος και η Κατερίνα απαιτούν το ίδιο επίπεδο πρόσβασης ασφαλείας σε έργα σε αυτήν την περιοχή πρακτικής.</span><span class="sxs-lookup"><span data-stu-id="c858f-145">Most of the project engagements require resources from Contoso India and Contoso US, and Prakash and Tricia require the same level of security access to projects in this practice area.</span></span> <span data-ttu-id="c858f-146">Ωστόσο, το κόστος των προγραμματιστών από την Contoso India διαφέρει σημαντικά από το κόστος των προγραμματιστών από την Contoso US.</span><span class="sxs-lookup"><span data-stu-id="c858f-146">However, the cost of developers from Contoso India differs significantly from the cost of developers from Contoso US.</span></span>

<span data-ttu-id="c858f-147">Εδώ είναι ένας βέλτιστος τρόπος για να σχεδιάσετε το σενάριο αυτό χρησιμοποιώντας το Dynamics 365 και το PSA.</span><span class="sxs-lookup"><span data-stu-id="c858f-147">Here is an optimal way to design for this scenario by using Dynamics 365 and PSA.</span></span>

1. <span data-ttu-id="c858f-148">Δημιουργήστε την πρακτική της τεχνολογίας της Microsoft ως επιχειρηματική μονάδα και συσχετίστε τον Φίλιππο και την Κατερίνα.</span><span class="sxs-lookup"><span data-stu-id="c858f-148">Create the Microsoft technology practice as a business unit, and associate Prakash and Tricia with it.</span></span> <span data-ttu-id="c858f-149">Με αυτόν τον τρόπο, μπορείτε να εγγυηθείτε ότι και οι δύο υπάλληλοι έχουν το ίδιο επίπεδο πρόσβασης ασφαλείας σε όλα τα έργα στην εν λόγω περιοχή πρακτικής.</span><span class="sxs-lookup"><span data-stu-id="c858f-149">In this way, you help guarantee that both employees have the same level of security access to any projects in that practice area.</span></span> <span data-ttu-id="c858f-150">Και οι δύο θα είναι σε θέση να ελέγχουν την πρόοδο και την αναφορά χρόνου, εξόδων και ενημερώσεων εργασιών.</span><span class="sxs-lookup"><span data-stu-id="c858f-150">They both will be able to check progress and report time, expenses, and task updates.</span></span> 
2. <span data-ttu-id="c858f-151">Δημιουργήστε δύο οργανωτικές μονάδες για να εγγυηθείτε ότι το κόστος του έργου αντικατοπτρίζεται σωστά.</span><span class="sxs-lookup"><span data-stu-id="c858f-151">Create two organizational units to hel guarantee that the cost to the project is correctly reflected.</span></span> 
3. <span data-ttu-id="c858f-152">Συσχετίστε την Κατερίνα με την Contoso US και τον Φίλιππο με την Contoso India.</span><span class="sxs-lookup"><span data-stu-id="c858f-152">Associate Tricia wtih Contoso US and associate Prakash with Contoso India.</span></span>
4. <span data-ttu-id="c858f-153">Ανάθεση κατάλληλων τιμοκαταλόγων κόστους και στις δύο οργανωτικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-153">Assign appropriate cost price lists to both organizational units.</span></span> <span data-ttu-id="c858f-154">Με αυτόν τον τρόπο, μπορείτε να εγγυηθείτε ότι το κόστος που καταγράφηκε στο έργο για τον Φίλιππο και την Κατερίνα αντικατοπτρίζει με ακρίβεια τη διαφορά κόστους ανάμεσα στις Contoso US και Contoso India.</span><span class="sxs-lookup"><span data-stu-id="c858f-154">TIn this way, you help guarantee that the costs that are recorded on the project for Prakash and Tricia accurately reflect the difference in costs between Contoso US and Contoso India.</span></span>

### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a><span data-ttu-id="c858f-155">Οι οργανωτικές μονάδες σχετίζονται με περιφέρειες πωλήσεων στο Dynamics 365;</span><span class="sxs-lookup"><span data-stu-id="c858f-155">Are organizational units related to sales territories in Dynamics 365?</span></span>

<span data-ttu-id="c858f-156">Δεν υπάρχει συσχετισμός ή σχέση ανάμεσα στις περιφέρειες πωλήσεων και τις οργανωτικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-156">There is no association or relationship between sales territories and organizational units.</span></span> <span data-ttu-id="c858f-157">Μια περιφέρεια πωλήσεων είναι συνήθως μια γεωγραφική περιοχή όπου πραγματοποιούνται οι πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="c858f-157">A sales territory is typically a geographical area where sales occur.</span></span> <span data-ttu-id="c858f-158">Ένας τιμοκατάλογος πωλήσεων μπορεί να συσχετιστεί με κάθε περιφέρεια πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="c858f-158">A sales price list can be associated with each sales territory.</span></span>

<span data-ttu-id="c858f-159">Μια οργανική μονάδα είναι μια εσωτερική ομάδα ή ένα τμήμα της εταιρείας που παρακολουθεί το κόστος για ένα σύνολο ρόλων που πωλεί σε άλλα τμήματα ή σε εξωτερικούς πελάτες.</span><span class="sxs-lookup"><span data-stu-id="c858f-159">An organizational unit is an internal group or division in the company that tracks costs for a set of roles that it sells to other divisions or to external customers.</span></span>

#### <a name="example-of-organizational-units-and-sales-territories"></a><span data-ttu-id="c858f-160">Παράδειγμα οργανωτικών μονάδων και περιφερειών πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="c858f-160">Example of organizational units and sales territories</span></span>

<span data-ttu-id="c858f-161">Η Contoso, Ltd. διαθέτει δύο κέντρα ανάπτυξης: την Contoso US και την Contoso India.</span><span class="sxs-lookup"><span data-stu-id="c858f-161">Contoso, Ltd. has two development centers: Contoso US and Contoso India.</span></span> <span data-ttu-id="c858f-162">Το κόστος των πόρων διαφέρει σημαντικά μεταξύ αυτών των δύο κέντρων ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="c858f-162">Costs of resources differ greatly between these two development centers.</span></span>

<span data-ttu-id="c858f-163">Η Contoso πουλά τις υπηρεσίες IT σε πολλές διεθνείς αγορές, όπως η Λατινική Αμερική, η Βόρεια Αμερική, η Ασία-Ειρηνικός, η Δυτική Ευρώπη και η Μέση Ανατολή.</span><span class="sxs-lookup"><span data-stu-id="c858f-163">Contoso sells its IT services in many international markets, such as Latin America, North America, Asia-Pacific, Western Europe, and the Middle East.</span></span> <span data-ttu-id="c858f-164">Τα ποσοστά χρέωσης για τους ίδιους ρόλους έργου μπορούν να ποικίλλουν σημαντικά στις εν λόγω αγορές.</span><span class="sxs-lookup"><span data-stu-id="c858f-164">Bill rates for the same project roles can vary widely across these markets.</span></span>

<span data-ttu-id="c858f-165">Οι Contoso US και Contoso India θα πρέπει να οριστούν ως οργανωτικές μονάδες και κάθε οργανωτική μονάδα θα πρέπει να έχει το δικό της τιμοκατάλογο κόστους.</span><span class="sxs-lookup"><span data-stu-id="c858f-165">Contoso US and Contoso India should be set up as organizational units, and each organizational unit should have its own cost price list.</span></span> <span data-ttu-id="c858f-166">Η Ασία-Ειρηνικός, η Λατινική Αμερική, η Βόρεια Αμερική, η Δυτική Ευρώπη και η Μέση Ανατολή θα πρέπει να οριστούν ως περιφέρειες πωλήσεων και κάθε περιφέρεια πωλήσεων θα πρέπει να έχει τον δικό της τιμοκατάλογο πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="c858f-166">Asia-Pacific, Latin America, North America, Western Europe, and the Middle East should be set up as sales territories, and each sales territory should have its own sales price list.</span></span>

### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a><span data-ttu-id="c858f-167">Γιατί υπάρχει περιορισμός στη συσχέτιση των τιμοκαταλόγου με οργανωτικές μονάδες;</span><span class="sxs-lookup"><span data-stu-id="c858f-167">Why is there a restriction on the association of price lists with organizational units?</span></span> 

<span data-ttu-id="c858f-168">Η τιμολόγηση των πωλήσεων είναι συνήθως μοναδική στις γεωγραφικές περιοχές ή στις αγορές όπου πωλούνται οι υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="c858f-168">Sales pricing is usually unique to the geographical areas or markets where services are sold.</span></span> <span data-ttu-id="c858f-169">Τα εσωτερικά τμήματα μιας εταιρείας δεν έχουν συνήθως τη δική τους τιμολόγηση πωλήσεων για τον ίδιο τύπο υπηρεσιών.</span><span class="sxs-lookup"><span data-stu-id="c858f-169">Internal divisions of a company don't usually have their own sales pricing for the same type of services.</span></span> <span data-ttu-id="c858f-170">Ωστόσο, οι εσωτερικές διαιρέσεις έχουν διαφορετικό κόστος πωληθέντων (COGS), ανάλογα με τις ικανότητες των ατόμων που χρησιμοποιούν και τις συνθήκες εργασίας της περιοχής όπου δραστηριοποιούνται.</span><span class="sxs-lookup"><span data-stu-id="c858f-170">However, internal divisions have a different cost of goods sold (COGS), depending on the skills of the people that they employ and the labor conditions of the region where they operate.</span></span> <span data-ttu-id="c858f-171">Επειδή οι οργανωτικές μονάδες διαμορφώνονται ως εσωτερικοί διαχωρισμοί μιας εταιρείας, μπορούν να έχουν μόνο τιμοκαταλόγους κόστους.</span><span class="sxs-lookup"><span data-stu-id="c858f-171">Because organizational units are modeled as internal divisions of a company, they can have only cost price lists.</span></span>

### <a name="why-cant-we-associate-sales-price-lists-to-organizational-units"></a><span data-ttu-id="c858f-172">Γιατί δεν είναι δυνατός ο συσχετισμός τιμοκαταλόγου πωλήσεων με τις οργανωτικές μονάδες;</span><span class="sxs-lookup"><span data-stu-id="c858f-172">Why can’t we associate sales price lists to organizational units?</span></span>

<span data-ttu-id="c858f-173">Στο PSA, οι τιμοκατάλογοι πωλήσεων μπορούν να συσχετιστούν με πελάτες και περιφέρειες πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="c858f-173">In PSA, sales price lists can be associated with customers and sales territories.</span></span> <span data-ttu-id="c858f-174">Οι οντότητες συναλλαγής, όπως η ευκαιρία, η προσφορά, η σύμβαση έργου και η χρήση τιμοκαταλόγου που είναι προσαρτημένες στο λογαριασμό πελάτη ή την περιφέρεια πωλήσεων, καθορίζουν τους συντελεστές χρέωσης και τα πιθανά έσοδα για την εμπλοκή του έργου.</span><span class="sxs-lookup"><span data-stu-id="c858f-174">Transactional entities like Opportunity, Quote, Project Contract, and Project use sales price lists that are attached to the customer account or the sales territory to determine bill rates and potential revenue on the project engagement.</span></span>

<span data-ttu-id="c858f-175">Οι τιμοκατάλογοι κόστους σχετίζονται με οργανωτικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-175">Cost price lists are associated with organizational units.</span></span> <span data-ttu-id="c858f-176">Οι οντότητες συναλλαγής, όπως οι λίστες ευκαιρίας, προσφοράς, σύμβασης έργου και χρήσης έργου, είναι προσαρτημένες στη μονάδα, για να καθορίσουν το κόστος σε μια δέσμευση έργου.</span><span class="sxs-lookup"><span data-stu-id="c858f-176">Transactional entities like Opportunity, Quote, Project Contract, and Project use cost price lists that are attached to the contracting unit to determine costs to a project engagement.</span></span>

### <a name="are-organizational-units-hierarchical-in-psa"></a><span data-ttu-id="c858f-177">Οι οργανωτικές μονάδες είναι ιεραρχικές στο PSA;</span><span class="sxs-lookup"><span data-stu-id="c858f-177">Are organizational units hierarchical in PSA?</span></span>

<span data-ttu-id="c858f-178">Αρ.</span><span class="sxs-lookup"><span data-stu-id="c858f-178">No.</span></span> <span data-ttu-id="c858f-179">Στην τρέχουσα έκδοση του PSA, οι οργανωτικές μονάδες δεν είναι ιεραρχικές.</span><span class="sxs-lookup"><span data-stu-id="c858f-179">In the current release of PSA, organizational units are not hierarchical.</span></span> <span data-ttu-id="c858f-180">Αυτό σημαίνει ότι δεν μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="c858f-180">This means that you can’t:</span></span>

- <span data-ttu-id="c858f-181">Ρυθμίστε τις παραμέτρους ενός μοτίβου για την προεπιλεγμένη τιμή κόστους που διασχίζει μια ιεραρχία.</span><span class="sxs-lookup"><span data-stu-id="c858f-181">Configure a pattern for defaulting cost prices that traverses up a hierarchy.</span></span> 
- <span data-ttu-id="c858f-182">Αναφορά εσόδων ή κόστους σε διαφορετικά επίπεδα της ιεραρχίας της οργανωτικής μονάδας.</span><span class="sxs-lookup"><span data-stu-id="c858f-182">Report revenue or cost rolled up at different levels of the organizational unit hierarchy.</span></span>

### <a name="were-a-big-multinational-firm-with-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-make-the-best-use-of-the-organizational-unit-concept-in-this-version-of-the-project-service-app"></a><span data-ttu-id="c858f-183">Είμαστε μια μεγάλη πολυεθνική εταιρεία με πολύπλοκη, πολυεπίπεδη ιεραρχία κέντρων κόστους, διαιρέσεων και γραφείων χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="c858f-183">We're a big multinational firm with a complex, multilevel hierarchy of cost centers, divisions, and billing offices.</span></span> <span data-ttu-id="c858f-184">Πώς μπορεί να χρησιμοποιηθεί καλύτερα η έννοια της οργανωτικής μονάδας σε αυτήν την έκδοση της εφαρμογής Project Service;</span><span class="sxs-lookup"><span data-stu-id="c858f-184">How can we make the best use of the organizational unit concept in this version of the Project Service app?</span></span>

<span data-ttu-id="c858f-185">Όταν έχετε μια πολύπλοκη ιεραρχία κέντρων κόστους, διαιρέσεων, γραφείων χρέωσης κ.λπ., ρυθμίστε τους κόμβους των φύλλων αυτής της ιεραρχίας ως ξεχωριστές οργανωτικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="c858f-185">When you have a complex hierarchy of cost centers, divisions, billing offices, etc., set up the leaf nodes of that hierarchy as distinct organizational units.</span></span>
<span data-ttu-id="c858f-186">Το παρακάτω παράδειγμα παρουσιάζει μια τυπική ιεραρχία:</span><span class="sxs-lookup"><span data-stu-id="c858f-186">The following example shows a typical hierarchy:</span></span>

<span data-ttu-id="c858f-187">**Contoso India**</span><span class="sxs-lookup"><span data-stu-id="c858f-187">**Contoso India**</span></span>

  - <span data-ttu-id="c858f-188">Πρακτική SAP</span><span class="sxs-lookup"><span data-stu-id="c858f-188">SAP Practice</span></span> 

    - <span data-ttu-id="c858f-189">Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-189">Technical Consultants</span></span> 
    - <span data-ttu-id="c858f-190">Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-190">Functional Consultants</span></span> 
    
  - <span data-ttu-id="c858f-191">Πρακτική τεχνολογίας της Microsoft</span><span class="sxs-lookup"><span data-stu-id="c858f-191">Microsoft Technology Practice</span></span> 

    - <span data-ttu-id="c858f-192">Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-192">Technical Consultants</span></span>
    - <span data-ttu-id="c858f-193">Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-193">Functional Consultants</span></span> 
    
<span data-ttu-id="c858f-194">**Contoso US**</span><span class="sxs-lookup"><span data-stu-id="c858f-194">**Contoso US**</span></span>

 - <span data-ttu-id="c858f-195">Πρακτική SAP</span><span class="sxs-lookup"><span data-stu-id="c858f-195">SAP Practice</span></span> 

    - <span data-ttu-id="c858f-196">Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-196">Technical Consultants</span></span> 
    - <span data-ttu-id="c858f-197">Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-197">Functional Consultants</span></span> 
    
 - <span data-ttu-id="c858f-198">Πρακτική τεχνολογίας της Microsoft</span><span class="sxs-lookup"><span data-stu-id="c858f-198">Microsoft Technology Practice</span></span> 

    - <span data-ttu-id="c858f-199">Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-199">Technical Consultants</span></span> 
    - <span data-ttu-id="c858f-200">Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-200">Functional Consultants</span></span> 
 
<span data-ttu-id="c858f-201">Εάν η ιεραρχία σας είναι παρόμοια, πρέπει να την ορίσετε ως επίπεδη λίστα, όπως παρουσιάζεται εδώ:</span><span class="sxs-lookup"><span data-stu-id="c858f-201">If your hierarchy is similar, you must set it up as a flat list, as shown here:</span></span>
- <span data-ttu-id="c858f-202">Contoso India - SAP πρακτική - Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-202">Contoso India - SAP Practice - Technical Consultants</span></span> 
- <span data-ttu-id="c858f-203">Contoso India - SAP πρακτική - Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-203">Contoso India - SAP Practice - Functional Consultants</span></span>       
- <span data-ttu-id="c858f-204">Contoso India - Πρακτική τεχνολογίας της Microsoft - Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-204">Contoso India - Microsoft Technology Practice Functional Consultants</span></span> 
- <span data-ttu-id="c858f-205">Contoso India - Πρακτική τεχνολογίας της Microsoft - Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-205">Contoso India - Microsoft Technology Practice Functional Consultants</span></span> 
- <span data-ttu-id="c858f-206">Contoso US - SAP πρακτική - Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-206">Contoso US - SAP Practice - Technical Consultants</span></span>  
- <span data-ttu-id="c858f-207">Contoso US - SAP πρακτική - Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-207">Contoso US - SAP Practice - Functional Consultants</span></span>  
- <span data-ttu-id="c858f-208">Contoso US - Πρακτική τεχνολογίας της Microsoft - Τεχνικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-208">Contoso US - Microsoft Technology Practice - Technical Consultants</span></span> 
- <span data-ttu-id="c858f-209">Contoso US - Πρακτική τεχνολογίας της Microsoft - Λειτουργικοί σύμβουλοι</span><span class="sxs-lookup"><span data-stu-id="c858f-209">Contoso US - Microsoft Technology Practice - Functional Consultants</span></span>

### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-organizational-unit-concept-in-the-current-version-of-psa"></a><span data-ttu-id="c858f-210">Είμαστε μια μικρή εταιρεία επαγγελματικής εξυπηρέτησης που λειτουργεί ως μόνο μία διεύθυνση.</span><span class="sxs-lookup"><span data-stu-id="c858f-210">We're a small professional services company that operates as only one division.</span></span> <span data-ttu-id="c858f-211">Πώς μπορεί να χρησιμοποιηθεί καλύτερα η έννοια της οργανωτικής μονάδας στην τρέχουσα έκδοση του PSA;</span><span class="sxs-lookup"><span data-stu-id="c858f-211">How can we best use the organizational unit concept in the current version of PSA?</span></span>

<span data-ttu-id="c858f-212">Εάν η εταιρεία σας λειτουργεί ως μία μονάδα που έχει έναν τιμοκατάλογο κόστους, δεν χρειάζεται να ορίσετε καμία οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-212">If your company operates as one unit that has one cost price list, you don't have to set up any organizational units.</span></span> <span data-ttu-id="c858f-213">Κατά τη διάρκεια της εγκατάστασης του PSA, το Dynamics 365 δημιουργεί μια προεπιλεγμένη οργανωτική μονάδα που έχει το ίδιο όνομα με τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="c858f-213">During PSA installation, Dynamics 365 creates one default organizational unit that has the same name as the organization.</span></span> <span data-ttu-id="c858f-214">Από προεπιλογή, όλοι οι υπάρχοντες πόροι αντιστοιχίζονται σε αυτήν την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-214">By default, all users are assigned to this organizational unit.</span></span> <span data-ttu-id="c858f-215">Κάθε φορά που το σύστημα απαιτεί να είναι επιλεγμένο μια οργανική μονάδα, αυτή η οργανωτική μονάδα επιλέγεται από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="c858f-215">Whenever the system requires that an organizational unit be selected, this organizational unit is selected by default.</span></span>

### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract-what-is-the-default-contracting-unit"></a><span data-ttu-id="c858f-216">Όταν δημιουργείται ένα έργο από μια προσφορά ή γραμμή σύμβασης έργου, η προεπιλεγμένη αναθέτουσα μονάδα προέρχεται από την προσφορά ή τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="c858f-216">When a project is created from a quote or project contract line, the default contracting unit comes from the quote or project contract.</span></span> <span data-ttu-id="c858f-217">Σε περίπτωση δημιουργίας ενός έργου πριν από τις οντότητες πωλήσεων, όπως η προσφορά ή η σύμβαση έργου, ποια είναι η προεπιλεγμένη αναθέτουσα μονάδα;</span><span class="sxs-lookup"><span data-stu-id="c858f-217">If a project is created before sales entities such as quote or project contract, what is the default contracting unit?</span></span>

<span data-ttu-id="c858f-218">Όταν ένα έργο δημιουργείται μόνο του, η προεπιλεγμένη αναθέτουσα μονάδα του έργου βασίζεται στο χρήστη που το δημιουργεί.</span><span class="sxs-lookup"><span data-stu-id="c858f-218">When a project is created on its own, the default contracting unit of the project is based on the user who creates it.</span></span> <span data-ttu-id="c858f-219">Αυτός ο χρήστης είναι επίσης ο προεπιλεγμένος διευθυντής έργου.</span><span class="sxs-lookup"><span data-stu-id="c858f-219">That user is also the default project manager.</span></span> <span data-ttu-id="c858f-220">Εάν το έργο έχει αντιστοιχιστεί σε μια οντότητα πωλήσεων, όπως μια προσφορά ή μια σύμβαση έργου, η αναθέτουσα μονάδα στο έργο βασίζεται αντί για την οντότητα "Πωλήσεις".</span><span class="sxs-lookup"><span data-stu-id="c858f-220">If the project is mapped to a sales entity such as a quote or project contract, the contracting unit on the project is based on the sales entity instead.</span></span> <span data-ttu-id="c858f-221">Σε αυτήν την περίπτωση, οι εκτιμήσεις έργου μπορεί να υπολογιστούν, επειδή ο τιμοκατάλογος κόστους χρησιμοποιείται για τον υπολογισμό των αλλαγών εκτίμησης κόστους σε περίπτωση που αλλάξει η αναθέτουσα μονάδα.</span><span class="sxs-lookup"><span data-stu-id="c858f-221">In this case, project estimates might be recalculated, because the cost price list is used to calculate the cost estimate changes if the contracting unit is changed.</span></span> <span data-ttu-id="c858f-222">Ο τιμοκατάλογος πωλήσεων χρησιμοποιείται για τον υπολογισμό των εκτιμήσεων πωλήσεων που θα αλλάξουν έτσι ώστε να είναι συγχρονισμένες με τον τιμοκατάλογο έργου της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="c858f-222">The sales price list is used to calculate the sales estimates that will be changed so that they are in sync with the project price list on the quote.</span></span>

<span data-ttu-id="c858f-223">Τα πεδία **Αναθέτουσα μονάδα** και **Νόμισμα** στο έργο κλειδώνονται για επεξεργασία, επειδή πρέπει να είναι συγχρονισμένα με τις τιμές της οντότητας πωλήσεων (προσφορά ή σύμβαση έργου) στην οποία έχει αντιστοιχιστεί το έργο.</span><span class="sxs-lookup"><span data-stu-id="c858f-223">The **Contracting Unit** and **Currency** fields on the project are locked for editing, because they must be in sync with the values on the sales entity (quote or project contract) that the project is mapped to.</span></span>