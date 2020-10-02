---
title: Ορισμός πολιτικών εξόδων
description: Μπορείτε να καθορίσετε πολιτικές εξόδων που πρέπει να ακολουθούν οι εργαζόμενοι σας όταν εισάγουν και υποβάλλουν αναφορές εξόδων και αιτήσεις μετάβασης.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: fbab7fd94fa429876216ee82b716da8d847fb01a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896641"
---
# <a name="define-expense-policies"></a><span data-ttu-id="73b54-103">Ορισμός πολιτικών εξόδων</span><span class="sxs-lookup"><span data-stu-id="73b54-103">Define expense policies</span></span>

<span data-ttu-id="73b54-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="73b54-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="73b54-105">Μπορείτε να καθορίσετε πολιτικές που πρέπει να ακολουθούν οι εργαζόμενοι σας όταν εισάγουν και υποβάλλουν αναφορές εξόδων και αιτήσεις μετάβασης.</span><span class="sxs-lookup"><span data-stu-id="73b54-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="73b54-106">Η υλοποίηση των πολιτικών δαπανών μπορεί να σας βοηθήσει να διαχειριστείτε αποτελεσματικά τις δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="73b54-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="73b54-107">Για παράδειγμα, μπορείτε να ορίσετε μια πολιτική εξόδων ξενοδοχείων στη Νέα Υόρκη, η οποία να αναφέρει ότι η χρέωση ανά διανυκτέρευση δεν μπορεί να υπερβαίνει τα 250 δολάρια ΗΠΑ.</span><span class="sxs-lookup"><span data-stu-id="73b54-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="73b54-108">Εάν ένας εργαζόμενος υποβάλει μια αναφορά εξόδων ή αίτημα ταξιδιού όπου η τιμή δωματίου υπερβαίνει αυτό το ποσό, το σύστημα θα ειδοποιήσει τον</span><span class="sxs-lookup"><span data-stu-id="73b54-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="73b54-109">εργαζόμενο ότι έχει γίνει υπέρβαση του ποσού της πολιτικής για το έξοδο.</span><span class="sxs-lookup"><span data-stu-id="73b54-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="73b54-110">Μπορείτε να ρυθμίσετε τις παραμέτρους του μηνύματος που θα λαμβάνει ο εργαζόμενος όταν</span><span class="sxs-lookup"><span data-stu-id="73b54-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="73b54-111">καθορίζετε την πολιτική.</span><span class="sxs-lookup"><span data-stu-id="73b54-111">define the policy.</span></span>      
        
<span data-ttu-id="73b54-112">Μπορείτε να ορίσετε τρεις τύπους πολιτικών:</span><span class="sxs-lookup"><span data-stu-id="73b54-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="73b54-113">**Προειδοποίηση**: Ο εργαζόμενος μπορεί να υποβάλει μια αναφορά εξόδων ή μια αίτηση για ταξίδι, αλλά η δαπάνη θα σημειωθεί για όλους τους υπεύθυνους έγκρισης και</span><span class="sxs-lookup"><span data-stu-id="73b54-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="73b54-114">για μεταγενέστερη αναφορά.</span><span class="sxs-lookup"><span data-stu-id="73b54-114">for later reporting.</span></span>        

- <span data-ttu-id="73b54-115">**Σφάλμα** : Απαιτεί από τον εργαζόμενο να αναθεωρήσει το έξοδο προκειμένου να συμμορφωθεί με την πολιτική πριν από την υποβολή της αναφοράς εξόδων ή της αίτησης ταξιδίου.</span><span class="sxs-lookup"><span data-stu-id="73b54-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="73b54-116">**Αιτιολόγηση**: Απαιτεί από τον εργαζόμενο ή έναν προϊστάμενο να καταχωρήσουν μια αιτιολόγηση για την υπέρβαση του ποσού της πολιτικής πριν από την υποβολή της αναφοράς εξόδων ή της αίτησης για ταξίδι.</span><span class="sxs-lookup"><span data-stu-id="73b54-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="73b54-117">Συμβουλές πολιτικής</span><span class="sxs-lookup"><span data-stu-id="73b54-117">Policy tips</span></span>
<span data-ttu-id="73b54-118">Ακολουθούν μερικές προτάσεις που μπορούν να σας βοηθήσουν κατά τη δημιουργία νέων πολιτικών για τη διαχείριση εξόδων:</span><span class="sxs-lookup"><span data-stu-id="73b54-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="73b54-119">Οι πολιτικές δεν έχουν αναδρομική ισχύ, κάτι που σημαίνει ότι μια πολιτική δεν θα ισχύσει εάν έχει δημιουργηθεί με ημερομηνία μεταγενέστερη από την ημερομηνία κατά την οποία έγινε το έξοδο.</span><span class="sxs-lookup"><span data-stu-id="73b54-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="73b54-120">Για παράδειγμα, μπορείτε να δημιουργήσετε μια νέα πολιτική σήμερα για την επιβολή μέγιστης δαπάνης γεύματος $50.</span><span class="sxs-lookup"><span data-stu-id="73b54-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="73b54-121">Τυχόν υπάρχοντα έξοδα που έχουν καταχωρηθεί από χθες δεν θα ελεγχθούν σε σχέση με αυτήν την πολιτική.</span><span class="sxs-lookup"><span data-stu-id="73b54-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="73b54-122">Κατά τη δημιουργία μιας πολιτικής για μια κατηγορία εξόδων που μπορεί να επιμερίζεται, εξετάστε το ενδεχόμενο προσθήκης μιας συνθήκης για τον τύπο γραμμής εξόδων.</span><span class="sxs-lookup"><span data-stu-id="73b54-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="73b54-123">Ορισμένες πολιτικές, όπως η απαίτηση απόδειξης, ενδεχομένως να μην έχουν νόημα για τις επιμερισμένες γραμμές.</span><span class="sxs-lookup"><span data-stu-id="73b54-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="73b54-124">Σε αυτήν την περίπτωση, η πολιτική εφαρμόζεται μόνο στη γραμμή κεφαλίδας ή σε μια μη επιμερισμένη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="73b54-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="73b54-125">Οι πολιτικές διαχείρισης εξόδων αξιολογούνται με βάση την οντότητα προέλευσης από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="73b54-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="73b54-126">Για σενάρια μεταξύ εταιρειών, μπορείτε αντίθετα να ορίσετε την πολιτική που θα αξιολογείται σε σχέση με την οντότητα προορισμού (οντότητα δανεισμού).</span><span class="sxs-lookup"><span data-stu-id="73b54-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="73b54-127">Για να εφαρμόζετε τις πολιτικές με βάση την οντότητα προορισμού, ενεργοποιήστε τη δυνατότητα **αξιολόγηση πολιτικής εξόδων για τη νομική οντότητα δυνατότητας δανεισμού** στο χώρο εργασίας **Διαχείριση δυνατοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="73b54-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="73b54-128">Πότε πρέπει να αξιολογούνται οι πολιτικές</span><span class="sxs-lookup"><span data-stu-id="73b54-128">When to evaluate policies</span></span>

<span data-ttu-id="73b54-129">Στις παραμέτρους διαχείρισης εξόδων, μπορείτε να επιλέξετε να αξιολογείτε τις πολιτικές διαχείρισης δαπανών όταν αποθηκεύεται μια γραμμή ή όταν υποβάλλεται μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="73b54-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="73b54-130">Εάν επιλέξετε να αξιολογείτε κατά την αποθήκευση μιας γραμμής, οι χρήστες θα έχουν νωρίτερα εικόνα σχετικά με το τι πρέπει να κάνουν προκειμένου να ολοκληρώσουν την αναφορά εξόδων τους ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="73b54-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="73b54-131">Διαφορετικά, μπορείτε να καθυστερήσετε την αξιολόγηση πολιτικής και να εξοικονομήσετε χρόνο με την επικύρωση στο τέλος, κατά την υποβολή στη ροή εργασιών.</span><span class="sxs-lookup"><span data-stu-id="73b54-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
