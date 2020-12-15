---
title: Δημιουργία λύσης για προσαρμοσμένες διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας λύσεων για προσαρμοσμένες διαστάσεις τιμολόγησης.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441501dff23d16960381b3f9fb4b2cceba2b3ba5
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513985"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="46d8f-103">Δημιουργία λύσης για προσαρμοσμένες διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="46d8f-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="46d8f-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="46d8f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="46d8f-105">Όλες οι αλλαγές διάστασης προσαρμοσμένων τιμών πρέπει να βρίσκονται σε ξεχωριστή λύση.</span><span class="sxs-lookup"><span data-stu-id="46d8f-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="46d8f-106">Αυτή η σημαντική βέλτιστη πρακτική επιτρέπει την ευελιξία ενημέρωσης ή κατάργησης αλλαγών όπου είναι απαραίτητο, με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αλλαγών σε άλλες παρουσίες.</span><span class="sxs-lookup"><span data-stu-id="46d8f-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="46d8f-107">Αφού πραγματοποιήσετε τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη** λύση και, έπειτα, εισαγάγετε σε άλλες παρουσίες, για επαναχρησιμοποίηση.</span><span class="sxs-lookup"><span data-stu-id="46d8f-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="46d8f-108">Δημιουργία λύσης για προσαρμοσμένες διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="46d8f-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="46d8f-109">Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και, στη συνέχεια, επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="46d8f-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="46d8f-110">Ονομάστε τη λύση, *διαστάσεις τιμολόγησης του <your organization name>*.</span><span class="sxs-lookup"><span data-stu-id="46d8f-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="46d8f-111">Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="46d8f-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![Δημιουργία λύσης διαστάσεων προσαρμοσμένης τιμολόγησης](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="46d8f-113">Προσθήκη όλων των απαιτούμενων οντοτήτων και σχετικών στοιχείων στη Λύση διάστασης τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="46d8f-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="46d8f-114">Προσθέστε τις παρακάτω οντότητες Project Service στη λύση τιμολόγησης για να κάνετε σημαντικές αλλαγές σχήματος στη λύση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="46d8f-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="46d8f-115">Αφού ολοκληρώσετε αυτήν τη διαδικασία, οι οντότητες θα αναγνωρίσουν τις νέες διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="46d8f-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="46d8f-116">Επιλέξτε **Ρυθμίσεις** > **Λύσεις** κι, έπειτα, κάντε διπλό κλικ στο **<*όνομα του οργανισμού σας*> διαστάσεις τιμολόγησης**.</span><span class="sxs-lookup"><span data-stu-id="46d8f-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="46d8f-117">Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Προσθήκη υπάρχουσας** > **Οντότητες**.</span><span class="sxs-lookup"><span data-stu-id="46d8f-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="46d8f-118">Στο παράθυρο διαλόγου **Στοιχεία λύσης**, επιλέξτε τις ακόλουθες οντότητες:</span><span class="sxs-lookup"><span data-stu-id="46d8f-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="46d8f-119">**Πραγματική**</span><span class="sxs-lookup"><span data-stu-id="46d8f-119">**Actual**</span></span>
   - <span data-ttu-id="46d8f-120">**Πόρος με δυνατότητα κράτησης**</span><span class="sxs-lookup"><span data-stu-id="46d8f-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="46d8f-121">**Γραμμή εκτίμησης**</span><span class="sxs-lookup"><span data-stu-id="46d8f-121">**Estimate Line**</span></span>
   - <span data-ttu-id="46d8f-122">**Εργασία έργου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-122">**Project Task**</span></span>
   - <span data-ttu-id="46d8f-123">**Λεπτομέρεια γραμμής τιμολογίου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="46d8f-124">**Γραμμή ημερολογίου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-124">**Journal Line**</span></span>
   - <span data-ttu-id="46d8f-125">**Λεπτομέρεια γραμμής σύμβασης έργου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="46d8f-126">**Μέλος ομάδας έργου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-126">**Project Team Member**</span></span>
   - <span data-ttu-id="46d8f-127">**Λεπτομέρειες γραμμής προσφοράς**</span><span class="sxs-lookup"><span data-stu-id="46d8f-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="46d8f-128">**Αύξηση τιμής ρόλου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="46d8f-129">**Τιμή ρόλου**</span><span class="sxs-lookup"><span data-stu-id="46d8f-129">**Role Price**</span></span>
   - <span data-ttu-id="46d8f-130">**Χρονική καταχώρηση**</span><span class="sxs-lookup"><span data-stu-id="46d8f-130">**Time Entry**</span></span>
 
   ![Προσθήκη λύσης διαστάσεων προσαρμοσμένης τιμολόγησης υπαρχουσών οντοτήτων](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="46d8f-132">Για κάθε οντότητα, εξετάστε τα στοιχεία που προστίθενται και την τελική λίστα των πάγιων στοιχείων μιας οντότητας για κάθε οντότητα.</span><span class="sxs-lookup"><span data-stu-id="46d8f-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="46d8f-133">Συμπεριλάβετε όλες τις φόρμες και τις προβολές για καθεμία από τις επιλεγμένες οντότητες.</span><span class="sxs-lookup"><span data-stu-id="46d8f-133">Include all forms and views for each of the selected entities.</span></span>

  ![Οντότητες που προστέθηκαν](./media/solution-component-selection.png)


5.  <span data-ttu-id="46d8f-135">Όταν σας ζητηθεί να συμπεριλάβετε εξαρτημένες οντότητες για τις επιλεγμένες οντότητες, επιλέξτε **Όχι, να μην συμπεριληφθούν τα απαιτούμενα στοιχεία.**</span><span class="sxs-lookup"><span data-stu-id="46d8f-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![Συμπερίληψη εξαρτημένων οντοτήτων](./media/Do-not-include-required.png)
