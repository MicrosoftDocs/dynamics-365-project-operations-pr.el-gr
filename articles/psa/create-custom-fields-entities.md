---
title: Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας συνόλων επιλογών και οντοτήτων στη δική σας λύση στην πλατφόρμα Power Apps.
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
ms.openlocfilehash: c58745a46e84a40b90fbb3cbf89b10e293588fc3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290533"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="1ad57-103">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="1ad57-103">Create custom fields and entities</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1ad57-104">Ολοκληρώστε τα παρακάτω βήματα κάθε φορά που θέλετε να δημιουργήσετε ένα προσαρμοσμένο σύνολο επιλογών ή μια οντότητα στην Power Apps πλατφόρμα.</span><span class="sxs-lookup"><span data-stu-id="1ad57-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="1ad57-105">Οι διαδικασίες αυτού του θέματος πρέπει να ολοκληρωθούν με χρήση του περιβάλλοντος εργασίας web του Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="1ad57-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1ad57-106">Συνιστούμε να κάνετε όλες τις προσαρμοσμένες αλλαγές διάστασης τιμολόγησης σε μια ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="1ad57-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="1ad57-107">Αυτή η σημαντική βέλτιστη πρακτική παρέχει την ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο, θα σας βοηθήσει με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία.</span><span class="sxs-lookup"><span data-stu-id="1ad57-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="1ad57-108">Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη λύση** και εισαγάγετέ την σε άλλες παρουσίες, για να επαναχρησιμοποιήσετε την ρύθμιση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="1ad57-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="1ad57-109">Δημιουργία προσαρμοσμένων πεδίων και συνόλων επιλογών στη λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="1ad57-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="1ad57-110">Μια διάσταση τιμολόγησης μπορεί να είναι μια σύνολο επιλογών ή μια οντότητα.</span><span class="sxs-lookup"><span data-stu-id="1ad57-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="1ad57-111">Και τα δύο πρέπει να δημιουργηθούν στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="1ad57-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="1ad57-112">Τα βήματα σε αυτήν τη διαδικασία εξηγούν πώς μπορείτε να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες και διαστάσεις που βασίζονται σε σύνολα επιλογών.</span><span class="sxs-lookup"><span data-stu-id="1ad57-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="1ad57-113">Διαστάσεις βάσει οντότητας</span><span class="sxs-lookup"><span data-stu-id="1ad57-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="1ad57-114">Στο PSA, κάντε κλικ στο **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-114">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="1ad57-115">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="1ad57-116">Κάντε κλικ στην επιλογή **Νέα** για να δημιουργήσετε μια νέα οντότητα που καλείται **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="1ad57-117">Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια, πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Ορισμός τυπικού τίτλου οντότητας](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="1ad57-119">Διαστάσεις που βασίζονται σε σύνολο επιλογών</span><span class="sxs-lookup"><span data-stu-id="1ad57-119">Option set-based dimensions</span></span> 
<span data-ttu-id="1ad57-120">Μπορείτε να δημιουργήσετε δύο διαστάσεις που βασίζονται σε σύνολο επιλογών.</span><span class="sxs-lookup"><span data-stu-id="1ad57-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="1ad57-121">Χρησιμοποιήστε την **Τοποθεσία εργασίας πόρου** για να παρακολουθήσετε την τιμή της **Αρχικής** τοποθεσίας εργασίας και την **Επί τόπου** εργασία και να χρησιμοποιήσετε τις **Ώρες εργασίας πόρου** με τιμές **Κανονικές** και **Υπερωρίες** για να εφαρμόσετε μια αύξηση όταν ολοκληρωθεί η εργασία.</span><span class="sxs-lookup"><span data-stu-id="1ad57-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="1ad57-122">Στο PSA, κάντε κλικ στο **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-122">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="1ad57-123">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Σύνολα επιλογών**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="1ad57-124">Επιλέξτε **Νέο** για να δημιουργήσετε ένα νέο σύνολο επιλογών, καταγράψτε τις υπόλοιπες απαιτούμενες πληροφορίες και πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="1ad57-125">Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Τοποθεσία εργασίας πόρου</span><span class="sxs-lookup"><span data-stu-id="1ad57-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="1ad57-126">Η διάσταση τιμολόγησης που βασίζεται σε σύνολο επιλογών καλείται Ώρες εργασίας πόρου</span><span class="sxs-lookup"><span data-stu-id="1ad57-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="1ad57-127">Δημιουργία δεδομένων για διαστάσεις βασισμένες σε οντότητες</span><span class="sxs-lookup"><span data-stu-id="1ad57-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="1ad57-128">Μπορείτε να δημιουργήσετε δεδομένα για διαστάσεις βασισμένες σε οντότητες με μη αυτόματο τρόπο ή χρησιμοποιώντας κλήσης εισαγωγής Microsoft Excel ή κλήσεις εξυπηρέτησης.</span><span class="sxs-lookup"><span data-stu-id="1ad57-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="1ad57-129">Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για τη δημιουργία δύο τυπικών τίτλων, **Μηχανικός συστημάτων** και **Επικεφαλής μηχανικός συστημάτων** από τη διάσταση βάσει οντότητας **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="1ad57-130">Εάν τα δεδομένα που θέλετε να δημιουργήσετε είναι μικρά, όπως στο παρακάτω παράδειγμα, μπορείτε να χρησιμοποιήσετε μια τυπική φόρμα.</span><span class="sxs-lookup"><span data-stu-id="1ad57-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="1ad57-131">Στο PSA, επιλέξτε **Εύρεση για προχωρημένους**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="1ad57-132">Επιλέξτε την οντότητα **Τυπικός τίτλος** και μετά επιλέξτε **Αποτελέσματα**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="1ad57-133">Θα εμφανιστούν όλες οι γραμμές στην οντότητα **Τυπικός τίτλος**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="1ad57-134">Επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-134">Click **New**.</span></span> <span data-ttu-id="1ad57-135">Στο πεδίο **Όνομα**, καταχωρίστε "Μηχανικός συστήματος" και μετά πατήστε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1ad57-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="1ad57-136">Κλείστε τη φόρμα.</span><span class="sxs-lookup"><span data-stu-id="1ad57-136">Close the form.</span></span> 
4. <span data-ttu-id="1ad57-137">Επαναλάβετε τα βήματα 1-3, για να δημιουργήσετε έναν άλλο τυπικό τίτλο για τον "επικεφαλής μηχανικό συστημάτων".</span><span class="sxs-lookup"><span data-stu-id="1ad57-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="1ad57-138">Δείγμα δεδομένων για την οντότητα τυπικού τίτλου</span><span class="sxs-lookup"><span data-stu-id="1ad57-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]