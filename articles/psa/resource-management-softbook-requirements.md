---
title: Απαιτήσεις προκαταρκτικής κράτησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εκπλήρωσης των απαιτήσεων προκαταρκτικής κράτησης.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 861e484ea2fc251e0082b4cb0cd5409a45a74057
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077126"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="3ab37-103">Απαιτήσεις προκαταρκτικής κράτησης</span><span class="sxs-lookup"><span data-stu-id="3ab37-103">Soft-book requirements</span></span>

<span data-ttu-id="3ab37-104">Είναι δυνατή η οριστική κράτηση μιας απαίτησης πόρου.</span><span class="sxs-lookup"><span data-stu-id="3ab37-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="3ab37-105">Μια οριστική κράτηση δημιουργεί μια πρόταση που καταναλώνει την παραγωγική ικανότητα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="3ab37-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="3ab37-106">Στη συνέχεια, η πρόταση αποστέλλεται εκ νέου στον αιτούντα για έγκριση.</span><span class="sxs-lookup"><span data-stu-id="3ab37-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="3ab37-107">Μια προκαταρκτική κράτηση προσθέτει έναν πόρο σε μια ομάδα έργου και έχει μια διαφορετική κατάσταση στον πίνακα χρονοδιαγράμματος, αλλά δεν καταναλώνει την παραγωγική ικανότητα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="3ab37-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="3ab37-108">Για να κάνετε προκαταρκτική κράτηση σε έναν πόρο από τον πίνακα χρονοδιαγράμματος ορίστε το πεδίο **Κατάσταση κράτησης** σε **Προκαταρκτική**.</span><span class="sxs-lookup"><span data-stu-id="3ab37-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![Η κατάσταση κράτησης έχει οριστεί σε προκαταρκτική](media/Resource-Management-image77.png)

<span data-ttu-id="3ab37-110">Όταν η καρτέλα **Ομάδα** βρίσκεται στην προβολή **Καθορισμένα μέλη ομάδας** , ο πόρος εμφανίζεται εκεί.</span><span class="sxs-lookup"><span data-stu-id="3ab37-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="3ab37-111">Οι ώρες προκαταρκτικής κράτησης αναφέρονται στη στήλη **Ώρες προκαταρκτικής κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="3ab37-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![Ώρες προκαταρκτικής κράτησης στην προβολή καθορισμένων μελών ομάδας](media/Resource-Management-image78.png)

<span data-ttu-id="3ab37-113">Τα μέλη της ομάδας για τα οποία έχει γίνει προκαταρκτική κράτηση δεν αντιστοιχίζονται σε εργασίες.</span><span class="sxs-lookup"><span data-stu-id="3ab37-113">Soft-booked team members can be assigned to tasks.</span></span>

![Τα μέλη της ομάδας για τα οποία έχει γίνει προκαταρκτική κράτηση δεν αντιστοιχίζονται σε εργασία](media/Resource-Management-image79.png)

<span data-ttu-id="3ab37-115">Στην καρτέλα **Εναρμόνιση** , δεν εμφανίζονται κρατήσεις για έναν πόρο με προκαταρκτική κράτηση επειδή η καρτέλα **Εναρμόνιση** λαμβάνει υπόψη μόνο τις οριστικές κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="3ab37-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![Πόρος με προκαταρκτική κράτηση χωρίς κράτηση στην καρτέλα "εναρμόνιση"](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="3ab37-117">Δεν μπορείτε να κάνετε προκαταρκτική κράτηση σε έναν πόρο από μια απαίτηση η οποία δημιουργήθηκε από ένα γενικό μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="3ab37-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="3ab37-118">Στον πίνακα χρονοδιαγράμματος, χρησιμοποιείται ένα άλλο χρώμα για προκαταρκτικές κρατήσεις για έναν πόρο.</span><span class="sxs-lookup"><span data-stu-id="3ab37-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![Προκαταρκτικές κρατήσεις στον πίνακα χρονοδιαγράμματος](media/Resource-Management-image81.png)

<span data-ttu-id="3ab37-120">Για να μετατρέψετε μια προκαταρκτική κράτηση σε οριστική, στον πίνακα χρονοδιαγράμματος, κάντε δεξί κλικ στην προκαταρκτική κράτηση και, επιλέξτε **Αλλαγή κατάστασης** \> **Οριστική κράτηση** \> **Οριστική**.</span><span class="sxs-lookup"><span data-stu-id="3ab37-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![Αλλαγή της κατάστασης κράτησης σε οριστική](media/Resource-Management-image82.png)

<span data-ttu-id="3ab37-122">Η κράτηση αλλάζει και η κατάσταση αλλάζει στον πίνακα χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="3ab37-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="3ab37-123">Επειδή η κατάσταση της κράτησής είναι πλέον **Οριστική** , ο πόρος εμφανίζεται ως "κρατηθείς" και η χωρητικότητά του και η διαθεσιμότητά του προσαρμόζονται.</span><span class="sxs-lookup"><span data-stu-id="3ab37-123">Because the booking status is now **Hard** , the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="3ab37-124">Μπορείτε να χρησιμοποιήσετε την ίδια μέθοδο για να ακυρώσετε μια προκαταρκτική κράτηση ή μια οριστική κράτηση από τον πίνακα χρονοδιαγράμματος.</span><span class="sxs-lookup"><span data-stu-id="3ab37-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="3ab37-125">Για να μετατρέψετε έναν πόρο με προκαταρκτική κράτηση σε οριστική κράτηση στην καρτέλα **Ομάδα** του έργου, επιλέξτε τον πόρο και, στη συνέχεια, επιλέξτε **Επιβεβαίωση**.</span><span class="sxs-lookup"><span data-stu-id="3ab37-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![Εντολή επιβεβαίωσης](media/Resource-Management-image83.png)
