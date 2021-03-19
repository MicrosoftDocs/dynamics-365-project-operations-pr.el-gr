---
title: Προσφορά, χρέωση και τιμολόγηση για προχωρημένους
description: Αυτό το θέμα παρέχει πληροφορίες για την προσφορά, τη χρέωση και την τιμολόγηση στο Project Service Automation.
author: kfend
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 2/14/2019
ms.topic: article
ms.author: kfend
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c4674aba1d152289c78a202f9da1f710e28f9960
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275223"
---
# <a name="advanced-quoting-pricing-and-billing-guide"></a><span data-ttu-id="5e9c1-103">Οδηγός σχετικά με την προηγμένη προσφορά, την τιμή και τη χρέωση</span><span class="sxs-lookup"><span data-stu-id="5e9c1-103">Advanced quoting, pricing, and billing guide</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5e9c1-104">Η δυνατότητα να βρείτε τους κατάλληλους πόρους την κατάλληλη στιγμή, να κάνετε κράτηση αυτών των πόρων σε έργα και να τους αξιοποιήσετε, βοηθάει τον οργανισμό να καλύψει τους στόχους εσόδων και τους στόχους ικανοποίησης πελατών.</span><span class="sxs-lookup"><span data-stu-id="5e9c1-104">The ability to find the right resources at the right time, book those resources on projects, and keep resources utilized helps organizations meet revenue targets and customer satisfaction goals.</span></span> 

<span data-ttu-id="5e9c1-105">Η σύνδεση PDF που ήταν προηγουμένως σε αυτό το θέμα έχει καταργηθεί και το περιεχόμενο έχει μετακινηθεί στα εξής θέματα:</span><span class="sxs-lookup"><span data-stu-id="5e9c1-105">The PDF link that was previously in this topic has been removed and the content has been moved to the following topics:</span></span>

- [<span data-ttu-id="5e9c1-106">Προσφορά, χρέωση και τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="5e9c1-106">Quoting, pricing, and billing</span></span>](../quote-bill-price.md)
- [<span data-ttu-id="5e9c1-107">Διαδικασίες πώλησης</span><span class="sxs-lookup"><span data-stu-id="5e9c1-107">Sales processes</span></span>](../basic-sales-process.md)
- [<span data-ttu-id="5e9c1-108">Προσφορές και γραμμές προσφορών</span><span class="sxs-lookup"><span data-stu-id="5e9c1-108">Quotes and quote lines</span></span>](../basic-quote-lines.md)
- [<span data-ttu-id="5e9c1-109">Γραμμές προσφοράς βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="5e9c1-109">Product-based quote lines</span></span>](../product-based-quote-lines.md)
- [<span data-ttu-id="5e9c1-110">Τιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="5e9c1-110">Pricing</span></span>](../basic-pricing.md)
- [<span data-ttu-id="5e9c1-111">Τιμολόγηση τιμοκαταλόγου</span><span class="sxs-lookup"><span data-stu-id="5e9c1-111">Product catalog pricing</span></span>](../product-catalog-pricing.md)
- [<span data-ttu-id="5e9c1-112">Επιχειρηματικές συναλλαγές</span><span class="sxs-lookup"><span data-stu-id="5e9c1-112">Business transactions</span></span>](../basic-business-transactions.md)
- [<span data-ttu-id="5e9c1-113">Εκτιμήσεις</span><span class="sxs-lookup"><span data-stu-id="5e9c1-113">Estimates</span></span>](../estimates.md)
- [<span data-ttu-id="5e9c1-114">Πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="5e9c1-114">Actuals</span></span>](../actuals.md)
- [<span data-ttu-id="5e9c1-115">Ανάλυση προσφορών έργου</span><span class="sxs-lookup"><span data-stu-id="5e9c1-115">Analyzing project quotes</span></span>](../basic-analyzing-quotes.md)
- [<span data-ttu-id="5e9c1-116">Οργανικές μονάδες</span><span class="sxs-lookup"><span data-stu-id="5e9c1-116">Organizational units</span></span>](../advanced-organizational.md)
- [<span data-ttu-id="5e9c1-117">Ομάδες μονάδων και μονάδες</span><span class="sxs-lookup"><span data-stu-id="5e9c1-117">Unit groups and units</span></span>](../advanced-units.md)
- [<span data-ttu-id="5e9c1-118">Σενάρια πολλαπλών νομισματικών μονάδων</span><span class="sxs-lookup"><span data-stu-id="5e9c1-118">Multi-currency scenarios</span></span>](../advanced-currency.md)
- [<span data-ttu-id="5e9c1-119">Καταγραφή πραγματικών τιμών</span><span class="sxs-lookup"><span data-stu-id="5e9c1-119">Recording actuals</span></span>](../advanced-actuals.md)

> [!NOTE]
> <span data-ttu-id="5e9c1-120">Αυτό το θέμα θα καταργηθεί σε μια μελλοντική ενημέρωση τεκμηρίωσης.</span><span class="sxs-lookup"><span data-stu-id="5e9c1-120">This topic will be removed in a future documentation update.</span></span> 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]