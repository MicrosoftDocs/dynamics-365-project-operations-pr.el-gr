---
title: Παρακολούθηση της προόδου και του κόστους ενός έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο παρακολούθησης της προόδου του έργου και του κόστους.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751654"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="37eac-103">Παρακολούθηση της προόδου και του κόστους ενός έργου</span><span class="sxs-lookup"><span data-stu-id="37eac-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="37eac-104">Η ανάγκη παρακολούθησης της προόδου σε σχέση με ένα χρονοδιάγραμμα ποικίλλει ανάλογα με τον κλάδο.</span><span class="sxs-lookup"><span data-stu-id="37eac-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="37eac-105">Μερικές βιομηχανίες παρακολουθούν σε λεπτομερέστερο επίπεδο ενώ άλλες βιομηχανίες παρακολουθούν σε ένα υψηλότερο επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="37eac-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="37eac-106">Αυτό το θέμα παρουσιάζει τον τρόπο προγραμματισμού, προκειμένου να πληρούνται οι απαιτήσεις του οργανισμού σας.</span><span class="sxs-lookup"><span data-stu-id="37eac-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="37eac-107">Προβολή παρακολούθησης προσπάθειας</span><span class="sxs-lookup"><span data-stu-id="37eac-107">Effort tracking view</span></span>

<span data-ttu-id="37eac-108">Η προβολή **Παρακολούθηση προσπάθειας** παρακολουθεί την πρόοδο των εργασιών στο χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="37eac-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="37eac-109">Συγκρίνει τις πραγματικές ώρες προσπάθειας που αφιερώθηκαν για μια εργασία μέχρι σήμερα με τις προγραμματισμένες ώρες προσπάθειας σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="37eac-110">Το PSA χρησιμοποιεί τους ακόλουθους τύπους για τον υπολογισμό των μετρικών παρακολούθησης:</span><span class="sxs-lookup"><span data-stu-id="37eac-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="37eac-111">Ποσοστό προόδου = πραγματική προσπάθεια που έγινε έως σήμερα ÷ προγραμματισμένη προσπάθεια για την εργασία</span><span class="sxs-lookup"><span data-stu-id="37eac-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="37eac-112">Εκτίμηση για ολοκλήρωση (ΕΚΟ) = προγραμματισμένη προσπάθεια – πραγματική προσπάθεια που έχει γίνει μέχρι σήμερα</span><span class="sxs-lookup"><span data-stu-id="37eac-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="37eac-113">Εκτίμηση για ολοκλήρωση (ΕΚΟ) = Υπόλοιπη προσπάθεια + πραγματική προσπάθεια που έχει γίνει μέχρι σήμερα</span><span class="sxs-lookup"><span data-stu-id="37eac-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="37eac-114">Προβαλλόμενη διακύμανση προσπάθειας = προγραμματισμένη προσπάθεια – ΕΚΟ</span><span class="sxs-lookup"><span data-stu-id="37eac-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="37eac-115">Το PSA εμφανίζει μια προβολή της διακύμανσης της προσπάθειας στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="37eac-116">Εάν το ΕΚΟ είναι κάτι περισσότερο από την προγραμματισμένη προσπάθεια, η εργασία προβλέπεται να διαρκέσει περισσότερο χρόνο από αυτόν που είχε αρχικά προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="37eac-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="37eac-117">Ως εκ τούτου, είναι πίσω από το χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="37eac-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="37eac-118">Εάν το ΕΚΟ είναι κάτι λιγότερο από την προγραμματισμένη προσπάθεια, η εργασία προβλέπεται να διαρκέσει λιγότερο χρόνο από αυτόν που είχε αρχικά προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="37eac-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="37eac-119">Ως εκ τούτου, είναι μπροστά από το χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="37eac-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="37eac-120">Εκ νέου προβολή προσπάθειας</span><span class="sxs-lookup"><span data-stu-id="37eac-120">Re-projecting effort</span></span>

<span data-ttu-id="37eac-121">Είναι σύνηθες για έναν υπεύθυνο έργου να αναθεωρεί τις αρχικές εκτιμήσεις σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="37eac-122">Η εκ νέου προβολή των προβολών έργου είναι η αντίληψη του υπεύθυνου έργου για τις προβλέψεις, δεδομένης της τρέχουσας κατάστασης ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="37eac-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="37eac-123">Δεν συνιστούμε οι υπεύθυνοι έργου να αλλάξουν τους αριθμούς βασικής γραμμής επειδή η βασική γραμμή του έργου είναι η καθορισμένη προέλευση της αλήθειας για τις εκτιμήσεις χρονοδιαγράμματος και κόστους του έργου με τις οποίες έχουν συμφωνήσει όλοι οι ενδιαφερόμενοι στο έργο.</span><span class="sxs-lookup"><span data-stu-id="37eac-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="37eac-124">Υπάρχουν δύο τρόποι με τους οποίους ένας υπεύθυνος έργου μπορεί να επαναλάβει την προσπάθεια έργου στις εργασίες:</span><span class="sxs-lookup"><span data-stu-id="37eac-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="37eac-125">Παράκαμψη του προεπιλεγμένου ETC με μια νέα εκτίμηση της πραγματικής εναπομένουσας προσπάθειας για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="37eac-126">Παράκαμψη του προεπιλεγμένου ποσοστού προόδου με μια νέα εκτίμηση της πραγματικής προόδου της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="37eac-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="37eac-127">Κάθε μία από αυτές τις προσεγγίσεις προκαλεί έναν εκ νέου υπολογισμό του ποσοστού ETC, EΚΟ και προόδου της εργασίας και της διακύμανσης προβαλλόμενης προσπάθειας σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="37eac-128">Επίσης, υπολογίζονται εκ νέου το ποσοστό ΕΚΟ, ETC και προόδου στις εργασίες σύνοψης και παράγεται μια νέα προβολή της διακύμανσης της προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="37eac-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="37eac-129">Εκ νέου προβολή της προσπάθειας στις εργασίες σύνοψης</span><span class="sxs-lookup"><span data-stu-id="37eac-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="37eac-130">Η προσπάθεια για εργασίες σύνοψης ή εργασίες κοντέινερ μπορεί να προβληθεί ξανά.</span><span class="sxs-lookup"><span data-stu-id="37eac-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="37eac-131">Ανεξάρτητα από το εάν ο χρήστης αναδιαμορφώσει τα έργα χρησιμοποιώντας την εναπομένουσα προσπάθεια ή το ποσοστό προόδου στις εργασίες σύνοψης, αρχίζει το ακόλουθο σύνολο υπολογισμών:</span><span class="sxs-lookup"><span data-stu-id="37eac-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="37eac-132">Υπολογίζεται το ποσοστό ΕΚΟ, ETC και προόδου στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="37eac-133">Το νέο ΕΚΟ κατανέμεται στις θυγατρικές εργασίες στην ίδια αναλογία με το αρχικό ΕΚΟ που βρισκόταν στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="37eac-134">Υπολογίζεται το νέο ΕΚΟ σε κάθε μία από τις μεμονωμένες εργασίες προς τις εργασίες του κόμβου φύλλου.</span><span class="sxs-lookup"><span data-stu-id="37eac-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="37eac-135">Οι επηρεαζόμενες θυγατρικές εργασίες στους κόμβους φύλλων έχουν υπολογίσει το ποσοστό του ΕΚΟ και της προόδου με βάση την τιμή του ΕΚΟ.</span><span class="sxs-lookup"><span data-stu-id="37eac-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="37eac-136">Αυτό έχει ως αποτέλεσμα μια νέα προβολή για την διακύμανση προσπάθειας της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="37eac-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="37eac-137">Τα ΕΚΟ των εργασιών σύνοψης στο ριζικό κόμβο υπολογίζονται εκ νέου.</span><span class="sxs-lookup"><span data-stu-id="37eac-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="37eac-138">Προβολή παρακολούθησης κόστους</span><span class="sxs-lookup"><span data-stu-id="37eac-138">Cost tracking view</span></span> 

<span data-ttu-id="37eac-139">Η προβολή **Παρακολούθηση κόστους** συγκρίνει το πραγματικό κόστος που δαπανήθηκε σε μια εργασία με το προγραμματισμένο κόστος μιας εργασίας.</span><span class="sxs-lookup"><span data-stu-id="37eac-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="37eac-140">Αυτή η προβολή εμφανίζει μόνο το κόστος εργασίας και δεν περιλαμβάνει το κόστος από τις εκτιμήσεις δαπανών.</span><span class="sxs-lookup"><span data-stu-id="37eac-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="37eac-141">Το PSA χρησιμοποιεί τους ακόλουθους τύπους για τον υπολογισμό των μετρικών παρακολούθησης:</span><span class="sxs-lookup"><span data-stu-id="37eac-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="37eac-142">Ποσοστό του κόστους = πραγματικό κόστος έως τώρα ÷ προγραμματισμένο κόστος για την εργασία</span><span class="sxs-lookup"><span data-stu-id="37eac-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="37eac-143">Κόστος για ολοκλήρωση (ΕΚΟ) = προγραμματισμένο κόστος – πραγματικό κόστος μέχρι σήμερα</span><span class="sxs-lookup"><span data-stu-id="37eac-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="37eac-144">ΕΚΟ = CTC + πραγματικό κόστος μέχρι σήμερα</span><span class="sxs-lookup"><span data-stu-id="37eac-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="37eac-145">Προβαλλόμενη διακύμανση κόστους = προγραμματισμένο κόστος – ΕΚΟ</span><span class="sxs-lookup"><span data-stu-id="37eac-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="37eac-146">Εμφανίζεται μια προβολή της διακύμανσης κόστους στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="37eac-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="37eac-147">Εάν το ΕΚΟ είναι κάτι περισσότερο από το προγραμματισμένο κόστος, η εργασία προβλέπεται να κοστίσει περισσότερο χρόνο από αυτόν που είχε αρχικά προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="37eac-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="37eac-148">Ως εκ τούτου, είναι πάνω από τον προϋπολογισμό.</span><span class="sxs-lookup"><span data-stu-id="37eac-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="37eac-149">Εάν το ΕΚΟ είναι κάτι λιγότερο από το προγραμματισμένο κόστος, η εργασία προβλέπεται να κοστίσει λιγότερο χρόνο από αυτόν που είχε αρχικά προγραμματιστεί.</span><span class="sxs-lookup"><span data-stu-id="37eac-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="37eac-150">Ως εκ τούτου, είναι κάτω από τον προϋπολογισμό.</span><span class="sxs-lookup"><span data-stu-id="37eac-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="37eac-151">Η εκ νέου προβολή του κόστους του υπεύθυνου έργου</span><span class="sxs-lookup"><span data-stu-id="37eac-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="37eac-152">Όταν η προσπάθεια προβάλλεται ξανά, το CTC, το ΕΚΟ και το ποσοστό κόστους και η προβαλλόμενη διακύμανση κόστους υπολογίζονται εκ νέου στην προβολή **Παρακολούθηση κόστους**.</span><span class="sxs-lookup"><span data-stu-id="37eac-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="37eac-153">Σύνοψη κατάστασης έργου</span><span class="sxs-lookup"><span data-stu-id="37eac-153">Project status summary</span></span>

<span data-ttu-id="37eac-154">Η παρακολούθηση δεδομένων στις προβολές **Παρακολούθηση προσπάθειας** και **Παρακολούθηση κόστους** δείχνει την πρόοδο και το κόστος στον ριζικό κόμβο έργου, στις εργασίες σύνοψης και τα επίπεδα εργασιών κόμβου φύλλου.</span><span class="sxs-lookup"><span data-stu-id="37eac-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="37eac-155">Η ενότητα **Κατάσταση** στη σελίδα **Οντότητα έργου** εμφανίζει μια σύνοψη της κατάστασης σε επίπεδο έργου.</span><span class="sxs-lookup"><span data-stu-id="37eac-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="37eac-156">Πεδία σύνοψης κατάστασης</span><span class="sxs-lookup"><span data-stu-id="37eac-156">Status summary fields</span></span>

<span data-ttu-id="37eac-157">Το πεδίο **Συνολική κατάσταση έργου** είναι ένα επεξεργάσιμο πεδίο που εμφανίζει τη συνολική κατάσταση του έργου.</span><span class="sxs-lookup"><span data-stu-id="37eac-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="37eac-158">Χρησιμοποιεί χρωματική κωδικοποίηση, όπως πράσινο, κίτρινο και κόκκινο, για να υποδείξει αυξημένο κίνδυνο.</span><span class="sxs-lookup"><span data-stu-id="37eac-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="37eac-159">Το πεδίο **Σχόλια** επιτρέπει στο διαχειριστή έργου να εισαγάγει συγκεκριμένα σχόλια σχετικά με την κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="37eac-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="37eac-160">Το πεδίο **Η κατάσταση ενημερώθηκε στις** δεν είναι επεξεργάσιμο και η τιμή είναι μια σήμανση χρόνου που υποδεικνύει την ημερομηνία τελευταίας ενημέρωσης της κατάστασης.</span><span class="sxs-lookup"><span data-stu-id="37eac-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="37eac-161">Τα πεδία **Απόδοση χρονοδιαγράμματος** και **Απόδοση κόστους** καθορίζονται από την ημερομηνία παρακολούθησης.</span><span class="sxs-lookup"><span data-stu-id="37eac-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="37eac-162">Όταν η διακύμανση χρονοδιαγράμματος και κόστους για τον ριζικό κόμβο στην προβολή **Παρακολούθηση προσπάθειας** είναι θετική, μπορείτε να ορίσετε αυτά τα πεδία σε **Ahead**.</span><span class="sxs-lookup"><span data-stu-id="37eac-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="37eac-163">Όταν το χρονοδιάγραμμα και η διακύμανση κόστους του ριζικού κόμβου είναι αρνητικά, μπορείτε να τα ορίσετε σε **Πίσω**.</span><span class="sxs-lookup"><span data-stu-id="37eac-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
