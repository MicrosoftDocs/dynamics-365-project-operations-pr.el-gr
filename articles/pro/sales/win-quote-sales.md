---
title: Κλείσιμο μιας προσφοράς - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το κλείσιμο προσφορών στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ad206232d616cdbdc83e2a17b9177cfb98ffda9
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175711"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="1e4af-103">Κλείσιμο μιας προσφοράς - lite</span><span class="sxs-lookup"><span data-stu-id="1e4af-103">Close a quote - lite</span></span>

<span data-ttu-id="1e4af-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1e4af-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1e4af-105">Μια προσφορά έργου μπορεί να κλείσει ως κερδισμένη ή χαμένη.</span><span class="sxs-lookup"><span data-stu-id="1e4af-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="1e4af-106">Οι λειτουργίες ενεργοποίησης και αναθεώρησης δεν υποστηρίζονται σε προσφορές στο Microsoft Dynamics 365 Project Operations έτσι μπορείτε να κλείσετε μια προσχέδια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="1e4af-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="1e4af-107">Κλείσιμο μιας προσφοράς ως κερδισμένης</span><span class="sxs-lookup"><span data-stu-id="1e4af-107">Close a quote as Won</span></span>

<span data-ttu-id="1e4af-108">Το κλείσιμο μιας προσφοράς έργου ως κερδισμένης θα κλείσει την προσφορά με κατάσταση Κλειστή και αιτιολογία κατάστασης θα είναι Κερδισμένη.</span><span class="sxs-lookup"><span data-stu-id="1e4af-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="1e4af-109">Το κλείσιμο των προσφορών τις καθιστά μόνο για ανάγνωση και δημιουργείται ένα προσχέδιο σύμβασης έργου με όλες τις πληροφορίες προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="1e4af-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="1e4af-110">Επειδή μια κλειστή προσφορά δεν είναι δυνατό να ξανανοίξει, ένα παράθυρο διαλόγου επιβεβαίωσης υπάρχει για να μπορέσουν να γίνουν οι αλλαγές αφού δεν είναι δυνατό το η εκ νέου άνοιγμα μιας κλειστής προσφοράς και οι αλλαγές δεν είναι αναστρέψιμες.</span><span class="sxs-lookup"><span data-stu-id="1e4af-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="1e4af-111">Εάν η προσφορά είναι συνημμένη σε μια ευκαιρία, οποιεσδήποτε άλλες προσφορές έργου στην ευκαιρία κλείνουν αυτόματα ως χαμένες.</span><span class="sxs-lookup"><span data-stu-id="1e4af-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="1e4af-112">Οικονομικός αντίκτυπος του κλεισίματος μιας προσφοράς ως κερδισμένης</span><span class="sxs-lookup"><span data-stu-id="1e4af-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="1e4af-113">Εάν έχουν σημειωθεί πραγματικές τιμές για το χρόνο που καταγράφηκε σε ένα έργο ενώ εξακολουθεί να είναι προσαρτημένο σε ένα προσχέδιο προσφοράς, καταγράφεται μόνο το κόστος του χρόνου ή της δαπάνης.</span><span class="sxs-lookup"><span data-stu-id="1e4af-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="1e4af-114">Αφού κλείσει μια προσφορά ως κερδισμένη, η εφαρμογή θα επαναφέρει το κόστος αντιστρέφοντας τα παλιότερα πραγματικά δεδομένα κόστους και θα δημιουργήσει εκ νέου νέες πραγματικές τιμές κόστους.</span><span class="sxs-lookup"><span data-stu-id="1e4af-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="1e4af-115">Η εφαρμογή θα επεξεργαστεί αυτά τα πραγματικά δεδομένα κόστους με βάση τη μέθοδο χρέωσης της συσχετισμένης γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="1e4af-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="1e4af-116">Εάν ο κωδικός κόστους αναφέρεται σε μια γραμμή σύμβασης χρόνου και υλικού, το σύστημα θα δημιουργήσει αυτόματα τα αντίστοιχα πραγματικά ποσά που δεν έχουν τιμολογηθεί για την ημερομηνία κλεισίματος της προσφοράς και τη δημιουργία της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="1e4af-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="1e4af-117">Εάν ο κωδικός κόστους αναφέρεται σε μια γραμμή σύμβασης προκαθορισμένης τιμής, η εφαρμογή θα σταματήσει την επεξεργασία των πραγματικών τιμών κόστους με βάση τους κανόνες διαίρεσης χρέωσης για τους πελάτες της σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="1e4af-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="1e4af-118">Κλείσιμο μιας προσφοράς ως χαμένης:</span><span class="sxs-lookup"><span data-stu-id="1e4af-118">Closing a quote as lost:</span></span>

<span data-ttu-id="1e4af-119">Το κλείσιμο μιας προσφοράς έργου ως χαμένης θα ορίσει την κατάσταση της προσφοράς σε Κλειστή και αιτιολογία κατάστασης θα είναι Χαμένη.</span><span class="sxs-lookup"><span data-stu-id="1e4af-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="1e4af-120">Εάν κλείσετε την προσφορά, η προσφορά έργου θα είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="1e4af-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="1e4af-121">Επειδή δεν είναι δυνατό το άνοιγμα μιας κλειστής προσφοράς, πριν κλείσετε μια προσφορά, το παράθυρο διαλόγου επιβεβαίωσης θα επιβεβαιώσει τις αλλαγές σας.</span><span class="sxs-lookup"><span data-stu-id="1e4af-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="1e4af-122">Εάν η προσφορά έργου που έχει κλείσει ως χαμένη έχει ένα έργο που αναφέρεται σε οποιαδήποτε από τις γραμμές του, αυτό το έργο επισημαίνεται επίσης ως κλειστό και οι κρατήσεις πόρων από εκείνη την ημέρα και μετά ακυρώνονται.</span><span class="sxs-lookup"><span data-stu-id="1e4af-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="1e4af-123">Στο Project Operations, η κλείσιμο μιας προσφοράς ως κερδισμένης ή χαμένης δεν θα επηρεάσει την εν λόγω κατάσταση της ευκαιρίας, η οποία θα παραμείνει ανοιχτή μέχρι να κλείσει με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="1e4af-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
