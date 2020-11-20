---
title: Ζητήματα αναβάθμισης για τη δομή ανάλυσης εργασίας
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναβάθμιση της δομής ανάλυσης εργασίας από το Project Service Automation 2.x σε 3.x.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121803"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="b0933-103">Ζητήματα αναβάθμισης για τη δομή ανάλυσης εργασίας</span><span class="sxs-lookup"><span data-stu-id="b0933-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="b0933-104">Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναβάθμιση της δομής ανάλυσης εργασίας από το Project Service Automation 2.x σε 3.x.</span><span class="sxs-lookup"><span data-stu-id="b0933-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="b0933-105">Αυτό το θέμα προσδιορίζει την εύρυθμη κατάσταση ενός έργου στο Project Service Automation (PSA) που απαιτείται για μια επιτυχημένη αναβάθμιση.</span><span class="sxs-lookup"><span data-stu-id="b0933-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="b0933-106">Υπάρχουν επίσης πληροφορίες σχετικά με τις συνηθισμένες συνθήκες αποκλεισμού που θα προκαλέσουν την αποτυχία της αναβάθμισης.</span><span class="sxs-lookup"><span data-stu-id="b0933-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="b0933-107">Για περισσότερες πληροφορίες σχετικά με τον καθορισμό εργασιών έργου και των λειτουργιών τους εντός χρονοδιαγράμματος έργου δείτε [Χρονοδιαγράμματα έργου](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="b0933-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="b0933-108">Βασικές οντότητες</span><span class="sxs-lookup"><span data-stu-id="b0933-108">Key entities</span></span>
<span data-ttu-id="b0933-109">Για μια ακριβή δομή ανάλυσης εργασίας που έχει ήδη φορτωθεί με πόρους, απαιτούνται οι ακόλουθες οντότητες:</span><span class="sxs-lookup"><span data-stu-id="b0933-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="b0933-110">Έργο</span><span class="sxs-lookup"><span data-stu-id="b0933-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="b0933-111">Ομάδα έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="b0933-112">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="b0933-113">Αναθέσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="b0933-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="b0933-114">Εξάρτηση εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="b0933-115">Πόροι με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="b0933-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="b0933-116">Για να καθορίσετε μια φορτωμένη δομή ανάλυσης εργασίας πόρου πρέπει να ολοκληρώσετε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="b0933-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="b0933-117">Δημιουργία νέου έργου.</span><span class="sxs-lookup"><span data-stu-id="b0933-117">Create a new project.</span></span> <span data-ttu-id="b0933-118">Για περισσότερες πληροφορίες σχετικά με τον τρόπο δημιουργίας ενός νέου έργου, δείτε [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="b0933-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="b0933-119">Δημιουργήστε μία ή περισσότερες εργασίες.</span><span class="sxs-lookup"><span data-stu-id="b0933-119">Create one or more tasks.</span></span> <span data-ttu-id="b0933-120">Για περισσότερες πληροφορίες σχετικά με τον τρόπο δημιουργίας μιας εργασίας δείτε [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="b0933-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="b0933-121">Καθορίστε τις εξαρτήσεις εργασιών.</span><span class="sxs-lookup"><span data-stu-id="b0933-121">Define the task dependencies.</span></span> <span data-ttu-id="b0933-122">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Εξάρτηση εργασίας έργου](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span><span class="sxs-lookup"><span data-stu-id="b0933-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="b0933-123">Ανάθεση μελών ομάδας έργου στο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-123">Assign project team members to the project.</span></span> <span data-ttu-id="b0933-124">Για περισσότερες πληροφορίες, δείτε [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)</span><span class="sxs-lookup"><span data-stu-id="b0933-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="b0933-125">Ανάθεση μελών ομάδας έργου σε εργασίες.</span><span class="sxs-lookup"><span data-stu-id="b0933-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="b0933-126">Για περισσότερες πληροφορίες, δείτε [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)</span><span class="sxs-lookup"><span data-stu-id="b0933-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="b0933-127">Σχέσεις ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-127">Project team relationships</span></span>

<span data-ttu-id="b0933-128">Για να εξασφαλίσετε μια επιτυχημένη αναβάθμιση, πρέπει να διατηρηθούν σωστά οι παρακάτω σχέσεις:</span><span class="sxs-lookup"><span data-stu-id="b0933-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="b0933-129">Όλα τα μέλη της ομάδας έργου πρέπει να συσχετιστούν με έναν πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="b0933-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="b0933-130">Όλα τα μέλη της ομάδας έργου πρέπει να συσχετιστούν με το ίδιο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="b0933-131">Σχέσεις εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-131">Project task relationships</span></span>
<span data-ttu-id="b0933-132">Για να εξασφαλίσετε μια επιτυχημένη αναβάθμιση, πρέπει να διατηρηθούν σωστά οι παρακάτω σχέσεις:</span><span class="sxs-lookup"><span data-stu-id="b0933-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="b0933-133">Οποιεσδήποτε σχετικές εργασίες πρέπει να συσχετιστούν με το ίδιο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="b0933-134">Κάθε εργασία με γραμμές πρέπει να έχει μια γονική εργασία.</span><span class="sxs-lookup"><span data-stu-id="b0933-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="b0933-135">Κάθε εργασία με γραμμές πρέπει να έχει ένα γονικό έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="b0933-136">Έγκυρες συνθήκες</span><span class="sxs-lookup"><span data-stu-id="b0933-136">Valid conditions</span></span>

- <span data-ttu-id="b0933-137">Όλες οι διάρκειες εργασιών πρέπει να είναι μεγαλύτερες ή ίσες με (> =) μία ώρα και λιγότερο από 1.800.000 λεπτά (1.250 ημέρες).\*</span><span class="sxs-lookup"><span data-stu-id="b0933-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="b0933-138">Όλες οι εργασίες πρέπει να έχουν ημερομηνία έναρξης όχι νωρίτερη από 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="b0933-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="b0933-139">Όλες οι εργασίες πρέπει να έχουν μια ημερομηνία έναρξης το αργότερο 17 ετών από την παρούσα ημερομηνία.\*</span><span class="sxs-lookup"><span data-stu-id="b0933-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="b0933-140">Όλες οι εργασίες πρέπει να έχουν μια ημερομηνία έναρξης προγενέστερη ή ίση με την ημερομηνία λήξης τους.</span><span class="sxs-lookup"><span data-stu-id="b0933-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="b0933-141">Όλοι οι τύποι συναλλαγών στις ταξινομήσεις (δαπάνη, υλικό, φόρος και χρόνος) πρέπει να έχουν τιμές για **Προεπιλεγμένη μονάδα** και **Ομάδα μονάδων**.</span><span class="sxs-lookup"><span data-stu-id="b0933-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="b0933-142">Πρέπει να αποφεύγονται οι μορφές ημερομηνιών με γράμματα.</span><span class="sxs-lookup"><span data-stu-id="b0933-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="b0933-143">Πιθανά βήματα άμβλυνσης</span><span class="sxs-lookup"><span data-stu-id="b0933-143">Potential mitigation steps</span></span>
- <span data-ttu-id="b0933-144">Χρησιμοποιήστε τα πρόσθετα κριτήρια εύρεσης για να αναγνωρίσετε εργασίες έργου που δεν περιέχουν αναγνωριστικό έργου.</span><span class="sxs-lookup"><span data-stu-id="b0933-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="b0933-145">Χρησιμοποιήστε τα πρόσθετα κριτήρια εύρεσης για να προσδιορίσετε τις εργασίες έργου όπου η προγραμματισμένη διάρκεια είναι μεγαλύτερη από > 1.800.000.</span><span class="sxs-lookup"><span data-stu-id="b0933-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="b0933-146">Πριν κάνετε αλλαγές στα δεδομένα, θα πρέπει να εξετάσετε τυχόν προσαρμογές που σχετίζονται με την οντότητα που μπορεί να οδήγησαν στο να λάβετε τα δεδομένα σε κακή κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="b0933-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="b0933-147">Αυτές οι προσαρμογές θα πρέπει να αντιμετωπιστούν πριν προχωρήσετε με τις ενημερώσεις που σχετίζονται με τα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="b0933-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="b0933-148">Για τις καθορισμένες εργασίες που έχουν μείνει ορφανές, δοκιμάστε να διαγράψετε αυτές τις εργασίες εάν δεν είναι απαραίτητες ή εάν πρέπει να συσχετιστούν με το σωστό γονικό έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="b0933-149">Για οποιεσδήποτε εργασίες όπου η διάρκεια είναι μεγαλύτερη από 1.250 ημέρες, δοκιμάστε να προσθέσετε πολλές εργασίες ώστε να αντιπροσωπεύουν τη συνολική διάρκεια, εάν είναι εφικτό.</span><span class="sxs-lookup"><span data-stu-id="b0933-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="b0933-150">Τα στοιχεία που σημειώνονται με αστερίσκο (\*) έχουν όρια που οφείλονται στο γεγονός ότι η διαχείριση πελατειακών σχέσεων (CRM) υποστηρίζει μόνο επεκτάσεις επαναλαμβανόμενης εμφάνισης 7.320.</span><span class="sxs-lookup"><span data-stu-id="b0933-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="b0933-151">Πρέπει να μείνετε κάτω από αυτό το όριο.</span><span class="sxs-lookup"><span data-stu-id="b0933-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="b0933-152">Σχέσεις ανάθεσης πόρων</span><span class="sxs-lookup"><span data-stu-id="b0933-152">Resource Assignment relationships</span></span>
<span data-ttu-id="b0933-153">Για να εξασφαλίσετε μια επιτυχημένη αναβάθμιση, πρέπει να διατηρηθούν σωστά οι παρακάτω σχέσεις:</span><span class="sxs-lookup"><span data-stu-id="b0933-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="b0933-154">Όλες οι αναθέσεις πόρων σε μια δομή ανάλυσης εργασίας πρέπει να σχετίζονται με το ίδιο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="b0933-155">Όλες οι αναθέσεις πόρων σε μια δομή ανάλυσης εργασίας πρέπει να σχετίζονται με τα μέλη ομάδας έργου στο ίδιο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="b0933-156">Πιθανά βήματα άμβλυνσης</span><span class="sxs-lookup"><span data-stu-id="b0933-156">Potential mitigation steps</span></span>
- <span data-ttu-id="b0933-157">Προσδιορίστε όλες τις εργασίες που δεν συμπεριλαμβάνονται στις συνθήκες που περιγράφονται παραπάνω.</span><span class="sxs-lookup"><span data-stu-id="b0933-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="b0933-158">Οι αναθέσεις πόρων που δεν είναι πλέον έγκυρες πρέπει να διαγραφούν.</span><span class="sxs-lookup"><span data-stu-id="b0933-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="b0933-159">Σχέσεις εξάρτησης εργασίας έργου</span><span class="sxs-lookup"><span data-stu-id="b0933-159">Project task dependency relationships</span></span>
<span data-ttu-id="b0933-160">Για να εξασφαλίσετε μια επιτυχημένη αναβάθμιση, πρέπει να διατηρηθούν σωστά οι παρακάτω σχέσεις:</span><span class="sxs-lookup"><span data-stu-id="b0933-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="b0933-161">Όλες οι εξαρτήσεις εργασιών έργου πρέπει να σχετίζονται με το ίδιο έργο.</span><span class="sxs-lookup"><span data-stu-id="b0933-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="b0933-162">Μια εργασία δεν μπορεί να έχει την ίδια εξάρτηση που αναφέρεται περισσότερες από μία φορές.</span><span class="sxs-lookup"><span data-stu-id="b0933-162">A task can't have the same dependency referenced more than once.</span></span>
