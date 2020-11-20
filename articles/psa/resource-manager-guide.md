---
title: Οδηγός υπεύθυνου πόρων
description: Οδηγίες για τη διαχείριση έργων στο Project Service
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
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
ms.openlocfilehash: 04ee87e5b1a2cf96434f4862e07d2b85bad9eace
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124008"
---
# <a name="resource-manager-guide-project-service"></a><span data-ttu-id="3ca44-103">Οδηγός υπεύθυνου πόρων (Project Service)</span><span class="sxs-lookup"><span data-stu-id="3ca44-103">Resource manager guide (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="3ca44-104">Οι δυνατότητες [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στο [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] σάς βοηθούν να βρίσκετε τους κατάλληλους πόρους την κατάλληλη στιγμή για το κατάλληλο έργο και να βεβαιώνεστε ότι όλοι οι πόροι χρησιμοποιούνται αποτελεσματικά.</span><span class="sxs-lookup"><span data-stu-id="3ca44-104">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] help you find the right resources at the right time for the right project and make sure all resources are utilized efficiently.</span></span>  
  
 <span data-ttu-id="3ca44-105">Χρησιμοποιήστε αποτελεσματικά και αποδοτικά τους συμβούλους της εταιρείας σας αξιοποιώντας το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="3ca44-105">Deploy your company’s consultants efficiently and effectively with the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="3ca44-106">Αυτοί σας παρέχουν τα εργαλεία που χρειάζεστε για τον προγραμματισμό των πόρων με βάση τις απαιτήσεις και τα χρονοδιαγράμματα των συμβουλευτικών έργων και τις δεξιότητες και τη διαθεσιμότητα των συμβούλων σας.</span><span class="sxs-lookup"><span data-stu-id="3ca44-106">These provide you with the tools you need to schedule resources based on the requirements and schedules of consulting projects and on the skills and availability of your consultants.</span></span> <span data-ttu-id="3ca44-107">Μπορείτε να βρείτε γρήγορα τους πιο κατάλληλους συμβούλους που είναι διαθέσιμοι για εργασία σε έργα και μπορείτε εύκολα να δείτε ποιος είναι ο καλύτερος τρόπος προγραμματισμού τους κατά τη διάρκεια κάθε έργου.</span><span class="sxs-lookup"><span data-stu-id="3ca44-107">You can quickly find the most qualified consultants who are available to work on projects, and you can easily see how to better schedule them during the course of each project.</span></span>  
  
 <span data-ttu-id="3ca44-108">Ο προγραμματισμός των πόρων σάς βοηθά να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3ca44-108">Resource scheduling helps you do the following:</span></span>  
  
- <span data-ttu-id="3ca44-109">Να αντιστοιχίσετε τους πόρους σε έργα, με βάση το πόσο καλά συμφωνούν τα επίπεδα δεξιοτήτων και επάρκειάς τους με τις απαιτήσεις πόρων του έργου.</span><span class="sxs-lookup"><span data-stu-id="3ca44-109">Match resources to projects, based on how well their skills and proficiency levels match the project resource requirements.</span></span>  
  
- <span data-ttu-id="3ca44-110">Να αντιστοιχίσετε το χρονοδιάγραμμα ενός πόρου σε ένα ημερολόγιο έργου, με βάση τη διαθεσιμότητα και την προγραμματισμένη άδεια.</span><span class="sxs-lookup"><span data-stu-id="3ca44-110">Match a resource’s schedule to a project calendar, based on their availability and scheduled time off.</span></span> <span data-ttu-id="3ca44-111">Το ημερολόγιο με χρωματική κωδικοποίηση σας παρέχει οπτικές ενδείξεις σχετικά με τη διαθεσιμότητα των πόρων.</span><span class="sxs-lookup"><span data-stu-id="3ca44-111">The color-coded calendar gives you visual cues about resource availability.</span></span>  
  
- <span data-ttu-id="3ca44-112">Εξετάστε τη διαθεσιμότητα κάθε συμβούλου και προσδιορίστε πώς χρησιμοποιείται αυτήν τη στιγμή η εν λόγω διαθεσιμότητα.</span><span class="sxs-lookup"><span data-stu-id="3ca44-112">Review the capacity of each consultant and determine how that capacity is currently used.</span></span> <span data-ttu-id="3ca44-113">Αυτό μπορεί να σας βοηθήσει να εντοπίσετε τα σημεία όπου δεν αξιοποιείται αρκετά ή αξιοποιείται περισσότερο απ' ό,τι πρέπει ένας σύμβουλος ή εάν η εργασία συμφωνεί με τη διαθεσιμότητα.</span><span class="sxs-lookup"><span data-stu-id="3ca44-113">This can help you find where a consultant might be under- or over-utilized, or if they’re working at capacity.</span></span>  
  
- <span data-ttu-id="3ca44-114">Αντιστοιχίστε ένα ποσοστό ή έναν συγκεκριμένο αριθμό ωρών στη διαθεσιμότητα ενός εργαζομένου σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="3ca44-114">Assign a percentage or a specific number of hours for a worker’s capacity to a project.</span></span>  
  
- <span data-ttu-id="3ca44-115">Δημιουργήστε κρατήσεις πόρων ομάδας.</span><span class="sxs-lookup"><span data-stu-id="3ca44-115">Make group resource bookings.</span></span>  
  
- <span data-ttu-id="3ca44-116">Κάντε προκαταρκτικές ή οριστικές κρατήσεις σε πόρους και μετατρέψτε τις ώρες προκαταρκτικών κρατήσεων σε οριστικές κρατήσεις με ένα βήμα.</span><span class="sxs-lookup"><span data-stu-id="3ca44-116">Soft book or hard book resources, and convert soft-booked hours into hard-booked hours in one step.</span></span>  
  
- <span data-ttu-id="3ca44-117">Διαμορφώστε αυτόματα μια ομάδα έργου βάσει των πόρων που καθορίζονται σε μια δομή ανάλυσης εργασίας για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="3ca44-117">Automatically form a project team based on resources defined in a work breakdown structure for a project.</span></span>  
  
- <span data-ttu-id="3ca44-118">Καλύψτε αιτήσεις πόρων (κρατήσεις, προτάσεις, βρείτε υποκατάστατα πόρων).</span><span class="sxs-lookup"><span data-stu-id="3ca44-118">Fulfill resource requests (book, propose, find substitute resources).</span></span>  
  
- <span data-ttu-id="3ca44-119">Εκχωρήστε πόρους σύμφωνα με ένα κεντρικό (εκχωρήσεις διαχειριστή πόρων) ή υβριδικό μοντέλο (μπορούν να κάνουν εκχωρήσεις ο διαχειριστής πόρων, αλλά και άλλοι διαχειριστές).</span><span class="sxs-lookup"><span data-stu-id="3ca44-119">Assign resources according to a central (resource manager assigns) or hybrid model (resource manager and other managers can assign).</span></span> <span data-ttu-id="3ca44-120">Για περισσότερες πληροφορίες σχετικά με τον ορισμό ενός κεντρικού έναντι ενός υβριδικού μοντέλου διαχείρισης πόρων, ανατρέξτε στην ενότητα [Ρύθμιση πρόσθετων ρυθμίσεων παραμέτρων (Project Service)](../psa/configure-additional-parameters-settings.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-120">For more information about setting a central versus hybrid resource management model, see [Configure additional parameters settings (Project Service)](../psa/configure-additional-parameters-settings.md).</span></span>  
  
  <span data-ttu-id="3ca44-121">Μπορείτε να διαχειριστείτε αποτελεσματικά πόρους σε έργα και να διασφαλίσετε ότι τα έργα στελεχώνεται όπως πρέπει.</span><span class="sxs-lookup"><span data-stu-id="3ca44-121">You can manage resources efficiently across projects and ensure that projects are staffed appropriately.</span></span> <span data-ttu-id="3ca44-122">Θα πρέπει να εκτελέσετε τις ακόλουθες εργασίες:</span><span class="sxs-lookup"><span data-stu-id="3ca44-122">You’ll need to perform the following tasks:</span></span>  
  
- <span data-ttu-id="3ca44-123">[Διαχείριση αιτήσεων πόρων](../psa/manage-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-123">[Manage resource requests](../psa/manage-resource-requests.md).</span></span> <span data-ttu-id="3ca44-124">Αντιστοιχίστε τις δεξιότητες και τις επάρκειες των συμβούλων σας στα κατάλληλα έργα.</span><span class="sxs-lookup"><span data-stu-id="3ca44-124">Match the skills and proficiencies of your consultants to the right projects.</span></span>  
  
- <span data-ttu-id="3ca44-125">[Προβολή διαθεσιμότητας πόρων](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-125">[View resource availability](../psa/view-resource-availability.md).</span></span> <span data-ttu-id="3ca44-126">Ελέγξτε τη διαθεσιμότητα των συμβούλων σε προβολή ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="3ca44-126">Check consultants’ availability in a calendar view.</span></span>  
  
- <span data-ttu-id="3ca44-127">[Προβολή χρήσης πόρων](../psa/view-resource-utilization.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-127">[View resource utilization](../psa/view-resource-utilization.md).</span></span> <span data-ttu-id="3ca44-128">Δείτε το ποσοστό του χρόνου για τον οποίο είναι δεσμευμένοι οι σύμβουλοί σας αυτήν τη στιγμή.</span><span class="sxs-lookup"><span data-stu-id="3ca44-128">See the percentage of time that your consultants are currently booked.</span></span>  
  
- <span data-ttu-id="3ca44-129">[Προγραμματισμός πόρων για ένα έργο](../psa/schedule-resources-project.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-129">[Schedule resources for a project](../psa/schedule-resources-project.md).</span></span> <span data-ttu-id="3ca44-130">Προγραμματισμός συμβούλων για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="3ca44-130">Schedule consultants for a project.</span></span>  
  
  <span data-ttu-id="3ca44-131">Για περισσότερες πληροφορίες σχετικά με την υποβολή αιτήσεων πόρων για μεμονωμένα έργα, ανατρέξτε στην ενότητα [Υποβολή αιτήσεων πόρων](../psa/submit-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="3ca44-131">For more information about submitting resource requests for individual projects, see [Submit resource requests](../psa/submit-resource-requests.md).</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="3ca44-132">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="3ca44-132">See Also</span></span>  
 <span data-ttu-id="3ca44-133">[Επισκόπηση του Project Service](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="3ca44-133">[Overview of Project Service](../psa/overview.md) </span></span>  
 <span data-ttu-id="3ca44-134">[Οδηγός διαχειριστή](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="3ca44-134">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="3ca44-135">[Οδηγός υπεύθυνου λογαριασμού](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="3ca44-135">[Account Manager Guiden](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="3ca44-136">[Οδηγός υπεύθυνου έργου](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="3ca44-136">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 [<span data-ttu-id="3ca44-137">Οδηγός Χρόνου, Εξόδων και Συνεργασίας</span><span class="sxs-lookup"><span data-stu-id="3ca44-137">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)
