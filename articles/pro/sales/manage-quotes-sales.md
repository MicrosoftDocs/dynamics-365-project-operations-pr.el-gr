---
title: Διαχείριση προσφορών έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις προσφορές έργου.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8e0b20d4780a14edc3c242e261e22d4905f783a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994811"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="430b0-103">Διαχείριση προσφορών έργου</span><span class="sxs-lookup"><span data-stu-id="430b0-103">Manage project quotes</span></span>

<span data-ttu-id="430b0-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="430b0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="430b0-105">Στο Dynamics 365 Project Operations, οι προσφορές έργου έχουν σχεδιαστεί για να σας βοηθήσουν να δημιουργήσετε προτάσεις για εργασίες έργου.</span><span class="sxs-lookup"><span data-stu-id="430b0-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="430b0-106">Η δομή μιας προσφοράς έργου στο Project Operations έχει σχεδιαστεί για προτάσεις έργου με τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="430b0-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="430b0-107">Γραμμές προσφοράς που προσδιορίζουν τα διακριτά στοιχεία του έργου που θα παρουσιαστούν ως στοιχεία υψηλού επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="430b0-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="430b0-108">Λεπτομέρειες της γραμμής προσφοράς που προσδιορίζουν και εκτιμούν την εργασία για κάθε στοιχείο ή γραμμή προσφοράς υψηλού επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="430b0-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="430b0-109">Οι εκτιμήσεις χρονοδιαγράμματος ή ημερομηνίας και οι οικονομικές πτυχές για την εργασία συνδέονται με αυτήν τη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="430b0-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="430b0-110">Τα συμβατικά μοντέλα και τα χρεώσιμα στοιχεία είναι ρυθμισμένα για κάθε γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="430b0-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="430b0-111">Αυτή η ρύθμιση βοηθάει στην εκτίμηση της εξάπλωσης των εσόδων, της δαπάνης και της κερδοφορίας για κάθε γραμμή προσφοράς και στη συνολική προσφορά.</span><span class="sxs-lookup"><span data-stu-id="430b0-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="430b0-112">Προβολή όλων των προσφορών βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="430b0-112">View all project-based quotes</span></span>

<span data-ttu-id="430b0-113">Μπορείτε να δείτε μια λίστα όλων των προσφορών από τη σελίδα λίστας **Προσφορές**.</span><span class="sxs-lookup"><span data-stu-id="430b0-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="430b0-114">Μεταβείτε στην επιλογή **Πωλήσεις** > **Προσφορές**.</span><span class="sxs-lookup"><span data-stu-id="430b0-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="430b0-115">Εμφανίζεται μια λίστα με όλες τις προσφορές έργου που έχετε στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="430b0-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="430b0-116">Χρησιμοποιήστε την **Εναλλαγή προβολής** για να επιλέξετε άλλες φιλτραρισμένες προβολές των προσφορών.</span><span class="sxs-lookup"><span data-stu-id="430b0-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="430b0-117">Χρησιμοποιώντας προσαρμοσμένα κριτήρια φιλτραρίσματος, μπορείτε να ρυθμίσετε τις δικές σας προβολές και επιλογές περιήγησης.</span><span class="sxs-lookup"><span data-stu-id="430b0-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="430b0-118">Οι προσφορές μπορούν να δημιουργηθούν ή να διαγραφούν από αυτήν τη σελίδα λίστας ή τις σελίδες λεπτομερειών.</span><span class="sxs-lookup"><span data-stu-id="430b0-118">Quotes can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]