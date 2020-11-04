---
title: Ρύθμιση τιμοκαταλόγου πωλήσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τους τιμοκαταλόγους πωλήσεων για την τιμολόγηση έργων.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 1d2c797b72666123eb0a18d2d0c1df9fe3d207f7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076971"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="d20e1-103">Ρύθμιση τιμοκαταλόγου πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="d20e1-103">Sales price list setup</span></span>

<span data-ttu-id="d20e1-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="d20e1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d20e1-105">Για τις προσφορές και τις συμβάσεις έργου, ο τιμοκατάλογος έργου έχει διαφορετικό μοτίβο παράκαμψης της τιμής σε σχέση με τον τιμοκατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="d20e1-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="d20e1-106">Σε μια γραμμή προσφοράς με βάση τον κατάλογο προϊόντων, μπορείτε να παρακάμψετε την τιμή σε ρόλους και κατηγορίες απευθείας στη γραμμή προσφοράς, επειδή κάθε γραμμή προσφοράς παραπέμπει σε ένα ακριβώς στοιχείο καταλόγου.</span><span class="sxs-lookup"><span data-stu-id="d20e1-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="d20e1-107">Ωστόσο, σε μια γραμμή προσφοράς βάσει έργου, δεν μπορείτε να παρακάμψετε την τιμή σε ρόλους και κατηγορίες απευθείας στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d20e1-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="d20e1-108">Μπορείτε να χρησιμοποιήσετε τον τιμοκατάλογο έργου για να εργαστείτε με τα δύο διακριτά μοτίβα παράκαμψης.</span><span class="sxs-lookup"><span data-stu-id="d20e1-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="d20e1-109">Συνιστούμε να διαθέτετε έναν ξεχωριστό τιμοκατάλογο για τους πόρους του έργου σας και τα στοιχεία του καταλόγου σας, εξαιτίας των διαφορών συμπεριφοράς μεταξύ των δύο όταν παρακάμπτετε την τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="d20e1-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="d20e1-110">Κάθε μία από τις ακόλουθες οντότητες μπορεί να έχει έναν ή περισσότερους συσχετισμένους τιμοκαταλόγους πώλησης για την τιμολόγηση έργου:</span><span class="sxs-lookup"><span data-stu-id="d20e1-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="d20e1-111">Πελάτης (λογαριασμός)</span><span class="sxs-lookup"><span data-stu-id="d20e1-111">Customer (account)</span></span> 
- <span data-ttu-id="d20e1-112">Ευκαιρία</span><span class="sxs-lookup"><span data-stu-id="d20e1-112">Opportunity</span></span> 
- <span data-ttu-id="d20e1-113">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="d20e1-113">Quote</span></span> 
- <span data-ttu-id="d20e1-114">Σύμβαση έργου</span><span class="sxs-lookup"><span data-stu-id="d20e1-114">Project Contract</span></span>

<span data-ttu-id="d20e1-115">Ο συσχετισμός αυτών των οντοτήτων με έναν τιμοκατάλογο υποδεικνύεται από τους τιμοκαταλόγους έργου.</span><span class="sxs-lookup"><span data-stu-id="d20e1-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="d20e1-116">Μπορείτε να συσχετίσετε έναν ή περισσότερους τιμοκαταλόγους με τις οντότητες "πελάτης", "ευκαιρία", "προσφορά" και "πωλήσεις σύμβασης έργου".</span><span class="sxs-lookup"><span data-stu-id="d20e1-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="d20e1-117">Ένας προεπιλεγμένος τιμοκατάλογος έργου δεν καταχωρείται αυτόματα σε μια καρτέλα πελάτη.</span><span class="sxs-lookup"><span data-stu-id="d20e1-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="d20e1-118">Ωστόσο, μπορείτε να επισυνάψετε έναν τιμοκατάλογο έργου στην καρτέλα πελάτη με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="d20e1-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="d20e1-119">Παρόλα αυτά, θα πρέπει να επισυνάψετε έναν τιμοκατάλογο έργου με μη αυτόματο τρόπο, μόνο όταν έχετε μια προσαρμοσμένη συμφωνία τιμολόγησης με τον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="d20e1-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="d20e1-120">Όταν ένας τιμοκατάλογος έργου επισυνάπτεται σε μια οντότητα πωλήσεων, επικυρώνονται οι παρακάτω πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="d20e1-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="d20e1-121">Ο τιμοκατάλογος έχει ένα περιβάλλον **Πωλήσεων**.</span><span class="sxs-lookup"><span data-stu-id="d20e1-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="d20e1-122">Το νόμισμα του τιμοκαταλόγου πρέπει να αντιστοιχεί στο νόμισμα του πελάτη.</span><span class="sxs-lookup"><span data-stu-id="d20e1-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="d20e1-123">Σε μια σύμβαση έργου, χρησιμοποιείται η ακόλουθη σειρά προτεραιότητας για τον αυτόματο καθορισμό σχετικών τιμοκαταλόγων έργου:</span><span class="sxs-lookup"><span data-stu-id="d20e1-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="d20e1-124">Προσφορά</span><span class="sxs-lookup"><span data-stu-id="d20e1-124">Quote</span></span>
2. <span data-ttu-id="d20e1-125">Ευκαιρία</span><span class="sxs-lookup"><span data-stu-id="d20e1-125">Opportunity</span></span>
3. <span data-ttu-id="d20e1-126">Πελάτης</span><span class="sxs-lookup"><span data-stu-id="d20e1-126">Customer</span></span> 
4. <span data-ttu-id="d20e1-127">Καθολικές ρυθμίσεις</span><span class="sxs-lookup"><span data-stu-id="d20e1-127">Global settings</span></span> 

<span data-ttu-id="d20e1-128">Όταν ένας τιμοκατάλογος έργου καταχωρείται από προεπιλογή, το σύστημα επιβεβαιώνει ότι η νομισματική μονάδα αντιστοιχεί στη νομισματική μονάδα του πελάτη και ότι οι προεπιλεγμένοι τιμοκατάλογοι που έχουν εισαχθεί έχουν ένα περιβάλλον **Πωλήσεων**.</span><span class="sxs-lookup"><span data-stu-id="d20e1-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="d20e1-129">Μπορείτε να συσχετίσετε πολλούς τιμοκαταλόγους με τις οντότητες "πελάτης", "ευκαιρία", "προσφορά" και "σύμβαση έργου".</span><span class="sxs-lookup"><span data-stu-id="d20e1-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="d20e1-130">Αυτή η δυνατότητα υποστηρίζει τις προεπιλεγμένες τιμές που αφορούν συγκεκριμένες ημερομηνίες για μια μακροχρόνια σύμβαση έργου, όπου μπορείτε να απαιτήσετε περισσότερους από έναν τιμοκαταλόγους οι οποίοι θα ληφθούν υπόψη για ενημερώσεις σχετικά με τις τιμές που προκύπτουν λόγω πληθωρισμού.</span><span class="sxs-lookup"><span data-stu-id="d20e1-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="d20e1-131">Ωστόσο, εάν οι τιμοκατάλογοι που συσχετίζετε με την οντότητα "πελάτης", "ευκαιρία", "προσφορά" ή "σύμβαση έργου" έχουν επικαλυπτόμενη ισχύ ημερομηνίας οι προεπιλεγμένες τιμές μπορεί να είναι εσφαλμένες.</span><span class="sxs-lookup"><span data-stu-id="d20e1-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="d20e1-132">Επομένως, θα πρέπει να βεβαιωθείτε ότι οι τιμοκατάλογοι έργου που έχουν ισχύ ημερομηνίας επικάλυψης δεν σχετίζονται με αυτές τις οντότητες.</span><span class="sxs-lookup"><span data-stu-id="d20e1-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
