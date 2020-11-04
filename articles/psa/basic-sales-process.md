---
title: Διαδικασίες πώλησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις βασικές διαδικασίες πωλήσεων.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: f09b30fe6d842faaf896cb97f44b060ec4049213
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077030"
---
# <a name="sales-processes"></a><span data-ttu-id="0a0c7-103">Διαδικασίες πώλησης</span><span class="sxs-lookup"><span data-stu-id="0a0c7-103">Sales processes</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="0a0c7-104">Οι διαδικασίες πωλήσεων που χρησιμοποιούνται σε έναν οργανισμό βάσει έργου διαφέρουν από τις διαδικασίες πωλήσεων που χρησιμοποιούνται σε έναν οργανισμό με βάση τα προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-104">The sales processes that are used in a project-based organization differ from the sales processes that are used in a product-based organization.</span></span> <span data-ttu-id="0a0c7-105">Αυτή η διαφορά συμβαίνει επειδή οι κύκλοι πωλήσεων για οργανισμούς που βασίζονται σε έργα είναι μακρύτεροι και απαιτούν τεχνικές προσαρμοσμένης εκτίμησης για την ανάλυση και τη δημιουργία προσφορών για κάθε συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-105">This difference occurs because the sales cycles for project-based organizations are longer and require customized estimation techniques to analyze and create quotes for each deal.</span></span> <span data-ttu-id="0a0c7-106">Το Dynamics 365 Project Service Automation χρησιμοποιεί ορισμένες από τις ίδιες λειτουργίες που χρησιμοποιούνται στη διαδικασία πωλήσεων για το Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-106">Dynamics 365 Project Service Automation uses some of the same functionality that is used in the sales process for Dynamics 365 Sales.</span></span> <span data-ttu-id="0a0c7-107">Ακολουθούν μερικά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="0a0c7-107">Here are some examples:</span></span>

- <span data-ttu-id="0a0c7-108">Μια οντότητα υποψήφιου πελάτη χρησιμοποιείται για την παρακολούθηση της διαδικασίας πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-108">A Lead entity is used to track the sales process.</span></span>
- <span data-ttu-id="0a0c7-109">Η έγκριση υποψήφιων πελατών παρακολουθείται ως ευκαιρίες.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-109">Qualifying leads are tracked as opportunities.</span></span> <span data-ttu-id="0a0c7-110">Η διαδικασία πωλήσεων μπορεί επίσης να ξεκινά με την ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-110">The sales process can also start with opportunity.</span></span>
- <span data-ttu-id="0a0c7-111">Γίνεται πρόσβαση σε όλα τα σχετικά τεχνουργήματα για μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-111">All related artifacts for an opportunity are accessed.</span></span> <span data-ttu-id="0a0c7-112">Αυτά τα τεχνουργήματα περιλαμβάνουν την ομάδα πωλήσεων, τα ενδιαφερόμενα μέρη, την πιθανότητα, την αξιολόγηση, τα στάδια πωλήσεων και τις επιχειρηματικές διαδικασίες.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-112">These artifacts include the sales team, stakeholders, probability, rating, sales stages, and business processes.</span></span>
- <span data-ttu-id="0a0c7-113">Δημιουργούνται πολλές προσφορές για μια ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-113">Multiple quotes are created for an opportunity.</span></span>
- <span data-ttu-id="0a0c7-114">Μια προσφορά επισημαίνετει ως **Κλειστή ως κερδισμένη** για να δημιουργηθεί μια παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-114">A quote is marked **Closed as Won** to create a sales order.</span></span> <span data-ttu-id="0a0c7-115">Στο PSA, η παραγγελία πώλησης προσαρμόζεται και ονομάζεται σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-115">In PSA, the sales order is customized and is called a project contract.</span></span>

<span data-ttu-id="0a0c7-116">Η εικόνα που ακολουθεί εμφανίζει μια τυπική διεργασία πωλήσεων σε έναν οργανισμό που βασίζεται σε έργο.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-116">The following illustration shows a typical sales process in a project-based organization.</span></span>

> ![Διεργασία πωλήσεων σε έναν οργανισμό βάσει έργου](media/basic-guide-1.png)

## <a name="estimating-a-sale"></a><span data-ttu-id="0a0c7-118">Εκτίμηση μιας πώλησης</span><span class="sxs-lookup"><span data-stu-id="0a0c7-118">Estimating a sale</span></span>
<span data-ttu-id="0a0c7-119">Η τιμή μιας πώλησης μπορεί να εκτιμηθεί με βάση τα έργα που έχουν προηγουμένως παραδοθεί και την πολυπλοκότητα των έργων.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-119">The value of a sale can be estimated based on projects that have previously been delivered and the complexity of projects.</span></span> <span data-ttu-id="0a0c7-120">Για έργα που αφορούν επεκτάσεις σε προηγούμενα έργα ή έργα όπου η εμπειρογνωμοσύνη του πωλητή είναι υψηλή και χρησιμοποιούνται πολύ γνωστά πρότυπα εργασίας, μπορείτε να χρησιμοποιήσετε μια απλούστερη διαδικασία εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-120">For projects that involve extensions to previous projects, or projects where the vendor's expertise is high and well-known work templates are used, you can use a simpler estimation process.</span></span> <span data-ttu-id="0a0c7-121">Τα πιο σύνθετα έργα έχουν συνήθως μια μακρύτερη διαδικασία αγοράς.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-121">More complex projects usually have a longer purchase process.</span></span> <span data-ttu-id="0a0c7-122">Για αυτόν το λόγο, υπάρχουν περισσότερα στάδια στη διεργασία εκτίμησης πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-122">Therefore, there are more stages in the sales estimation process.</span></span> <span data-ttu-id="0a0c7-123">Νωρίς στη διαδικασία, η ομάδα πωλήσεων χρησιμοποιεί τα δεδομένα των υπευθύνων διαχείρισης λογαριασμών και εμπειρογνωμόνων θεμάτων (ΜΜΕ) για να αρχίσει να δημιουργεί μια εκτίμηση υψηλού επιπέδου για κάθε ξεχωριστό στοιχείο εργασίας που αναφέρεται.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-123">Early in the process, the sales team uses the input of account managers and subject matter experts (SMEs) to start to create a high-level estimate for each distinct component of work that is quoted.</span></span> <span data-ttu-id="0a0c7-124">Αυτά τα στοιχεία εργασίας αντιπροσωπεύονται από τις γραμμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-124">These components of work are represented by quote lines.</span></span> 

<span data-ttu-id="0a0c7-125">Μπορείτε να δημιουργήσετε μια εκτίμηση υψηλού επιπέδου για την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-125">You can create a high-level estimate of the quote.</span></span> <span data-ttu-id="0a0c7-126">Τελικά, αυτή η εκτίμηση υψηλού επιπέδου θα αντικατασταθεί από μια πιο λεπτομερή εκτίμηση η οποία βασίζεται σε ένα σχέδιο έργου που δημιουργείτε χρησιμοποιώντας τα τυποποιημένα πρότυπα έργου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-126">Eventually, this high-level estimate will be replaced by a more detailed estimate that is based on a project plan that you create by using the standardized project templates.</span></span> <span data-ttu-id="0a0c7-127">Αυτά τα πρότυπα σάς βοηθούν να δημιουργήσετε ένα χρονοδιάγραμμα και να καθορίσετε νομισματικές τιμές στην προσφορά και τα στοιχεία της (γραμμές προσφοράς).</span><span class="sxs-lookup"><span data-stu-id="0a0c7-127">These templates help you build a schedule and determine monetary values on the quote and its components (quote lines).</span></span> 

<span data-ttu-id="0a0c7-128">Μπορείτε να δημιουργήσετε πολλαπλές προσφορές για ένα έργο και να τις ομαδοποιήσετε με έναν μεμονωμένο τύπο οντότητας ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-128">You can create multiple quotes for a project and group them under a single opportunity entity type.</span></span> <span data-ttu-id="0a0c7-129">Τελικά, μία από αυτές τις προσφορές επισημαίνεται ως **Κλειστή ως κερδισμένη** και δημιουργείται μια σύμβαση έργου ή μια δήλωση εργασίας (SOW).</span><span class="sxs-lookup"><span data-stu-id="0a0c7-129">Eventually, one of those quotes is marked **Closed as Won** , and a project contract or statement of work (SOW) is created.</span></span> <span data-ttu-id="0a0c7-130">Μια σύμβαση έργου συγκρατεί τη συμβατική τιμή για κάθε στοιχείο (γραμμή σύμβασης) που έχει γίνει αποδεκτή από τον πελάτη για παράδοση.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-130">A project contract holds the contracted value for each component (contract line) that is accepted by the customer for delivery.</span></span> <span data-ttu-id="0a0c7-131">Ένα SOW συνήθως δημιουργείται ως έγγραφο Microsoft Word.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-131">An SOW is usually created as a Microsoft Word document.</span></span> <span data-ttu-id="0a0c7-132">Όλα τα τιμολόγια που αποστέλλονται στον πελάτη κατά τη διάρκεια της παράδοσης του έργου αναφέρονται στη σύμβαση έργου ή στο SOW.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-132">All invoices that are sent to the customer over the course of the project's delivery reference the project contract or SOW.</span></span>

<span data-ttu-id="0a0c7-133">Μπορείτε, επίσης, να δημιουργήσετε εναλλακτικές προσφορές με έναν τύπο οντότητας ευκαιρίας ή να ρυθμίσετε το σύστημα έτσι, ώστε να δημιουργείται μια σύμβαση έργου κατά την νίκη μιας προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-133">You can also create alternate quotes under one opportunity entity type or set up the system so that a project contract is created when a quote is won.</span></span> <span data-ttu-id="0a0c7-134">Σε αυτήν την περίπτωση, μπορείτε να επισυνάψετε ένα έγγραφο του Word που αντιπροσωπεύει το SOW στην καρτέλα σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-134">In this case, you can attach a Word document that represents the SOW to the project contract record.</span></span>

![Κλείσιμο προσφοράς για τη δημιουργία σύμβασης έργου](media/basic-guide-2.png)

## <a name="configuring-the-sales-process"></a><span data-ttu-id="0a0c7-136">Ρύθμιση παραμέτρων της διαδικασίας πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="0a0c7-136">Configuring the sales process</span></span>
<span data-ttu-id="0a0c7-137">Μπορείτε να χρησιμοποιήσετε ροές επιχειρηματικών διεργασιών (BPF) στο Microsoft Dynamics 365 για να ρυθμίσετε τις παραμέτρους της διαδικασίας πωλήσεών σας.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-137">You can use business process flows (BPFs) in Microsoft Dynamics 365 to configure your sales process.</span></span> <span data-ttu-id="0a0c7-138">Τα BPF παρέχουν στο προσωπικό πωλήσεων μια καθοδηγούμενη οπτική διασύνδεση που μπορεί να χρησιμοποιηθεί για την προώθηση προσφορών μέσω των πιο συνηθισμένων σταδίων για την εταιρεία σας.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-138">BPFs give your sales staff a guided visual interface that they can use to move deals forward through the stages that are typical for your company.</span></span>

<span data-ttu-id="0a0c7-139">Για παράδειγμα, η εταιρεία σας μπορεί να έχει τα εξής έξι στάδια στη διαδικασία πωλήσεων:</span><span class="sxs-lookup"><span data-stu-id="0a0c7-139">For example, your company might have the following six stages in the sales process:</span></span>

1. <span data-ttu-id="0a0c7-140">Έγκριση</span><span class="sxs-lookup"><span data-stu-id="0a0c7-140">Qualify</span></span>
2. <span data-ttu-id="0a0c7-141">Εκτίμηση</span><span class="sxs-lookup"><span data-stu-id="0a0c7-141">Estimate</span></span>
3. <span data-ttu-id="0a0c7-142">Εσωτερική αξιολόγηση</span><span class="sxs-lookup"><span data-stu-id="0a0c7-142">Internal review</span></span>
4. <span data-ttu-id="0a0c7-143">Σύμβαση</span><span class="sxs-lookup"><span data-stu-id="0a0c7-143">Contract</span></span>
5. <span data-ttu-id="0a0c7-144">Παράδοση</span><span class="sxs-lookup"><span data-stu-id="0a0c7-144">Deliver</span></span>
6. <span data-ttu-id="0a0c7-145">Κλείσιμο</span><span class="sxs-lookup"><span data-stu-id="0a0c7-145">Close</span></span>

<span data-ttu-id="0a0c7-146">Αυτά τα έξι στάδια αντιπροσωπεύονται από chevron (\>) που επιλέγετε για επέκταση σε κάθε τύπο οντότητας ευκαιρίας που δημιουργείτε.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-146">These six stages are represented by chevrons (\>) that you select to expand in each opportunity entity type that you create.</span></span>

![Ρύθμιση επιχειρηματικής διαδικασίας στο Dynamics 365](media/basic-guide-3.png)
 
<span data-ttu-id="0a0c7-148">Ο οργανισμός σας ενδέχεται να χρησιμοποιεί διαφορετικές οντότητες για να αντιπροσωπεύσει την ίδια συμφωνία καθώς εξελίσσεται.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-148">Your organization might use different entities to represent the same deal as it evolves.</span></span> <span data-ttu-id="0a0c7-149">Νωρίς στη διαδικασία πωλήσεων, μια συμφωνία αντιπροσωπεύεται από την οντότητα "ευκαιρία".</span><span class="sxs-lookup"><span data-stu-id="0a0c7-149">Early in the sales process, a deal is represented by the Opportunity entity.</span></span> <span data-ttu-id="0a0c7-150">Με την πάροδο του χρόνου και την ανάδυση περισσότερων λεπτομερειών, μπορείτε να χρησιμοποιήσετε εκτιμήσεις υψηλού επιπέδου για να δημιουργήσετε μία ή περισσότερες προσφορές.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-150">As time passes and more details emerge, you might use high-level estimates to create one or more quotes.</span></span> <span data-ttu-id="0a0c7-151">Εάν κάποια από αυτές τις προσφορές αναθεωρηθεί από εσωτερικούς και ενδιαφερόμενους πελατών, η οντότητα "προσφορά" αντιπροσωπεύει τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-151">If one of these quotes is reviewed by internal and customer stakeholders, the Quote entity represents the deal.</span></span> <span data-ttu-id="0a0c7-152">Αφού ο πελάτης αποδεχτεί την προσφορά, μια σύμβαση έργου ή ένα SOW αντιπροσωπεύει τη συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-152">After the customer accepts the quote, a project contract or SOW represents the deal.</span></span> <span data-ttu-id="0a0c7-153">Για να υποστηρίξετε αυτήν τη συμπεριφορά, τα BPF είναι δομημένο έτσι, ώστε κάθε στάδιο της διεργασίας να συνδέεται με έναν διαφορετικό πίνακα βάσης δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-153">To support this behavior, BPFs are structured so that each stage in the process is linked to a different database table.</span></span>

<span data-ttu-id="0a0c7-154">Το στάδιο **Έγκριση** στη διαδικασία πωλήσεων υποστηρίζεται από μια οντότητα "ευκαιρία".</span><span class="sxs-lookup"><span data-stu-id="0a0c7-154">The **Qualify** stage in the sales process can be backed by an Opportunity entity.</span></span> <span data-ttu-id="0a0c7-155">Τα στάδια **Εκτίμηση** και **Εσωτερικός έλεγχος** υποστηρίζονται από μια οντότητα προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-155">The **Estimate** and **Internal Review** stages can be backed by a Quote entity.</span></span> <span data-ttu-id="0a0c7-156">Τα στάδια **Σύμβαση** , **Παράδοση** και **Κλείσιμο** μπορούν να υποστηρίξουν μια οντότητα σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-156">The **Contract** , **Delivery** , and **Close** stages can be backed by a Project Contract entity.</span></span>

<span data-ttu-id="0a0c7-157">Καθώς μετακινείτε συμφωνίες μέσω των σταδίων, θα σας ζητηθεί να δημιουργήσετε την κατάλληλη καρτέλα οντότητας για να σας βοηθήσει και να σας καθοδηγήσει στη διαδικασία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-157">As you move deals through the stages, you're prompted to create the appropriate entity record to help and guide you through the process.</span></span> <span data-ttu-id="0a0c7-158">Τα στάδια μπορεί να είναι υπό όρους.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-158">The stages can be conditional.</span></span> <span data-ttu-id="0a0c7-159">Για παράδειγμα, εάν απαιτείτε μια εσωτερική αναθεώρηση μιας προσφοράς μόνο εάν η προσφορά χρησιμοποιεί έναν προσαρμοσμένο τιμοκατάλογο, μπορείτε να ρυθμίσετε τις παραμέτρους αυτής της συνθήκης στο κατάλληλο στάδιο της επιχειρηματικής διαδικασίας.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-159">For example, if you require an internal review of a quote only if the quote uses a custom price list, you can configure that condition in the appropriate stage of the business process.</span></span> <span data-ttu-id="0a0c7-160">Το στάδιο **Εσωτερικός έλεγχος** εμφανίζεται μόνο για προσφορές που χρησιμοποιούν έναν προσαρμοσμένο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-160">The **Internal Review** stage is then shown only for quotes that use a custom price list.</span></span> <span data-ttu-id="0a0c7-161">Για όλες τις άλλες συμφωνίες και προσφορές, το στάδιο **Εκτίμηση** ακολουθείται από το στάδιο **Σύμβαση**.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-161">For all other deals and quotes, the **Estimate** stage is followed by the **Contract** stage.</span></span>

> [!NOTE]
> <span data-ttu-id="0a0c7-162">Το PSA έχει συγκεκριμένες σελίδες για τις οντότητες ευκαιρίας, προσφοράς, παραγγελίας και τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-162">PSA has specific pages for the Opportunity, Quote, Order, and Invoice entities.</span></span> <span data-ttu-id="0a0c7-163">Πρέπει να δημιουργήσετε τις ευκαιρίες, τις προσφορές, τις παραγγελίες και τα τιμολόγια της υπηρεσίας έργου χρησιμοποιώντας τις σελίδες πληροφοριών έργου για αυτές τις οντότητες.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-163">You must create project service opportunities, quotes, orders, and invoices using the project information pages for these entities.</span></span> <span data-ttu-id="0a0c7-164">Εάν χρησιμοποιείτε μια άλλη σελίδα για να δημιουργήσετε μια καρτέλα, δεν θα έχετε τη δυνατότητα να ανοίξετε την καρτέλα από τη σελίδα **Πληροφορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-164">If you use another page to create a record, you won't be able to open the record from the **Project Information** page.</span></span> <span data-ttu-id="0a0c7-165">Εάν θέλετε να ανοίξετε μια καρτέλα από τη σελίδα **Πληροφορίες έργου** , πρέπει να διαγράψετε την καρτέλα και να τη δημιουργήσετε εκ νέου χρησιμοποιώντας τη σελίδα **Πληροφορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-165">If you want to open a record from the **Project Information** page, you must delete the record and recreate it using the **Project Information** page.</span></span> <span data-ttu-id="0a0c7-166">Στη σελίδα **Πληροφορίες έργου** , η επιχειρηματική λογική για κάθε έναν από αυτούς τους τύπους οντότητας διασφαλίζει ότι το πεδίο **Τύπος** της καρτέλας έχει ρυθμιστεί σωστά και ότι όλες οι υποχρεωτικές έννοιες έχουν προετοιμαστεί σωστά.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-166">On the **Project Information** page, business logic for each of these entity types ensures that the **Type** field of the record is set correctly, and all of the mandatory concepts are properly initialized.</span></span>

> ![Πληροφορίες έργου για μια νέα παραγγελία](media/basic-guide-4.png)
 
## <a name="differences-between-project-service-automation-and-sales"></a><span data-ttu-id="0a0c7-168">Διαφορές μεταξύ Project Service Automation και Sales</span><span class="sxs-lookup"><span data-stu-id="0a0c7-168">Differences between Project Service Automation and Sales</span></span>
<span data-ttu-id="0a0c7-169">Παρόλο που η διεργασία πωλήσεων στο PSA χρησιμοποιεί τις βασικές δυνατότητες της διαδικασίας πωλήσεων στις πωλήσεις, έχει ορισμένες βασικές διαφορές λόγω των αποκλίσεων στις επιχειρηματικές πρακτικές των οργανισμών που βασίζονται σε έργο.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-169">Although the sales process in PSA uses the basic capabilities of the sales process in Sales, it does have some key differences because of variations in the business practices of project-based organizations.</span></span> <span data-ttu-id="0a0c7-170">Ακολουθούν μερικά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="0a0c7-170">Here are some examples:</span></span>

- <span data-ttu-id="0a0c7-171">**Προσφορές έργου** - Στο Project Service Automation, μια προσφορά κλείνει μετά τη δημιουργία μιας σύμβασης έργου από μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-171">**Project quotes** – In Project Service Automation, a quote is closed after a project contract is created from a quote.</span></span> <span data-ttu-id="0a0c7-172">Στο Sales, μπορείτε να κρατήσετε μια προσφορά αφού την κερδίσατε.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-172">In Sales, you can keep a quote open after you've won it.</span></span> <span data-ttu-id="0a0c7-173">Ο λόγος για αυτήν τη διαφορά είναι ότι η αντιστοιχία μεταξύ μιας προσφοράς και μιας σύμβασης έργου είναι καλύτερη για οργανισμούς που βασίζονται σε έργο.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-173">The reason for this difference is that a match between a quote and a project contract is better for project-based organizations.</span></span> 
- <span data-ttu-id="0a0c7-174">**Ενεργοποίηση και αναθεωρήσεις** - Στο PSA, η ενεργοποίηση και οι αναθεωρήσεις δεν υποστηρίζονται για προσφορές έργου.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-174">**Activation and revisions** – In PSA, activation and revisions aren't supported for project quotes.</span></span> <span data-ttu-id="0a0c7-175">Στο Sales, μια προσφορά μπορεί να κλειδωθεί για να αποτραπούν πρόσθετες αλλαγές.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-175">In Sales, a quote can be locked to prevent additional edits.</span></span>
- <span data-ttu-id="0a0c7-176">**Κλείσιμο μιας προσφοράς ως χαμένης ή κερδισμένης** - Στο PSA, όταν μια προσφορά έργου κλείνει ως κερδισμένη ή χαμένη, η ευκαιρία παραμένει ανοιχτή.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-176">**Closing a quote as lost or won** – In PSA, when a project quote is closed as won or lost, the opportunity remains open.</span></span> <span data-ttu-id="0a0c7-177">Όλες οι άλλες προσφορές στην ευκαιρία κλείνουν ως χαμένες.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-177">All other quotes on the opportunity are closed as lost.</span></span> <span data-ttu-id="0a0c7-178">Στο Sales όταν μια προσφορά κλείνει ως κερδισμένη ή χαμένη, ζητείται από το χρήστη να ενεργήσει με την ευκαιρία.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-178">In Sales, when a quote is closed as won or lost, the user is prompted to take an action on the opportunity.</span></span> <span data-ttu-id="0a0c7-179">Ανάλογα με την εισαγωγή του χρήστη, η υποκείμενη ευκαιρία μπορεί να είναι κλειστή ή να παραμένει ανοιχτή.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-179">Depending on the user input, the underlying opportunity might be closed or left open.</span></span>

## <a name="tracking-revisions-to-quotes-and-project-plans-in-the-sales-cycle"></a><span data-ttu-id="0a0c7-180">Παρακολούθηση αναθεωρήσεων σε προσφορές και σχέδια έργου στον κύκλο πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="0a0c7-180">Tracking revisions to quotes and project plans in the sales cycle</span></span>
<span data-ttu-id="0a0c7-181">Στο PSA, δεν μπορείτε να παρακολουθείτε τις αναθεωρήσεις που πραγματοποιούνται σε μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-181">In PSA, you can't track revisions that are made to a quote.</span></span> <span data-ttu-id="0a0c7-182">Αντί για αυτό, θα πρέπει να επισημάνετε την υπάρχουσα προσφορά **Έκλεισε ως χαμένη,** και, στη συνέχεια, να δημιουργήσετε μια νέα προσφορά.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-182">Instead, you must mark the existing quote **Closed as Lost** and then create a new quote.</span></span> <span data-ttu-id="0a0c7-183">Μπορείτε να αντιγράψετε μια προσφορά ή να κλωνοποιήσετε μια προσφορά βάσει έργου χρησιμοποιώντας το PSA.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-183">You can copy a quote or clone a project-based quote by using PSA.</span></span>

## <a name="tracking-comments-and-approvals-of-quotes-and-project-contracts"></a><span data-ttu-id="0a0c7-184">Παρακολούθηση σχολίων και εγκρίσεων προσφορών και συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="0a0c7-184">Tracking comments and approvals of quotes and project contracts</span></span>
<span data-ttu-id="0a0c7-185">Μπορείτε να διαχειριστείτε την αναθεώρηση και την έγκριση προσφορών και συμβάσεων έργου με χρήση του τείχους εγγραφών και καταχωρήσεων.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-185">You can manage the review and approval of quotes and project contracts by using the record wall and posts.</span></span> <span data-ttu-id="0a0c7-186">Ο οργανισμός σας μπορεί να δημιουργήσει προσαρμοσμένες ροές εργασιών και προσθήκες για την ανάθεση, την ανακατεύθυνση, την κλιμάκωση και τη διαχείριση ειδοποιήσεων σχετικά με τα στοιχεία εργασίας ελέγχου και έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="0a0c7-186">Your organization can create custom workflows and plug-ins to assign, redirect, escalate, and manage notifications of review and approval work items.</span></span>