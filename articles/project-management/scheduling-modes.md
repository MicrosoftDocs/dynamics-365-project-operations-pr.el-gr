---
title: Λειτουργίες προγραμματισμού
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις λειτουργίες προγραμματισμού.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 508ff1df8f7e31066712fab6f8871dfdb107a43b
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116707"
---
# <a name="scheduling-modes"></a><span data-ttu-id="842ac-103">Λειτουργίες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="842ac-103">Scheduling modes</span></span>

<span data-ttu-id="842ac-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="842ac-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="842ac-105">Το Dynamics 365 Project Operations παρέχει στους οργανισμούς τη δυνατότητα να καθορίζουν τον τρόπο με τον οποίο διαχειρίζονται τις αλλαγές σε βασικές μεταβλητές σε εργασίες εντός της δομής ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="842ac-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="842ac-106">Με βάση τις συγκεκριμένες ανάγκες του οργανισμού, οι διαχειριστές έργου μπορούν να κάνουν αλλαγές στη λειτουργία προγραμματισμού κατά τη δημιουργία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="842ac-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="842ac-107">Υπάρχουν τρεις λειτουργίες προγραμματισμού διαθέσιμες στο Project Operations:</span><span class="sxs-lookup"><span data-stu-id="842ac-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="842ac-108">Σταθερή διάρκεια (αυτή είναι η προεπιλεγμένη λειτουργία)</span><span class="sxs-lookup"><span data-stu-id="842ac-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="842ac-109">Σταθερή προσπάθεια (*Εργασία*)</span><span class="sxs-lookup"><span data-stu-id="842ac-109">Fixed effort (*Work*)</span></span>
  - <span data-ttu-id="842ac-110">Σταθερές μονάδες</span><span class="sxs-lookup"><span data-stu-id="842ac-110">Fixed units</span></span>

<span data-ttu-id="842ac-111">Οι τιμές που επηρεάζουν τον ορισμό μιας συγκεκριμένης λειτουργίας προγραμματισμού καθορίζονται από τον ακόλουθο τύπο:</span><span class="sxs-lookup"><span data-stu-id="842ac-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="842ac-112">Προσπάθεια = Διάρκεια x Μονάδες</span><span class="sxs-lookup"><span data-stu-id="842ac-112">Effort  = Duration x Units</span></span>

<span data-ttu-id="842ac-113">Όταν ορίζετε τη λειτουργία προγραμματισμού ενός έργου, ορίζετε μία από αυτές τις τιμές, οι οποίες στη συνέχεια δεν μπορούν να αλλάξουν.</span><span class="sxs-lookup"><span data-stu-id="842ac-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="842ac-114">Κρατώντας αυτήν την τιμή ως σταθερή, η τιμή αυτή έχει προτεραιότητα, γεγονός που ειδοποιεί το σύστημα να μην την αλλάξει όταν αλλάξουν οι άλλες δύο τιμές.</span><span class="sxs-lookup"><span data-stu-id="842ac-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="842ac-115">Ο παρακάτω πίνακας παρέχει πληροφορίες σχετικά με τις επιπτώσεις από την επιλογή μιας συγκεκριμένης λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="842ac-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="842ac-116">**Σε αυτή την εργασία**</span><span class="sxs-lookup"><span data-stu-id="842ac-116">**In this task**</span></span>             | <span data-ttu-id="842ac-117">**Εάν αναθεωρήσετε μονάδες**</span><span class="sxs-lookup"><span data-stu-id="842ac-117">**If you revise units**</span></span>   | <span data-ttu-id="842ac-118">**Εάν αναθεωρήσετε διάρκεια**</span><span class="sxs-lookup"><span data-stu-id="842ac-118">**If you revise duration**</span></span> | <span data-ttu-id="842ac-119">**Εάν αναθεωρήσετε έργο**</span><span class="sxs-lookup"><span data-stu-id="842ac-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="842ac-120">Εργασία σταθερών μονάδων</span><span class="sxs-lookup"><span data-stu-id="842ac-120">Fixed units task</span></span>     | <span data-ttu-id="842ac-121">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-121">Duration is recalculated.</span></span> | <span data-ttu-id="842ac-122">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-122">Effort is recalculated.</span></span>    | <span data-ttu-id="842ac-123">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="842ac-124">Εργασία σταθερού έργου</span><span class="sxs-lookup"><span data-stu-id="842ac-124">Fixed effort task</span></span>    | <span data-ttu-id="842ac-125">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-125">Duration is recalculated.</span></span> | <span data-ttu-id="842ac-126">Οι μονάδες υπολογίζονται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-126">Units are recalculated.</span></span>    | <span data-ttu-id="842ac-127">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="842ac-128">Εργασία με σταθερή διάρκεια</span><span class="sxs-lookup"><span data-stu-id="842ac-128">Fixed duration task</span></span>  | <span data-ttu-id="842ac-129">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-129">Effort is recalculated.</span></span>   | <span data-ttu-id="842ac-130">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-130">Effort is recalculated.</span></span>    | <span data-ttu-id="842ac-131">Οι μονάδες υπολογίζονται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="842ac-131">Units are recalculated.</span></span>   |

<span data-ttu-id="842ac-132">Για περισσότερες πληροφορίες σχετικά με τις επιπτώσεις μιας δεδομένης λειτουργίας, ανατρέξτε στο θέμα [Αλλαγή του τύπου εργασίας για πιο ακριβή προγραμματισμό](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="842ac-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="842ac-133">Στο θέμα, ο όρος **Εργασία** χρησιμοποιείται αντί για τον όρο **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="842ac-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="842ac-134">Αλλαγή της λειτουργίας προγραμματισμού του οργανισμού</span><span class="sxs-lookup"><span data-stu-id="842ac-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="842ac-135">Ολοκληρώστε τα παρακάτω βήματα για να καθορίσετε τη λειτουργία προγραμματισμού ενός οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="842ac-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="842ac-136">Μεταβείτε στο **Ρυθμίσεις** \> **Γενικά** \> **Παράμετροι** και, στη συνέχεια, επιλέξτε την παράμετρο έργου.</span><span class="sxs-lookup"><span data-stu-id="842ac-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="842ac-137">Στη σελίδα **Παράμετροι έργου**, επιλέξτε την προεπιλεγμένη λειτουργία προγραμματισμού για τον οργανισμό και, στη συνέχεια, ορίστε τη δυνατότητα του διαχειριστή έργου να παρακάμπτει τη ρύθμιση κατά τη δημιουργία ενός νέου έργου.</span><span class="sxs-lookup"><span data-stu-id="842ac-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="842ac-138">Αλλαγή της ρύθμισης λειτουργίας προγραμματισμού σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="842ac-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="842ac-139">Εάν ένας οργανισμός επιτρέπει στο διαχειριστή έργου να αντικαταστήσει την προεπιλεγμένη λειτουργία προγραμματισμού, ο Διαχειριστής έργου μπορεί να κάνει αυτήν την αλλαγή όταν δημιουργεί ένα νέο έργο.</span><span class="sxs-lookup"><span data-stu-id="842ac-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="842ac-140">Ωστόσο, αφού αποθηκευτεί το έργο, η λειτουργία προγραμματισμού δεν μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="842ac-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="842ac-141">Έργα που αντιγράφηκαν</span><span class="sxs-lookup"><span data-stu-id="842ac-141">Copied projects</span></span>

<span data-ttu-id="842ac-142">Επειδή ένα έργο δημιουργείται κατά την υλοποίηση της ενέργειας αντιγραφής έργου, ο Διαχειριστής έργου δεν μπορεί να ορίσει τη λειτουργία προγραμματισμού.</span><span class="sxs-lookup"><span data-stu-id="842ac-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="842ac-143">Το έργο προορισμού θα είναι πάντα προεπιλεγμένο στη λειτουργία που ορίζεται στο οργανωτικό επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="842ac-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="842ac-144">Εργασίες που έχουν αντιγραφεί</span><span class="sxs-lookup"><span data-stu-id="842ac-144">Copied tasks</span></span>

<span data-ttu-id="842ac-145">Όταν μια εργασία αντιγράφεται από ένα έργο σε ένα άλλο, η εργασία μεταβιβάζεται στη λειτουργία προγραμματισμού του έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="842ac-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
