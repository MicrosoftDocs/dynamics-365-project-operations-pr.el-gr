---
title: Γιατί η τιμή είναι μηδέν κατά προεπιλογή στις πραγματικές δαπάνες κόστους;
description: Οι παρακάτω τρεις έλεγχοι θα σας βοηθήσουν να αντιμετωπίσετε το γιατί η τιμή είναι κατά προεπιλογή 0 σε πραγματικές δαπάνες κόστους.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
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
ms.openlocfilehash: 5840bda4f74c720bfcdc7f4e84c8f22e0c6163ec
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076936"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-sales-actuals"></a><span data-ttu-id="a1637-103">Γιατί η τιμή είναι μηδέν κατά προεπιλογή στις πραγματικές δαπάνες κόστους;</span><span class="sxs-lookup"><span data-stu-id="a1637-103">Why is the price defaulting to zero on expense sales actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a1637-104">Αυτές οι συνήθεις ερωτήσεις εφαρμόζονται σε πραγματικά στοιχεία όπου η κλάση συναλλαγής έχει οριστεί σε Έξοδο και ο τύπος συναλλαγής είναι Μη χρεωμένες πωλήσεις.</span><span class="sxs-lookup"><span data-stu-id="a1637-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Unbilled Sales.</span></span> <span data-ttu-id="a1637-105">Οι παρακάτω τρεις έλεγχοι θα σας βοηθήσουν να αντιμετωπίσετε το γιατί η τιμή (ποσοστό χρέωσης) είναι κατά προεπιλογή 0 σε πραγματικό χρόνο εξόδου.</span><span class="sxs-lookup"><span data-stu-id="a1637-105">The following three checks will help you troubleshoot why price (bill rate) is defaulting to 0 on expense sales actuals.</span></span>

## <a name="check-1-identify-the-sales-price-list-for-project"></a><span data-ttu-id="a1637-106">Έλεγχος 1: Προσδιορισμός τιμοκαταλόγου πωλήσεων για το έργο</span><span class="sxs-lookup"><span data-stu-id="a1637-106">Check 1: Identify the sales price list for project</span></span>

<span data-ttu-id="a1637-107">Βρείτε το έργο από το πεδίο έργου και στη συνέχεια μεταβείτε στη σελίδα έργου.</span><span class="sxs-lookup"><span data-stu-id="a1637-107">Find the project from the project field of the actual and go to the project page.</span></span> <span data-ttu-id="a1637-108">Στη συνέχεια, μεταβείτε στην καρτέλα "Πωλήσεις" και στο πλέγμα γραμμών σύμβασης έργου, κάντε κλικ στο πεδίο Σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="a1637-108">Then go to the Sales tab. On the Project Contract lines grid, click on the link in the Project Contract field.</span></span> <span data-ttu-id="a1637-109">Θα ανοίξει η σελίδα σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="a1637-109">The Project Contract page will open.</span></span> <span data-ttu-id="a1637-110">Στη σελίδα σύμβασης έργου, μεταβείτε στην καρτέλα Τιμοκατάλογοι έργου. Ελέγξτε αν υπάρχει τουλάχιστον ένας τιμοκατάλογος.</span><span class="sxs-lookup"><span data-stu-id="a1637-110">On the Project Contract page, go to the Project Price Lists tab. Check if there is at least one price list attached here.</span></span>

<span data-ttu-id="a1637-111">Εάν δεν υπάρχει τιμοκατάλογος στο πλέγμα τιμοκαταλόγων έργου της σύμβασης έργου, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="a1637-111">If there is no price list attached in the Project Price Lists grid of the Project Contract do the following:</span></span>

- <span data-ttu-id="a1637-112">Επισυνάψετε έναν τιμοκατάλογο στο πλέγμα τιμοκαταλόγων έργου.</span><span class="sxs-lookup"><span data-stu-id="a1637-112">Attach a price list to the Project Price lists grid.</span></span> <span data-ttu-id="a1637-113">Οι τιμοκατάλογοι που επιτρέπεται να επισυνάπτονται εδώ θα πρέπει να έχουν το πεδίο περιβάλλοντος ορισμένο σε Πωλήσεις και το πεδίο νομισματικής μονάδας στον τιμοκατάλογο πρέπει να ταιριάζει με το πεδίο νομισματικής μονάδας της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="a1637-113">The price lists allowed to be attached here should have the context field set to Sales and the currency field on the price list should match the currency field on the Project Contract.</span></span> <span data-ttu-id="a1637-114">Μόλις κάνετει τις απαιτούμενες επιδιορθώσεις, δημιουργήστε ξανά μια καταχώρηση εξόδου, εγκρίνετέ την και επιβεβαιώστε ότι τα πραγματικά στοιχεία μη χρεωμένων πωλήσεων εμφανίζουν μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-114">Once you’ve made the required fixes, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span>
- <span data-ttu-id="a1637-115">Εάν έχετε έναν ή περισσότερους τιμοκαταλόγους στο πλέγμα τιμοκαταλόγων έργου της σύμβασης έργου, συνεχίστε στον Έλεγχο 2.</span><span class="sxs-lookup"><span data-stu-id="a1637-115">If you have one or more price lists attached in the Project Price Lists grid of the Project Contract, go to Check 2.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-expense-actual"></a><span data-ttu-id="a1637-116">Έλεγχος 2: Είναι οι τιμοκατάλογοι που προσδιορίζονται παραπάνω έγκυροι για τη συγκεκριμένη ημερομηνία πραγματικού εξόδου;</span><span class="sxs-lookup"><span data-stu-id="a1637-116">Check 2: Are any of the price lists identified above valid for the specific date of the expense actual?</span></span>

<span data-ttu-id="a1637-117">Για να λάβει το Project Service υπόψη έναν τιμοκατάλογο για προεπιλογή τιμής, ο ίδιος τιμοκατάλογος πρέπει να ισχύει για την ημερομηνία κατά τον πραγματικό χρόνο εξόδου.</span><span class="sxs-lookup"><span data-stu-id="a1637-117">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the expense sales actual.</span></span> <span data-ttu-id="a1637-118">Ελέγξτε τα ακόλουθα για να δείτε εάν ισχύουν οι τιμοκατάλογοι που αναφέρονται:</span><span class="sxs-lookup"><span data-stu-id="a1637-118">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="a1637-119">Ξεκινήστε ελέγχοντας αν οι ημερομηνίες έναρξης και λήξης της καρτέλας Γενικά για τους τιμοκαταλόγους δεν είναι κενές.</span><span class="sxs-lookup"><span data-stu-id="a1637-119">Start by checking if start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="a1637-120">Εάν οι ημερομηνίες έναρξης και λήξης στους τιμοκαταλόγους που αναφέρονται είναι κενές, τότε έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a1637-120">If the start and end dates on the price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="a1637-121">Καταχωρίστε μια σημείωση του πεδίου ημερομηνίας έναρξης στις πραγματικές δαπάνες κόστους και ελέγξτε εάν οποιοσδήποτε από τους τιμοκαταλόγους που έχουν προσδιοριστεί είναι διαθέσιμος για αυτήν την ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="a1637-121">Make a note of the start date field on your expense sales actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="a1637-122">Για παράδειγμα, η ημερομηνία του πραγματικού εξόδου θα πρέπει να εμπίπτει με την ημερομηνία έναρξης και λήξης στον τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="a1637-122">For example, the date of the expense actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="a1637-123">Εάν δεν υπάρχει τιμοκατάλογος που καλύπτει αυτήν την ημερομηνία σε πραγματικές δαπάνες κόστους, έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a1637-123">If there is no price list that covers that date on the expense sales actual, you have isolated the problem.</span></span> <span data-ttu-id="a1637-124">Τροποποιήστε το τις ημερομηνίες έναρξης και λήξης του τιμοκαταλόγου για να εξασφαλίσετε ότι ο τιμοκατάλογος καλύπτει την ημερομηνία του πραγματικού εξόδου.</span><span class="sxs-lookup"><span data-stu-id="a1637-124">Modify the start and end dates of the price list to ensure that the price list covers the date of the expense actual.</span></span> 
    - <span data-ttu-id="a1637-125">Εάν υπάρχουν πάνω από ένας τιμοκατάλογοι που καλύπτουν την ημερομηνία πραγματικού εξόδου, έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a1637-125">If there is more than one price list that covers the date on the expense sales actual, you have isolated the problem.</span></span> <span data-ttu-id="a1637-126">Μπορείτε να διορθώσετε αυτό το πρόβλημα με την επεξεργασία των ημερομηνιών έναρξης και λήξης από τους τιμοκαταλόγους, έτσι ώστε να υπάρχει μόνο ένας τιμοκατάλογος που να καλύπτει την ημερομηνία πραγματικού εξόδου.</span><span class="sxs-lookup"><span data-stu-id="a1637-126">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the expense actual.</span></span> 
    - <span data-ttu-id="a1637-127">Εάν υπάρχει μόνο ένας τιμοκατάλογος που καλύπτει το πραγματικό έξοδο, μεταβείτε στον έλεγχο 3.</span><span class="sxs-lookup"><span data-stu-id="a1637-127">If there is only one price list that covers that date of the expense actual, move to Check 3.</span></span>
<span data-ttu-id="a1637-128">Μόλις κάνετε τις απαιτούμενες επιδιορθώσεις, δημιουργήστε ξανά μια καταχώρηση εξόδου, εγκρίνετέ την και επιβεβαιώστε ότι τα πραγματικά στοιχεία μη χρεωμένων πωλήσεων εμφανίζουν μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-128">Once you’ve done made the required fixes, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-valid-price-for-the-expense-category-in-the-applicable-project-price-list"></a><span data-ttu-id="a1637-129">Έλεγχος 3: Υπάρχει μια έγκυρη τιμή για την κατηγορία δαπανών στον τιμοκατάλογο έργου;</span><span class="sxs-lookup"><span data-stu-id="a1637-129">Check 3: Is there a valid price for the expense category in the applicable project price list?</span></span> 

<span data-ttu-id="a1637-130">Εάν έχετε ολοκληρώσει με επιτυχία τους ελέγχους 1 και 2, πρέπει να έχετε μόνο έναν τιμοκατάλογο έργου που να ισχύει για την ημερομηνία των πραγματικών δαπανών κόστους.</span><span class="sxs-lookup"><span data-stu-id="a1637-130">If you have successfully completed Check 1 and Check 2, you should now have only one project price list that is applicable for the date of the expense sales actual.</span></span> <span data-ttu-id="a1637-131">Ανοίξτε αυτόν τον τιμοκατάλογο έργου και μεταβείτε στην καρτέλα Τιμές κατηγοριών. Βεβαιωθείτε ότι υπάρχει μια γραμμή στο πλέγμα για τη συγκεκριμένη κατηγορία εξόδου στο πραγματικό έξοδο.</span><span class="sxs-lookup"><span data-stu-id="a1637-131">Open this Project Price List and go to the Category Prices tab. Make sure that there is a row in the grid for the specific expense category on the Expense actual.</span></span>
 
- <span data-ttu-id="a1637-132">Εάν δεν υπάρχει γραμμή, έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a1637-132">If there is no row, then you have isolated the problem.</span></span> <span data-ttu-id="a1637-133">Δημιουργήστε μια γραμμή στο πλέγμα τιμών κατηγορίας για την κατηγορία στο πραγματικό σας έξοδο.</span><span class="sxs-lookup"><span data-stu-id="a1637-133">Create a row in the Category price grid for the category on your expense actual.</span></span> <span data-ttu-id="a1637-134">Μόλις το κάνετε αυτό, δημιουργήστε ξανά μια καταχώρηση εξόδου, εγκρίνετέ την και επιβεβαιώστε ότι τα πραγματικά στοιχεία μη χρεωμένων πωλήσεων εμφανίζουν μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-134">Once this is done, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span> 
- <span data-ttu-id="a1637-135">Εάν υπάρχει μια γραμμή για την κατηγορία δαπανών στο πλαίσιο τιμών "κατηγορία", ελέγξτε εάν έχει μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-135">If there is a row for the expense category in the category prices grid, check if it has a valid price.</span></span>

<span data-ttu-id="a1637-136">Για να κατανοήσετε τι είναι μια έγκυρη τιμή, χρησιμοποιήστε τις παρακάτω μεθόδους:</span><span class="sxs-lookup"><span data-stu-id="a1637-136">To understand what a valid price is, use these methods:</span></span>

- <span data-ttu-id="a1637-137">Εάν το πεδίο μέθοδος τιμολόγησης της γραμμής τιμής κατηγορίας έχει οριστεί σε κόστος, τότε η τιμή μονάδας στα πραγματικά στοιχεία πωλήσεων εξόδων θα έχει κατά προεπιλογή την τιμή στην καταχώρηση δαπανών.</span><span class="sxs-lookup"><span data-stu-id="a1637-137">If the Pricing Method field on the Category price line is set to At Cost, then the unit rate on your Expense sales actual will be defaulted to the value in the Expense entry.</span></span>
- <span data-ttu-id="a1637-138">Αν το πεδίο μέθοδος τιμολόγησης της γραμμής τιμής κατηγορίας έχει οριστεί σε ποσοστό σήμανσης, ελέγξτε, στη συνέχεια, εάν το πεδίο ποσοστού έχει οριστεί σε μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-138">If the Pricing Method field on the Category price line is set to Markup Percentage, then check if the Percent field is set to a valid value.</span></span> <span data-ttu-id="a1637-139">Η τιμή μονάδας στις πραγματικές δαπάνες πωλήσεων έχει προεπιλεγεί εφαρμόζοντας ποσοστό σήμανσης της τιμής στην καταχώρηση δαπανών.</span><span class="sxs-lookup"><span data-stu-id="a1637-139">The unit rate on your Expense sales actual is defaulted by applying this markup percent to the price in the Expense entry.</span></span>
- <span data-ttu-id="a1637-140">Αν το πεδίο μέθοδος τιμολόγησης της γραμμής τιμής κατηγορίας έχει οριστεί σε τιμή ανά μονάδα, ελέγξτε, στη συνέχεια, εάν το πεδίο τιμής έχει οριστεί σε μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-140">If the Pricing Method field on the Category price line is set to Price per Unit, then check if the Price field is set to a valid value.</span></span> <span data-ttu-id="a1637-141">Η τιμή μονάδας στις πραγματικές δαπάνες πωλήσεων έχει κατά προεπιλογή το ποσό νομισματικής μονάδας που καθορίζεται στο πεδίο "τιμή".</span><span class="sxs-lookup"><span data-stu-id="a1637-141">The unit rate on your Expense sales actual will be defaulted to the currency amount specified in the Price field.</span></span>

<span data-ttu-id="a1637-142">Εάν η ρύθμιση της τιμής για την κατηγορία δαπανών δεν είναι έγκυρη, τότε έχετε απομονώσει το πρόβλημα.</span><span class="sxs-lookup"><span data-stu-id="a1637-142">If the price setup for the expense category isn't valid, then you have isolated the problem.</span></span> <span data-ttu-id="a1637-143">Η λύση είναι να επεξεργαστείτε τη γραμμή τιμής κατηγορίας με μια έγκυρη τιμή για την κατηγορία δαπανών σύμφωνα με τους παραπάνω κανόνες.</span><span class="sxs-lookup"><span data-stu-id="a1637-143">The solution is to edit the category price line with a valid price for the expense category in accordance with the rules above.</span></span> <span data-ttu-id="a1637-144">Μόλις το κάνετε αυτό, δημιουργήστε ξανά μια καταχώρηση εξόδου, εγκρίνετέ την και επιβεβαιώστε ότι τα πραγματικά στοιχεία μη χρεωμένων πωλήσεων εμφανίζουν μια έγκυρη τιμή.</span><span class="sxs-lookup"><span data-stu-id="a1637-144">Once you’ve done that, recreate an expense entry, approve it, and then check that the unbilled sales actual gets a valid price.</span></span>

<span data-ttu-id="a1637-145">Εάν και πάλι δεν βλέπετε μια έγκυρη τιμή στις πραγματικές δαπάνες πωλήσεων μετά από τους τρεις ελέγχους, στείλτε ένα δελτίο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="a1637-145">If you still don't see a valid price on your expense sales actual after doing the three checks above, please log a support ticket.</span></span>

