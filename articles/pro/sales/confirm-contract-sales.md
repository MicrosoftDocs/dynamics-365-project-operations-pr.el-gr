---
title: Επιβεβαίωση σύμβασης έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο επιβεβαίωσης μιας σύμβασης στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: babce9c64098a9c87072786d914d2340251a8986
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077036"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="1bdfe-103">Επιβεβαίωση σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="1bdfe-103">Confirm a project contract</span></span>

<span data-ttu-id="1bdfe-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1bdfe-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1bdfe-105">Μια σύμβαση έργου στο Dynamics 365 Project Operations μπορεί να είναι ενεργή με αιτία **Επιβεβαιώθηκε** ή να έχει κλείσει με αιτία **Χάθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed** , or closed with a reason of **Lost**.</span></span> <span data-ttu-id="1bdfe-106">Όταν επιβεβαιώνετε μια σύμβαση έργου, οι καταστάσεις ενημερώνονται από **Προσχέδιο** σε **Ενεργό** και η αιτιολογία κατάστασης είναι **Επιβεβαιώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="1bdfe-107">Δεν είναι δυνατή η επεξεργασία ή το εκ νέου άνοιγμα μιας ενεργής ή κλειστής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="1bdfe-108">Δημοσιονομικές επιπτώσεις από την επιβεβαίωση μιας σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="1bdfe-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="1bdfe-109">Αφού επιβεβαιωθεί μια σύμβαση έργου, η εφαρμογή υπολογίζει ξανά τα κόστη αντιστρέφοντας τα παλιότερα πραγματικά δεδομένα κόστους και δημιουργώντας νέες πραγματικές τιμές κόστους.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="1bdfe-110">Οι νέες πραγματικές τιμές κόστους τίθενται σε επεξεργασία με βάση τη μέθοδο χρέωσης της συσχετισμένης γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="1bdfe-111">Εάν η αναφορά πραγματικών τιμών κόστους είναι μια γραμμή σύμβασης χρόνου και υλικού, η εφαρμογή δημιουργεί εκ νέου αυτόματα τις αντίστοιχες πραγματικές τιμές μη τιμολογημένων πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="1bdfe-112">Εάν οι πραγματικές τιμές κόστους αναφέρουν μια γραμμή σύμβασης προκαθορισμένης τιμής, η εφαρμογή διακόπτει την επεξεργασία των πραγματικών τιμών κόστους.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="1bdfe-113">Τα όρια μη υπέρβασης, η ρύθμιση χρεωσιμότητας και η τιμολόγηση και η κοστολόγηση των πραγματικών τιμών αξιολογούνται και, στη συνέχεια, ενημερώνονται ως μέρος της διεργασίας των επιβεβαιώσεων.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="1bdfe-114">Κλείσιμο σύμβασης έργου ως χαμένη</span><span class="sxs-lookup"><span data-stu-id="1bdfe-114">Close a project contract as lost</span></span>

<span data-ttu-id="1bdfe-115">Όταν κλείνετε μια σύμβαση έργου ως χαμένη, η κατάσταση της σύμβασης ενημερώνεται σε **Κλειστή** και η αιτιολογία κατάστασης είναι **Χαμένη**.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="1bdfe-116">Η σύμβαση έργου γίνεται μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-116">The project contract becomes read-only.</span></span> <span data-ttu-id="1bdfe-117">Ένα παράθυρο διαλόγου επιβεβαίωσης παρέχεται πριν ολοκληρωθούν οι αλλαγές, επειδή δεν μπορείτε να ανοίξετε εκ νέου μια κλειστή σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="1bdfe-118">Εάν η σύμβαση έργου που έχει κλείσει ως χαμένη αναφέρει ένα έργο στις γραμμές της, αυτό το έργο επισημαίνεται επίσης ως κλειστό.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="1bdfe-119">Οι κρατήσεις πόρων από εκείνη την ημέρα και μετά ακυρώνονται.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="1bdfe-120">Οι πραγματικές τιμές μη τιμολογημένων πωλήσεων στη σύμβαση έργου που δεν βρίσκονται ήδη σε ένα τιμολόγιο, θα αντιστραφούν.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="1bdfe-121">Στο Dynamics 365 Project Operations, το κλείσιμο μιας σύμβασης έργου ως χαμένης δεν θα επηρεάσει την εν λόγω κατάσταση της συσχετισμένης ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="1bdfe-122">Η ευκαιρία θα παραμείνει ανοιχτή και πρέπει να κλείσει με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-122">The opportunity will remain open and must be manually closed.</span></span>