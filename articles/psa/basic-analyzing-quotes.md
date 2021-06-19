---
title: Ανάλυση προσφορών έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την ανάλυση των προσφορών έργου.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012451"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="2d0b4-103">Ανάλυση προσφορών έργου</span><span class="sxs-lookup"><span data-stu-id="2d0b4-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2d0b4-104">Το Dynamics 365 Project Service Automation αναλύει τις προσφορές του έργου για την εκτίμηση της κερδοφορίας.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="2d0b4-105">Επίσης, αναλύει πόσο καλά εναρμονίζεται η προσφορά με τις προσδοκίες των πελατών σχετικά με την ημερομηνία παράδοσης ή την ημερομηνία ολοκλήρωσης και σχετικά με τον προϋπολογισμό.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="2d0b4-106">Ανάλυση κερδοφορίας</span><span class="sxs-lookup"><span data-stu-id="2d0b4-106">Profitability analysis</span></span>

<span data-ttu-id="2d0b4-107">Το Project Service Automation αναλύει την κερδοφορία με χρήση του περιθωρίου ακαθάριστου κέρδους και του προσαρμοσμένου περιθωρίου ακαθάριστου κέρδους.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="2d0b4-108">Τα περιθώρια ακαθάριστου κέρδους υπολογίζονται με χρήση του ακόλουθου τύπου:</span><span class="sxs-lookup"><span data-stu-id="2d0b4-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="2d0b4-109">Τα προσαρμοσμένα περιθώρια ακαθάριστου κέρδους υπολογίζονται με χρήση του ακόλουθου τύπου:</span><span class="sxs-lookup"><span data-stu-id="2d0b4-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="2d0b4-110">Εάν οι τιμές για το περιθώριο ακαθάριστου κέρδους και το προσαρμοσμένο περιθώριο ακαθάριστου κέρδους διαφέρουν λόγω μεγάλου περιθωρίου, το μεγαλύτερο μέρος της εργασίας στην προσφορά ταξινομείται ως μη χρεώσιμο.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="2d0b4-111">Ανάλυση των προσδοκιών του πελάτη</span><span class="sxs-lookup"><span data-stu-id="2d0b4-111">Analysis of customer expectations</span></span>

<span data-ttu-id="2d0b4-112">Μπορείτε να αναλύσετε προσφορές και να δημιουργήσετε γραφήματα για τις προσδοκίες των πελατών σχετικά με το χρονοδιάγραμμα και τον προϋπολογισμό, εάν καταχωρείτε τιμές για τα ακόλουθα πεδία:</span><span class="sxs-lookup"><span data-stu-id="2d0b4-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="2d0b4-113">Το πεδίο **Ημερομηνία παράδοσης που ζητήθηκε** στην επικεφαλίδα της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="2d0b4-114">Το πεδίο **Προϋπολογισμός πελάτη** για κάθε γραμμή προσφοράς (για γραμμές βάσει έργου και γραμμές βάσει προϊόντων).</span><span class="sxs-lookup"><span data-stu-id="2d0b4-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="2d0b4-115">Η ανάλυση των προσδοκιών του πελάτη σχετικά με το χρονοδιάγραμμα γίνεται με τη σύγκριση της πιο πρόσφατης ημερομηνίας λήξης της λεπτομέρειας της γραμμής προσφοράς με την αιτούμενη ημερομηνία παράδοσης σε όλες τις γραμμές προσφοράς της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="2d0b4-116">Η ανάλυση των προσδοκιών του πελάτη σχετικά με τον προϋπολογισμό γίνεται με τη σύγκριση του αθροίσματος του συνολικού προϋπολογισμού του πελάτη με το ποσό της προσφοράς σε όλες τις γραμμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2d0b4-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]