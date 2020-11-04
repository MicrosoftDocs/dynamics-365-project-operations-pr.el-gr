---
title: Δημιουργία προσαρμοσμένων λύσεων για διαστάσεις τιμολόγησης
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας μιας προσαρμοσμένης λύσης κατά τη δημιουργία προσαρμοσμένων διαστάσεων τιμολόγησης.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3e437fce5b9f1fb330a713788e24100a4fe02948
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076925"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="cb973-103">Δημιουργία προσαρμοσμένων λύσεων για διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="cb973-103">Create custom solutions for pricing dimensions</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cb973-104">Όλες οι αλλαγές διάστασης προσαρμοσμένων τιμών πρέπει να βρίσκονται σε ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="cb973-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="cb973-105">Αυτή η σημαντική βέλτιστη πρακτική παρέχει την ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο, θα σας βοηθήσει με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία.</span><span class="sxs-lookup"><span data-stu-id="cb973-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="cb973-106">Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη λύση** και εισαγάγετέ την σε άλλες παρουσίες, για να επαναχρησιμοποιήσετε την ρύθμιση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="cb973-106">After you make the required changes, export this solution as a **Managed solution** , and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="cb973-107">Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και, στη συνέχεια, επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="cb973-107">Select **Settings** > **Solutions** , and then select **New**.</span></span> 
2. <span data-ttu-id="cb973-108">Ονομάστε τη λύση, **\<your organization name> διαστάσεις τιμολόγησης** , καταχωρίστε τις υπόλοιπες πληροφορίες και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="cb973-108">Name the solution, **\<your organization name> pricing dimensions** , enter the remaining required information, and then select **Save**.</span></span>

> ![Δημιουργία προσαρμοσμένης λύσης για διαστάσεις τιμολόγησης](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="cb973-110">Προσθήκη όλων των απαιτούμενων οντοτήτων και σχετικών στοιχείων στη Λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="cb973-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="cb973-111">Θα πρέπει να προσθέσετε τις παρακάτω οντότητες Project Service στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="cb973-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="cb973-112">Ολοκληρώστε τα βήματα σε αυτήν τη διαδικασία για να κάνετε κάποιες σημαντικές αλλαγές σχήματος στη λύση τιμολόγησης, έτσι ώστε οι οντότητες να συνειδητοποιήσουν τις νέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="cb973-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="cb973-113">Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="cb973-113">Select **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="cb973-114">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Προσθήκη υπάρχουσας** > **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="cb973-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="cb973-115">Στο παράθυρο διαλόγου **Στοιχεία λύσης** , επιλέξτε τις ακόλουθες οντότητες:</span><span class="sxs-lookup"><span data-stu-id="cb973-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="cb973-116">Πραγματική</span><span class="sxs-lookup"><span data-stu-id="cb973-116">Actual</span></span>
- <span data-ttu-id="cb973-117">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="cb973-117">Bookable Resource</span></span>
- <span data-ttu-id="cb973-118">Γραμμή εκτίμησης</span><span class="sxs-lookup"><span data-stu-id="cb973-118">Estimate Line</span></span>
- <span data-ttu-id="cb973-119">Εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="cb973-119">Project Task</span></span>
- <span data-ttu-id="cb973-120">Λεπτομέρεια γραμμής τιμολογίου</span><span class="sxs-lookup"><span data-stu-id="cb973-120">Invoice Line Detail</span></span>
- <span data-ttu-id="cb973-121">Γραμμή ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="cb973-121">Journal Line</span></span>
- <span data-ttu-id="cb973-122">Λεπτομέρεια γραμμής σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="cb973-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="cb973-123">Μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="cb973-123">Project Team Member</span></span>
- <span data-ttu-id="cb973-124">Λεπτομέρειες γραμμής προσφοράς</span><span class="sxs-lookup"><span data-stu-id="cb973-124">Quote Line Detail</span></span>
- <span data-ttu-id="cb973-125">Αύξηση τιμής ρόλου</span><span class="sxs-lookup"><span data-stu-id="cb973-125">Role Price Markup</span></span>
- <span data-ttu-id="cb973-126">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="cb973-126">Role Price</span></span> 
- <span data-ttu-id="cb973-127">Χρονική καταχώρηση</span><span class="sxs-lookup"><span data-stu-id="cb973-127">Time Entry</span></span> 

> ![Προσθήκη υπαρχουσών οντοτήτων στη λύση "διαστάσεις τιμολόγησης"](media/Existing-entities-to-PD-solution.png)

> ![Επιλέξτε στοιχεία λύσης](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="cb973-130">Βεβαιωθείτε ότι θα συμπεριλάβετε όλες τις φόρμες και τις προβολές για κάθε μια από τις οντότητες που επιλέγονται.</span><span class="sxs-lookup"><span data-stu-id="cb973-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="cb973-131">Όταν σας ζητηθεί να συμπεριλάβετε εξαρτημένες οντότητες για τις επιλεγμένες οντότητες, επιλέξτε **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="cb973-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Να μην συμπεριληφθούν όλα τα απαιτούμενα στοιχεία.](media/Do-not-include-required.png)


