---
title: Βασικές έννοιες διαχείρισης πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις δυνατότητες διαχείρισης πόρων στο Microsoft Dynamics Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a14f0ec328049d1b199201955c384df9fac61e39
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123873"
---
# <a name="resource-management-key-concepts"></a><span data-ttu-id="1dc39-103">Βασικές έννοιες διαχείρισης πόρων</span><span class="sxs-lookup"><span data-stu-id="1dc39-103">Resource management key concepts</span></span>

<span data-ttu-id="1dc39-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1dc39-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1dc39-105">Οι πόροι είναι το πιο σημαντικό πάγιο στοιχείο ενός οργανισμού που βασίζεται σε υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="1dc39-105">Resources are the most important asset of a service-based organization.</span></span> <span data-ttu-id="1dc39-106">Η δυνατότητα να βρείτε τους κατάλληλους πόρους την κατάλληλη στιγμή, να κάνετε κράτηση αυτών των πόρων σε έργα και να τους αξιοποιήσετε, βοηθάει τον οργανισμό να καλύψει τους στόχους εσόδων και τους στόχους ικανοποίησης πελατών.</span><span class="sxs-lookup"><span data-stu-id="1dc39-106">The ability to find the right resources at the right time, book those resources on projects and keep them utilized, helps the organization meet revenue targets and customer satisfaction goals.</span></span> <span data-ttu-id="1dc39-107">Μπορείτε να χρησιμοποιήσετε τη λειτουργία αντιστοίχισης πόρων σε έργα στο Dynamics 365 Project Operations για να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="1dc39-107">You can use the project resourcing functionality in Dynamics 365 Project Operations to do the following tasks:</span></span>

- <span data-ttu-id="1dc39-108">Να σχηματίσετε ομάδες έργου κάνοντας κράτηση διαθέσιμων και εγκεκριμένων πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-108">Form project teams by booking available and qualified resources.</span></span>
- <span data-ttu-id="1dc39-109">Να δημιουργήσετε καρτέλες γενικών μελών ομάδων και καθορίστε τους ρόλους τους και τη μονάδα οργανισμού πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-109">Create generic team member records and define their roles and resource organization unit.</span></span>
- <span data-ttu-id="1dc39-110">Να δημιουργήσετε απαιτήσεις πόρων για τα γενικά μέλη της ομάδας από τις αναθέσεις εργασιών τους.</span><span class="sxs-lookup"><span data-stu-id="1dc39-110">Generate resource requirements for generic team members from their task assignments.</span></span>
- <span data-ttu-id="1dc39-111">Να αντιστοιχίσετε δεξιότητες εντοπίζοντας τις δεξιότητες που καθορίζονται στην απαίτηση πόρων για τις διαθέσιμες δεξιότητες πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-111">Match skills by identifying the skills defined on the resource demand against available resource skills.</span></span>
- <span data-ttu-id="1dc39-112">Να υποκαταστήσετε πόρους.</span><span class="sxs-lookup"><span data-stu-id="1dc39-112">Substitute resources.</span></span>
- <span data-ttu-id="1dc39-113">Να αντιστοιχίσετε αναθέσεις χρονοδιαγράμματος έργου και κρατήσεων πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-113">Align project schedule assignments and resource bookings.</span></span>
- <span data-ttu-id="1dc39-114">Να συμφιλιώσετε τις διαφορές στις κρατήσεις και τις αναθέσεις.</span><span class="sxs-lookup"><span data-stu-id="1dc39-114">Reconcile differences in bookings and assignments.</span></span>
- <span data-ttu-id="1dc39-115">Να κάνετε αλλαγή των κρατήσεων πόρων ως απόκριση σε κατάσταση εκτός γραφείου.</span><span class="sxs-lookup"><span data-stu-id="1dc39-115">Change resource bookings in response to out-of-office status.</span></span>
- <span data-ttu-id="1dc39-116">Να συνεργαστείτε με τους διευθυντές έργου και τους διευθυντές πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-116">Collaborate between project managers and resource managers.</span></span>
- <span data-ttu-id="1dc39-117">Να δείτε το ιστορικό χρήσης του πόρου σε σχέση με ένα στόχο, συμπεριλαμβανομένης μιας ανάλυσης για τον τρόπο χρήσης του χρόνου των πόρων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-117">View the history of resource utilization against a target, including a breakdown of how the resources' time was utilized.</span></span>
- <span data-ttu-id="1dc39-118">Να διατηρήσετε δεξιότητες και αποθετήριο γνώσεων.</span><span class="sxs-lookup"><span data-stu-id="1dc39-118">Maintain a skills and proficiency repository.</span></span>


<span data-ttu-id="1dc39-119">Μπορείτε να επανδρώσετε το έργο σας με μια ομάδα γενικών ή ονομαστικών πόρων στο Project Operations.</span><span class="sxs-lookup"><span data-stu-id="1dc39-119">You can staff your project with a team of generic or named resources in Project Operations.</span></span> <span data-ttu-id="1dc39-120">Μπορείτε να χρησιμοποιήσετε διάφορες μεθόδους για να προσθέσετε και να αναθέσετε μέλη της ομάδας και να διαχειριστείτε τις κρατήσεις και τις αναθέσεις τους.</span><span class="sxs-lookup"><span data-stu-id="1dc39-120">You can use various methods to add and assign team members and to manage their bookings and assignments.</span></span> 
