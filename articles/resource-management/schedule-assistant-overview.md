---
title: Επισκόπηση βοηθού χρονοδιαγράμματος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με τον βοηθό χρονοδιαγράμματος για την κράτηση πόρων.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 92b12bd9272805a736286bf7e0ff926cb6361c05
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125628"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="5145f-103">Επισκόπηση βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="5145f-103">Schedule assistant overview</span></span>

<span data-ttu-id="5145f-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="5145f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5145f-105">Ο βοηθός χρονοδιαγράμματος χρησιμοποιείται για τη κράτηση πόρων με βάση τις απαιτήσεις που καθορίζονται από το διαχειριστή έργου.</span><span class="sxs-lookup"><span data-stu-id="5145f-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="5145f-106">Ο βοηθός χρονοδιαγράμματος βασίζεται στις παραμέτρους που παρέχονται στην απαίτηση πόρου για την εύρεση του πόρου.</span><span class="sxs-lookup"><span data-stu-id="5145f-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="5145f-107">Ο βοηθός χρονοδιαγράμματος συνιστά πόρους που αντιστοιχίζονται σε σχετικές απαιτήσεις, όπως τα παράθυρα χρόνου ή οι δεξιότητες που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="5145f-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="5145f-108">Μετά την ταυτοποίηση των κατάλληλων πόρων, ο πόρος ή ο διαχειριστής έργου μπορούν να κάνουν κράτηση του πόρου στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="5145f-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5145f-109">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="5145f-109">Prerequisites</span></span>

<span data-ttu-id="5145f-110">Ο βοηθός χρονοδιαγράμματος αποτελεί μέρος της Universal Resource Scheduling λύσης.</span><span class="sxs-lookup"><span data-stu-id="5145f-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="5145f-111">Αυτή η λύση περιλαμβάνεται και εγκαθίσταται με το Dynamics 365 Project Operations, το Dynamics 365 Field Service και το Dynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="5145f-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="5145f-112">Απαιτήσεις και πόροι αντιστοίχισης</span><span class="sxs-lookup"><span data-stu-id="5145f-112">Matching requirements and resources</span></span>

<span data-ttu-id="5145f-113">Μια απαίτηση πόρου που δημιουργείται βασίζεται σε λεπτομέρειες όπως:</span><span class="sxs-lookup"><span data-stu-id="5145f-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="5145f-114">Χαρακτηριστικά</span><span class="sxs-lookup"><span data-stu-id="5145f-114">Characteristics</span></span>
-   <span data-ttu-id="5145f-115">Ρόλοι</span><span class="sxs-lookup"><span data-stu-id="5145f-115">Roles</span></span>
-   <span data-ttu-id="5145f-116">Επιχειρηματικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="5145f-116">Business units</span></span>
-   <span data-ttu-id="5145f-117">Προτιμήσεις πόρου</span><span class="sxs-lookup"><span data-stu-id="5145f-117">Resource preferences</span></span>
-   <span data-ttu-id="5145f-118">Καμπύλες προσπάθειας</span><span class="sxs-lookup"><span data-stu-id="5145f-118">Effort contours</span></span>
-   <span data-ttu-id="5145f-119">Ζώνη ώρας</span><span class="sxs-lookup"><span data-stu-id="5145f-119">Time zone</span></span>

<span data-ttu-id="5145f-120">Ο βοηθός χρονοδιαγράμματος χρησιμοποιεί αυτές τις λεπτομέρειες για το φιλτράρισμα των πόρων.</span><span class="sxs-lookup"><span data-stu-id="5145f-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="5145f-121">Εκκίνηση του βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="5145f-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="5145f-122">Υπάρχουν δύο τρόποι με τους οποίους ξεκινά ο βοηθός χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="5145f-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="5145f-123">Εάν χρησιμοποιείτε την υβριδική λειτουργία, στο πλέγμα μελών ομάδας μπορείτε να επιλέξετε οποιοδήποτε μέλος της ομάδας με υποχρέωση που δεν έχει εκπληρωθεί και, στη συνέχεια, να επιλέξετε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="5145f-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="5145f-124">Εάν χρησιμοποιείτε την κεντρική λειτουργία, ο διαχειριστής πόρων εντοπίζει και επιλέγει τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="5145f-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="5145f-125">Φίλτρα βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="5145f-125">Schedule assistant filters</span></span>

<span data-ttu-id="5145f-126">Μετά την εκτέλεση του βοηθού χρονοδιαγράμματος, οι λεπτομέρειες από την απαίτηση πόρου εμφανίζονται ως φιλτραρισμένες τιμές στο αριστερό παράθυρο.</span><span class="sxs-lookup"><span data-stu-id="5145f-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="5145f-127">Ο διαχειριστής πόρων ή ο διαχειριστής έργου μπορεί να τελειοποιήσει τα αποτελέσματα προσαρμόζοντας τα φίλτρα για να καλύψει τις ανάγκες προγραμματισμού.</span><span class="sxs-lookup"><span data-stu-id="5145f-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="5145f-128">Το παράθυρο φίλτρων εμφανίζει επιλογές που σχετίζονται με την εργασία, όπως:</span><span class="sxs-lookup"><span data-stu-id="5145f-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="5145f-129">Έναρξη και λήξη εργασίας</span><span class="sxs-lookup"><span data-stu-id="5145f-129">Work start and end</span></span>
-   <span data-ttu-id="5145f-130">Χαρακτηριστικά</span><span class="sxs-lookup"><span data-stu-id="5145f-130">Characteristics</span></span>
-   <span data-ttu-id="5145f-131">Ρόλοι</span><span class="sxs-lookup"><span data-stu-id="5145f-131">Roles</span></span>
-   <span data-ttu-id="5145f-132">Οργανικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="5145f-132">Organizational units</span></span>
-   <span data-ttu-id="5145f-133">Εταιρεία πόρων</span><span class="sxs-lookup"><span data-stu-id="5145f-133">Resourcing company</span></span>
-   <span data-ttu-id="5145f-134">Τύποι πόρων</span><span class="sxs-lookup"><span data-stu-id="5145f-134">Resource types</span></span>
-   <span data-ttu-id="5145f-135">Προτιμώμενοι πόροι</span><span class="sxs-lookup"><span data-stu-id="5145f-135">Preferred resources</span></span>
