---
title: Να επιχειρηθεί να μην υπάρξει υπέρβαση κατάστασης και επικυρώσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τους ελέγχους ορίων που δεν πρέπει να υπερβαίνονται και οι οποίοι εκτελούνται στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 09dea414e91a365f33bd23089c427b5f63f55c8e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129993"
---
# <a name="manage-not-to-exceed-status-and-validations"></a><span data-ttu-id="76cb6-103">Να επιχειρηθεί να μην υπάρξει υπέρβαση κατάστασης και επικυρώσεων</span><span class="sxs-lookup"><span data-stu-id="76cb6-103">Manage not-to-exceed status and validations</span></span> 

<span data-ttu-id="76cb6-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="76cb6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="not-to-exceed-on-approvals"></a><span data-ttu-id="76cb6-105">Όρια που δεν πρέπει να υπερβαίνονται κατά τις εγκρίσεις</span><span class="sxs-lookup"><span data-stu-id="76cb6-105">Not-to-exceed on approvals</span></span>

<span data-ttu-id="76cb6-106">Όταν υποβάλλεται μια καταχώρηση χρόνου ή εξόδων, δημιουργείται μια εγγραφή έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="76cb6-106">When a time or expense entry is submitted, an approval record is created.</span></span> <span data-ttu-id="76cb6-107">Εάν η έγκριση είναι χρεώσιμη και αντιστοιχεί σε μια γραμμή σύμβασης χρόνου και υλικού, το σύστημα ολοκληρώνει έναν έλεγχο επικύρωσης που δεν πρέπει να υπερβεί στα ακόλουθα επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="76cb6-107">If the approval is chargeable and maps to a time and material contract line, the system completes a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="76cb6-108">Έλεγχος με βάση το όριο που έχει οριστεί για τον πελάτη στη γραμμή σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="76cb6-108">Check against the limit set up for the customer on the project contract line</span></span>
  - <span data-ttu-id="76cb6-109">Έλεγχος με βάση το όριο που έχει οριστεί στη γραμμή σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="76cb6-109">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="76cb6-110">Έλεγχος με βάση το όριο που έχει οριστεί για τον πελάτη</span><span class="sxs-lookup"><span data-stu-id="76cb6-110">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="76cb6-111">Έλεγχος με βάση το όριο που έχει οριστεί στη σύμβαση</span><span class="sxs-lookup"><span data-stu-id="76cb6-111">Check against the limit set up on the contract</span></span>

<span data-ttu-id="76cb6-112">Οι έλεγχοι σε κάθε επίπεδο διασφαλίζουν ότι το ποσό της αξίας πωλήσεων σε αυτήν την έγκριση δεν θα παραβιάζει το όριο σε αυτό το επίπεδο, αφού ληφθεί υπόψη το ποσό της λίστας εκκρεμοτήτων χρέωσης που έχει ήδη καταγραφεί και το ποσό που έχει τιμολογηθεί μέχρι σήμερα σε αυτό το επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="76cb6-112">The checks at each level involve ensuring that the amount of sales value on this approval will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="76cb6-113">Εάν ο έλεγχος είναι επιτυχής, η έγκριση λαμβάνει μια κατάσταση επικύρωσης **Επιτυχία**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-113">If the check passes, the approval is given a validation status of **Success**.</span></span>

<span data-ttu-id="76cb6-114">Εάν ο έλεγχος αποτύχει, η έγκριση λαμβάνει μια κατάσταση επικύρωσης **Αποτυχία**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-114">If the check fails, the approval is given a validation status of **Failed**.</span></span> <span data-ttu-id="76cb6-115">Η λεπτομέρεια επικύρωσης μη υπέρβασης θα ενημερώσει το χρήστη σε ποιο επίπεδο απέτυχε η επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="76cb6-115">The not-to-exceed validation detail will inform the user at which level the validation failed.</span></span>

<span data-ttu-id="76cb6-116">Όταν η καταχώρηση χρόνου ή εξόδων που υποβάλλεται θεωρείται μη χρεώσιμη, η κατάσταση επικύρωσης μη υπέρβασης ορίζεται σε **Δεν ισχύει** με τις λεπτομέρειες επικύρωσης ίσες με **Δεν ισχύει**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-116">When the submitted time or expense entry is considered non-chargeable, the not-to-exceed validation status is set to **Not Applicable** with the validation detail equal to **Not applicable**.</span></span>

## <a name="not-to-exceed-on-unbilled-sales-actuals"></a><span data-ttu-id="76cb6-117">Μη υπέρβαση σε μη τιμολογημένα πραγματικά στοιχεία πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="76cb6-117">Not-to-exceed on unbilled sales actuals</span></span>

<span data-ttu-id="76cb6-118">Όταν εγκρίνεται μια εγγραφή χρόνου ή εξόδων, δημιουργούνται εγγραφές κόστους και μη τιμολογημένων πραγματικών πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="76cb6-118">When a time or expense entry is approved, cost and unbilled sales actuals records are created.</span></span> <span data-ttu-id="76cb6-119">Εάν η μη τιμολογημένη πραγματική πώληση που δημιουργείται είναι χρεώσιμη και αντιστοιχεί σε μια γραμμή σύμβασης χρόνου και υλικού, η εφαρμογή εκτελεί έναν έλεγχο επικύρωσης μη υπέρβασης στα ακόλουθα επίπεδα:</span><span class="sxs-lookup"><span data-stu-id="76cb6-119">If the unbilled sales actual being created is chargeable and maps to a time and material contract line, the application performs a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="76cb6-120">Έλεγχος με βάση το όριο που έχει οριστεί για τον πελάτη στη γραμμή σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="76cb6-120">Check against the limit set up for the customer of the project contract line</span></span>
  - <span data-ttu-id="76cb6-121">Έλεγχος με βάση το όριο που έχει οριστεί στη γραμμή σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="76cb6-121">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="76cb6-122">Έλεγχος με βάση το όριο που έχει οριστεί για τον πελάτη</span><span class="sxs-lookup"><span data-stu-id="76cb6-122">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="76cb6-123">Έλεγχος με βάση το όριο που έχει οριστεί στη σύμβαση</span><span class="sxs-lookup"><span data-stu-id="76cb6-123">Check against the limit set up on the contract</span></span>

<span data-ttu-id="76cb6-124">Οι έλεγχοι σε κάθε επίπεδο διασφαλίζουν ότι το ποσό της αξίας πωλήσεων σε αυτό το πραγματικό στοιχείο δεν θα παραβιάζει το όριο σε αυτό το επίπεδο, αφού ληφθεί υπόψη το ποσό της λίστας εκκρεμοτήτων χρέωσης που έχει ήδη καταγραφεί και το ποσό που έχει τιμολογηθεί μέχρι σήμερα σε αυτό το επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="76cb6-124">The checks at each level ensure that the amount of sales value on the actual will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="76cb6-125">Εάν ο έλεγχος είναι επιτυχής, η πραγματική μη τιμολογημένη πώληση λαμβάνει μια κατάσταση μη υπέρβασης **Δεσμεύτηκε**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-125">If the check passes, the unbilled sales actual is given a not-to-exceed status of **Committed**.</span></span>

<span data-ttu-id="76cb6-126">Εάν ο έλεγχος αποτύχει, η πραγματική μη τιμολογημένη πώληση λαμβάνει μια κατάσταση μη υπέρβασης **Απέτυχε**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-126">If the check fails, the unbilled sales actual is given a not-to-exceed status of **Failed**.</span></span> <span data-ttu-id="76cb6-127">Η λεπτομέρεια επικύρωσης θα ενημερώσει το χρήστη σε ποιο επίπεδο απέτυχε η επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="76cb6-127">The validation detail informs the user at which level the validation failed.</span></span>

<span data-ttu-id="76cb6-128">Όταν η πραγματική μη τιμολογημένη πώληση θεωρείται μη χρεώσιμη ή δωρεάν, εάν δεν υπάρχει ρύθμιση ορίου μη υπέρβασης σε οποιοδήποτε από τα τέσσερα επίπεδα ή εάν το πραγματικό που δημιουργείται είναι "Κόστος", "Διατήρηση", "Μονάδα πόρων" ή "Πωλήσεις μεταξύ οργανισμών", τα πεδία **Κατάσταση μη υπέρβασης** και **Λεπτομέρεια επικύρωσης μη Υπέρβασης** πρέπει να οριστούν σε **Δεν ισχύει**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-128">When the unbilled sales actual is considered non-chargeable or complimentary, if there is no not-to-exceed limit setup at any of the four levels, or if the actual being created is Cost, Retainer, Resourcing Unit, or Inter-organization Sales, the **Not-to-Exceed Status** and **Not-to-Exceed Validation Detail** fields must be set to **Not Applicable**.</span></span>

## <a name="reset-the-not-to-exceed-status"></a><span data-ttu-id="76cb6-129">Επαναφορά κατάστασης "μη υπέρβαση"</span><span class="sxs-lookup"><span data-stu-id="76cb6-129">Reset the not-to-exceed status</span></span>

<span data-ttu-id="76cb6-130">Μπορείτε να εκτελέσετε μαζική επαναφορά της κατάστασης μη υπέρβασης.</span><span class="sxs-lookup"><span data-stu-id="76cb6-130">You can perform a bulk reset of the not-to-exceed status.</span></span> <span data-ttu-id="76cb6-131">Αυτό επιτρέπει στους διαχειριστές έργου να προσαρμόζουν την επικύρωση μη υπέρβασης για να δίνουν προτεραιότητα στην τιμολόγηση ενός συγκεκριμένου σώματος εργασίας, χρόνου ή εξόδων σε σχέση με άλλα που έχουν ήδη δεσμευτεί από το διαθέσιμο ποσό μη υπέρβασης.</span><span class="sxs-lookup"><span data-stu-id="76cb6-131">This allows Project managers to adjust not-to-exceed validation to prioritize invoicing of one particular body of work, time, or expenses over others that are already committed from the available not-to-exceed amount.</span></span>

<span data-ttu-id="76cb6-132">Μετά την επαναφορά της κατάστασης μη υπέρβασης σε πραγματικά στοιχεία πωλήσεων που δεν έχουν τιμολογηθεί, το δεσμευμένο ποσό μειώνεται.</span><span class="sxs-lookup"><span data-stu-id="76cb6-132">After the not-to-exceed status is reset on unbilled sales actuals, the committed amount is reduced.</span></span> <span data-ttu-id="76cb6-133">Ο διαχειριστής έργου μπορεί να επιλέξει ένα άλλο σώμα εργασίας, χρόνου ή εξόδων που προηγουμένως απέτυχε στην επικύρωση μη υπέρβασης και να τα επαναξιολογήσει.</span><span class="sxs-lookup"><span data-stu-id="76cb6-133">The Project manager can select another body of work, time, or expenses that previously failed the not-to-exceed validation and reevaluate them.</span></span> <span data-ttu-id="76cb6-134">Με τη μείωση του δεσμευμένου ποσού, αυτά τα πραγματικά στοιχεία θα περάσουν τώρα την επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="76cb6-134">With the reduction in the committed amount, these actuals will now pass the validation.</span></span> <span data-ttu-id="76cb6-135">Αυτό βοηθά το διαχειριστή έργου να ασκήσει μεγαλύτερη επιρροή και έλεγχο στις συναλλαγές με δυνατότητα τιμολόγησης για αυτήν την περίοδο.</span><span class="sxs-lookup"><span data-stu-id="76cb6-135">This helps the Project manager exert greater influence and control over the invoiceable transactions for that period.</span></span>

<span data-ttu-id="76cb6-136">Για να επαναφέρετε την κατάσταση μη υπέρβασης, επιλέξτε ένα ή περισσότερα πραγματικά στοιχεία από την προβολή **Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού** και **Πραγματικά στοιχεία** και, στη συνέχεια, επιλέξτε **Επαναφορά κατάστασης μη υπέρβασης**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-136">To reset the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and then select **Reset Not-to-Exceed Status**.</span></span>

<span data-ttu-id="76cb6-137">Η κατάσταση μη υπέρβασης επαναφέρεται σε **Δεν έχει αξιολογηθεί** σε όλα τα σχετικά επιλεγμένα πραγματικά στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="76cb6-137">The not-to-exceed status is reset to **Not Evaluated** on all of the relevant selected actuals.</span></span> <span data-ttu-id="76cb6-138">Τα πραγματικά στοιχεία στα οποία δεν έχει γίνει επαναφορά της κατάστασης μη υπέρβασης είναι πραγματικά στοιχεία μη τιμολογημένων πωλήσεων που δεν έχουν τιμολογηθεί και δεν έχουν συνταχθεί σε ένα πρόχειρο τιμολόγιο και επισημαίνονται ως χρεώσιμα.</span><span class="sxs-lookup"><span data-stu-id="76cb6-138">Actuals that have their not-to-exceed status reset are unbilled sales actuals that aren't already invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="76cb6-139">Μόνο άλλα επιλεγμένα πραγματικά στοιχεία παραβλέπονται.</span><span class="sxs-lookup"><span data-stu-id="76cb6-139">Any other selected actuals are ignored.</span></span>

## <a name="reevaluate-not-to-exceed-status"></a><span data-ttu-id="76cb6-140">Εκ νέου αξιολόγηση της κατάστασης "μη υπέρβαση"</span><span class="sxs-lookup"><span data-stu-id="76cb6-140">Reevaluate not-to-exceed status</span></span>

<span data-ttu-id="76cb6-141">Μπορείτε να εκτελέσετε μαζική επανεκτίμηση της κατάστασης μη υπέρβασης.</span><span class="sxs-lookup"><span data-stu-id="76cb6-141">You can perform a bulk re-evaluation of the not-to-exceed status.</span></span> <span data-ttu-id="76cb6-142">Η επαναξιολόγηση της κατάστασης μη υπέρβασης είναι χρήσιμη όταν:</span><span class="sxs-lookup"><span data-stu-id="76cb6-142">Re-evaluation of the not-to-exceed status is useful when:</span></span>

  - <span data-ttu-id="76cb6-143">Υπήρξε επαναδιαπραγμάτευση των ορίων μη υπέρβασης με τον πελάτη και τα πραγματικά στοιχεία θα πρέπει να επαναξιολογηθούν.</span><span class="sxs-lookup"><span data-stu-id="76cb6-143">There was a renegotiation of not-to-exceed limits with the customer and actuals will need to be reevaluated.</span></span>
  - <span data-ttu-id="76cb6-144">Ο διαχειριστής έργου θέλει να τελειοποιήσει την τιμολόγηση της λίστας εκκρεμοτήτων μη τιμολογημένων πωλήσεων, δίνοντας προτεραιότητα σε ένα σώμα εργασίας έναντι ενός άλλου.</span><span class="sxs-lookup"><span data-stu-id="76cb6-144">The Project manager wants to fine-tune the invoicing of unbilled sales backlog by prioritizing one body of work over another.</span></span>

<span data-ttu-id="76cb6-145">Για να επαναξιολογήσετε την κατάσταση μη υπέρβασης, επιλέξτε ένα ή περισσότερα πραγματικά στοιχεία από την προβολή **Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού** και **Πραγματικά στοιχεία** και, στη συνέχεια, επιλέξτε **Επαναξιολόγηση κατάστασης μη υπέρβασης**.</span><span class="sxs-lookup"><span data-stu-id="76cb6-145">To reevaluate the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and select **Reevaluate Not-to-Exceed Status**.</span></span>

<span data-ttu-id="76cb6-146">Όλα τα σχετικά επιλεγμένα πραγματικά στοιχεία με όριο μη υπέρβασης θα αξιολογηθούν με βάση την παραμετροποίηση του ορίου μη υπέρβασης.</span><span class="sxs-lookup"><span data-stu-id="76cb6-146">All of the relevant selected actuals with a not-to-exceed limit will be evaluated against the not-to-exceed limit setup.</span></span> <span data-ttu-id="76cb6-147">Τα πραγματικά στοιχεία που είναι σχετικά με την επαναξιολόγηση της κατάστασης μη υπέρβασης είναι μη τιμολογημένες πραγματικές πωλήσεις που δεν τιμολογούνται και δεν περιλαμβάνονται σε ένα πρόχειρο τιμολόγιο και επισημαίνονται ως χρεώσιμα.</span><span class="sxs-lookup"><span data-stu-id="76cb6-147">Actuals that are relevant for re-evaluating the not-to-exceed status are unbilled sales actuals that are not invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="76cb6-148">Έχουν επιλεγεί άλλα πραγματικά στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="76cb6-148">Any other select actuals selected.</span></span>