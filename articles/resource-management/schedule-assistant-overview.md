---
title: Επισκόπηση βοηθού χρονοδιαγράμματος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με τον βοηθό χρονοδιαγράμματος για την κράτηση πόρων.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: da551e805f395e466952df1dbb7d193bdddba358
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076772"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="c67c9-103">Επισκόπηση βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="c67c9-103">Schedule assistant overview</span></span>

<span data-ttu-id="c67c9-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="c67c9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c67c9-105">Ο βοηθός χρονοδιαγράμματος χρησιμοποιείται για τη κράτηση πόρων με βάση τις απαιτήσεις που καθορίζονται από το διαχειριστή έργου.</span><span class="sxs-lookup"><span data-stu-id="c67c9-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="c67c9-106">Ο βοηθός χρονοδιαγράμματος βασίζεται στις παραμέτρους που παρέχονται στην απαίτηση πόρου για την εύρεση του πόρου.</span><span class="sxs-lookup"><span data-stu-id="c67c9-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="c67c9-107">Ο βοηθός χρονοδιαγράμματος συνιστά πόρους που αντιστοιχίζονται σε σχετικές απαιτήσεις, όπως τα παράθυρα χρόνου ή οι δεξιότητες που απαιτούνται.</span><span class="sxs-lookup"><span data-stu-id="c67c9-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="c67c9-108">Μετά την ταυτοποίηση των κατάλληλων πόρων, ο πόρος ή ο διαχειριστής έργου μπορούν να κάνουν κράτηση του πόρου στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="c67c9-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c67c9-109">Προαπαιτούμενα στοιχεία</span><span class="sxs-lookup"><span data-stu-id="c67c9-109">Prerequisites</span></span>

<span data-ttu-id="c67c9-110">Ο βοηθός χρονοδιαγράμματος αποτελεί μέρος της Universal Resource Scheduling λύσης.</span><span class="sxs-lookup"><span data-stu-id="c67c9-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="c67c9-111">Αυτή η λύση περιλαμβάνεται και εγκαθίσταται με το Dynamics 365 Project Operations, το Dynamics 365 Field Service και το Dynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="c67c9-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="c67c9-112">Απαιτήσεις και πόροι αντιστοίχισης</span><span class="sxs-lookup"><span data-stu-id="c67c9-112">Matching requirements and resources</span></span>

<span data-ttu-id="c67c9-113">Μια απαίτηση πόρου που δημιουργείται βασίζεται σε λεπτομέρειες όπως:</span><span class="sxs-lookup"><span data-stu-id="c67c9-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="c67c9-114">Χαρακτηριστικά</span><span class="sxs-lookup"><span data-stu-id="c67c9-114">Characteristics</span></span>
-   <span data-ttu-id="c67c9-115">Ρόλοι</span><span class="sxs-lookup"><span data-stu-id="c67c9-115">Roles</span></span>
-   <span data-ttu-id="c67c9-116">Επιχειρηματικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="c67c9-116">Business units</span></span>
-   <span data-ttu-id="c67c9-117">Προτιμήσεις πόρου</span><span class="sxs-lookup"><span data-stu-id="c67c9-117">Resource preferences</span></span>
-   <span data-ttu-id="c67c9-118">Καμπύλες προσπάθειας</span><span class="sxs-lookup"><span data-stu-id="c67c9-118">Effort contours</span></span>
-   <span data-ttu-id="c67c9-119">Ζώνη ώρας</span><span class="sxs-lookup"><span data-stu-id="c67c9-119">Time zone</span></span>

<span data-ttu-id="c67c9-120">Ο βοηθός χρονοδιαγράμματος χρησιμοποιεί αυτές τις λεπτομέρειες για το φιλτράρισμα των πόρων.</span><span class="sxs-lookup"><span data-stu-id="c67c9-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="c67c9-121">Εκκίνηση του βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="c67c9-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="c67c9-122">Υπάρχουν δύο τρόποι με τους οποίους ξεκινά ο βοηθός χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="c67c9-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="c67c9-123">Εάν χρησιμοποιείτε την υβριδική λειτουργία, στο πλέγμα μελών ομάδας μπορείτε να επιλέξετε οποιοδήποτε μέλος της ομάδας με υποχρέωση που δεν έχει εκπληρωθεί και, στη συνέχεια, να επιλέξετε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="c67c9-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="c67c9-124">Εάν χρησιμοποιείτε την κεντρική λειτουργία, ο διαχειριστής πόρων εντοπίζει και επιλέγει τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="c67c9-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="c67c9-125">Φίλτρα βοηθού χρονοδιαγράμματος</span><span class="sxs-lookup"><span data-stu-id="c67c9-125">Schedule assistant filters</span></span>

<span data-ttu-id="c67c9-126">Μετά την εκτέλεση του βοηθού χρονοδιαγράμματος, οι λεπτομέρειες από την απαίτηση πόρου εμφανίζονται ως φιλτραρισμένες τιμές στο αριστερό παράθυρο.</span><span class="sxs-lookup"><span data-stu-id="c67c9-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="c67c9-127">Ο διαχειριστής πόρων ή ο διαχειριστής έργου μπορεί να τελειοποιήσει τα αποτελέσματα προσαρμόζοντας τα φίλτρα για να καλύψει τις ανάγκες προγραμματισμού.</span><span class="sxs-lookup"><span data-stu-id="c67c9-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="c67c9-128">Το παράθυρο φίλτρων εμφανίζει επιλογές που σχετίζονται με την εργασία, όπως:</span><span class="sxs-lookup"><span data-stu-id="c67c9-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="c67c9-129">Έναρξη και λήξη εργασίας</span><span class="sxs-lookup"><span data-stu-id="c67c9-129">Work start and end</span></span>
-   <span data-ttu-id="c67c9-130">Χαρακτηριστικά</span><span class="sxs-lookup"><span data-stu-id="c67c9-130">Characteristics</span></span>
-   <span data-ttu-id="c67c9-131">Ρόλοι</span><span class="sxs-lookup"><span data-stu-id="c67c9-131">Roles</span></span>
-   <span data-ttu-id="c67c9-132">Οργανικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="c67c9-132">Organizational units</span></span>
-   <span data-ttu-id="c67c9-133">Εταιρεία πόρων</span><span class="sxs-lookup"><span data-stu-id="c67c9-133">Resourcing company</span></span>
-   <span data-ttu-id="c67c9-134">Τύποι πόρων</span><span class="sxs-lookup"><span data-stu-id="c67c9-134">Resource types</span></span>
-   <span data-ttu-id="c67c9-135">Προτιμώμενοι πόροι</span><span class="sxs-lookup"><span data-stu-id="c67c9-135">Preferred resources</span></span>
