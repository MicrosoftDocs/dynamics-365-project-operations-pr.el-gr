---
title: Χρήση της κατηγορίας συναλλαγών ως διάστασης τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση μιας κατηγορίας συναλλαγής ως διάσταση τιμολόγησης.
author: Rumant
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
ms.openlocfilehash: 0019571a1d37d3b6a503e7221db3c3b51365c236
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077000"
---
# <a name="use-transaction-category-as-a-pricing-dimension"></a><span data-ttu-id="8386c-103">Χρήση της κατηγορίας συναλλαγών ως διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="8386c-103">Use transaction category as a pricing dimension</span></span>
<span data-ttu-id="8386c-104">Αυτό το θέμα δείχνει πώς να χρησιμοποιήσετε μια κατηγορία συναλλαγής ως διάσταση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="8386c-104">This topic shows how to use a transaction category as a pricing dimension.</span></span> <span data-ttu-id="8386c-105">Πριν ξεκινήσετε, εάν δεν έχετε ήδη δημιουργήσει μια λύση διάστασης τιμολόγησης, θα πρέπει να δημιουργήσετε μια νέα.</span><span class="sxs-lookup"><span data-stu-id="8386c-105">Before you begin, if you have not already created a pricing dimension solution, you will need to create a new one.</span></span> <span data-ttu-id="8386c-106">Εάν έχετε ήδη μια λύση διάστασης τιμολόγησης, τότε μπορείτε να κάνετε τις αλλαγές σας σε αυτήν τη λύση.</span><span class="sxs-lookup"><span data-stu-id="8386c-106">If you already have a pricing dimension solution, then you can make your changes in that solution.</span></span> <span data-ttu-id="8386c-107">Εάν δεν έχετε δημιουργήσει μια νέα λύση διάστασης τιμολόγησης για τον οργανισμό σας, ολοκληρώστε τις διαδικασίες στο θέμα [Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων](create-custom-fields-entities.md).</span><span class="sxs-lookup"><span data-stu-id="8386c-107">If you have not created a new pricing dimension solution for your organization, complete the procedures in the [Create custom fields and entities](create-custom-fields-entities.md) topic.</span></span>

## <a name="add-transaction-category-to-forms-and-views"></a><span data-ttu-id="8386c-108">Προσθήκη κατηγορίας συναλλαγής σε φόρμες και προβολές</span><span class="sxs-lookup"><span data-stu-id="8386c-108">Add transaction category to forms and views</span></span>
<span data-ttu-id="8386c-109">Για να είναι ορατή η κατηγορία συναλλαγής στο περιβάλλον εργασίας χρήστη στη λύση διάστασης τιμολόγησης, θα πρέπει να περιηγηθείτε σε όλες τις φόρμες και τις προβολές των βασικών οντοτήτων και να προσθέσετε αυτά τα πεδία στις φόρμες και τις προβολές αυτών των οντοτήτων.</span><span class="sxs-lookup"><span data-stu-id="8386c-109">To make transaction category visible in the UI in the pricing dimension solution, you will need to walk through all the forms and views of the key entities and add these fields to the forms and views of those entities.</span></span>
<span data-ttu-id="8386c-110">Ο παρακάτω πίνακας είναι μια αναλυτική λίστα με τις έτοιμες φόρμες και προβολές οι οποίες παρατίθενται ανά οντότητα και οι οποίες θα πρέπει να ενημερωθούν με τα νέα πεδία.</span><span class="sxs-lookup"><span data-stu-id="8386c-110">The following table is a comprehensive list of the out-of-the box forms and views, listed by entity, that will need to be updated with the new fields.</span></span> <span data-ttu-id="8386c-111">Εάν υπάρχουν πρόσθετες προβολές ή φόρμες στις προσαρμογές σας σε αυτές τις οντότητες, προσθέστε και αυτά τα νέα πεδία.</span><span class="sxs-lookup"><span data-stu-id="8386c-111">If there any additional views or forms in your customizations on these entities, add the new fields to those as well.</span></span>

|  <span data-ttu-id="8386c-112">Οντότητα</span><span class="sxs-lookup"><span data-stu-id="8386c-112">Entity</span></span>        | <span data-ttu-id="8386c-113">Φόρμες</span><span class="sxs-lookup"><span data-stu-id="8386c-113">Forms</span></span>     |<span data-ttu-id="8386c-114">Προβολές</span><span class="sxs-lookup"><span data-stu-id="8386c-114">Views</span></span>        |
| ------------------------------|---------------------------------|----------------------------------|
|  <span data-ttu-id="8386c-115">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="8386c-115">Role Price</span></span>|<span data-ttu-id="8386c-116">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-116">• Information</span></span> |<span data-ttu-id="8386c-117">• Ενεργές τιμές κατηγοριών πόρων</span><span class="sxs-lookup"><span data-stu-id="8386c-117">• Active Resource Category Prices</span></span><br> <span data-ttu-id="8386c-118">• Συσχετισμένη προβολή τιμής κατηγορίας πόρου</span><span class="sxs-lookup"><span data-stu-id="8386c-118">• Resource Category Price Associated View</span></span>|
|  <span data-ttu-id="8386c-119">Αύξηση τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="8386c-119">Role Price Markup</span></span>|<span data-ttu-id="8386c-120">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-120">• Information</span></span>|<span data-ttu-id="8386c-121">• Ενεργή αύξηση τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="8386c-121">• Active Role Price Markup</span></span><br><span data-ttu-id="8386c-122">• Συσχετισμένη προβολή αύξησης τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="8386c-122">• Role Price Markup Associated View</span></span>|
|  <span data-ttu-id="8386c-123">Λεπτομέρεια γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="8386c-123">Quote line detail</span></span>|<span data-ttu-id="8386c-124">• Πληροφορίες έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-124">• Project Information</span></span><br><span data-ttu-id="8386c-125">• Γρήγορη δημιουργία έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-125">• Project Quick Create</span></span>|<span data-ttu-id="8386c-126">• Ενεργή λεπτομέρεια γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="8386c-126">• Active Quote Line Detail</span></span><br><span data-ttu-id="8386c-127">• Συνδυασμένες λεπτομέρειες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="8386c-127">• Combined Quote Line Details</span></span><br><span data-ttu-id="8386c-128">• Συσχετισμένη προβολή λεπτομέρειας γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="8386c-128">• Quote Line Detail associated view</span></span>|
|  <span data-ttu-id="8386c-129">Λεπτομέρεια γραμμής σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-129">Project Contract line detail</span></span>|<span data-ttu-id="8386c-130">• Πληροφορίες έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-130">• Project Information</span></span><br><span data-ttu-id="8386c-131">• Γρήγορη δημιουργία έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-131">• Project Quick Create</span></span>|<span data-ttu-id="8386c-132">• Συνδυασμένες λεπτομέρειες γραμμής σύμβασης</span><span class="sxs-lookup"><span data-stu-id="8386c-132">• Combined Contract line Details</span></span><br><span data-ttu-id="8386c-133">• Ενεργές λεπτομέρειες γραμμής σύμβασης</span><span class="sxs-lookup"><span data-stu-id="8386c-133">• Active Contract Line Details</span></span><br><span data-ttu-id="8386c-134">• Συσχετισμένη προβολή λεπτομερειών γραμμής σύμβασης</span><span class="sxs-lookup"><span data-stu-id="8386c-134">• Contract Line Detail associated view</span></span>|
|  <span data-ttu-id="8386c-135">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-135">Project Task</span></span>|<span data-ttu-id="8386c-136">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-136">• Information</span></span><br><span data-ttu-id="8386c-137">• Νέα φόρμα</span><span class="sxs-lookup"><span data-stu-id="8386c-137">• New Form</span></span>||
|  <span data-ttu-id="8386c-138">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-138">Project Team Member</span></span>|<span data-ttu-id="8386c-139">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-139">• Information</span></span><br><span data-ttu-id="8386c-140">• Νέα φόρμα</span><span class="sxs-lookup"><span data-stu-id="8386c-140">• New Form</span></span>|<span data-ttu-id="8386c-141">• Ενεργά μέλη ομάδων έργων</span><span class="sxs-lookup"><span data-stu-id="8386c-141">• Active Project Team Members</span></span><br><span data-ttu-id="8386c-142">• Μέλη ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="8386c-142">• Project Team Members</span></span><br><span data-ttu-id="8386c-143">• Συσχετισμένη προβολή μελών ομάδων έργων</span><span class="sxs-lookup"><span data-stu-id="8386c-143">• Project Team members associated View</span></span>|
|  <span data-ttu-id="8386c-144">Χρονική καταχώρηση</span><span class="sxs-lookup"><span data-stu-id="8386c-144">Time Entry</span></span>|<span data-ttu-id="8386c-145">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-145">• Information</span></span><br><span data-ttu-id="8386c-146">• Δημιουργία χρονικής καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="8386c-146">• Create Time Entry</span></span>|<span data-ttu-id="8386c-147">• Οι χρονικές καταχωρήσεις μου κατά ημέρα</span><span class="sxs-lookup"><span data-stu-id="8386c-147">• My Time Entries By Date</span></span><br><span data-ttu-id="8386c-148">• Οι χρονικές καταχωρήσεις μου για αυτήν την εβδομάδα</span><span class="sxs-lookup"><span data-stu-id="8386c-148">• My time Entries for this week</span></span><br><span data-ttu-id="8386c-149">• Χρονικές καταχωρήσεις για έγκριση</span><span class="sxs-lookup"><span data-stu-id="8386c-149">• Time entries for approval</span></span>|
|  <span data-ttu-id="8386c-150">Γραμμή ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-150">Journal Line</span></span>|<span data-ttu-id="8386c-151">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-151">• Information</span></span><br><span data-ttu-id="8386c-152">• Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="8386c-152">• Quick create</span></span>|<span data-ttu-id="8386c-153">• Ενεργές γραμμές ημερολογίων</span><span class="sxs-lookup"><span data-stu-id="8386c-153">• Active journal lines</span></span><br><span data-ttu-id="8386c-154">• Συσχετισμένη προβολή γραμμής ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-154">• Journal Line associated view</span></span>|
|  <span data-ttu-id="8386c-155">Λεπτομέρεια γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-155">Invoice Line Detail</span></span>|<span data-ttu-id="8386c-156">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-156">• Information</span></span><br><span data-ttu-id="8386c-157">• Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="8386c-157">• Quick create</span></span>|<span data-ttu-id="8386c-158">• Ενεργές λεπτομέρειες γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-158">• Active Invoice Line Details</span></span><br><span data-ttu-id="8386c-159">• Χρεώσιμες συναλλαγές τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-159">• Chargeable Invoice Transactions</span></span><br><span data-ttu-id="8386c-160">• Δωρεάν συναλλαγές τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-160">• Complimentary Invoice Transactions</span></span><br><span data-ttu-id="8386c-161">• Συσχετισμένη προβολή λεπτομερειών γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-161">• Invoice Line Detail associated view</span></span><br><span data-ttu-id="8386c-162">• Μη χρεώσιμη συναλλαγή τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="8386c-162">• Non-Chargeable Invoice Transactions</span></span>|
|  <span data-ttu-id="8386c-163">Πραγματικό</span><span class="sxs-lookup"><span data-stu-id="8386c-163">Actual</span></span>|<span data-ttu-id="8386c-164">• Πληροφορίες</span><span class="sxs-lookup"><span data-stu-id="8386c-164">• Information</span></span><br><span data-ttu-id="8386c-165">• Ενεργές πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="8386c-165">• Active Actuals</span></span>|<span data-ttu-id="8386c-166">• Πραγματική συσχετισμένη προβολή</span><span class="sxs-lookup"><span data-stu-id="8386c-166">• Actual Associated view</span></span>|

## <a name="set-up-transaction-category-as-a-pricing-dimension"></a><span data-ttu-id="8386c-167">Ρύθμιση της κατηγορίας συναλλαγών ως διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="8386c-167">Set up transaction category as a pricing dimension</span></span>

1. <span data-ttu-id="8386c-168">Στο περιβάλλον εργασίας Web, μεταβείτε στα στοιχεία **Project Service** > **Ρυθμίσεις** > **Παράμετροι**.</span><span class="sxs-lookup"><span data-stu-id="8386c-168">In the web interface, go to **Project Service** > **Settings** > **Parameters**.</span></span> 
2. <span data-ttu-id="8386c-169">Στη σελίδα **Παράμετροι** , στην καρτέλα **Διαστάσεις τιμολόγησης βάσει ποσού** σημειώστε ότι το πλέγμα στην καρτέλα εμφανίζει τις καρτέλες στην οντότητα **Διαστάσεις τιμολόγησης**.</span><span class="sxs-lookup"><span data-stu-id="8386c-169">On the **Parameters** page, on the **Amount-Based Pricing Dimensions** tab, note the grid on the tab shows the records in the **Pricing Dimensions** entity.</span></span>
3. <span data-ttu-id="8386c-170">Προσθέστε την **Κατηγορία συναλλαγής** σε αυτήν τη λίστα και ορίστε τα πεδία **Ισχύει για κόστος** και **Ισχύει για πωλήσεις** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="8386c-170">Add **Transaction Category** to this list and set the **Applicable to Cost** and **Applicable to Sale** fields set to **Yes**.</span></span>
4. <span data-ttu-id="8386c-171">Στο πεδίο **Τύπος διάστασης** , επιλέξτε **Βάσει ποσού** και, στη συνέχεια, επιλέξτε την προτεραιότητα για την **Κατηγορία συναλλαγής** που σχετίζεται με το κόστος και τις πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="8386c-171">In the **Dimension Type** field, select **Amount-based** , and then select the priority for **Transaction Category** related to cost and sales.</span></span>