---
title: Δημιουργία χρονικών καταχώρησεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας χρονικών καταχωρήσεων.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 878413a24baa340b745a045a6991a63a00851c8b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077007"
---
# <a name="create-time-entries"></a><span data-ttu-id="e6bd3-103">Δημιουργία χρονικών καταχώρησεων</span><span class="sxs-lookup"><span data-stu-id="e6bd3-103">Create time entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e6bd3-104">Σε προηγούμενες εκδόσεις του Dynamics 365 Project Service Automation, καταχωρήθηκαν καταχωρήσεις χρόνου σε εβδομαδιαία βάση.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="e6bd3-105">Στην έκδοση 3 του Project Service Automation, οι καταχωρήσεις χρόνου καταχωρούνται σε καθημερινή βάση.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="e6bd3-106">Ωστόσο, μετά από τη δημιουργία μερικών καταχωρήσεων χρόνου, μπορείτε να τις δημιουργήσετε ή να τις αντιγράψετε μαζικά.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="e6bd3-107">Δημιουργία χρονικής καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="e6bd3-107">Create a time entry</span></span>

<span data-ttu-id="e6bd3-108">Για να δημιουργήσετε μια χρονική καταχώρηση, ακολουθήστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="e6bd3-109">Στη σελίδα **Χρονικές καταχωρήσεις** , επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="e6bd3-110">Στο παράθυρο διαλόγου **Γρήγορη δημιουργία: καταχώρηση χρόνου** , πληκτρολογήστε τη διάρκεια της καταχώρησης του χρόνου σε λεπτά, ώρες ή ημέρες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="e6bd3-111">Η εισαγωγή της διάρκειας πρέπει να ακολουθεί την εξής μορφή: *x* λεπτά", *x* ώρες ή *x* ημέρες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="e6bd3-112">Κατά την εισαγωγή των ωρών και των ημερών μπορούν επίσης να χρησιμοποιούνται δεκαδικά ψηφία, για παράδειγμα *x,x* ώρες ή *x,x* ημέρες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="e6bd3-113">Επιλέξτε τον τύπο της καταχώρησης ώρας και το έργο στο οποίο εισαγάγετε την καταχώρηση του χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="e6bd3-114">Στο πεδίο **Εργασία έργου** , βρείτε την εργασία για αυτήν την καταχώρηση ώρας.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e6bd3-115">Εάν δημιουργείτε μια καταχώρηση χρόνου για μια εργασία που δεν έχει ανατεθεί σε ένα χρήστη, στο πεδίο **Εργασία έργου** , επιλέξτε το κουμπί **Αναζήτηση** , επιλέξτε **Αλλαγή προβολής** και μετά **Όλες οι ενεργές εργασίες έργου** για να δείτε όλες τις εργασίες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View** , and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="e6bd3-116">Καταγράψτε μια περιγραφή, εάν απαιτείται μια περιγραφή και, στη συνέχεια επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="e6bd3-117">Μετά τη δημιουργία και την αποθήκευση της καταχώρησης χρόνου, μπορείτε να την επεξεργαστείτε στο πλέγμα χρονικών καταχωρίσεων.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="e6bd3-118">Το πλέγμα χρονικών καταχωρίσεων υποστηρίζει δύο μορφές:</span><span class="sxs-lookup"><span data-stu-id="e6bd3-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="e6bd3-119">Μπορείτε να εισάγετε καταχωρήσεις χρόνου σε μορφή **ωω:λλ**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="e6bd3-120">Στη συνέχεια, αυτή η μορφή μετατρέπεται σε ώρες και κλάσματα.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="e6bd3-121">Μπορείτε να εισάγετε απευθείας τις ώρες και τα κλάσματα.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="e6bd3-122">Λάβετε υπόψη σας ότι τα κλάσματα μιας ώρας δεν είναι λεπτά.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="e6bd3-123">Ως εκ τούτου, 1,5 ώρες αντιπροσωπεύει 1 ώρα και 30 λεπτά.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="e6bd3-124">Ο ίδιος κανόνας ισχύει για τα κλάσματα μιας ημέρας.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="e6bd3-125">Μια ημέρα είναι 24 ώρες και 0,5 ημέρες αντιπροσωπεύουν 12 ώρες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="e6bd3-126">Μαζική δημιουργία χρονικών καταχώρησεων</span><span class="sxs-lookup"><span data-stu-id="e6bd3-126">Bulk create time entries</span></span>

<span data-ttu-id="e6bd3-127">Μετά τη δημιουργία μερικών χρονικών καταχωρήσεων, μπορείτε να τις αντιγράψετε για να δημιουργήσετε μαζικά πρόσθετες χρονικές καταχωρήσεις.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="e6bd3-128">Στη σελίδα **Χρονικές καταχωρήσεις** , επιλέξτε **Αντιγραφή εβδομάδας**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="e6bd3-129">Στην ομάδα πεδίων **Από την περίοδο** , χρησιμοποιήστε τα πεδία **Ημερομηνία έναρξης** και **Ημερομηνία λήξης** για να ορίσετε το εύρος ημερομηνιών από τις οποίες θα κάνετε αντιγραφή καταχωρήσεων χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="e6bd3-130">Στην ομάδα πεδίων **Έως περίοδο** , στο πεδίο **Ημερομηνία έναρξης** , καθορίστε την ημερομηνία δημιουργίας καταχωρήσεων χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="e6bd3-131">Επιλέξτε **Αντιγραφή** για να δημιουργήσετε ένα αντίγραφο των χρονικών καταχωρήσεων που αντιστοιχούν στην ημέρα της εβδομάδας που καθορίζεται στην ομάδα πεδίων **Έως περίοδο**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="e6bd3-132">Για παράδειγμα, η καταχώρηση χρόνου για Δευτέρα από την προηγούμενη εβδομάδα θα αντιγραφεί στη Δευτέρα για την εβδομάδα που υποδεικνύεται στην ομάδα πεδίων **Έως περίοδο**.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="e6bd3-133">Εισαγωγή δεδομένων για χρονικές καταχωρίσεις</span><span class="sxs-lookup"><span data-stu-id="e6bd3-133">Import data for time entries</span></span>

<span data-ttu-id="e6bd3-134">Μπορείτε να εισαγάγετε δεδομένα από τις κρατήσεις και τις αναθέσεις του έργου.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="e6bd3-135">Όταν εισάγετε δεδομένα, μπορείτε να καθορίσετε το εύρος ημερομηνιών των κρατήσεων που θα εισαγάγετε και, στη συνέχεια, να επιλέξετε ρητά τις κρατήσεις που θα πρέπει να δημιουργηθούν ως **προσχέδια** καταχωρήσεων χρόνου.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="e6bd3-136">Ομαδοποίηση κατά, ταξινόμηση, αναζήτηση και φιλτράρισμα</span><span class="sxs-lookup"><span data-stu-id="e6bd3-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="e6bd3-137">Μπορείτε να ομαδοποιήσετε και να φιλτράρετε καταχωρήσεις χρόνου με βάση τις διαστάσεις που καθορίζονται στις στήλες.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="e6bd3-138">Στο πεδίο **Ομαδοποίηση κατά** , επιλέξτε τη διάσταση που θα χρησιμοποιηθεί για την φιλτράρισμα καταχωρήσεων ώρας.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="e6bd3-139">Μπορείτε, επίσης, να ταξινομήσετε τις καρτέλες της καταχώρησης ώρας σε αύξουσα ή φθίνουσα σειρά χρησιμοποιώντας το βέλος ταξινόμησης στις επικεφαλίδες των στηλών.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="e6bd3-140">Επιπλέον, μπορείτε να εμφανίσετε ή να αποκρύψετε καταχωρήσεις επιλέγοντας το κουμπί **Φίλτρο** στις επικεφαλίδες των στηλών και, στη συνέχεια, στο πλαίσιο **Αναζήτηση** , εισάγοντας το κείμενο που θα πρέπει να χρησιμοποιηθεί για την αναζήτηση καταχωρήσεων χρόνου κατά όνομα έργου, εργασία έργου, ώρα καταχώρηση ή πόρο.</span><span class="sxs-lookup"><span data-stu-id="e6bd3-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>
