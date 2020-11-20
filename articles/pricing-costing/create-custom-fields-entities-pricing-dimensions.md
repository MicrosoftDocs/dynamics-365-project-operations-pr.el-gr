---
title: Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προσαρμοσμένων συνόλων επιλογών ή οντοτήτων.
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
ms.openlocfilehash: 616bcd5758b434b45bd06aa1a026f32efc8b7f99
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130893"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="d37b9-103">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="d37b9-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="d37b9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d37b9-105">Ολοκληρώστε τα παρακάτω βήματα κάθε φορά που θέλετε να δημιουργήσετε ένα προσαρμοσμένο σύνολο επιλογών ή μια οντότητα.</span><span class="sxs-lookup"><span data-stu-id="d37b9-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d37b9-106">Συνιστούμε να κάνετε όλες τις προσαρμοσμένες αλλαγές διάστασης τιμολόγησης σε μια ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="d37b9-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="d37b9-107">Αυτή η σημαντική βέλτιστη πρακτική παρέχει την ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο, θα σας βοηθήσει με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία.</span><span class="sxs-lookup"><span data-stu-id="d37b9-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="d37b9-108">Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη λύση** και εισαγάγετέ την σε άλλες παρουσίες, για να επαναχρησιμοποιήσετε την ρύθμιση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="d37b9-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="d37b9-109">Δημιουργία προσαρμοσμένης λύσης για διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="d37b9-110">Κάντε κλικ στις **Ρυθμίσεις** > **Λύσεις** και μετά επιλέξτε **Νέα** για να δημιουργήσετε μια νέα λύση.</span><span class="sxs-lookup"><span data-stu-id="d37b9-110">Go to **Settings** > **Solutions**, and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="d37b9-111">Ονομάστε τη λύση, **\<your organization name> διαστάσεις τιμολόγησης**, καταχωρίστε τις υπόλοιπες πληροφορίες και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="d37b9-112">Δημιουργία προσαρμοσμένων πεδίων και συνόλων επιλογών στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="d37b9-113">Μια διάσταση τιμολόγησης μπορεί να είναι μια σύνολο επιλογών ή μια οντότητα.</span><span class="sxs-lookup"><span data-stu-id="d37b9-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="d37b9-114">Και τα δύο πρέπει να δημιουργηθούν στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="d37b9-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="d37b9-115">Τα βήματα σε αυτήν τη διαδικασία εξηγούν πώς μπορείτε να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες και διαστάσεις που βασίζονται σε σύνολα επιλογών.</span><span class="sxs-lookup"><span data-stu-id="d37b9-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="d37b9-116">Διαστάσεις βάσει οντότητας</span><span class="sxs-lookup"><span data-stu-id="d37b9-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="d37b9-117">Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-117">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="d37b9-118">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="d37b9-119">Επιλέξτε **Νέα** για να δημιουργήσετε μια νέα οντότητα που καλείται **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="d37b9-120">Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="d37b9-121">Διαστάσεις που βασίζονται σε σύνολο επιλογών</span><span class="sxs-lookup"><span data-stu-id="d37b9-121">Option set-based dimensions</span></span> 
<span data-ttu-id="d37b9-122">Μπορείτε να δημιουργήσετε δύο διαστάσεις που βασίζονται σε σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="d37b9-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="d37b9-123">Χρησιμοποιήστε την **Τοποθεσία εργασίας πόρου** για να παρακολουθήσετε την τιμή της **Αρχικής** τοποθεσίας εργασίας και την **Επί τόπου** εργασία και να χρησιμοποιήσετε τις **Ώρες εργασίας πόρου** με τιμές **Κανονικές** και **Υπερωρίες** για να εφαρμόσετε μια αύξηση όταν ολοκληρωθεί η εργασία.</span><span class="sxs-lookup"><span data-stu-id="d37b9-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="d37b9-124">Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-124">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="d37b9-125">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Σύνολα επιλογών**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="d37b9-126">Επιλέξτε **Νέο** για να δημιουργήσετε ένα νέο σύνολο επιλογών, καταγράψτε τις υπόλοιπες απαιτούμενες πληροφορίες και επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="d37b9-127">Δημιουργία δεδομένων για διαστάσεις βασισμένες σε οντότητες</span><span class="sxs-lookup"><span data-stu-id="d37b9-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="d37b9-128">Μπορείτε να δημιουργήσετε δεδομένα για διαστάσεις βασισμένες σε οντότητες με μη αυτόματο τρόπο ή χρησιμοποιώντας κλήσης εισαγωγής Microsoft Excel ή κλήσεις εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="d37b9-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="d37b9-129">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για τη δημιουργία δύο τυπικών τίτλων, **Μηχανικός συστημάτων** και **Επικεφαλής μηχανικός συστημάτων** από τη διάσταση βάσει οντότητας **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="d37b9-130">Εάν τα δεδομένα που θέλετε να δημιουργήσετε είναι μικρά, όπως στο παρακάτω παράδειγμα, μπορείτε να χρησιμοποιήσετε μια τυπική φόρμα.</span><span class="sxs-lookup"><span data-stu-id="d37b9-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="d37b9-131">Επιλέξτε **Πρόσθετα κριτήρια εύρεσης**, επιλέξτε την οντότητα **Τυπικός τίτλος** και, στη συνέχεια, επιλέξτε **Αποτελέσματα**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-131">Select **Advanced Find**, select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="d37b9-132">Θα εμφανιστούν όλες οι γραμμές στην οντότητα **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="d37b9-133">Επιλέξτε **Νέο** και στο πεδίο **Όνομα**, καταχωρίστε "Μηχανικός συστήματος" και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-133">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="d37b9-134">Κλείσιμο της φόρμας.</span><span class="sxs-lookup"><span data-stu-id="d37b9-134">Close the form.</span></span> 
4. <span data-ttu-id="d37b9-135">Επαναλάβετε τα βήματα 1-3, για να δημιουργήσετε έναν άλλο τυπικό τίτλο για τον "επικεφαλής μηχανικό συστημάτων".</span><span class="sxs-lookup"><span data-stu-id="d37b9-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="d37b9-136">Προσθήκη όλων των απαιτούμενων οντοτήτων και σχετικών στοιχείων στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="d37b9-137">Θα πρέπει να προσθέσετε τις παρακάτω οντότητες στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="d37b9-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="d37b9-138">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για να κάνετε κάποιες σημαντικές αλλαγές σχήματος στη λύση τιμολόγησης, έτσι ώστε οι οντότητες να συνειδητοποιήσουν τις νέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="d37b9-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="d37b9-139">Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-139">Select **Settings** > **Solutions**, and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="d37b9-140">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Προσθήκη υπάρχουσας** > **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="d37b9-141">Στο παράθυρο διαλόγου **Στοιχεία λύσης**, επιλέξτε τις ακόλουθες οντότητες:</span><span class="sxs-lookup"><span data-stu-id="d37b9-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="d37b9-142">Πραγματικό</span><span class="sxs-lookup"><span data-stu-id="d37b9-142">Actual</span></span>
  - <span data-ttu-id="d37b9-143">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-143">Bookable Resource</span></span>
  - <span data-ttu-id="d37b9-144">Γραμμή εκτίμησης</span><span class="sxs-lookup"><span data-stu-id="d37b9-144">Estimate Line</span></span>
  - <span data-ttu-id="d37b9-145">Λεπτομέρεια γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="d37b9-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="d37b9-146">Γραμμή ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="d37b9-146">Journal Line</span></span>
  - <span data-ttu-id="d37b9-147">Λεπτομέρεια γραμμής σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="d37b9-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="d37b9-148">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="d37b9-148">Project Team Member</span></span>
  - <span data-ttu-id="d37b9-149">Λεπτομέρειες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="d37b9-149">Quote Line Detail</span></span>
  - <span data-ttu-id="d37b9-150">Αύξηση τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="d37b9-150">Role Price Markup</span></span>
  - <span data-ttu-id="d37b9-151">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="d37b9-151">Role Price</span></span> 
  - <span data-ttu-id="d37b9-152">Χρονική καταχώρηση</span><span class="sxs-lookup"><span data-stu-id="d37b9-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="d37b9-153">Βεβαιωθείτε ότι θα συμπεριλάβετε όλες τις φόρμες και τις προβολές για κάθε μια από τις οντότητες που επιλέγονται.</span><span class="sxs-lookup"><span data-stu-id="d37b9-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="d37b9-154">Όταν σας ζητηθεί να συμπεριλάβετε εξαρτημένες οντότητες για τις οντότητες που επιλέξατε παραπάνω, επιλέξτε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="d37b9-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

