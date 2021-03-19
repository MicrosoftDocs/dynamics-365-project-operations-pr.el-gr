---
title: Ρύθμιση πολιτικών εξόδων
description: Μπορείτε να καθορίσετε πολιτικές εξόδων που πρέπει να ακολουθούν οι εργαζόμενοι σας όταν εισάγουν και υποβάλλουν αναφορές εξόδων και αιτήσεις μετάβασης στο Microsoft Dynamics 365 Finance.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9c014b0593a87ce50f09175b77d9cf498a65391e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271263"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="8af9d-103">Ρύθμιση πολιτικών εξόδων</span><span class="sxs-lookup"><span data-stu-id="8af9d-103">Set up expense policies</span></span>

<span data-ttu-id="8af9d-104">Μπορείτε να καθορίσετε πολιτικές που πρέπει να ακολουθούν οι εργαζόμενοι σας όταν εισάγουν και υποβάλλουν αναφορές εξόδων και αιτήσεις μετάβασης.</span><span class="sxs-lookup"><span data-stu-id="8af9d-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="8af9d-105">Η υλοποίηση των πολιτικών δαπανών μπορεί να σας βοηθήσει να διαχειριστείτε αποτελεσματικά τις δαπάνες.</span><span class="sxs-lookup"><span data-stu-id="8af9d-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="8af9d-106">Για παράδειγμα, μπορείτε να ορίσετε μια πολιτική εξόδων ξενοδοχείων στη Νέα Υόρκη, η οποία να αναφέρει ότι η χρέωση ανά διανυκτέρευση δεν μπορεί να υπερβαίνει τα 250 δολάρια ΗΠΑ.</span><span class="sxs-lookup"><span data-stu-id="8af9d-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="8af9d-107">Εάν ένας εργαζόμενος υποβάλει μια αναφορά εξόδων ή αίτημα ταξιδιού όπου η τιμή δωματίου υπερβαίνει αυτό το ποσό, το σύστημα θα ειδοποιήσει τον</span><span class="sxs-lookup"><span data-stu-id="8af9d-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="8af9d-108">εργαζόμενο ότι έχει γίνει υπέρβαση του ποσού της πολιτικής για το έξοδο.</span><span class="sxs-lookup"><span data-stu-id="8af9d-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="8af9d-109">Μπορείτε να ρυθμίσετε τις παραμέτρους του μηνύματος που θα λαμβάνει ο εργαζόμενος όταν</span><span class="sxs-lookup"><span data-stu-id="8af9d-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="8af9d-110">καθορίζετε την πολιτική.</span><span class="sxs-lookup"><span data-stu-id="8af9d-110">define the policy.</span></span>      
        
<span data-ttu-id="8af9d-111">Μπορείτε να ορίσετε τρεις τύπους πολιτικών:</span><span class="sxs-lookup"><span data-stu-id="8af9d-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="8af9d-112">Προειδοποίηση - Ο εργαζόμενος μπορεί να υποβάλει μια αναφορά εξόδων ή μια αίτηση για ταξίδι, αλλά η δαπάνη θα σημειωθεί για όλους τους υπεύθυνους έγκρισης και</span><span class="sxs-lookup"><span data-stu-id="8af9d-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="8af9d-113">για μεταγενέστερη αναφορά.</span><span class="sxs-lookup"><span data-stu-id="8af9d-113">for later reporting.</span></span>        

- <span data-ttu-id="8af9d-114">Σφάλμα - Απαιτεί από τον εργαζόμενο να αναθεωρήσει το έξοδο προκειμένου να συμμορφωθεί με την πολιτική πριν από την υποβολή της αναφοράς εξόδων ή της αίτησης ταξιδίου.</span><span class="sxs-lookup"><span data-stu-id="8af9d-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="8af9d-115">Αιτιολόγηση - Απαιτεί από τον εργαζόμενο ή έναν προϊστάμενο να καταχωρήσουν μια αιτιολόγηση για την υπέρβαση του ποσού της πολιτικής πριν από την υποβολή της αναφοράς εξόδων ή της αίτησης για ταξίδι.</span><span class="sxs-lookup"><span data-stu-id="8af9d-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="8af9d-116">Συμβουλές πολιτικής</span><span class="sxs-lookup"><span data-stu-id="8af9d-116">Policy tips</span></span>
<span data-ttu-id="8af9d-117">Ακολουθούν μερικές προτάσεις που μπορούν να σας βοηθήσουν κατά τη δημιουργία νέων πολιτικών για τη διαχείριση εξόδων.</span><span class="sxs-lookup"><span data-stu-id="8af9d-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="8af9d-118">Οι πολιτικές δεν έχουν αναδρομική ισχύ, κάτι που σημαίνει ότι μια πολιτική δεν θα ισχύσει εάν έχει δημιουργηθεί με ημερομηνία μεταγενέστερη από την ημερομηνία κατά την οποία έγινε το έξοδο.</span><span class="sxs-lookup"><span data-stu-id="8af9d-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="8af9d-119">Για παράδειγμα, εάν δημιουργείτε μια νέα πολιτική σήμερα για την επιβολή μιας μέγιστης δαπάνης γεύματος $50, τότε όλα τα υπάρχοντα έξοδα που έχουν καταχωρηθεί από χθες δεν θα ελεγχθούν σε σχέση με αυτήν την πολιτική.</span><span class="sxs-lookup"><span data-stu-id="8af9d-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="8af9d-120">Κατά τη δημιουργία μιας πολιτικής για μια κατηγορία εξόδων που μπορεί να επιμερίζεται, εξετάστε το ενδεχόμενο προσθήκης μιας συνθήκης για τον τύπο γραμμής εξόδων.</span><span class="sxs-lookup"><span data-stu-id="8af9d-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="8af9d-121">Ορισμένες πολιτικές όπως η απαίτηση απόδειξης ενδεχομένως να μην έχουν νόημα για τις αναλυτικές γραμμές και πρέπει να εφαρμόζονται μόνο στη γραμμή κεφαλίδας ή σε μια μη αναλυτική γραμμή.</span><span class="sxs-lookup"><span data-stu-id="8af9d-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="8af9d-122">Οι πολιτικές διαχείρισης εξόδων αξιολογούνται με βάση την οντότητα προέλευσης από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="8af9d-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="8af9d-123">Για σενάρια μεταξύ εταιρειών, μπορείτε αντίθετα να ορίσετε την πολιτική που θα αξιολογείται σε σχέση με την οντότητα προορισμού (οντότητα δανεισμού).</span><span class="sxs-lookup"><span data-stu-id="8af9d-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="8af9d-124">Για να εφαρμόζετε τις πολιτικές με βάση την οντότητα προορισμού, ενεργοποιήστε τη δυνατότητα αξιολόγηση πολιτικής εξόδων για τη νομική οντότητα δυνατότητας δανεισμού στο χώρο εργασίας **Διαχείριση δυνατοτήτων**.</span><span class="sxs-lookup"><span data-stu-id="8af9d-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="8af9d-125">Πότε πρέπει να αξιολογούνται οι πολιτικές</span><span class="sxs-lookup"><span data-stu-id="8af9d-125">When to evaluate policies</span></span>

<span data-ttu-id="8af9d-126">Στις παραμέτρους διαχείρισης εξόδων, μπορείτε να επιλέξετε να αξιολογείτε τις πολιτικές διαχείρισης δαπανών όταν αποθηκεύεται μια γραμμή ή όταν υποβάλλεται μια αναφορά εξόδων.</span><span class="sxs-lookup"><span data-stu-id="8af9d-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="8af9d-127">Εάν επιλέξετε να αξιολογείτε κατά την αποθήκευση μιας γραμμής, οι χρήστες θα έχουν νωρίτερα εικόνα σχετικά με το τι πρέπει να κάνουν προκειμένου να ολοκληρώσουν την αναφορά εξόδων τους ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="8af9d-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="8af9d-128">Διαφορετικά, μπορείτε να καθυστερήσετε την αξιολόγηση πολιτικής και να εξοικονομήσετε χρόνο με την επικύρωση στο τέλος, κατά την υποβολή στη ροή εργασιών.</span><span class="sxs-lookup"><span data-stu-id="8af9d-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]