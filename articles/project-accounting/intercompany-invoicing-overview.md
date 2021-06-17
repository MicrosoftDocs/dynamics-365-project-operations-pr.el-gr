---
title: Επισκόπηση διεταιρικής τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες και παραδείγματα σχετικά με τη διεταιρική τιμολόγηση για έργα.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42af89105f8325f1c94df6d2133d2c329facf2b3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002641"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="e23d0-103">Επισκόπηση διεταιρικής τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="e23d0-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="e23d0-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="e23d0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e23d0-105">Ο οργανισμός σας μπορεί να έχει πολλαπλά τμήματα, θυγατρικές και άλλες νομικές οντότητες που μεταφέρουν τα προϊόντα και τις υπηρεσίες μεταξύ τους για τα έργα.</span><span class="sxs-lookup"><span data-stu-id="e23d0-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="e23d0-106">Η νομική οντότητα που παρέχει την υπηρεσία ή το προϊόν ονομάζεται *νομική οντότητα που δανείζει*.</span><span class="sxs-lookup"><span data-stu-id="e23d0-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="e23d0-107">Η νομική οντότητα που λαμβάνει την υπηρεσία ή το προϊόν ονομάζεται *νομική οντότητα που δανείζεται*.</span><span class="sxs-lookup"><span data-stu-id="e23d0-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="e23d0-108">Παρακάτω παρουσιάζεται ένα τυπικό σενάριο, όπου δύο νομικές οντότητες, η Contoso Robotics USA (το νομικό πρόσωπο που δανείζεται) και η Contoso Robotics UK. (το νομικό πρόσωπο που δανείζει) μοιράζονται πόρους για την παροχή ενός έργου για τον πελάτη, Adventure works.</span><span class="sxs-lookup"><span data-stu-id="e23d0-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="e23d0-109">Για το συγκεκριμένο σενάριο, η Contoso Robotics USA έχει συμβάσεις για την παράδοση της εργασίας στην Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="e23d0-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Διεταιρική τιμολόγηση](./media/IntercompanyScenario.png) 

<span data-ttu-id="e23d0-111">Το Dynamics 365 Project Operations χρησιμοποιεί την ακόλουθη ροή για την επεξεργασία διεταιρικών συναλλαγών:</span><span class="sxs-lookup"><span data-stu-id="e23d0-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="e23d0-112">Οι πόροι από τη νομική οντότητα που δανείζει καταγράφουν τις διεταιρικές ώρες ή τις συναλλαγές εξόδων με κράτηση χρόνου και εξόδων για έργα στη νόμιμη οντότητα που δανείζεται.</span><span class="sxs-lookup"><span data-stu-id="e23d0-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="e23d0-113">Το κόστος χρόνου και εξόδων καταγράφεται στην εταιρεία που δανείζει χρησιμοποιώντας τον τιμοκατάλογο του μοναδιαίου κόστους της εταιρείας που δανείζεται.</span><span class="sxs-lookup"><span data-stu-id="e23d0-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="e23d0-114">Οι διεταιρικές, μη χρεωμένες συναλλαγές πωλήσεων καταγράφονται στην εταιρεία που δανείζει χρησιμοποιώντας τον τιμοκατάλογο του μοναδιαίου κόστους της εταιρείας που δανείζεται.</span><span class="sxs-lookup"><span data-stu-id="e23d0-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="e23d0-115">Τα μη χρεωμένα έσοδα καταχωρούνται στην εταιρεία που δανείζεται χρησιμοποιώντας τον τιμοκατάλογο πωλήσεων σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="e23d0-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="e23d0-116">Ο πελάτης μπορεί να χρεωθεί όταν καταγράφονται έσοδα που δεν έχουν χρεωθεί.</span><span class="sxs-lookup"><span data-stu-id="e23d0-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="e23d0-117">Ο πελάτης δεν χρειάζεται να περιμένει μέχρι να ολοκληρωθεί η επεξεργασία διεταιρικών τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="e23d0-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="e23d0-118">Τα διεταιρικά τιμολόγια πελατών δημιουργούνται σε περιοδική βάση στην εταιρεία που δανείζει.</span><span class="sxs-lookup"><span data-stu-id="e23d0-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="e23d0-119">Τα τιμολόγια δημιουργούνται με μη αυτόματο τρόπο ή με χρήση μιας περιοδικής αυτοματοποιημένης διεργασίας.</span><span class="sxs-lookup"><span data-stu-id="e23d0-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="e23d0-120">Μπορεί να δημιουργηθεί ένα μόνο τιμολόγιο για κάθε νομική οντότητα που δανείζεται ή μπορεί να δημιουργηθούν ξεχωριστά τιμολόγια ανά έργο.</span><span class="sxs-lookup"><span data-stu-id="e23d0-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="e23d0-121">Όταν το διεταιρικό τιμολόγιο πελάτη καταχωρείται στην νομική οντότητα που δανείζει, το αντίστοιχο τιμολόγιο πωλητή σε εκκρεμότητα δημιουργείται στη νομική οντότητα που δανείζει.</span><span class="sxs-lookup"><span data-stu-id="e23d0-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="e23d0-122">Το κόστος στο τιμολόγιο πωλητή που εκκρεμεί θα καταχωρηθεί στο δευτερεύον καθολικό έργου όταν καταχωρηθεί το τιμολόγιο.</span><span class="sxs-lookup"><span data-stu-id="e23d0-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="e23d0-123">Στο ακόλουθο διάγραμμα απεικονίζεται η διεταιρική τιμολόγηση, όπως σχετίζεται με τα λογιστικά συμβάντα και τις αναμενόμενες καταχωρήσεις στο γενικό καθολικό.</span><span class="sxs-lookup"><span data-stu-id="e23d0-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Διεταιρική ροή](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="e23d0-125">Πρόσθετοι πόροι</span><span class="sxs-lookup"><span data-stu-id="e23d0-125">Additional resources</span></span>

- [<span data-ttu-id="e23d0-126">Ρύθμιση παραμέτρων διεταιρικής τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="e23d0-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="e23d0-127">Καταγραφή διεταιρικών συναλλαγών</span><span class="sxs-lookup"><span data-stu-id="e23d0-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="e23d0-128">Δημιουργία διεταιρικών τιμολογίων πελατών και προμηθευτών</span><span class="sxs-lookup"><span data-stu-id="e23d0-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]