---
title: Λειτουργίες προγραμματισμού
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις λειτουργίες προγραμματισμού.
author: ruhercul
manager: AnnBe
ms.date: 05/04/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe54944999617b248ff925148a78601dd4be7aca
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981435"
---
# <a name="scheduling-modes"></a><span data-ttu-id="c1788-103">Λειτουργίες προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="c1788-103">Scheduling modes</span></span>

<span data-ttu-id="c1788-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="c1788-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c1788-105">Το Dynamics 365 Project Operations παρέχει στους οργανισμούς τη δυνατότητα να καθορίζουν τον τρόπο με τον οποίο διαχειρίζονται τις αλλαγές σε βασικές μεταβλητές σε εργασίες εντός της δομής ανάλυσης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="c1788-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="c1788-106">Με βάση τις συγκεκριμένες ανάγκες του οργανισμού, οι διαχειριστές έργου μπορούν να κάνουν αλλαγές στη λειτουργία προγραμματισμού κατά τη δημιουργία ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="c1788-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="c1788-107">Υπάρχουν τρεις λειτουργίες προγραμματισμού διαθέσιμες στο Project Operations:</span><span class="sxs-lookup"><span data-stu-id="c1788-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="c1788-108">Σταθερή διάρκεια (αυτή είναι η προεπιλεγμένη λειτουργία)</span><span class="sxs-lookup"><span data-stu-id="c1788-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="c1788-109">Σταθερή εργασία</span><span class="sxs-lookup"><span data-stu-id="c1788-109">Fixed work</span></span>
  - <span data-ttu-id="c1788-110">Σταθερές μονάδες</span><span class="sxs-lookup"><span data-stu-id="c1788-110">Fixed units</span></span>

<span data-ttu-id="c1788-111">Οι τιμές που επηρεάζουν τον ορισμό μιας συγκεκριμένης λειτουργίας προγραμματισμού καθορίζονται από τον ακόλουθο τύπο:</span><span class="sxs-lookup"><span data-stu-id="c1788-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="c1788-112">Έργο (*Εργασία*) = Διάρκεια x Μονάδες</span><span class="sxs-lookup"><span data-stu-id="c1788-112">Effort (*Work*) = Duration x Units</span></span>

<span data-ttu-id="c1788-113">Όταν ορίζετε τη λειτουργία προγραμματισμού ενός έργου, ορίζετε μία από αυτές τις τιμές, οι οποίες στη συνέχεια δεν μπορούν να αλλάξουν.</span><span class="sxs-lookup"><span data-stu-id="c1788-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="c1788-114">Κρατώντας αυτήν την τιμή ως σταθερή, η τιμή αυτή έχει προτεραιότητα, γεγονός που ειδοποιεί το σύστημα να μην την αλλάξει όταν αλλάξουν οι άλλες δύο τιμές.</span><span class="sxs-lookup"><span data-stu-id="c1788-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="c1788-115">Ο παρακάτω πίνακας παρέχει πληροφορίες σχετικά με τις επιπτώσεις από την επιλογή μιας συγκεκριμένης λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="c1788-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="c1788-116">**Σε αυτή την εργασία**</span><span class="sxs-lookup"><span data-stu-id="c1788-116">**In this task**</span></span>             | <span data-ttu-id="c1788-117">**Εάν αναθεωρήσετε μονάδες**</span><span class="sxs-lookup"><span data-stu-id="c1788-117">**If you revise units**</span></span>   | <span data-ttu-id="c1788-118">**Εάν αναθεωρήσετε διάρκεια**</span><span class="sxs-lookup"><span data-stu-id="c1788-118">**If you revise duration**</span></span> | <span data-ttu-id="c1788-119">**Εάν αναθεωρήσετε έργο**</span><span class="sxs-lookup"><span data-stu-id="c1788-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="c1788-120">Εργασία σταθερών μονάδων</span><span class="sxs-lookup"><span data-stu-id="c1788-120">Fixed units task</span></span>     | <span data-ttu-id="c1788-121">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-121">Duration is recalculated.</span></span> | <span data-ttu-id="c1788-122">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-122">Effort is recalculated.</span></span>    | <span data-ttu-id="c1788-123">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="c1788-124">Εργασία σταθερού έργου</span><span class="sxs-lookup"><span data-stu-id="c1788-124">Fixed effort task</span></span>    | <span data-ttu-id="c1788-125">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-125">Duration is recalculated.</span></span> | <span data-ttu-id="c1788-126">Οι μονάδες υπολογίζονται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-126">Units are recalculated.</span></span>    | <span data-ttu-id="c1788-127">Η διάρκεια υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="c1788-128">Εργασία με σταθερή διάρκεια</span><span class="sxs-lookup"><span data-stu-id="c1788-128">Fixed duration task</span></span>  | <span data-ttu-id="c1788-129">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-129">Effort is recalculated.</span></span>   | <span data-ttu-id="c1788-130">Το έργο υπολογίζεται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-130">Effort is recalculated.</span></span>    | <span data-ttu-id="c1788-131">Οι μονάδες υπολογίζονται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="c1788-131">Units are recalculated.</span></span>   |

<span data-ttu-id="c1788-132">Για περισσότερες πληροφορίες σχετικά με τις επιπτώσεις μιας δεδομένης λειτουργίας, ανατρέξτε στο θέμα [Αλλαγή του τύπου εργασίας για πιο ακριβή προγραμματισμό](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="c1788-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="c1788-133">Στο θέμα, ο όρος **Εργασία** χρησιμοποιείται αντί για τον όρο **Έργο**.</span><span class="sxs-lookup"><span data-stu-id="c1788-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="c1788-134">Αλλαγή της λειτουργίας προγραμματισμού του οργανισμού</span><span class="sxs-lookup"><span data-stu-id="c1788-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="c1788-135">Ολοκληρώστε τα παρακάτω βήματα για να καθορίσετε τη λειτουργία προγραμματισμού ενός οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="c1788-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="c1788-136">Μεταβείτε στο **Ρυθμίσεις** \> **Γενικά** \> **Παράμετροι** και, στη συνέχεια, επιλέξτε την παράμετρο έργου.</span><span class="sxs-lookup"><span data-stu-id="c1788-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="c1788-137">Στη σελίδα **Παράμετροι έργου**, επιλέξτε την προεπιλεγμένη λειτουργία προγραμματισμού για τον οργανισμό και, στη συνέχεια, ορίστε τη δυνατότητα του διαχειριστή έργου να παρακάμπτει τη ρύθμιση κατά τη δημιουργία ενός νέου έργου.</span><span class="sxs-lookup"><span data-stu-id="c1788-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="c1788-138">Αλλαγή της ρύθμισης λειτουργίας προγραμματισμού σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="c1788-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="c1788-139">Εάν ένας οργανισμός επιτρέπει στο διαχειριστή έργου να αντικαταστήσει την προεπιλεγμένη λειτουργία προγραμματισμού, ο Διαχειριστής έργου μπορεί να κάνει αυτήν την αλλαγή όταν δημιουργεί ένα νέο έργο.</span><span class="sxs-lookup"><span data-stu-id="c1788-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="c1788-140">Ωστόσο, αφού αποθηκευτεί το έργο, η λειτουργία προγραμματισμού δεν μπορεί να αλλάξει.</span><span class="sxs-lookup"><span data-stu-id="c1788-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="c1788-141">Έργα που αντιγράφηκαν</span><span class="sxs-lookup"><span data-stu-id="c1788-141">Copied projects</span></span>

<span data-ttu-id="c1788-142">Επειδή ένα έργο δημιουργείται κατά την υλοποίηση της ενέργειας αντιγραφής έργου, ο Διαχειριστής έργου δεν μπορεί να ορίσει τη λειτουργία προγραμματισμού.</span><span class="sxs-lookup"><span data-stu-id="c1788-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="c1788-143">Το έργο προορισμού θα είναι πάντα προεπιλεγμένο στη λειτουργία που ορίζεται στο οργανωτικό επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="c1788-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="c1788-144">Εργασίες που έχουν αντιγραφεί</span><span class="sxs-lookup"><span data-stu-id="c1788-144">Copied tasks</span></span>

<span data-ttu-id="c1788-145">Όταν μια εργασία αντιγράφεται από ένα έργο σε ένα άλλο, η εργασία μεταβιβάζεται στη λειτουργία προγραμματισμού του έργου προορισμού.</span><span class="sxs-lookup"><span data-stu-id="c1788-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
