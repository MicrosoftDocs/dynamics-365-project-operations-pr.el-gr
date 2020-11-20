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
ms.openlocfilehash: 454b8931db53739a7bc19364911109802a1ed087
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127360"
---
# <a name="resource-estimates"></a><span data-ttu-id="498a2-103">Εκτιμήσεις πόρων</span><span class="sxs-lookup"><span data-stu-id="498a2-103">Resource estimates</span></span>

<span data-ttu-id="498a2-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="498a2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="498a2-105">Οι εκτιμήσεις πόρων προέρχονται από την προσπάθεια με χρονική κλιμάκωση που καθορίζεται στη δομή ανάλυσης εργασίας μαζί με τις εφαρμοστέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="498a2-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="498a2-106">Συνήθως, ο υπολογισμός είναι **τιμή/ώρα για κάθε ρόλο x ώρες.**</span><span class="sxs-lookup"><span data-stu-id="498a2-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="498a2-107">Η προσπάθεια με χρονική κλιμάκωση για κάθε πόρο αποθηκεύεται στην καρτέλα ανάθεσης πόρου.</span><span class="sxs-lookup"><span data-stu-id="498a2-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="498a2-108">Η τιμολόγηση αποθηκεύεται σε έναν προκαθορισμένο τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="498a2-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="498a2-109">Η μετατροπή μονάδας εφαρμόζεται με βάση τον ισχύοντα τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="498a2-109">Unit conversion is applied based on the applicable price list.</span></span>

![Εκτιμήσεις πόρων](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="498a2-111">Προεπιλογές τιμής κόστους και νομίσματος κόστους</span><span class="sxs-lookup"><span data-stu-id="498a2-111">Default cost price and cost currency</span></span>

<span data-ttu-id="498a2-112">Οι τιμές κόστους είναι προεπιλεγμένες από την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="498a2-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="498a2-113">Προεπιλογές συντελεστή χρέωσης και νομίσματος πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="498a2-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="498a2-114">Οι τιμές πώλησης εφαρμόζονται μία φορά ανά συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="498a2-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="498a2-115">Η ιεραρχία για την προεπιλογή τιμοκαταλόγου προς πώληση έχει ως εξής:</span><span class="sxs-lookup"><span data-stu-id="498a2-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="498a2-116">Εταιρεία</span><span class="sxs-lookup"><span data-stu-id="498a2-116">Organization</span></span>
2. <span data-ttu-id="498a2-117">Πελάτης</span><span class="sxs-lookup"><span data-stu-id="498a2-117">Customer</span></span>
3. <span data-ttu-id="498a2-118">Προσφορά/σύμβαση</span><span class="sxs-lookup"><span data-stu-id="498a2-118">Quote/contract</span></span>
