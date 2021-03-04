---
title: Κλείσιμο μιας προσφοράς - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το κλείσιμο προσφορών στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8d387816f51f63ecd95df6534c7c012b323e6ddc
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764864"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="91ad9-103">Κλείσιμο μιας προσφοράς - lite</span><span class="sxs-lookup"><span data-stu-id="91ad9-103">Close a quote - lite</span></span>

<span data-ttu-id="91ad9-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="91ad9-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="91ad9-105">Μια προσφορά έργου μπορεί να κλείσει ως κερδισμένη ή χαμένη.</span><span class="sxs-lookup"><span data-stu-id="91ad9-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="91ad9-106">Ένα προσχέδιο προσφοράς μπορεί να κλείσει, επειδή οι λειτουργίες ενεργοποίησης και αναθεώρησης σε προσφορές δεν υποστηρίζονται στο Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="91ad9-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="91ad9-107">Κλείσιμο μιας προσφοράς ως κερδισμένης</span><span class="sxs-lookup"><span data-stu-id="91ad9-107">Close a quote as Won</span></span>

<span data-ttu-id="91ad9-108">Όταν κλείνετε μια προσφορά έργου ως κερδισμένη, η κατάσταση ορίζεται σε Κλειστή και η αιτιολογία κατάστασης είναι Κερδισμένη.</span><span class="sxs-lookup"><span data-stu-id="91ad9-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="91ad9-109">Το κλείσιμο των προσφορών τις καθιστά μόνο για ανάγνωση και δημιουργείται ένα προσχέδιο σύμβασης έργου με όλες τις πληροφορίες προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="91ad9-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="91ad9-110">Επειδή δεν είναι δυνατό το άνοιγμα μιας κλειστής προσφοράς, ένα παράθυρο διαλόγου επιβεβαίωσης θα επιβεβαιώσει τις αλλαγές σας.</span><span class="sxs-lookup"><span data-stu-id="91ad9-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="91ad9-111">Εάν η προσφορά είναι συνημμένη σε μια ευκαιρία, οποιεσδήποτε άλλες προσφορές έργου στην ευκαιρία κλείνουν αυτόματα ως χαμένες.</span><span class="sxs-lookup"><span data-stu-id="91ad9-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="91ad9-112">Οικονομικός αντίκτυπος του κλεισίματος μιας προσφοράς ως κερδισμένης</span><span class="sxs-lookup"><span data-stu-id="91ad9-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="91ad9-113">Εάν υπάρχουν πραγματικές τιμές για το χρόνο σε ένα έργο, ενώ εξακολουθεί να είναι συνημμένες σε ένα προσχέδιο προσφοράς, καταγράφεται μόνο το κόστος του χρόνου ή των δαπανών.</span><span class="sxs-lookup"><span data-stu-id="91ad9-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="91ad9-114">Αφού κλείσει μια προσφορά ως κερδισμένη, η εφαρμογή θα επαναφέρει το κόστος αντιστρέφοντας τα παλιότερα πραγματικά δεδομένα κόστους και θα δημιουργήσει εκ νέου νέες πραγματικές τιμές κόστους.</span><span class="sxs-lookup"><span data-stu-id="91ad9-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="91ad9-115">Η εφαρμογή θα επεξεργαστεί αυτά τα πραγματικά δεδομένα κόστους με βάση τη μέθοδο χρέωσης της συσχετισμένης γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="91ad9-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="91ad9-116">Εάν οι πραγματικές τιμές κόστους αναφέρονται σε μια γραμμή σύμβασης χρόνου και υλικού, οι αντίστοιχες πραγματικές τιμές των πωλήσεων χωρίς χρέωση δημιουργούνται για το κλείσιμο της προσφοράς και τη δημιουργία της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="91ad9-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="91ad9-117">Εάν οι πραγματικές τιμές κόστους αναφέρονται σε μια γραμμή σύμβασης προκαθορισμένης τιμής, η εφαρμογή θα σταματήσει την επανεπεξεργασία των πραγματικών τιμών κόστους που βασίζονται στους κανόνες διαίρεσης χρέωσης για τους πελάτες της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="91ad9-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="91ad9-118">Κλείσιμο μιας προσφοράς ως χαμένης:</span><span class="sxs-lookup"><span data-stu-id="91ad9-118">Closing a quote as lost:</span></span>

<span data-ttu-id="91ad9-119">Όταν κλείνετε μια προσφορά έργου ως χαμένη, η κατάσταση ορίζεται σε Κλειστή και η αιτιολογία κατάστασης είναι Χαμένη.</span><span class="sxs-lookup"><span data-stu-id="91ad9-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="91ad9-120">Εάν κλείσετε την προσφορά, η προσφορά έργου θα είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="91ad9-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="91ad9-121">Επειδή δεν είναι δυνατό το άνοιγμα μιας κλειστής προσφοράς, πριν κλείσετε μια προσφορά, το παράθυρο διαλόγου επιβεβαίωσης θα επιβεβαιώσει τις αλλαγές σας.</span><span class="sxs-lookup"><span data-stu-id="91ad9-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="91ad9-122">Εάν η προσφορά έργου που κλείνει ως Χαμένη αναφέρεται σε ένα έργο σε οποιαδήποτε από τις γραμμές του, αυτό το έργο επισημαίνεται επίσης ως Κλειστό.</span><span class="sxs-lookup"><span data-stu-id="91ad9-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="91ad9-123">Οι κρατήσεις πόρων από εκείνη την ημέρα και μετά ακυρώνονται.</span><span class="sxs-lookup"><span data-stu-id="91ad9-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="91ad9-124">Στο Project Operations, η κλείσιμο μιας προσφοράς ως κερδισμένης ή χαμένης δεν θα επηρεάσει την εν λόγω κατάσταση της ευκαιρίας, η οποία θα παραμείνει ανοιχτή μέχρι να κλείσει με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="91ad9-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
