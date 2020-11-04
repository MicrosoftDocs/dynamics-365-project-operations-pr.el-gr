---
title: Δημιουργία χρονοδιαγραμμάτων τιμολογίων σε μια γραμμή σύμβασης βάσει έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία χρονοδιαγραμμάτων τιμολογίων και ορόσημων για γραμμές σύμβασης.
author: rumant
manager: Annbe
ms.date: 10/17/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2183b915dd2f67e03964246cb0689003e48363f7
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/20/2020
ms.locfileid: "4077150"
---
# <a name="creating-invoice-schedules-on-a-project-based-contract-line"></a><span data-ttu-id="50434-103">Δημιουργία χρονοδιαγραμμάτων τιμολογίων σε μια γραμμή σύμβασης βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="50434-103">Creating invoice schedules on a project-based contract line</span></span>

<span data-ttu-id="50434-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="50434-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="50434-105">Μπορείτε να δημιουργήσετε ένα χρονοδιάγραμμα τιμολογίου σε μια γραμμή σύμβασης βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="50434-105">You can an invoice schedule to a  project-based contract line.</span></span> <span data-ttu-id="50434-106">Η τιμολόγηση επιτρέπεται μόνο αφού κερδηθεί η σύμβαση και δημιουργείτε μια σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="50434-106">Invoicing is only allowed after the contract is won to and you are creating a project contract.</span></span> <span data-ttu-id="50434-107">Ένα χρονοδιάγραμμα τιμολογίου επιτρέπει την αυτόματη δημιουργία προσχεδίων τιμολογίων για μια ουρά σύμβασης βασισμένη σε έργα.</span><span class="sxs-lookup"><span data-stu-id="50434-107">An invoice schedule allows draft invoices for a project-based contract line to be automatically created.</span></span> <span data-ttu-id="50434-108">Εάν, όμως, δημιουργήσετε μόνο τιμολόγια με μη αυτόματο τρόπο, μπορείτε να παραλείψετε τη δημιουργία χρονοδιαγραμμάτων τιμολόγησης σε γραμμές σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="50434-108">If however, you only manually create invoices, you can skip creating invoice schedules on contract lines.</span></span>

## <a name="create-a-time-and-material-invoice-schedule-for-a-contract-line"></a><span data-ttu-id="50434-109">Δημιουργία χρονοδιαγράμματος χρόνου και υλικού για μια γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="50434-109">Create a time and material invoice schedule for a contract line</span></span>

<span data-ttu-id="50434-110">Όταν η γραμμή σύμβασης βάσει έργου έχει μια μέθοδο χρέωσης χρόνου και υλικού μπορείτε να δημιουργήσετε ένα χρονοδιάγραμμα τιμολογίου που βασίζεται σε ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="50434-110">When a project-based contract line has a time and material billing method, you can create a date-based invoice schedule.</span></span> <span data-ttu-id="50434-111">Για να δημιουργήσετε αυτόματα ένα χρονοδιάγραμμα τιμολογίου με βάση την ημερομηνία, ολοκληρώστε τα παρακάτω βήματα.</span><span class="sxs-lookup"><span data-stu-id="50434-111">To automatically generate a date-based invoice schedule, complete the following steps.</span></span>

1. <span data-ttu-id="50434-112">Μεταβείτε στις **Ρυθμίσεις** > **Συχνότητες τιμολογίου** και ρυθμίστε μια συχνότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="50434-112">Go to **Settings** > **Invoice frequencies** and set up an invoice frequence.</span></span>
2. <span data-ttu-id="50434-113">Μεταβείτε στην καρτέλα σύμβασης έργου και στην καρτέλα **Σύνοψη** στο πεδίο **Ημερομηνία παράδοσης που ζητήθηκε** , επιλέξτε μια ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="50434-113">Go to the project contract record, and on the **Summary** tab, in the **Requested Delivery Date** field, select a date.</span></span>
3. <span data-ttu-id="50434-114">Ανοίξτε τη γραμμή σύμβασης **Χρόνος και Υλικό** για την οποία δημιουργείτε ένα χρονοδιάγραμμα τιμολογίου με βάση την ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="50434-114">Open the **Time and Material** contract line that you are making the date-based invoice schedule for.</span></span> 
4. <span data-ttu-id="50434-115">Στην καρτέλα **Χρονοδιάγραμμα τιμολογίου** , επιλέξτε την ημερομηνία έναρξης τιμολόγησης και τη συχνότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="50434-115">On the **Invoice Schedule** tab, select the billing start date and the invoice frequency.</span></span>
5. <span data-ttu-id="50434-116">Στο υπο-πλέγμα, επιλέξτε **Δημιουργία χρονοδιαγράμματος τιμολόγησης**.</span><span class="sxs-lookup"><span data-stu-id="50434-116">On the subgrid, select **Generate Invoice Schedule**.</span></span> <span data-ttu-id="50434-117">Η εφαρμογή δημιουργεί το χρονοδιάγραμμα τιμολόγησης με τα πεδία **Ημερομηνία εκτέλεσης του τιμολογίου** , την **Ημερομηνία αποκοπής της συναλλαγής** και **Κατάσταση εκτέλεσης** που έχουν οριστεί με τον ακόλουθο τρόπο:</span><span class="sxs-lookup"><span data-stu-id="50434-117">The invoice schedule is generated with the **Invoice Run Date** , **Transaction Cutoff Date** and **Run Status** fields set as follows:</span></span>

    - <span data-ttu-id="50434-118">**Ημερομηνία εκτέλεσης του τιμολογίου** : Αυτή η ημερομηνία υπαγορεύεται με βάση τη συχνότητα τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="50434-118">**Invoice Run Date** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="50434-119">**Ημερομηνία αποκοπής συναλλαγής** : Η ημέρα πριν από την ημερομηνία εκτέλεσης τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="50434-119">**Transaction Cutoff Date** : The day before the invoice run date.</span></span>
    - <span data-ttu-id="50434-120">**Κατάσταση εκτέλεσης** : Ορίζεται αυτόματα σε **Να μην εκτελεστεί**.</span><span class="sxs-lookup"><span data-stu-id="50434-120">**Run Status** : Automatically set to **Not Run**.</span></span> <span data-ttu-id="50434-121">Όταν η εργασία δημιουργίας αυτόματης τιμολόγησης εκτελείται για μια συγκεκριμένη ημερομηνία εκτέλεσης τιμολογίου, θα ενημερώσει αυτό το πεδίο σε **Επιτυχής εκτέλεση** ή **Αποτυχία εκτέλεσης**.</span><span class="sxs-lookup"><span data-stu-id="50434-121">When the automatic invoice creation job runs for a certain invoice run date, this field is updated to **Run Successful** or **Run Failed**.</span></span>


## <a name="create-a-fixed-price-invoice-schedule-for-a-contract-line"></a><span data-ttu-id="50434-122">Δημιουργία χρονοδιαγράμματος τιμολογίου προκαθορισμένης τιμής για μια γραμμή σύμβασης</span><span class="sxs-lookup"><span data-stu-id="50434-122">Create a fixed price invoice schedule for a contract line</span></span>

<span data-ttu-id="50434-123">Όταν η γραμμή σύμβασης βάσει έργου έχει μια μέθοδο τιμολόγησης σταθερής τιμής, μπορείτε να δημιουργήσετε ένα χρονοδιάγραμμα τιμολογίου με βάση τα ορόσημα.</span><span class="sxs-lookup"><span data-stu-id="50434-123">When the contract line has a fixed billing method, you can create a milestone-based invoice schedule.</span></span> <span data-ttu-id="50434-124">Ολοκληρώστε τα παρακάτω βήματα για να δημιουργήσετε ένα χρονοδιάγραμμα τιμολογίου βάσει ορόσημου για ένα σταθερό σύνολο ορόσημων, τα οποία κατανέμονται ισότιμα και για την ημερολογιακή περίοδο.</span><span class="sxs-lookup"><span data-stu-id="50434-124">Complete the following steps to generate a milestone-based invoice schedule for a fixed set of equally distributed milestones for the calendar period.</span></span>

1. <span data-ttu-id="50434-125">Μεταβείτε στις **Ρυθμίσεις** > **Συχνότητες τιμολογίου** και ρυθμίστε μια συχνότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="50434-125">Go to **Settings** > **Invoice frequencies** and set up an invoice frequence.</span></span>
2. <span data-ttu-id="50434-126">Μεταβείτε στην καρτέλα σύμβασης έργου και στην καρτέλα **Σύνοψη** στο πεδίο **Ημερομηνία παράδοσης που ζητήθηκε** , επιλέξτε μια ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="50434-126">Go to the project contract record, and on the **Summary** tab, in the **Requested Delivery Date** field, select a date.</span></span>
3. <span data-ttu-id="50434-127">Ανοίξτε τη γραμμή σύμβασης **Σταθερή τιμή** για την οποία δημιουργείτε ένα χρονοδιάγραμμα ορόσημου.</span><span class="sxs-lookup"><span data-stu-id="50434-127">Open the **Fixed Price** contract line that you are creating the milestone schedule for.</span></span> <span data-ttu-id="50434-128">Στην καρτέλα **Ορόσημα χρέωσης** , επιλέξτε την ημερομηνία έναρξης τιμολόγησης και τη συχνότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="50434-128">On the **Billing Milestones** tab, select the billing start date and the invoice frequency.</span></span> 
4. <span data-ttu-id="50434-129">Στο υπο-πλέγμα, επιλέξτε **Δημιουργία περιοδικών ορόσημων**.</span><span class="sxs-lookup"><span data-stu-id="50434-129">On the subgrid, select **Generate Periodic Milestones**.</span></span> <span data-ttu-id="50434-130">Το χρονοδιάγραμμα τιμολογίου δημιουργείται με τα πεδία **Όνομα ορόσημου** , **Ημερομηνία ορόσημου** και **Ποσό ορόσημου** που έχουν οριστεί ως εξής:</span><span class="sxs-lookup"><span data-stu-id="50434-130">The  invoice schedule is generated with the **Milestone Name** , **Milestone Date** , and **Milestone Amount** fields set as follows:</span></span>

    - <span data-ttu-id="50434-131">**Όνομα ορόσημου** : Αυτή η ημερομηνία υπαγορεύεται με βάση τη συχνότητα τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="50434-131">**Milestone Name** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="50434-132">**Ημερομηνία ορόσημου** : Αυτή η ημερομηνία υπαγορεύεται με βάση τη συχνότητα τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="50434-132">**Milestone Date** : This date is dictated by the invoice frequency.</span></span>
    - <span data-ttu-id="50434-133">**Ποσό ορόσημου** : Αυτό το ποσό υπολογίζεται με τη διαίρεση του ποσού σύμβασης στη γραμμή σύμβασης με βάση τον αριθμό των ορόσημων, όπως υπαγορεύονται από την ημερομηνία έναρξης και λήξης της χρέωσης και τις ημερομηνίες παράδοσης που ζητήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="50434-133">**Milestone Amount** : This amount is calculated by dividing the contract amount on the contract line by the number of milestones as dictated by the frequency, billing start, and requested delivery dates.</span></span>

    <span data-ttu-id="50434-134">Εάν η γραμμή σύμβασης έχει μια τιμή στο πεδίο **Εκτιμώμενο ποσό φόρου** , τότε αυτό το πεδίο κατανέμεται επίσης σε κάθε ορόσημο ισότιμα κατά τη δημιουργία περιοδικών ορόσημων.</span><span class="sxs-lookup"><span data-stu-id="50434-134">If the contract line has a value in the **Estimated Tax amount** field, then this field is also apportioned to each milestone equally when generating periodic milestones.</span></span>

<span data-ttu-id="50434-135">Τα ορόσημα χρέωσης θα πρέπει να ισούνται με την τιμή σύμβασης της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="50434-135">Billing milestones should equal the contracted value of the contract line.</span></span> <span data-ttu-id="50434-136">Σε αντίθετη περίπτωση, θα λάβετε ένα μήνυμα σφάλματος στη σελίδα **Γραμμή σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="50434-136">If they don't, you will receive an  error on the **Contract Line** page.</span></span> <span data-ttu-id="50434-137">Μπορείτε να διορθώσετε το σφάλμα, επαληθεύοντας ότι τα ορόσημα χρέωσης συναθροίζουν την τιμή σύμβασης κατά γραμμή δημιουργώντας, θέτοντας σε επεξεργασία ή διαγράφοντας ορόσημα.</span><span class="sxs-lookup"><span data-stu-id="50434-137">You can fix the error by verifying that the billing milestones total the contracted value of the line by creating, editing, or deleting milestones.</span></span> <span data-ttu-id="50434-138">Μετά την πραγματοποίηση των αλλαγών, ανανεώστε τη σελίδα για να καταργήσετε το σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="50434-138">After the changes are made, refresh the page to remove the error.</span></span>

### <a name="manually-create-milestones"></a><span data-ttu-id="50434-139">Μη αυτόματη δημιουργία ορόσημων</span><span class="sxs-lookup"><span data-stu-id="50434-139">Manually create milestones</span></span>

<span data-ttu-id="50434-140">Μπορείτε να δημιουργήσετε ορόσημα προκαθορισμένης τιμής με μη αυτόματο τρόπο, όταν δεν διαχωρίζονται περιοδικά.</span><span class="sxs-lookup"><span data-stu-id="50434-140">You can generate fixed price milestones manually when they are not periodically split.</span></span> <span data-ttu-id="50434-141">Ολοκληρώστε τα παρακάτω βήματα για να δημιουργήσετε μη αυτόματα ένα ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="50434-141">Complete the following steps to manually create a milestone.</span></span>

1. <span data-ttu-id="50434-142">Ανοίξτε τη γραμμή σύμβασης σταθερής τιμής για την οποία δημιουργείτε ένα ορόσημο και στην καρτέλα **Χρονοδιάγραμμα τιμολογίου** , στο υποπλέγμα, επιλέξτε **+ Δημιουργία νέου ορόσημου γραμμής σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="50434-142">Open the fixed price contract line that you are creating a milestone for, and on the **Invoice Schedule** tab, on the subgrid, select **+ Create new Contract line milestone**.</span></span> 
2. <span data-ttu-id="50434-143">Στη σελίδα **Δημιουργία ορόσημου** , καταχωρίστε τις απαιτούμενες πληροφορίες με βάση τον ακόλουθο πίνακα.</span><span class="sxs-lookup"><span data-stu-id="50434-143">On the **Milestone Creation** page, enter the required information based on the following table.</span></span>

| <span data-ttu-id="50434-144">Πεδίο</span><span class="sxs-lookup"><span data-stu-id="50434-144">Field</span></span> | <span data-ttu-id="50434-145">Τοποθεσία</span><span class="sxs-lookup"><span data-stu-id="50434-145">Location</span></span> | <span data-ttu-id="50434-146">Συνάφεια, σκοπός και καθοδήγηση</span><span class="sxs-lookup"><span data-stu-id="50434-146">Relevance, purpose, and guidance</span></span> | <span data-ttu-id="50434-147">Κατάντη επίπτωση</span><span class="sxs-lookup"><span data-stu-id="50434-147">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="50434-148">Όνομα ορόσημου</span><span class="sxs-lookup"><span data-stu-id="50434-148">Milestone Name</span></span> | <span data-ttu-id="50434-149">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-149">Quick Create</span></span> | <span data-ttu-id="50434-150">Πεδίο κειμένου για το όνομα του ορόσημου.</span><span class="sxs-lookup"><span data-stu-id="50434-150">Text field for the name of the milestone.</span></span> | <span data-ttu-id="50434-151">Αυτό μεταβιβάζεται στο ορόσημο της γραμμής σύμβασης έργου και στο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="50434-151">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="50434-152">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="50434-152">Project Task</span></span> | <span data-ttu-id="50434-153">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-153">Quick Create</span></span> | <span data-ttu-id="50434-154">Εάν το ορόσημο συνδέεται με την εργασία έργου, μπορείτε να χρησιμοποιήσετε αυτήν την αναφορά για να προσθέσετε προσαρμοσμένη λογική με βάση την κατάσταση της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="50434-154">If the milestone is tied to project task, use this reference to add custom logic to set the milestone status based on the task status.</span></span> | <span data-ttu-id="50434-155">Η εφαρμογή δεν έχει επιπτώσεις κατάντη αυτής της αναφοράς σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="50434-155">The application, doesn't have any downstream impact of this reference to a task.</span></span> |
| <span data-ttu-id="50434-156">Ημερομηνία ορόσημου</span><span class="sxs-lookup"><span data-stu-id="50434-156">Milestone Date</span></span> | <span data-ttu-id="50434-157">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-157">Quick Create</span></span> | <span data-ttu-id="50434-158">Ορίστε την ημερομηνία κατά την οποία θα πρέπει η διαδικασία αυτόματης δημιουργίας τιμολογίου να αναζητήσει την κατάσταση του ορόσημου για να ληφθεί υπόψη για τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="50434-158">Set the date on which the automatic invoice creation process should look for the status of this milestone to consider it for invoicing.</span></span> | <span data-ttu-id="50434-159">Αυτό μεταβιβάζεται στο ορόσημο της γραμμής σύμβασης έργου και στο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="50434-159">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="50434-160">Κατάσταση τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="50434-160">Invoice Status</span></span> | <span data-ttu-id="50434-161">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-161">Quick Create</span></span> | <span data-ttu-id="50434-162">Όταν δημιουργείται ένα ορόσημο, αυτή η κατάσταση ορίζεται πάντα σε **Δεν είναι έτοιμο για τιμολόγηση** ή **Δεν έχει ξεκινήσει**.</span><span class="sxs-lookup"><span data-stu-id="50434-162">When a milestone is created, this status is always set to **Not Ready for Invoicing** or **Not Started**.</span></span> | <span data-ttu-id="50434-163">Αυτό μεταβιβάζεται στο ορόσημο της γραμμής σύμβασης έργου και στο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="50434-163">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="50434-164">Ποσό γραμμής</span><span class="sxs-lookup"><span data-stu-id="50434-164">Line Amount</span></span> | <span data-ttu-id="50434-165">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-165">Quick Create</span></span> | <span data-ttu-id="50434-166">Το ποσό ή η τιμή του ορόσημου που θα τιμολογηθεί στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="50434-166">Amount or value of the milestone that will be invoiced to the customer.</span></span> | <span data-ttu-id="50434-167">Αυτό μεταβιβάζεται στο ορόσημο της γραμμής σύμβασης έργου και στο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="50434-167">This is carried over to the project contract line milestone and the invoice.</span></span> |
| <span data-ttu-id="50434-168">Φόρος</span><span class="sxs-lookup"><span data-stu-id="50434-168">Tax</span></span> | <span data-ttu-id="50434-169">Γρήγορη δημιουργία</span><span class="sxs-lookup"><span data-stu-id="50434-169">Quick Create</span></span> | <span data-ttu-id="50434-170">Το ποσό του φόρου που εφαρμόστηκε στο ορόσημο.</span><span class="sxs-lookup"><span data-stu-id="50434-170">The tax amount applied on the milestone.</span></span> | <span data-ttu-id="50434-171">Αυτό μεταβιβάζεται στο ορόσημο της γραμμής σύμβασης έργου και στο τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="50434-171">This is carried over to the project contract line milestone and the invoice.</span></span> |

3. <span data-ttu-id="50434-172">Επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="50434-172">Select **Save and Close**.</span></span>
<span data-ttu-id="50434-173">| Ποσό γραμμής | Γρήγορη δημιουργία | Ποσό ή τιμή του ορόσημου που θα τιμολογηθεί στον πελάτη | Αυτό μεταβιβάζεται στο ορόσημο γραμμής σύμβασης έργου και στο τιμολόγιο | | Φόρος | Γρήγορη δημιουργία | Ποσό φόρου που θα εφαρμοστεί στο ορόσημο | Αυτό μεταβιβάζεται στο ορόσημο γραμμής σύμβασης έργου και στο τιμολόγιο |</span><span class="sxs-lookup"><span data-stu-id="50434-173">| Line Amount | Quick create | Amount or Value of the Milestone that will be invoiced to the customer | This is propagated to the Project contract line Milestone and to the Invoice | | Tax | Quick create | Tax amount that will be applied on the Milestone | This is propagated to the Project contract line Milestone and to the Invoice |</span></span>