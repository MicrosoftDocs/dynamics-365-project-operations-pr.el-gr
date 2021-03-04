---
title: Προβολή χρεώσιμης χρήσης για πόρους
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την προβολή χρήσης του πόρου.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: 4516c562e7eaf35c5fef638183967eef5a033b11
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146393"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="c9ec9-103">Προβολή χρεώσιμης χρήσης για πόρους</span><span class="sxs-lookup"><span data-stu-id="c9ec9-103">View chargeable utilization for resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]
 
<span data-ttu-id="c9ec9-104">Η **Προβολή χρήστης** στη σελίδα **Χρήση πόρου Project Service** εμφανίζει τη χρέωση χρήσης για κάθε πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="c9ec9-105">Επειδή η προβολή βασίζεται στον πίνακα χρονοδιαγράμματος, θα βρείτε πολλές από τις ίδιες λειτουργίες.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![Στιγμιότυπο οθόνης της προβολής χρήσης](media/FAQ-utilization-1.png)
 

<span data-ttu-id="c9ec9-107">Ο υπολογισμός χρεώσιμης χρήσης λειτουργεί ως εξής:</span><span class="sxs-lookup"><span data-stu-id="c9ec9-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="c9ec9-108">Χρεώσιμη χρήση = (χρεώσιμες πραγματικές ώρες) / (παραγωγική ικανότητα)</span><span class="sxs-lookup"><span data-stu-id="c9ec9-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="c9ec9-109">Τα κελιά αντιπροσωπεύουν την υπολογιζόμενη χρεώσιμη χρήση για την περίοδο που επιλέξατε για προβολή (ημέρες, εβδομάδες ή μήνες).</span><span class="sxs-lookup"><span data-stu-id="c9ec9-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="c9ec9-110">Τα χρώματα σε κάθε κελί εμφανίζεται η χρεώσιμη χρήση για έναν πόρο σε σύγκριση με τη χρεώσιμη χρήση-στόχο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="c9ec9-111">Η χρήση-στόχος μπορεί να οριστεί είτε στον προεπιλεγμένο ρόλο πόρου ή στον ίδιο τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="c9ec9-112">Ο υπολογισμός εξετάζει το άτομο για την τιμή πρώτα, στη συνέχεια για τον προεπιλεγμένο ρόλο του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="c9ec9-113">Ορισμός τιμής-στόχου σε έναν πόρο</span><span class="sxs-lookup"><span data-stu-id="c9ec9-113">Set target on a resource</span></span>

1. <span data-ttu-id="c9ec9-114">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="c9ec9-115">Επιλέξτε έναν πόρο για να ανοίξετε την καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="c9ec9-116">Στην καρτέλα **Project Service**, μπορείτε να ορίσετε τη χρήση του προορισμού του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![Στιγμιότυπο οθόνης χρήσης της καρτέλας Project Service για να ορίσετε τη χρήση-στόχο](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="c9ec9-118">Ορισμός της χρήσης του προορισμού σε ένα ρόλο</span><span class="sxs-lookup"><span data-stu-id="c9ec9-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="c9ec9-119">Μεταβείτε στα στοιχεία **Πόροι** \> **Ρόλοι πόρου**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="c9ec9-120">Επιλέξτε έναν ρόλο και ανοίξτε την καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="c9ec9-121">Ορίστε τη χρήση-στόχο για το ρόλο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-121">Set the target utilization for the role.</span></span>

> ![Στιγμιότυπο οθόνης χρήσης των ρόλων πόρων για να ορίσετε τη χρήση-στόχο](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="c9ec9-123">Υπολογισμός χρεώσιμης χρήσης για πόρους</span><span class="sxs-lookup"><span data-stu-id="c9ec9-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="c9ec9-124">Για να υπολογίσετε τη χρεώσιμη χρήση για έναν πόρο, πρέπει να πληροίτε ορισμένες προϋποθέσεις.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="c9ec9-125">Ορισμός προεπιλεγμένου ρόλου για μεμονωμένο πόρο</span><span class="sxs-lookup"><span data-stu-id="c9ec9-125">Set default role for individual resource</span></span>

<span data-ttu-id="c9ec9-126">Πρώτα, η χρήση-στόχος πρέπει να οριστεί είτε στον μεμονωμένο πόρο ή σε ρόλους πόρων.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="c9ec9-127">Εάν χρησιμοποιείτε ρόλους πόρων για τους στόχους, κάθε μεμονωμένος πόρος πρέπει να έχει έναν προεπιλεγμένο ρόλο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="c9ec9-128">Για να κάνετε τη ρύθμιση μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="c9ec9-129">Επιλέξτε έναν πόρο, ανοίξτε την καρτέλα και, στη συνέχεια, επιλέξτε **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="c9ec9-130">Στο πλέγμα **Ρόλος πόρου**, βεβαιωθείτε ότι υπάρχει ένας ρόλος για τον πόρο και ότι το στοιχείο **Είναι προεπιλογή** έχει οριστεί σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="c9ec9-131">Αλλάξτε τον τύπο χρέωσης για αυτόν το ρόλο πόρου</span><span class="sxs-lookup"><span data-stu-id="c9ec9-131">Change billing type for resource role</span></span>

<span data-ttu-id="c9ec9-132">Οι ρόλοι πόρων πρέπει να οριστούν να έχουν τύπο χρέωσης **Χρεώσιμο**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="c9ec9-133">Μεταβείτε στα στοιχεία **Πόροι** \> **Ρόλοι πόρου**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="c9ec9-134">Ανοίξτε την καρτέλα που θέλετε να ενημερώσετε και στη συνέχεια, ορίστε τον προεπιλεγμένο τύπο χρέωσης σε **Χρεώσιμο**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="c9ec9-135">Ορισμός ωρών εργασίας για ρόλο πόρου</span><span class="sxs-lookup"><span data-stu-id="c9ec9-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="c9ec9-136">Ο πόρος πρέπει να έχει ώρες εργασίας για τον υπολογισμό της παραγωγικής ικανότητας.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="c9ec9-137">Μεταβείτε στα στοιχεία **Πόροι** \> **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="c9ec9-138">Επιλέξτε έναν πόρο για να ανοίξετε την καρτέλα και μετά επιλέξτε **Εμφάνιση εργάσιμων ωρών**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="c9ec9-139">Μπορείτε να κάνετε μαζική ενημέρωση της λίστας πόρων εφαρμόζοντας ένα **Πρότυπο ωρών εργασίας** από την προβολή **Λίστα πόρων**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="c9ec9-140">Αντιμετώπιση προβλημάτων με πραγματικές χρεώσιμες ώρες</span><span class="sxs-lookup"><span data-stu-id="c9ec9-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="c9ec9-141">Οι πραγματικές χρεώσιμες ώρες προέρχονται από την ενότητα **Πραγματικές τιμές**.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="c9ec9-142">Τα πραγματικά στοιχεία με τύπο χρέωσης **Χρεώσιμο** συμπεριλαμβάνονται στον υπολογισμό και για αυτόν το λόγο πρέπει να έχετε έργα όπου οι πραγματικές τιμές είναι τιμολογημένες.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="c9ec9-143">Εάν δεν βλέπετε χρεώσιμη χρήση, ακολουθούν ορισμένα στοιχεία που μπορείτε να ελέγξετε:</span><span class="sxs-lookup"><span data-stu-id="c9ec9-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="c9ec9-144">Ο πόρος έχει εργάσιμες ώρες για την παραγωγική ικανότητα.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="c9ec9-145">Ο πόρος έχει μεμονωμένο στόχο χρήσης ή έχει προεπιλεγμένο ρόλο που έχει αντιστοιχιστεί σε αυτόν.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="c9ec9-146">Ο ρόλος έχει στόχο χρήσης.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="c9ec9-147">Οι πραγματικές τιμές έχουν τύπο χρέωσης **Χρεώσιμο** για την περίοδο που αναμένετε ένας υπολογισμός χρήσης.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="c9ec9-148">Ελέγξτε τα παρακάτω εάν βλέπετε τα πραγματικά στοιχεία με τύπους χρέωσης πέραν του χρεώσιμου:</span><span class="sxs-lookup"><span data-stu-id="c9ec9-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="c9ec9-149">Ο ρόλος που χρησιμοποιείται στα πραγματικά στοιχεία έχει προεπιλεγμένο τύπο χρέωσης διαφορετικό από χρεώσιμο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="c9ec9-150">Ο ρόλος της γραμμής σύμβασης έργου έχει οριστεί σε μη χρεώσιμο.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="c9ec9-151">Το έργο σύμβασης δεν έχει συσχετισμένη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="c9ec9-151">The project does not have an associated contract line.</span></span>

