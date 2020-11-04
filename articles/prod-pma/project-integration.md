---
title: Ενοποίηση του Microsoft Project client
description: Ο προγραμματισμός και η συντήρηση ενός χρονοδιαγράμματος έργου μπορεί να είναι πολύπλοκα, επομένως οι διαχειριστές έργου πρέπει να χρησιμοποιούν τα εργαλεία που τους βοηθούν να διαχειρίζονται αυτήν την εργασία. Με την ενοποίηση με το Microsoft Project Client παρέχεται υποστήριξη για το άνοιγμα και τη διαχείριση μιας δομής ανάλυσης εργασίας έργου.
author: Yowelle
manager: AnnBe
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 732b72d9819fc149c4b2c783b3dc7f7eec3f0393
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076977"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="164a4-104">Ενοποίηση του Microsoft Project client</span><span class="sxs-lookup"><span data-stu-id="164a4-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="164a4-105">Ο προγραμματισμός και η συντήρηση ενός χρονοδιαγράμματος έργου μπορεί να είναι πολύπλοκα, επομένως οι διαχειριστές έργου πρέπει να χρησιμοποιούν τα εργαλεία που τους βοηθούν να διαχειρίζονται αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="164a4-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="164a4-106">Με την ενοποίηση με το Microsoft Project Client παρέχεται υποστήριξη για το άνοιγμα και τη διαχείριση μιας δομής ανάλυσης εργασίας έργου.</span><span class="sxs-lookup"><span data-stu-id="164a4-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="164a4-107">Ο υπεύθυνος έργου μπορεί να δημοσιεύσει τυχόν αλλαγές στη δομή ανάλυσης εργασίας έργου Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="164a4-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="164a4-108">Εάν χρησιμοποιείτε την ενημέρωση Ιουλίου (έκδοση 10.0.4), πρέπει να εγκαταστήσετε το KB 4054797 και το 4055884.</span><span class="sxs-lookup"><span data-stu-id="164a4-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="164a4-109">Ρύθμιση παραμέτρων του πρόσθετου Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="164a4-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="164a4-110">Για να είναι δυνατή η ενοποίηση με το Microsoft Project Client, ένα πρόσθετο Microsoft Dynamics 365 απαιτείται να εγκατασταθεί στην εφαρμογή Microsoft Project του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="164a4-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="164a4-111">Αυτό επιτυγχάνεται με το άνοιγμα του στοιχείου **Χώρος εργασίας διαχείρισης έργου**.</span><span class="sxs-lookup"><span data-stu-id="164a4-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="164a4-112">•   Κάντε κλικ στην επιλογή **Ρύθμιση παραμέτρων πρόσθετου προγράμματος-πελάτη** από την ενότητα **Συνδέσεις** > **Ρύθμιση** του χώρου εργασίας.</span><span class="sxs-lookup"><span data-stu-id="164a4-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="164a4-113">•   Επιλέξτε **Άνοιγμα** και, στη συνέχεια, κάντε κλικ στην επιλογή **Εκτέλεση** όταν σας ζητηθεί.</span><span class="sxs-lookup"><span data-stu-id="164a4-113">•   Click **Open** , then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="164a4-114">Ανοίξτε και κλείστε μια υπάρχουσα προσχέδια δομή ανάλυσης εργασίας στο Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="164a4-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="164a4-115">Εάν ένα έργο στο Dynamics 365 Finance έχει ήδη δημιουργήσει μια δομή ανάλυσης εργασίας, η δομή ανάλυσης εργασίας μπορεί να ανοίξει στην εφαρμογή Microsoft Project Client εάν η δομή ανάλυσης εργασίας βρίσκεται σε κατάσταση προσχεδίου.</span><span class="sxs-lookup"><span data-stu-id="164a4-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="164a4-116">Για να ανοίξετε από τη σελίδα **Έργο** , κάντε κλικ στη σύνδεση **Άνοιγμα στο Microsoft Project** από την καρτέλα **Σχεδιασμός**. Μπορείτε, επίσης, να ανοίξετε αυτήν τη σελίδα μέσα από την εφαρμογή Microsoft Project Client κάνοντας κλικ στο **Άνοιγμα** στην καρτέλα **Microsoft Dynamics 365**. Επιλέξτε τη **Νομική οντότητα** και το **Έργο** από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="164a4-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="164a4-117">Εάν χρησιμοποιείτε το Internet Explorer ως πρόγραμμα περιήγησής σας, θα πρέπει να κάνετε κλικ στην επιλογή **Αποθήκευση** για να ανοίξετε με μη αυτόματο τρόπο από τη θέση στην οποία θα γίνει λήψη του αρχείου.</span><span class="sxs-lookup"><span data-stu-id="164a4-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="164a4-118">Εναλλακτικά, κάντε κλικ στην επιλογή **Αποθήκευση και άνοιγμα** για να ανοίξετε το αρχείο στο Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="164a4-119">Μην μετονομάσετε το όνομα του αρχείου κατά την αποθήκευση.</span><span class="sxs-lookup"><span data-stu-id="164a4-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="164a4-120">Πριν κάνετε οποιαδήποτε επεξεργασία στο αρχείο χρησιμοποιώντας το Microsoft Project Client, θα πρέπει να το δείτε. Επιλέξτε **Έλεγχος** στην καρτέλα **Microsoft Dynamics 365**. Με αυτόν τον τρόπο οι άλλοι χρήστες δεν θα μπορούν να επεξεργαστούν τη δομή ανάλυσης εργασίας μέσα από το Finance την ίδια στιγμή.</span><span class="sxs-lookup"><span data-stu-id="164a4-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="164a4-121">Για να δημοσιεύσετε τη δομή ανάλυσης εργασίας μετά από την ολοκλήρωση οποιασδήποτε επεξεργασίας, κάντε κλικ στην επιλογή **Εισαγωγή** στην καρτέλα **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="164a4-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="164a4-122">Εάν μια ομάδα έργου έχει ήδη προστεθεί στο έργο στο Finance, η λίστα πόρων θα συμπληρωθεί με τα μέλη της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="164a4-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="164a4-123">Εάν μια ομάδα έργου δεν έχει προστεθεί ακόμα στο έργο, μπορείτε να επιλέξετε πόρους και να δημιουργήσετε την ομάδα εντός του Microsoft Project Client κάνοντας κλικ στο κουμπί **Πόροι** στην καρτέλα **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="164a4-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="164a4-124">Τα ακόλουθα δεδομένα θα συγχρονιστούν ξανά στο Finance ως μέρος της διεργασίας εισαγωγής:</span><span class="sxs-lookup"><span data-stu-id="164a4-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="164a4-125">•   Όνομα εργασίας</span><span class="sxs-lookup"><span data-stu-id="164a4-125">•   Task name</span></span>

<span data-ttu-id="164a4-126">•   Ημερομηνία έναρξης</span><span class="sxs-lookup"><span data-stu-id="164a4-126">•   Start date</span></span>

<span data-ttu-id="164a4-127">•   Ημερομηνία ολοκλήρωσης</span><span class="sxs-lookup"><span data-stu-id="164a4-127">•   Finish date</span></span>

<span data-ttu-id="164a4-128">•   Προκάτοχοι</span><span class="sxs-lookup"><span data-stu-id="164a4-128">•   Predecessors</span></span>

<span data-ttu-id="164a4-129">•   Ονόματα πόρων</span><span class="sxs-lookup"><span data-stu-id="164a4-129">•   Resource names</span></span>

<span data-ttu-id="164a4-130">•   Κατηγορία</span><span class="sxs-lookup"><span data-stu-id="164a4-130">•   Category</span></span>

<span data-ttu-id="164a4-131">•   Κατηγορία πόρου</span><span class="sxs-lookup"><span data-stu-id="164a4-131">•   Resource category</span></span>

<span data-ttu-id="164a4-132">•   Ώρες εργασίας</span><span class="sxs-lookup"><span data-stu-id="164a4-132">•   Work hours</span></span>

<span data-ttu-id="164a4-133">•   Σημειώσεις</span><span class="sxs-lookup"><span data-stu-id="164a4-133">•   Notes</span></span>

<span data-ttu-id="164a4-134">•   Προτεραιότητα</span><span class="sxs-lookup"><span data-stu-id="164a4-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="164a4-135">Εάν προσθέσετε άλλες στήλες στο αρχείο Microsoft Project Client, δεν θα αποθηκευτούν στο αρχείο και δεν θα εμφανίζονται όταν το αρχείο θα ανοίξει ξανά.</span><span class="sxs-lookup"><span data-stu-id="164a4-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="164a4-136">Δημιουργία της δομής ανάλυσης εργασίας για ένα υπάρχον έργο με χρήση του Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="164a4-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="164a4-137">Για δημιουργία της δομής ανάλυσης εργασίας για ένα υπάρχον έργο με χρήση του Microsoft Project Client ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="164a4-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="164a4-138">Ανοίξτε το Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="164a4-139">Στην καρτέλα **Microsoft Dynamics 365** , επιλέξτε **Άνοιγμα**.</span><span class="sxs-lookup"><span data-stu-id="164a4-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="164a4-140">Επιλέξτε τη **Νομική οντότητα** για το έργο.</span><span class="sxs-lookup"><span data-stu-id="164a4-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="164a4-141">Επιλέξτε το **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="164a4-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="164a4-142">Κάντε κλικ στην επιλογή **Έλεγχος** στην καρτέλα **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="164a4-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="164a4-143">Όταν είστε έτοιμοι να δημοσιεύσετε στο Finance, κάντε κλικ στην επιλογή **Εισαγωγή** στην καρτέλα **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="164a4-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="164a4-144">Αντικατάσταση της υπάρχουσας δομής ανάλυσης εργασίας για ένα υπάρχον έργο με χρήση του Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="164a4-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="164a4-145">Για να δημιουργήσετε μια νέα δομή ανάλυσης εργασίας χρησιμοποιώντας το Microsoft Project Client και να αντικαταστήσετε μια υπάρχουσα δομή ανάλυσης εργασίας για ένα υπάρχον έργο, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="164a4-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="164a4-146">Ανοίξτε το Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="164a4-147">Δημιουργήστε ένα χρονοδιάγραμμα στο Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="164a4-148">Στην καρτέλα **Microsoft Dynamics 365** , κάντε κλικ στην επιλογή **Αποθήκευση αλλαγών** > **Αντικατάσταση υπάρχοντος έργου**.</span><span class="sxs-lookup"><span data-stu-id="164a4-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="164a4-149">Επιλέξτε τη **Νομική οντότητα** για το έργο.</span><span class="sxs-lookup"><span data-stu-id="164a4-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="164a4-150">Επιλέξτε το **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="164a4-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="164a4-151">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="164a4-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="164a4-152">Δημιουργία νέου έργου μέσα από το Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="164a4-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="164a4-153">Ανοίξτε το Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="164a4-154">Δημιουργήστε ένα χρονοδιάγραμμα στο Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="164a4-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="164a4-155">Στην καρτέλα **Microsoft Dynamics 365** , κάντε κλικ στην επιλογή **Αποθήκευση αλλαγών** > **Αποθήκευση σε νέο έργο**.</span><span class="sxs-lookup"><span data-stu-id="164a4-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="164a4-156">Επιλέξτε τη **Νομική οντότητα** για το έργο.</span><span class="sxs-lookup"><span data-stu-id="164a4-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="164a4-157">Καταχωρίστε το **Αναγνωριστικό έργου** , εάν είναι απαραίτητο.</span><span class="sxs-lookup"><span data-stu-id="164a4-157">Enter the **Project ID** , if necessary.</span></span>

6.  <span data-ttu-id="164a4-158">Καταχωρίστε το **Όνομα έργου**.</span><span class="sxs-lookup"><span data-stu-id="164a4-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="164a4-159">Επιλέξτε **Τύπο έργου** , **Ομάδα έργου** και **Αναγνωριστικό σύμβασης έργου**.</span><span class="sxs-lookup"><span data-stu-id="164a4-159">Select the **Project type** , **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="164a4-160">Εναλλακτικά, μπορείτε να δημιουργήσετε μια νέα σύμβαση έργου κάνοντας κλικ στην επιλογή **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="164a4-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="164a4-161">Επιλέξτε το **Ημερολόγιο** που θα χρησιμοποιηθεί για την επιλογή των πόρων.</span><span class="sxs-lookup"><span data-stu-id="164a4-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="164a4-162">Κάντε κλικ στο κουμπί **OK**.</span><span class="sxs-lookup"><span data-stu-id="164a4-162">Click **OK**.</span></span>
