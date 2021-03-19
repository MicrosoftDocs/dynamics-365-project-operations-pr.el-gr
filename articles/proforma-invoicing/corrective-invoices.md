---
title: Διορθωμένα τιμολόγια
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με διορθωμένα τιμολόγια.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 734dc01e15339a31ac21f92bb3fb20d634a075ad
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287823"
---
# <a name="corrected-invoices"></a><span data-ttu-id="64865-103">Διορθωμένα τιμολόγια</span><span class="sxs-lookup"><span data-stu-id="64865-103">Corrected invoices</span></span>

<span data-ttu-id="64865-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="64865-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="64865-105">Είναι δυνατή η επεξεργασία των επιβεβαιωμένων τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="64865-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="64865-106">Όταν κάνετε επεξεργασία σε ένα επιβεβαιωμένο τιμολόγιο, δημιουργείται ένα νέο προσχέδιο του διορθωμένου τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="64865-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="64865-107">Επειδή η παραδοχή είναι ότι θέλετε να αντιστρέψετε όλες τις συναλλαγές και τις ποσότητες από το αρχικό τιμολόγιο, αυτό το διορθωμένο τιμολόγιο περιλαμβάνει όλες τις συναλλαγές από το αρχικό τιμολόγιο και όλες οι ποσότητες σε αυτό είναι μηδέν (0).</span><span class="sxs-lookup"><span data-stu-id="64865-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="64865-108">Όταν οι συναλλαγές δεν απαιτούν διόρθωση, μπορείτε να τις καταργήσετε από το προσχέδιο διορθωτικού τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="64865-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="64865-109">Για να κάνετε αντιστροφή ή επιστροφή μόνο μιας μερικής ποσότητας, μπορείτε να επεξεργαστείτε το πεδίο Ποσότητα στη λεπτομέρεια γραμμής.</span><span class="sxs-lookup"><span data-stu-id="64865-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="64865-110">Εάν ανοίξετε τη λεπτομέρεια της γραμμής τιμολογίου, μπορείτε να δείτε την αρχική ποσότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="64865-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="64865-111">Στη συνέχεια, μπορείτε να επεξεργαστείτε την τρέχουσα ποσότητα τιμολογίου, έτσι ώστε να είναι μικρότερη ή μεγαλύτερη από την αρχική ποσότητα τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="64865-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="64865-112">Όταν επιβεβαιώνετε ένα διορθωτικό τιμολόγιο, η αρχικά τιμολογημένη πραγματική πώληση αντιστρέφεται και δημιουργείται ένα νέο πραγματικό τιμολόγησης πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="64865-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="64865-113">Εάν η ποσότητα μειώθηκε, η διαφορά θα προκαλέσει επίσης τη δημιουργία ενός νέου πραγματικού πωλητή που δεν έχει χρεωθεί.</span><span class="sxs-lookup"><span data-stu-id="64865-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="64865-114">Για παράδειγμα, εάν η αρχική τιμολογημένη πώληση ήταν για οκτώ ώρες και η αναλυτική γραμμή διορθωτικού τιμολογίου έχει μειωμένη ποσότητα έξι ωρών, αντιστρέφεται η αρχική τιμολογημένη γραμμή πωλήσεων και δημιουργούνται δύο νέες πραγματικές τιμές:</span><span class="sxs-lookup"><span data-stu-id="64865-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="64865-115">Μια πραγματική τιμολόγηση πωλήσεων για έξι ώρες.</span><span class="sxs-lookup"><span data-stu-id="64865-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="64865-116">Μια πραγματική πώληση που δεν έχει χρεωθεί για τις υπόλοιπες δύο ώρες.</span><span class="sxs-lookup"><span data-stu-id="64865-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="64865-117">Αυτή η συναλλαγή μπορεί είτε να χρεωθεί αργότερα είτε να χαρακτηριστεί ως μη τιμολογημένη, ανάλογα με τις διαπραγματεύσεις με τον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="64865-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]