---
title: Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας συνόλων επιλογών και οντοτήτων στη δική σας λύση στην πλατφόρμα Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751661"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="7d091-103">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="7d091-103">Create custom fields and entities</span></span> 

<span data-ttu-id="7d091-104">Ολοκληρώστε τα παρακάτω βήματα κάθε φορά που θέλετε να δημιουργήσετε ένα προσαρμοσμένο σύνολο επιλογών ή μια οντότητα στην Power Apps πλατφόρμα.</span><span class="sxs-lookup"><span data-stu-id="7d091-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="7d091-105">Οι διαδικασίες αυτού του θέματος πρέπει να ολοκληρωθούν με χρήση του περιβάλλοντος εργασίας web του Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="7d091-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7d091-106">Συνιστούμε να κάνετε όλες τις προσαρμοσμένες αλλαγές διάστασης τιμολόγησης σε μια ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="7d091-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="7d091-107">Αυτή η σημαντική βέλτιστη πρακτική παρέχει την ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο, θα σας βοηθήσει με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία.</span><span class="sxs-lookup"><span data-stu-id="7d091-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="7d091-108">Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη λύση** και εισαγάγετέ την σε άλλες παρουσίες, για να επαναχρησιμοποιήσετε την ρύθμιση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="7d091-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="7d091-109">Δημιουργία προσαρμοσμένης λύσης για διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="7d091-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="7d091-110">Στο PSA, κάντε κλικ στις **Ρυθμίσεις** > **Λύσεις** και μετά επιλέξτε **Νέα** για να δημιουργήσετε μια νέα λύση.</span><span class="sxs-lookup"><span data-stu-id="7d091-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="7d091-111">Ονομάστε τη λύση, **\<το όνομα του οργανισμού σας> διαστάσεις τιμολόγησης**, καταχωρίστε τις υπόλοιπες πληροφορίες και πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="7d091-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![Δημιουργία προσαρμοσμένης λύσης για διαστάσεις τιμολόγησης](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="7d091-113">Δημιουργία προσαρμοσμένων πεδίων και συνόλων επιλογών στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="7d091-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="7d091-114">Μια διάσταση τιμολόγησης μπορεί να είναι μια σύνολο επιλογών ή μια οντότητα.</span><span class="sxs-lookup"><span data-stu-id="7d091-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="7d091-115">Και τα δύο πρέπει να δημιουργηθούν στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="7d091-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="7d091-116">Τα βήματα σε αυτήν τη διαδικασία εξηγούν πώς μπορείτε να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες και διαστάσεις που βασίζονται σε σύνολα επιλογών.</span><span class="sxs-lookup"><span data-stu-id="7d091-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="7d091-117">Διαστάσεις βάσει οντότητας</span><span class="sxs-lookup"><span data-stu-id="7d091-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="7d091-118">Στο PSA, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και μετά κάντε διπλό κλικ στο **\<your organization name> pricing dimensions**.</span><span class="sxs-lookup"><span data-stu-id="7d091-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="7d091-119">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="7d091-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="7d091-120">Κάντε κλικ στην επιλογή **Νέα** για να δημιουργήσετε μια νέα οντότητα που καλείται **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="7d091-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="7d091-121">Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια, πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="7d091-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![Ορισμός τυπικού τίτλου οντότητας](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="7d091-123">Διαστάσεις που βασίζονται σε σύνολο επιλογών</span><span class="sxs-lookup"><span data-stu-id="7d091-123">Option set-based dimensions</span></span> 
<span data-ttu-id="7d091-124">Μπορείτε να δημιουργήσετε δύο διαστάσεις που βασίζονται σε σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="7d091-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="7d091-125">Χρησιμοποιήστε την **Τοποθεσία εργασίας πόρου** για να παρακολουθήσετε την τιμή της **Αρχικής** τοποθεσίας εργασίας και την **Επί τόπου** εργασία και να χρησιμοποιήσετε τις **Ώρες εργασίας πόρου** με τιμές **Κανονικές** και **Υπερωρίες** για να εφαρμόσετε μια αύξηση όταν ολοκληρωθεί η εργασία.</span><span class="sxs-lookup"><span data-stu-id="7d091-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="7d091-126">Στο PSA, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και μετά κάντε διπλό κλικ στο **\<your organization name> pricing dimensions**.</span><span class="sxs-lookup"><span data-stu-id="7d091-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="7d091-127">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Σύνολα επιλογών**.</span><span class="sxs-lookup"><span data-stu-id="7d091-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="7d091-128">Επιλέξτε **Νέο** για να δημιουργήσετε ένα νέο σύνολο επιλογών, καταγράψτε τις υπόλοιπες απαιτούμενες πληροφορίες και πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="7d091-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="7d091-129">Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Τοποθεσία εργασίας πόρου</span><span class="sxs-lookup"><span data-stu-id="7d091-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="7d091-130">Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Ώρες εργασίας πόρου</span><span class="sxs-lookup"><span data-stu-id="7d091-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="7d091-131">Δημιουργία δεδομένων για διαστάσεις βασισμένες σε οντότητες</span><span class="sxs-lookup"><span data-stu-id="7d091-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="7d091-132">Μπορείτε να δημιουργήσετε δεδομένα για διαστάσεις βασισμένες σε οντότητες με μη αυτόματο τρόπο ή χρησιμοποιώντας κλήσης εισαγωγής Microsoft Excel ή κλήσεις εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="7d091-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="7d091-133">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για τη δημιουργία δύο τυπικών τίτλων, **Μηχανικός συστημάτων** και **Επικεφαλής μηχανικός συστημάτων** από τη διάσταση βάσει οντότητας **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="7d091-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="7d091-134">Εάν τα δεδομένα που θέλετε να δημιουργήσετε είναι μικρά, όπως στο παρακάτω παράδειγμα, μπορείτε να χρησιμοποιήσετε μια τυπική φόρμα.</span><span class="sxs-lookup"><span data-stu-id="7d091-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="7d091-135">Στο PSA, επιλέξτε **Εύρεση για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="7d091-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="7d091-136">Επιλέξτε την οντότητα **Τυπικός τίτλος** και μετά επιλέξτε **Αποτελέσματα**.</span><span class="sxs-lookup"><span data-stu-id="7d091-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="7d091-137">Θα εμφανιστούν όλες οι γραμμές στην οντότητα **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="7d091-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="7d091-138">Επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="7d091-138">Click **New**.</span></span> <span data-ttu-id="7d091-139">Στο πεδίο **Όνομα**, καταχωρίστε "Μηχανικός συστήματος" και μετά πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="7d091-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="7d091-140">Κλείστε τη φόρμα.</span><span class="sxs-lookup"><span data-stu-id="7d091-140">Close the form.</span></span> 
4. <span data-ttu-id="7d091-141">Επαναλάβετε τα βήματα 1-3, για να δημιουργήσετε έναν άλλο τυπικό τίτλο για τον "επικεφαλής μηχανικό συστημάτων".</span><span class="sxs-lookup"><span data-stu-id="7d091-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="7d091-142">Δείγμα δεδομένων για την οντότητα τυπικού τίτλου</span><span class="sxs-lookup"><span data-stu-id="7d091-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="7d091-143">Προσθήκη όλων των απαιτούμενων οντοτήτων PSA και σχετικών στοιχείων στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="7d091-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="7d091-144">Θα πρέπει να προσθέσετε τις παρακάτω οντότητες Project Service στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="7d091-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="7d091-145">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για να κάνετε κάποιες σημαντικές αλλαγές σχήματος στη λύση τιμολόγησης, έτσι ώστε οι οντότητες να συνειδητοποιήσουν τις νέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="7d091-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="7d091-146">Στο PSA, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και μετά κάντε διπλό κλικ στο **\<your organization name> pricing dimensions**.</span><span class="sxs-lookup"><span data-stu-id="7d091-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="7d091-147">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Προσθήκη υπάρχουσας** > **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="7d091-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="7d091-148">Στο παράθυρο διαλόγου **Στοιχεία λύσης**, επιλέξτε τις ακόλουθες οντότητες:</span><span class="sxs-lookup"><span data-stu-id="7d091-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="7d091-149">Πραγματικό</span><span class="sxs-lookup"><span data-stu-id="7d091-149">Actual</span></span>
- <span data-ttu-id="7d091-150">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="7d091-150">Bookable Resource</span></span>
- <span data-ttu-id="7d091-151">Γραμμή εκτίμησης</span><span class="sxs-lookup"><span data-stu-id="7d091-151">Estimate Line</span></span>
- <span data-ttu-id="7d091-152">Λεπτομέρεια γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="7d091-152">Invoice Line Detail</span></span>
- <span data-ttu-id="7d091-153">Γραμμή ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="7d091-153">Journal Line</span></span>
- <span data-ttu-id="7d091-154">Λεπτομέρεια γραμμής σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="7d091-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="7d091-155">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="7d091-155">Project Team Member</span></span>
- <span data-ttu-id="7d091-156">Λεπτομέρειες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="7d091-156">Quote Line Detail</span></span>
- <span data-ttu-id="7d091-157">Αύξηση τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="7d091-157">Role Price Markup</span></span>
- <span data-ttu-id="7d091-158">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="7d091-158">Role Price</span></span> 
- <span data-ttu-id="7d091-159">Χρονική καταχώρηση</span><span class="sxs-lookup"><span data-stu-id="7d091-159">Time Entry</span></span> 

> ![Προσθήκη υπαρχουσών οντοτήτων στη λύση "διαστάσεις τιμολόγησης"](media/Existing-entities-to-PD-solution.png)

> ![Επιλέξτε στοιχεία λύσης](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="7d091-162">Βεβαιωθείτε ότι θα συμπεριλάβετε όλες τις φόρμες και τις προβολές για κάθε μια από τις οντότητες που επιλέγονται.</span><span class="sxs-lookup"><span data-stu-id="7d091-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="7d091-163">Όταν σας ζητηθεί να συμπεριλάβετε εξαρτημένες οντότητες για τις οντότητες που επιλέξατε παραπάνω πατήστε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="7d091-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![Να μην συμπεριληφθούν όλα τα απαιτούμενα στοιχεία.](media/Do-not-include-required.png)


