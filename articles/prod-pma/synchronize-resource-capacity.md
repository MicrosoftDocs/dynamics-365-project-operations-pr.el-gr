---
title: Συγχρονισμός παραγωγικής ικανότητας πόρου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο συγχρονισμού της παραγωγικής ικανότητας ενός πόρου σε ημερολόγια και έργα.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e6b63ccb5b0f04dedb8a942e22d6e1993204dc20
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288560"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="21b36-103">Συγχρονισμός παραγωγικής ικανότητας πόρου</span><span class="sxs-lookup"><span data-stu-id="21b36-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="21b36-104">Οι διαδικασίες για τον συγχρονισμό των πόρων εγγυώνται ότι οι πληροφορίες για το ημερολόγιο και το ημερολόγιο βάσης θα μετατραπούν σε προγραμματισμό πόρων έργου.</span><span class="sxs-lookup"><span data-stu-id="21b36-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="21b36-105">Εάν γίνει αλλαγή του ημερολογίου, οι διεργασίες κάνουν τις απαιτούμενες ενημερώσεις στον προγραμματισμό των πόρων έργου.</span><span class="sxs-lookup"><span data-stu-id="21b36-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="21b36-106">Επίσης, οι διαδικασίες βοηθούν στη βελτίωση των επιδόσεων, επειδή οι πληροφορίες πόρου του ημερολογίου συγχρονίζονται εκ των προτέρων.</span><span class="sxs-lookup"><span data-stu-id="21b36-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="21b36-107">Ως εκ τούτου, οι ενημερώσεις των πληροφοριών προγραμματισμού πόρων εμφανίζονται πιο γρήγορα.</span><span class="sxs-lookup"><span data-stu-id="21b36-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="21b36-108">Συνιστούμε να προγραμματίζετε τις διεργασίες ομαδικά δέσμες αντί για μία κάθε φορά.</span><span class="sxs-lookup"><span data-stu-id="21b36-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="21b36-109">Διαφορετικά, υπάρχει ο κίνδυνος να ξεχάσει κάποιος τις ημερομηνίες χωρίς αποκλεισμούς, όταν οι πληροφορίες συγχρονίστηκαν για τελευταία φορά.</span><span class="sxs-lookup"><span data-stu-id="21b36-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="21b36-110">Εάν δεν χρησιμοποιηθούν ημερομηνίες χωρίς αποκλεισμούς, ενδέχεται να προκύψουν κενά κατά το συγχρονισμό ημερομηνιών.</span><span class="sxs-lookup"><span data-stu-id="21b36-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![Συγχρονισμός ημερολογίου](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="21b36-112">Συγχρονισμός συναθροίσεων παραγωγικής ικανότητας πόρου</span><span class="sxs-lookup"><span data-stu-id="21b36-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="21b36-113">Η διαδικασία συγχρονισμού έχει σχεδιαστεί για το συγχρονισμό όλων των πληροφοριών του ημερολογίου πόρου.</span><span class="sxs-lookup"><span data-stu-id="21b36-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="21b36-114">Αυτές οι πληροφορίες περιλαμβάνουν πληροφορίες βασικού ημερολογίου σχετικά με τυχόν αλλαγές στον πίνακα παραγωγικής ικανότητας ημερολογίου πόρου του έργου.</span><span class="sxs-lookup"><span data-stu-id="21b36-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="21b36-115">Εάν προστεθούν νέοι πόροι στο έργο, ο συγχρονισμός εγγυάται ότι οι πληροφορίες του ενημερωμένου ημερολογίου είναι διαθέσιμες.</span><span class="sxs-lookup"><span data-stu-id="21b36-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="21b36-116">Αυτός ο συγχρονισμός μπορεί να γίνει οποιαδήποτε στιγμή.</span><span class="sxs-lookup"><span data-stu-id="21b36-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="21b36-117">Συνιστούμε να χρησιμοποιήσετε μια ομάδα.</span><span class="sxs-lookup"><span data-stu-id="21b36-117">We recommend that you use a batch.</span></span> <span data-ttu-id="21b36-118">Οι επιλογές είναι διαθέσιμες κατά το συγχρονισμό των δεσμεύσεων παραγωγικής ικανότητας.</span><span class="sxs-lookup"><span data-stu-id="21b36-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="21b36-119">Επιλέξτε **Διαχείριση έργου και λογιστικής** &gt; **Περιοδικός** &gt; **Συγχρονισμός παραγωγικής ικανότητας** &gt; **Συγχρονισμός συναθροίσεων παραγωγικής ικανότητας πόρων**.</span><span class="sxs-lookup"><span data-stu-id="21b36-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="21b36-120">Ορίστε τις επιλογές στον πίνακα που ακολουθεί.</span><span class="sxs-lookup"><span data-stu-id="21b36-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="21b36-121">Επιλογή</span><span class="sxs-lookup"><span data-stu-id="21b36-121">Option</span></span>      | <span data-ttu-id="21b36-122">Περιγραφή</span><span class="sxs-lookup"><span data-stu-id="21b36-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="21b36-123">Κωδικός περιόδου</span><span class="sxs-lookup"><span data-stu-id="21b36-123">Period code</span></span> | <span data-ttu-id="21b36-124">Προαιρετικά, επιλέξτε τον κωδικό χρονικού διαστήματος ημερομηνιών γενικής λογιστικής για να ορίσετε τις ημερομηνίες έναρξης και λήξης για τη διαδικασία συγχρονισμού για τις συναθροίσεις παραγωγικής ικανότητας πόρων.</span><span class="sxs-lookup"><span data-stu-id="21b36-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="21b36-125">Ημερομηνία έναρξης</span><span class="sxs-lookup"><span data-stu-id="21b36-125">Start date</span></span>  | <span data-ttu-id="21b36-126">Καταγράψτε την ημερομηνία έναρξης για τη διαδικασία συγχρονισμού για τις συναθροίσεις παραγωγικής ικανότητας πόρων.</span><span class="sxs-lookup"><span data-stu-id="21b36-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="21b36-127">Ημερομηνία λήξης</span><span class="sxs-lookup"><span data-stu-id="21b36-127">End date</span></span>    | <span data-ttu-id="21b36-128">Καταγράψτε την ημερομηνία λήξης για τη διαδικασία συγχρονισμού για τις συναθροίσεις παραγωγικής ικανότητας πόρων.</span><span class="sxs-lookup"><span data-stu-id="21b36-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="21b36-129">[![Διαδικασία συγχρονισμού](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="21b36-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]