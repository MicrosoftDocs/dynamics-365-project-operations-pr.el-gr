---
title: Απενεργοποίηση τιμοκαταλόγων
description: Αυτό θέμα εξηγεί τον τρόπο απενεργοποίησης ή κατάργησης των μη χρησιμοποιούμενων ή παλιών τιμοκαταλόγων.
author: rumant
manager: AnnBe
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3fa902e93815002be7d6915880cd7759dbbde5ef
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701934"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="76228-103">Απενεργοποίηση τιμοκαταλόγων</span><span class="sxs-lookup"><span data-stu-id="76228-103">Deactivate price lists</span></span> 

<span data-ttu-id="76228-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="76228-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="76228-105">Για να καταργήσετε παλιούς ή αχρησιμοποίητους τιμοκατακλόγους από το Dynamics 365 Project Operations, πρέπει να ολοκληρώσετε δύο βήματα.</span><span class="sxs-lookup"><span data-stu-id="76228-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="76228-106">Καταργήστε ή διαγράψτε τον τιμοκατάλογο από συγκεκριμένες σελίδες.</span><span class="sxs-lookup"><span data-stu-id="76228-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="76228-107">Απενεργοποιήστε ή διαγράψτε τον τιμοκατάλογο από τους ενεργούς τιμοκαταλόγους στη σελίδα **Τιμοκατάλογοι**.</span><span class="sxs-lookup"><span data-stu-id="76228-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="76228-108">Πρέπει να ολοκληρώσετε και τα δύο βήματα για να καταργήσετε πλήρως έναν τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="76228-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="76228-109">Δεν αρκεί μόνο η εκτέλεση του βήματος 2, το οποίο είναι η άμεση διαγραφή ή απενεργοποίηση του τιμοκαταλόγου από την προβολή "Ενεργοί τιμοκατάλογοι".</span><span class="sxs-lookup"><span data-stu-id="76228-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="76228-110">Πρέπει επίσης να διαγράψετε τη συσχέτιση αυτού του τιμοκαταλόγου από όλα τα σημεία που αναφέρονται στο βήμα 1.</span><span class="sxs-lookup"><span data-stu-id="76228-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="76228-111">Διαγράψτε τον τιμοκατάλογο από συγκεκριμένες σελίδες</span><span class="sxs-lookup"><span data-stu-id="76228-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="76228-112">Για να διαγράψετε έναν τιμοκατάλογο από το Project Operations, μεταβείτε στις ακόλουθες σελίδες:</span><span class="sxs-lookup"><span data-stu-id="76228-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="76228-113">Σελίδα **παράμετροι έργου** > καρτέλα **Τιμοκατάλογοι**</span><span class="sxs-lookup"><span data-stu-id="76228-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="76228-114">Σελίδα **Οργανωτική μονάδα** > πλέγμα **Τιμοκατάλογοι**</span><span class="sxs-lookup"><span data-stu-id="76228-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="76228-115">Σελίδα **Λογαριασμός** > πλέγμα **Τιμοκατάλογοι έργου**</span><span class="sxs-lookup"><span data-stu-id="76228-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="76228-116">Σελίδα **Προσφορές έργου** > πλέγμα **Τιμοκατάλογοι έργου**: αυτό ισχύει για όλες τις ενεργές προσφορές έργου.</span><span class="sxs-lookup"><span data-stu-id="76228-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="76228-117">Σελίδα **Συμβάσεις έργου** > πλέγμα **Τιμοκατάλογοι έργου**: αυτό ισχύει για όλες τις ενεργές συμβάσεις έργου.</span><span class="sxs-lookup"><span data-stu-id="76228-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="76228-118">Για κάθε σελίδα, πρέπει να επιλέξετε τον τιμοκατάλογο που θέλετε να διαγράψετε και, στη συνέχεια, να επιλέξετε **Διαγραφή**.</span><span class="sxs-lookup"><span data-stu-id="76228-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="76228-119">Διαγράψτε ή απενεργοποιήστε τον τιμοκατάλογο από τη σελίδα "Τιμοκατάλογοι"</span><span class="sxs-lookup"><span data-stu-id="76228-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="76228-120">Για να διαγράψετε έναν τιμοκατάλογο από τους ενεργούς τιμοκαταλόγους, μεταβείτε στην επιλογή **Πωλήσεις** > **Πελάτες** > **Τιμοκατάλογοι**.</span><span class="sxs-lookup"><span data-stu-id="76228-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="76228-121">Αναζητήστε τον τιμοκατάλογο που θέλετε να διαγράψετε και, έπειτα, επιλέξτε **Διαγραφή**.</span><span class="sxs-lookup"><span data-stu-id="76228-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="76228-122">Αν ο τιμοκατάλογος αναφέρεται σε οποιεσδήποτε υπάρχουσες συναλλαγές, δεν θα μπορείτε να τον διαγράψετε.</span><span class="sxs-lookup"><span data-stu-id="76228-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="76228-123">Εάν συμβεί αυτό, μπορείτε να απενεργοποιήσετε τον τιμοκατάλογο, ώστε να μην εμφανίζεται σε καμία από τις προβολές.</span><span class="sxs-lookup"><span data-stu-id="76228-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="76228-124">Για να απενεργοποιήσετε τον τιμοκατάλογο, επιλέξτε ξανά τον τιμοκατάλογο και, στη συνέχεια, επιλέξτε **Απενεργοποίηση**.</span><span class="sxs-lookup"><span data-stu-id="76228-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
