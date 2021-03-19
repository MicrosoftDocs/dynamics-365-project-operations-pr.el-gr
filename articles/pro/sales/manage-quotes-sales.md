---
title: Διαχείριση προσφορών έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις προσφορές έργου.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 87921221ea210e67a3ddc53bd124f292de80de99
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272928"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="b9ca8-103">Διαχείριση προσφορών έργου</span><span class="sxs-lookup"><span data-stu-id="b9ca8-103">Manage project quotes</span></span>

<span data-ttu-id="b9ca8-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="b9ca8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b9ca8-105">Στο Dynamics 365 Project Operations, οι προσφορές έργου έχουν σχεδιαστεί για να σας βοηθήσουν να δημιουργήσετε προτάσεις για εργασίες έργου.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="b9ca8-106">Η δομή μιας προσφοράς έργου στο Project Operations έχει σχεδιαστεί για προτάσεις έργου με τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="b9ca8-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="b9ca8-107">Γραμμές προσφοράς που προσδιορίζουν τα διακριτά στοιχεία του έργου που θα παρουσιαστούν ως στοιχεία υψηλού επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="b9ca8-108">Λεπτομέρειες της γραμμής προσφοράς που προσδιορίζουν και εκτιμούν την εργασία για κάθε στοιχείο ή γραμμή προσφοράς υψηλού επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="b9ca8-109">Οι εκτιμήσεις χρονοδιαγράμματος ή ημερομηνίας και οι οικονομικές πτυχές για την εργασία συνδέονται με αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="b9ca8-110">Τα συμβατικά μοντέλα και τα χρεώσιμα στοιχεία είναι ρυθμισμένα για κάθε γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="b9ca8-111">Αυτή η ρύθμιση βοηθάει στην εκτίμηση της εξάπλωσης των εσόδων, της δαπάνης και της κερδοφορίας για κάθε γραμμή προσφοράς και στη συνολική προσφορά.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="b9ca8-112">Προβολή όλων των προσφορών βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="b9ca8-112">View all project-based quotes</span></span>

<span data-ttu-id="b9ca8-113">Μπορείτε να δείτε μια λίστα όλων των προσφορών από τη σελίδα λίστας **Προσφορές**.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="b9ca8-114">Μεταβείτε στην επιλογή **Πωλήσεις** > **Προσφορές**.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="b9ca8-115">Εμφανίζεται μια λίστα με όλες τις προσφορές έργου που έχετε στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="b9ca8-116">Χρησιμοποιήστε την **Εναλλαγή προβολής** για να επιλέξετε άλλες φιλτραρισμένες προβολές των προσφορών.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="b9ca8-117">Χρησιμοποιώντας προσαρμοσμένα κριτήρια φιλτραρίσματος, μπορείτε να ρυθμίσετε τις δικές σας προβολές και επιλογές περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="b9ca8-118">Οι προσφορές μπορούν να δημιουργηθούν ή να διαγραφούν από αυτήν τη σελίδα λίστας ή τις σελίδες λεπτομερειών.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-118">Quotes can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]