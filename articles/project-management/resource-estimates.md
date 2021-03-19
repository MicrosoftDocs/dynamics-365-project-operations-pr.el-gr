---
title: Εκτιμήσεις πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο υπολογισμού των εκτιμήσεων πόρων στο Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286518"
---
# <a name="resource-estimates"></a><span data-ttu-id="cd192-103">Εκτιμήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="cd192-103">Resource estimates</span></span>

<span data-ttu-id="cd192-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="cd192-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cd192-105">Οι εκτιμήσεις πόρων προέρχονται από την προσπάθεια με χρονική κλιμάκωση που καθορίζεται στη δομή ανάλυσης εργασίας μαζί με τις εφαρμοστέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="cd192-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="cd192-106">Συνήθως, ο υπολογισμός είναι **τιμή/ώρα για κάθε ρόλο x ώρες.**</span><span class="sxs-lookup"><span data-stu-id="cd192-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="cd192-107">Η προσπάθεια με χρονική κλιμάκωση για κάθε πόρο αποθηκεύεται στην καρτέλα ανάθεσης πόρου.</span><span class="sxs-lookup"><span data-stu-id="cd192-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="cd192-108">Η τιμολόγηση αποθηκεύεται σε έναν προκαθορισμένο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="cd192-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="cd192-109">Η μετατροπή μονάδας εφαρμόζεται με βάση τον ισχύοντα τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="cd192-109">Unit conversion is applied based on the applicable price list.</span></span>

![Εκτιμήσεις πόρων](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="cd192-111">Προεπιλογές τιμής κόστους και νομίσματος κόστους</span><span class="sxs-lookup"><span data-stu-id="cd192-111">Default cost price and cost currency</span></span>

<span data-ttu-id="cd192-112">Οι τιμές κόστους είναι προεπιλεγμένες από την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="cd192-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="cd192-113">Προεπιλογές συντελεστή χρέωσης και νομίσματος πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="cd192-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="cd192-114">Οι τιμές πώλησης εφαρμόζονται μία φορά ανά συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="cd192-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="cd192-115">Η ιεραρχία για την προεπιλογή τιμοκαταλόγου προς πώληση έχει ως εξής:</span><span class="sxs-lookup"><span data-stu-id="cd192-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="cd192-116">Εταιρεία</span><span class="sxs-lookup"><span data-stu-id="cd192-116">Organization</span></span>
2. <span data-ttu-id="cd192-117">Πελάτης</span><span class="sxs-lookup"><span data-stu-id="cd192-117">Customer</span></span>
3. <span data-ttu-id="cd192-118">Προσφορά/σύμβαση</span><span class="sxs-lookup"><span data-stu-id="cd192-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]