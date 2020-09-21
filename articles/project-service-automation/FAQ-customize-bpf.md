---
title: Πώς μπορώ να προσαρμόσω τα στάδια ροής επιχειρηματικής διαδικασίας έργου;
description: Επισκόπηση του τρόπου προσαρμογής της ροής επιχειρηματικής διαδικασίας σταδίων έργου.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x
author: JohnPBurrows
ms.assetid: 36f7df9e-117d-4f85-af4b-d842e93321bd
ms.author: john.burrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: d4b99f67e929ebcd1a684bcd1124756140107d17
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751551"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="14304-103">Πώς μπορώ να προσαρμόσω τα στάδια ροής επιχειρηματικής διαδικασίας έργου;</span><span class="sxs-lookup"><span data-stu-id="14304-103">How do I customize the Project Stages business process flow?</span></span>
[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="14304-104">Υπάρχει ένας γνωστός περιορισμός σε προηγούμενες εκδόσεις της εφαρμογής Project Service που ορίζει ότι τα ονόματα των σταδίων στη ροή επιχειρηματικής διαδικασίας των σταδίων έργου πρέπει να συμφωνούν απόλυτα με τα αναμενόμενα αγγλικά ονόματα (**Quote**, **Plan**, **Close**).</span><span class="sxs-lookup"><span data-stu-id="14304-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="14304-105">Διαφορετικά, η επιχειρηματική λογική, η οποία βασίζεται στα αγγλικά ονόματα σταδίων δεν λειτουργεί όπως αναμένεται.</span><span class="sxs-lookup"><span data-stu-id="14304-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="14304-106">Για αυτόν τον λόγο δεν βλέπετε οικείες ενέργειες όπως **Εναλλαγή διεργασίας** ή **Επεξεργασία διαδικασίας** διαθέσιμες στη φόρμα έργου και η προσαρμογή της ροής επιχειρηματικής διαδικασίας δεν συνιστάται.</span><span class="sxs-lookup"><span data-stu-id="14304-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="14304-107">Αυτός ο περιορισμός έχει αντιμετωπιστεί στην έκδοση 2.4.5.48 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="14304-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="14304-108">Αυτό το άρθρο παρέχει εναλλακτικές λύσεις εάν θέλετε να προσαρμόσετε την προεπιλεγμένη ροή επιχειρηματικής διαδικασίας για νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="14304-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="14304-109">Η επιχειρηματική λογική απαιτεί δεδομένα που συμφωνούν απόλυτα με τα αγγλικά ονόματα σταδίων</span><span class="sxs-lookup"><span data-stu-id="14304-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="14304-110">Η ροή επιχειρηματικής διαδικασίας σταδίων έργου περιλαμβάνει επιχειρηματική λογική που αυξάνει τις ακόλουθες συμπεριφορές στην εφαρμογή:</span><span class="sxs-lookup"><span data-stu-id="14304-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="14304-111">Όταν το έργο έχει συσχετιστεί με μια προσφορά, ο κωδικός ρυθμίζει τη ροή επιχειρηματικής διαδικασίας στο στάδιο **Quote**.</span><span class="sxs-lookup"><span data-stu-id="14304-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="14304-112">Όταν το έργο έχει συσχετιστεί με μια σύμβαση, ο κωδικός ρυθμίζει τη ροή επιχειρηματικής διαδικασίας στο στάδιο **Plan**.</span><span class="sxs-lookup"><span data-stu-id="14304-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="14304-113">Όταν η ροή επιχειρηματικής διαδικασίας προχωρά στο στάδιο **Close**, η καρτέλα έργου είναι απενεργοποιημένη.</span><span class="sxs-lookup"><span data-stu-id="14304-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="14304-114">Όταν απενεργοποιείται το έργο, η φόρμα έργου και η δομή ανάλυσης εργασίας (WBS) έχουν οριστεί μόνο για ανάγνωση, οι κρατήσεις πόρων με όνομα είναι διαθέσιμες και τυχόν συσχετισμένοι τιμοκατάλογοι απενεργοποιούνται.</span><span class="sxs-lookup"><span data-stu-id="14304-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="14304-115">Αυτή η επιχειρηματική λογική βασίζεται στα Αγγλικά ονόματα για τα στάδια έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="14304-116">Αυτή η εξάρτηση από τα αγγλικά ονόματα σταδίων είναι ο κύριος λόγος για τον οποίο δεν συνιστάται η προσαρμογή της ροής επιχειρηματικής διαδικασίας των σταδίων έργου καθώς και ο λόγος για τον οποίο δεν βλέπετε τις συνήθεις ενέργειες ροής επιχειρηματικής διαδικασίας όπως η **Εναλλαγή διεργασίας** ή η **Επεξεργασία διεργασίας** στην οντότητα "έργο".</span><span class="sxs-lookup"><span data-stu-id="14304-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="14304-117">Τι θα συμβεί εάν τα ονόματα σταδίων δεν ταιριάζουν με τα ονόματα;</span><span class="sxs-lookup"><span data-stu-id="14304-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="14304-118">Στην εφαρμογή Project Service έκδοση 1.x στην πλατφόρμα 8.2, όταν τα ονόματα σταδίων στη ροή επιχειρηματικής διαδικασίας δεν συμφωνούν με τα αγγλικά ονόματα σταδίων, παρακάμπτεται η επιχειρηματική λογική που ορίζει το σωστό στάδιο για προσφορές ή συμβάσεις ή η λογική που που κλείνει το έργο παραλείπεται.</span><span class="sxs-lookup"><span data-stu-id="14304-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="14304-119">Δεν εμφανίζονται μηνύματα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="14304-119">No error messages are displayed.</span></span> <span data-ttu-id="14304-120">Επομένως, μπορείτε να προσαρμόσετε τη ροή επιχειρηματικής διαδικασίας σταδίων έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="14304-121">Ωστόσο, δεν θα βλέπετε καμία από τις αυτόματες ροές εργασιών για προσφορές, συμβάσεις και κλείσιμο έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="14304-122">Στην έκδοση εφαρμογής Project Service 2.4.4.30 ή προγενέστερη στην πλατφόρμα 9.0 παρουσιάστηκε μια σημαντική αλλαγή αρχιτεκτονικής στις ροές επιχειρηματικής διαδικασίας, που απαιτούσαν εκ νέου εγγραφή της επιχειρηματικής λογικής ροής επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="14304-123">Κατά συνέπεια, εάν τα ονόματα σταδίων διαδικασίας δεν συμφωνούν με τα αναμενόμενα αγγλικά ονόματα, λαμβάνετε ένα μήνυμα σφάλματος.</span><span class="sxs-lookup"><span data-stu-id="14304-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="14304-124">Επομένως, εάν θέλετε να προσαρμόσετε τη ροή επιχειρηματικής διαδικασίας σταδίων έργου για την οντότητα έργου, μπορείτε να προσθέσετε μόνο νέα στάδια στην προεπιλεγμένη ροή επιχειρηματικής διαδικασίας για την οντότητα έργου, ενώ παράλληλα να διατηρήσετε τα στάδια **Quote**, **Plan** και **Close** ως έχουν.</span><span class="sxs-lookup"><span data-stu-id="14304-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="14304-125">Αυτός ο περιορισμός εξασφαλίζει ότι δεν μπορείτε να λάβετε σφάλματα από την επιχειρηματική λογική που αναμένει τα αγγλικά ονόματα σταδίων στη ροή επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="14304-126">Στην έκδοση 2.4.5.48 ή νεότερη, η επιχειρηματική λογική που περιγράφεται σε αυτό το άρθρο έχει καταργηθεί από την προεπιλεγμένη ροή επιχειρηματικής διαδικασίας για την οντότητα του έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="14304-127">Η αναβάθμιση σε αυτήν την έκδοση ή σε νεότερη θα σας επιτρέψει να προσαρμόσετε ή να αντικαταστήσετε την προεπιλεγμένη ροή επιχειρηματικής διαδικασίας με μία από τις δικές σας.</span><span class="sxs-lookup"><span data-stu-id="14304-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="14304-128">Λύσεις για νεότερες εκδόσεις</span><span class="sxs-lookup"><span data-stu-id="14304-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="14304-129">Εάν η αναβάθμιση δεν είναι μια επιλογή, μπορείτε να προσαρμόσετε τη ροή επιχειρηματικής διαδικασίας σταδίων έργου για την οντότητα έργου με έναν από τους εξής δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="14304-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="14304-130">Προσθήκη επιπλέον σταδίων στην προεπιλεγμένη ρύθμιση παραμέτρων, διατηρώντας τα αγγλικά ονόματα σταδίων για τα **Quote**, **Plan** και **Close**.</span><span class="sxs-lookup"><span data-stu-id="14304-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-131">![Στιγμιότυπο οθόνης προσθήκης σταδίων στην προεπιλεγμένη ρύθμιση παραμέτρων](media/FAQ-Customize-BPF-1.png)</span><span class="sxs-lookup"><span data-stu-id="14304-131">![Screenshot of adding stages to default configuration](media/FAQ-Customize-BPF-1.png)</span></span>
 
2. <span data-ttu-id="14304-132">Δημιουργήστε τη δική σας ροή επιχειρηματικής διαδικασίας και κάντε την κύρια ροή επιχειρηματικής διαδικασίας για την οντότητα έργου, η οποία σάς επιτρέπει να έχετε όποιο όνομα σταδίου θέλετε.</span><span class="sxs-lookup"><span data-stu-id="14304-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="14304-133">Ωστόσο, εάν θέλετε να χρησιμοποιήσετε τα ίδια τυπικά στάδια έργου **Quote**, **Plan** και **Close**, θα πρέπει να κάνετε ορισμένες προσαρμογές που βασίζονται σε προσαρμοσμένα ονόματα σταδίων.</span><span class="sxs-lookup"><span data-stu-id="14304-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="14304-134">Η πιο περίπλοκη λογική είναι το κλείσιμο του έργου, το οποίο μπορείτε να ενεργοποιήσετε απενεργοποιώντας απλώς την καρτέλα έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-135">![Στιγμιότυπο οθόνης προσαρμογής BPF](media/FAQ-Customize-BPF-2.png)</span><span class="sxs-lookup"><span data-stu-id="14304-135">![Screenshot of BPF customization](media/FAQ-Customize-BPF-2.png)</span></span>

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="14304-136">Επιπλέον ζητήματα για την έκδοση εφαρμογής Project Service 2.4.4.30 ή νωρίτερη στην πλατφόρμα 9.0</span><span class="sxs-lookup"><span data-stu-id="14304-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="14304-137">Στο Project Service 2.4.4.30 ή νωρίτερη στην πλατφόρμα 9.0, με μια προσαρμοσμένη ροή επιχειρηματικής διαδικασίας το πεδίο **Όνομα σταδίου** πεδίο στην οντότητα έργου που χρησιμοποιήθηκε στο διάγραμμα **Έργο κατά στάδιο** δεν θα ενημερωθεί διότι συνδέεται με την προεπιλεγμένη ροή επιχειρηματικής διαδικασίας σταδίων έργου.</span><span class="sxs-lookup"><span data-stu-id="14304-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="14304-138">Μπορείτε να αντιμετωπίσετε αυτό το ζήτημα με τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="14304-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="14304-139">Προσθέστε ένα προσαρμοσμένο πεδίο για να καταγράψετε το τρέχον στάδιο ροής επιχειρηματικής διαδικασίας που ενημερώνεται καθώς ο χρήστης προχωρά στην προσαρμοσμένη ροή επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="14304-140">Τροποποιήστε το γράφημα **Έργο κατά στάδιο** για να εργαστείτε με το προσαρμοσμένο πεδίο αντί με την προεπιλεγμένη ρύθμιση παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="14304-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="14304-141">Βήματα για να δημιουργήσετε τις δικές σας ροές επιχειρηματικής διαδικασίας για την οντότητα έργου</span><span class="sxs-lookup"><span data-stu-id="14304-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="14304-142">Για να δημιουργήσετε τις δικές σας ροές επιχειρηματικής διαδικασίας για την οντότητα έργου κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="14304-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="14304-143">Μεταβείτε στην επιλογή **Ρυθμίσεις** > **Κέντρο διεργασίας**.</span><span class="sxs-lookup"><span data-stu-id="14304-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="14304-144">Μην αντιγράψετε τη ροή επιχειρηματικής διαδικασία σταδίων έργου διότι έτσι αντιγράφεται η επιχειρηματική λογική του Project Service.</span><span class="sxs-lookup"><span data-stu-id="14304-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-145">![Στιγμιότυπο οθόνης προσαρμογής BPF](media/FAQ-Customize-BPF-3.png)</span><span class="sxs-lookup"><span data-stu-id="14304-145">![Screenshot of BPF customization](media/FAQ-Customize-BPF-3.png)</span></span>

2. <span data-ttu-id="14304-146">Χρησιμοποιήστε τη σχεδίαση της διαδικασίας για να δημιουργήσετε τα ονόματα σταδίων που θέλετε.</span><span class="sxs-lookup"><span data-stu-id="14304-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="14304-147">Εάν θέλετε την ίδια λειτουργικότητα με τα προεπιλεγμένα στάδια για **Quote**, **Plan** και **Close**, θα πρέπει να δημιουργήσετε ανάλογα με τα ονόματα σταδίων της προσαρμοσμένης επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-148">![Στιγμιότυπο οθόνης του σχεδιασμού διαδικασίας για την προσαρμογή BPF](media/FAQ-Customize-BPF-4.png)</span><span class="sxs-lookup"><span data-stu-id="14304-148">![Screenshot of Process Designer used to customize BPF](media/FAQ-Customize-BPF-4.png)</span></span> 

3. <span data-ttu-id="14304-149">Στη σχεδίαση διαδικασίας, κάντε κλικ στο κουμπί **Σειρά ροής διαδικασίας** για να καταστεί η προσαρμοσμένη ροή επιχειρηματικής διαδικασίας ως κύρια ροή επιχειρηματικής διαδικασίας για την οντότητα έργου, μετακινώντας την επάνω από τη ροή επιχειρηματικής διαδικασίας σταδίων έργου στο επάνω μέρος της λίστας.</span><span class="sxs-lookup"><span data-stu-id="14304-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-150">![Στιγμιότυπο οθόνης χρήσης της σειράς ροής διαδικασίας](media/FAQ-Customize-BPF-5-720.png)</span><span class="sxs-lookup"><span data-stu-id="14304-150">![Screenshot of using Order Process Flow](media/FAQ-Customize-BPF-5-720.png)</span></span>

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="14304-151">Τα παρακάτω βήματα ισχύουν για την εφαρμογή Project Service 2.4.4.30 ή προγενέστερη στην πλατφόρμα 9.0</span><span class="sxs-lookup"><span data-stu-id="14304-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="14304-152">Προσθέστε ένα νέο προσαρμοσμένο πεδίο στην οντότητα "έργου" για να καταγράψετε τα προσαρμοσμένα στάδια στην προσαρμοσμένη ροή επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="14304-153">Θα πρέπει να προσθέσετε την επιχειρηματική λογική (Προσθήκη/ροή εργασίας) για να ενημερώσετε αυτό το πεδίο όταν ενημερώνεται το στάδιο στην προσαρμοσμένη ροή επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="14304-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-154">![Στιγμιότυπο οθόνης της προσαρμογής οντοτήτων έργου](media/FAQ-Customize-BPF-6-720.png)</span><span class="sxs-lookup"><span data-stu-id="14304-154">![Screenshot of customizing Project entity](media/FAQ-Customize-BPF-6-720.png)</span></span>

5. <span data-ttu-id="14304-155">Τροποποιήστε το γράφημα **Έργο κατά στάδιο** για να χρησιμοποιήσετε το νέο προσαρμοσμένο πεδίο για στάδια.</span><span class="sxs-lookup"><span data-stu-id="14304-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-156">![Στιγμιότυπο οθόνης της χρήσης του γραφήματος Έργο κατά στάδιο](media/FAQ-Customize-BPF-7-720.png)</span><span class="sxs-lookup"><span data-stu-id="14304-156">![Screenshot of using the Project By Stage chart](media/FAQ-Customize-BPF-7-720.png)</span></span>

6. <span data-ttu-id="14304-157">Τροποποιήστε τυχόν προβολές για την οντότητα έργου για να συμπεριλάβετε το νέο προσαρμοσμένο πεδίο για τα στάδια.</span><span class="sxs-lookup"><span data-stu-id="14304-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   > [!div class="mx-imgBorder"] 
   > <span data-ttu-id="14304-158">![Στιγμιότυπο οθόνης τροποποίησης προβολών στην οντότητα Έργο](media/FAQ-Customize-BPF-8-720.png)</span><span class="sxs-lookup"><span data-stu-id="14304-158">![Screenshot of modifying views on the Project entity](media/FAQ-Customize-BPF-8-720.png)</span></span>

