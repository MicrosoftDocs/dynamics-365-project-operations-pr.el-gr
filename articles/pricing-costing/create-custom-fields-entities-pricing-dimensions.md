---
title: Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προσαρμοσμένων συνόλων επιλογών ή οντοτήτων.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
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
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642813"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="13992-103">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="13992-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="13992-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="13992-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="13992-105">Ολοκληρώστε τα παρακάτω βήματα όταν θέλετε να δημιουργήσετε ένα προσαρμοσμένο σύνολο επιλογών ή μια οντότητα για χρήση ως διάσταση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="13992-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="13992-106">Για περισσότερες πληροφορίες, δείτε την ενότητα [Επισκόπηση διαστάσεων τιμολόγησης](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="13992-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="13992-107">Συνιστούμε να κάνετε όλες τις προσαρμοσμένες αλλαγές διάστασης τιμολόγησης σε μια ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="13992-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="13992-108">Αυτή η σημαντική βέλτιστη πρακτική παρέχει ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο.</span><span class="sxs-lookup"><span data-stu-id="13992-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="13992-109">Αυτό θα σας βοηθήσει επίσης με την περαιτέρω χρήση της εργασίας σας και θα διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία. Μετά την πραγματοποίηση όλων των απαιτούμενων αλλαγών, την εξαγωγή αυτής της λύσης ως **διαχειριζόμενη λύση** και την εισαγωγή της σε άλλες παρουσίες για την επαναχρησιμοποίηση της ρύθμισης τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="13992-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="13992-110">Δημιουργία προσαρμοσμένων πεδίων και συνόλων επιλογών στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="13992-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="13992-111">Μια διάσταση τιμολόγησης μπορεί να είναι μια σύνολο επιλογών ή μια οντότητα.</span><span class="sxs-lookup"><span data-stu-id="13992-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="13992-112">Και τα δύο πρέπει να δημιουργηθούν στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="13992-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="13992-113">Τα βήματα σε αυτήν τη διαδικασία εξηγούν πώς μπορείτε να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες και διαστάσεις που βασίζονται σε σύνολα επιλογών.</span><span class="sxs-lookup"><span data-stu-id="13992-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="13992-114">Διαστάσεις βάσει οντότητας</span><span class="sxs-lookup"><span data-stu-id="13992-114">Entity-based dimensions</span></span>
<span data-ttu-id="13992-115">Για να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="13992-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="13992-116">Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="13992-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="13992-117">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="13992-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="13992-118">Επιλέξτε **Νέα** για να δημιουργήσετε μια νέα οντότητα που καλείται **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="13992-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="13992-119">Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="13992-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![Ορισμός τυπικού τίτλου οντότητας](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="13992-121">Διαστάσεις που βασίζονται σε σύνολο επιλογών</span><span class="sxs-lookup"><span data-stu-id="13992-121">Option set-based dimensions</span></span> 
<span data-ttu-id="13992-122">Μπορείτε να δημιουργήσετε δύο διαστάσεις που βασίζονται σε σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="13992-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="13992-123">Χρησιμοποιήστε τη **Θέση εργασίας πόρου** για να παρακολουθήσετε την τιμή της εργασίας τοποθεσίας **Αρχική** και της εργασίας **Επιτόπου**.</span><span class="sxs-lookup"><span data-stu-id="13992-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="13992-124">Χρησιμοποιήστε τις **Ώρες εργασίας πόρου** με τις τιμές **Κανονικές** και **Υπερωρίες** για να εφαρμόσετε μια αύξηση όταν ολοκληρωθεί η εργασία.</span><span class="sxs-lookup"><span data-stu-id="13992-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="13992-125">Το παρακάτω γραφικό παρέχει μια προβολή της διάστασης **Θέση εργασίας πόρου**.</span><span class="sxs-lookup"><span data-stu-id="13992-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Τοποθεσία εργασίας πόρου](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="13992-127">Το παρακάτω γραφικό παρέχει μια προβολή της διάστασης **Ώρες εργασίας πόρου**.</span><span class="sxs-lookup"><span data-stu-id="13992-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Ώρες εργασίας πόρου](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="13992-129">Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="13992-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="13992-130">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Σύνολα επιλογών**.</span><span class="sxs-lookup"><span data-stu-id="13992-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="13992-131">Επιλέξτε **Νέο** για να δημιουργήσετε ένα νέο σύνολο επιλογών, καταγράψτε τις υπόλοιπες απαιτούμενες πληροφορίες και επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="13992-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="13992-132">Δημιουργία δεδομένων για διαστάσεις βασισμένες σε οντότητες</span><span class="sxs-lookup"><span data-stu-id="13992-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="13992-133">Μπορείτε να δημιουργήσετε δεδομένα για διαστάσεις βασισμένες σε οντότητες με μη αυτόματο τρόπο ή χρησιμοποιώντας κλήσης εισαγωγής Microsoft Excel ή κλήσεις εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="13992-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="13992-134">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για τη δημιουργία δύο τυπικών τίτλων, **Μηχανικός συστημάτων** και **Επικεφαλής μηχανικός συστημάτων** από τη διάσταση βάσει οντότητας **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="13992-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="13992-135">Εάν τα δεδομένα που θέλετε να δημιουργήσετε είναι μικρά, όπως στο παρακάτω παράδειγμα, μπορείτε να χρησιμοποιήσετε μια τυπική φόρμα.</span><span class="sxs-lookup"><span data-stu-id="13992-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="13992-136">Επιλέξτε **Πρόσθετα κριτήρια εύρεσης**.</span><span class="sxs-lookup"><span data-stu-id="13992-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="13992-137">Επιλέξτε την οντότητα **Τυπικός τίτλος** και μετά επιλέξτε **Αποτελέσματα**.</span><span class="sxs-lookup"><span data-stu-id="13992-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="13992-138">Θα εμφανιστούν όλες οι γραμμές στην οντότητα **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="13992-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="13992-139">Επιλέξτε **Νέο** και στο πεδίο **Όνομα**, καταχωρίστε "Μηχανικός συστήματος" και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="13992-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="13992-140">Κλείστε τη σελίδα.</span><span class="sxs-lookup"><span data-stu-id="13992-140">Close the page.</span></span> 
5. <span data-ttu-id="13992-141">Επαναλάβετε τα βήματα 1-3, για να δημιουργήσετε έναν άλλο τυπικό τίτλο για τον "επικεφαλής μηχανικό συστημάτων".</span><span class="sxs-lookup"><span data-stu-id="13992-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![Δείγμα δεδομένων για την οντότητα τυπικού τίτλου](media/ST-data.png)
