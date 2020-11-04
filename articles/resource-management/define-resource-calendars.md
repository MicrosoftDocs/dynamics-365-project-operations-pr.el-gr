---
title: Καθορισμός ημερολογίων πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ορισμού των ημερολογίων ώρας εργασίας για πόρους στο Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076764"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="400cf-103">Καθορισμός ημερολογίων πόρων</span><span class="sxs-lookup"><span data-stu-id="400cf-103">Define resource calendars</span></span>

<span data-ttu-id="400cf-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="400cf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="400cf-105">Κάθε πόρος με δυνατότητα κράτησης που εργάζεται σε ένα έργο πρέπει να έχει ένα ημερολόγιο ωρών εργασίας, για να καθορίζει τη διαθεσιμότητά του.</span><span class="sxs-lookup"><span data-stu-id="400cf-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="400cf-106">Οι ώρες εργασίας για έναν πόρο μπορούν να οριστούν με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="400cf-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="400cf-107">Καθορισμός κανόνων μεμονωμένων ημερολογίων για έναν πόρο</span><span class="sxs-lookup"><span data-stu-id="400cf-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="400cf-108">Εφαρμογή υπάρχοντος προτύπου ημερολογίου για τον πόρο</span><span class="sxs-lookup"><span data-stu-id="400cf-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="400cf-109">Ορισμός ωρών εργασίας πόρου</span><span class="sxs-lookup"><span data-stu-id="400cf-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="400cf-110">Στο μενού **Πόροι** , επιλέξτε **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="400cf-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="400cf-111">Από την προβολή πλέγματος, επιλέξτε τον εφαρμοστέο **Πόρο με δυνατότητα κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="400cf-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="400cf-112">Στη σελίδα **Λεπτομέρειες πόρου** , επιλέξτε την καρτέλα **Ώρες εργασίας**. Από προεπιλογή, το ημερολόγιο πόρων με δυνατότητα κράτησης προκαθορίζει τις ώρες εργασίας του προεπιλεγμένου προτύπου ωρών εργασίας που έχει οριστεί για τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="400cf-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="400cf-113">Για να ενημερώσετε τις ώρες εργασίας, κάντε δεξί κλικ στην ημερομηνία έναρξης του προτεινόμενου κανόνα ημερολογίου που θα καθοριστεί.</span><span class="sxs-lookup"><span data-stu-id="400cf-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="400cf-114">Χρησιμοποιήστε το μενού κανόνων ημερολογίου για να καθορίσετε έναν κανόνα ημερολογίου για μια συγκεκριμένη ημέρα, το υπόλοιπο της σειράς ή ολόκληρο το ημερολόγιο.</span><span class="sxs-lookup"><span data-stu-id="400cf-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="400cf-115">Αφού ενεργοποιηθεί η επιλογή, στη συνέχεια, μπορείτε να καθορίσετε:</span><span class="sxs-lookup"><span data-stu-id="400cf-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="400cf-116">Την ημέρα της εβδομάδας κατά την οποία θα ισχύσουν οι ώρες εργασίας.</span><span class="sxs-lookup"><span data-stu-id="400cf-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="400cf-117">Τις ώρες εργασίας εντός κάθε ημέρας.</span><span class="sxs-lookup"><span data-stu-id="400cf-117">The working times within each day.</span></span>
    - <span data-ttu-id="400cf-118">Τη ζώνη ώρας για τον κανόνα ημερολογίου.</span><span class="sxs-lookup"><span data-stu-id="400cf-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="400cf-119">Εάν ισχύει, μπορεί να καθοριστεί και ο μη εργάσιμος χρόνος για τον κανόνα.</span><span class="sxs-lookup"><span data-stu-id="400cf-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="400cf-120">Εφαρμογή προτύπου ημερολογίου σε πόρο</span><span class="sxs-lookup"><span data-stu-id="400cf-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="400cf-121">Στο μενού **Πόροι** , επιλέξτε **Πόροι**.</span><span class="sxs-lookup"><span data-stu-id="400cf-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="400cf-122">Από την προβολή πλέγματος, επιλέξτε έως και 25 **πόρους με δυνατότητα κράτησης** για ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="400cf-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="400cf-123">Επιλέξτε **Ορισμός ημερολογίου** και ένα παράθυρο διαλόγου θα σας ζητήσει μια λίστα με τα διαθέσιμα πρότυπα ωρών εργασίας.</span><span class="sxs-lookup"><span data-stu-id="400cf-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="400cf-124">Επιλέξτε το πρότυπο που θέλετε να χρησιμοποιήσετε και, στη συνέχεια, επιλέξτε **Εφαρμογή**.</span><span class="sxs-lookup"><span data-stu-id="400cf-124">Select the template you want to use, and then select **Apply**.</span></span>