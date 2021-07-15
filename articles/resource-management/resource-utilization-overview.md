---
title: Επισκόπηση χρήσης πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση πόρου στο Project Operations.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: c9464b1de87211f8317a39a1d749e619769309ae
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367936"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="8f1d9-103">Επισκόπηση χρήσης πόρων</span><span class="sxs-lookup"><span data-stu-id="8f1d9-103">Resource utilization overview</span></span>

<span data-ttu-id="8f1d9-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="8f1d9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8f1d9-105">Οι πόροι μπορούν να έχουν μια χρεώσιμη χρήση-στόχο.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="8f1d9-106">Αυτή η χρήση-στόχος καθορίζεται είτε ως χαρακτηριστικό του προεπιλεγμένου ρόλου ενός πόρου ή ορίζεται στην καρτέλα του μεμονωμένου πόρου με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="8f1d9-107">Οι υπολογισμοί χρήσης βασίζονται στις πραγματικές ώρες που ανέφεραν οι πόροι χρησιμοποιώντας εγκεκριμένες καταχωρήσεις χρόνου.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="8f1d9-108">Οι ακόλουθοι τύποι χρησιμοποιούνται για τον υπολογισμό της χρήσης:</span><span class="sxs-lookup"><span data-stu-id="8f1d9-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="8f1d9-109">Χρεώσιμη χρήση = χρεώσιμες πραγματικές ώρες ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="8f1d9-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="8f1d9-110">Μη χρεώσιμη χρήση = πραγματικός χρόνος με αναγνωριστικό τύπου χρέωσης = μη χρεώσιμο, συμπληρωματικό ή μη διαθέσιμο ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="8f1d9-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="8f1d9-111">Εσωτερικό = πραγματικός χρόνος χωρίς σύμβαση πωλήσεων ÷ παραγωγική ικανότητα πόρου</span><span class="sxs-lookup"><span data-stu-id="8f1d9-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="8f1d9-112">Παραγωγική ικανότητα πόρου = ώρες εργασίας πόρου – εκτός γραφείου – μη εργάσιμες ημέρες</span><span class="sxs-lookup"><span data-stu-id="8f1d9-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="8f1d9-113">Μπορείτε να βρείτε την προβολή **Χρήση πόρου** στο παράθυρο **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="8f1d9-114">Κάθε κελί στο πλέγμα αντιπροσωπεύει το ποσοστό χρέωσης χρήσης του πόρου σε μια περίοδο, όπως μια ημέρα, μια εβδομάδα ή ένα μήνα.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="8f1d9-115">Οι ακόλουθοι τύποι χρησιμοποιούνται για τον χρωματισμό των κελιών:</span><span class="sxs-lookup"><span data-stu-id="8f1d9-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="8f1d9-116">**Πράσινο**: χρεώσιμη χρήση > = χρήση-στόχος πόρου</span><span class="sxs-lookup"><span data-stu-id="8f1d9-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="8f1d9-117">**Κίτρινο**: χρήση-στόχος – 20 < = χρεώσιμη χρήση < χρήση-στόχος.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="8f1d9-118">**Κόκκινο**: χρεώσιμη χρήση < = χρήση-στόχο - 20.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="8f1d9-119">Επειδή η προβολή **Χρήση πόρου** βασίζεται στον πίνακα χρονοδιαγράμματος, μπορείτε να χρησιμοποιήσετε τις δυνατότητες φιλτραρίσματος του πίνακα χρονοδιαγράμματος για να φιλτράρετε τα αποτελέσματά σας.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="8f1d9-120">Το πλέγμα απαιτεί να ορίσετε μια χρήση-στόχος στον ρόλο ή στον μεμονωμένο πόρο.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="8f1d9-121">Για να κάνετε αυτή τη ρύθμιση, μεταβείτε στα στοιχεία **Πόροι** > **Ρόλοι πόρων**.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="8f1d9-122">Επιπλέον, ένας προεπιλεγμένος ρόλος πρέπει να ανατεθεί σε κάθε πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="8f1d9-123">Μεταβείτε στα στοιχεία **Πόροι** > **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="8f1d9-124">Στην καρτέλα **Project Service** επαληθεύστε ότι καθορίζεται ένας ρόλος πόρου και ότι το πεδίο **Είναι προεπιλογή** έχει οριστεί σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="8f1d9-125">Μπορείτε να προσθέσετε επιπλέον ρόλους όπου το στοιχείο **Είναι προεπιλογή**  = **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="8f1d9-126">Ο ρόλος όπου το στοιχείο **Είναι προεπιλογή** = **Ναι** χρησιμοποιείται για την αξιολόγηση της χρήσης του πόρου σε σχέση με τον προορισμό για αυτόν το ρόλο.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="8f1d9-127">Στην καρτέλα **Project Service** μπορείτε επίσης να ορίσετε μια μεμονωμένη χρήση-στόχο για τον πόρο.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="8f1d9-128">Στη συνέχεια, ο υπολογισμός χρήσης χρησιμοποιεί την εν λόγω χρήση-στόχο για την αξιολόγηση του στόχου πόρου αντί του στόχου του προεπιλεγμένου ρόλου του πόρου.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="8f1d9-129">Η χρήση εμφανίζεται για έναν πόρο εάν αυτός ο πόρος έχει εγκρίνει τον χρεώσιμο χρόνο κατά τη διάρκεια της περιόδου που εμφανίζεται στο πλέγμα.</span><span class="sxs-lookup"><span data-stu-id="8f1d9-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]