---
title: Δημιουργήστε έναν τιμοκατάλογο
description: Πώς γίνεται η δημιουργία τιμοκαταλόγου στο Project Service
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0732ccca43e404412efae8a91873e43c28d041ca
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290314"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="8d076-103">Δημιουργία τιμοκαταλόγου (Project Service)</span><span class="sxs-lookup"><span data-stu-id="8d076-103">Create a price list (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="8d076-104">Οι τιμοκατάλογοι παρέχουν ένα πρότυπο, το οποίο μπορούν να χρησιμοποιήσουν οι υπεύθυνοι λογαριασμού σας για τη δημιουργία προσφορών και έργων, καθώς και για τον καθορισμό του κόστους ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="8d076-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="8d076-105">Παρέχουν μια λίστα στοιχείων γραμμής ρόλων και εξόδων, καθώς και την τιμή που θα χρεώνετε για καθένα από αυτά.</span><span class="sxs-lookup"><span data-stu-id="8d076-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="8d076-106">Μπορείτε να δημιουργήσετε πολλαπλούς τιμοκαταλόγους ώστε να έχετε τη δυνατότητα να διατηρείτε ξεχωριστές δομές τιμών για διαφορετικές περιοχές όπου πουλάτε τα προϊόντα σας ή κανάλια πώλησης.</span><span class="sxs-lookup"><span data-stu-id="8d076-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="8d076-107">Είναι καλή ιδέα να δημιουργήσετε τουλάχιστον έναν τιμοκατάλογο για κάθε νομισματική μονάδα στην οποία σκοπεύετε να χρεώσετε τους πελάτες σας.</span><span class="sxs-lookup"><span data-stu-id="8d076-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="8d076-108">Για τη δημιουργία οικονομικών εκτιμήσεων για την εργασία που πρέπει να παραδοθεί, βεβαιωθείτε ότι όλα τα έργα έχουν υποστηρικτικό τιμοκατάλογο κόστους και πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="8d076-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="8d076-109">Ορίστε έναν προκαθορισμένο τιμοκατάλογο κόστους και πωλήσεων, ο οποίος θα ισχύει για όλα τα έργα που δημιουργούνται στον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="8d076-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="8d076-110">Οι τιμοκατάλογοι βασίζονται σε κατηγορίες ρόλων και εξόδων, επομένως πριν δημιουργήσετε έναν τιμοκατάλογο, βεβαιωθείτε ότι έχετε ήδη ρυθμίσει τις παραμέτρους των κατηγοριών των ρόλων και των εξόδων που θέλετε να χρησιμοποιήσετε κατά τη δημιουργία του τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="8d076-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="8d076-111">Μεταβείτε στο μενού **Project Service > Τιμοκατάλογοι**.</span><span class="sxs-lookup"><span data-stu-id="8d076-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="8d076-112">Επιλέξτε **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="8d076-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="8d076-113">Στο πεδίο **Πλαίσιο**, επιλέξτε αν ο τιμοκατάλογος θα αφορά τα στοιχεία **Κόστος**, **Αγορά** ή **Πωλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="8d076-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="8d076-114">Στο πεδίο **Όνομα**, πληκτρολογήστε ένα όνομα για τον τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="8d076-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="8d076-115">Στο πεδίο **Νομισματική μονάδα**, επιλέξτε τη νομισματική μονάδα που πρόκειται να χρησιμοποιήσετε για τη χρέωση και την κοστολόγηση.</span><span class="sxs-lookup"><span data-stu-id="8d076-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="8d076-116">Στο πεδίο **Χρονική μονάδα**, καθορίστε το χρονικό διάστημα για το οποίο ισχύει η τιμή, όπως ημέρα ή ώρα.</span><span class="sxs-lookup"><span data-stu-id="8d076-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="8d076-117">Συμπληρώστε τα πεδία **Ημερομηνία έναρξης**, **Ημερομηνία λήξης** και **Περιγραφή** ανάλογα με τις ανάγκες σας.</span><span class="sxs-lookup"><span data-stu-id="8d076-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="8d076-118">Επιλέξτε **Αποθήκευση**, για να δημιουργήσετε την εγγραφή, έτσι ώστε να μπορείτε να συνεχίσετε να την επεξεργάζεστε.</span><span class="sxs-lookup"><span data-stu-id="8d076-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="8d076-119">Για να προσθέσετε μια τιμή ρόλου στον τιμοκατάλογο, κάντε κλικ στο κουμπί **+** στις **Τιμές ρόλων**.</span><span class="sxs-lookup"><span data-stu-id="8d076-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="8d076-120">Στο παράθυρο διαλόγου **Τιμή ρόλου**, συμπληρώστε τα στοιχεία και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="8d076-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8d076-121">Συνεχίστε προσθέτοντας τιμές ρόλων, ανάλογα με τις απαιτήσεις.</span><span class="sxs-lookup"><span data-stu-id="8d076-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="8d076-122">Μόλις τελειώσετε, επιλέξτε **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="8d076-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="8d076-123">Για να προσθέσετε μια τιμή κατηγορίας εξόδων στον τιμοκατάλογο, κάντε κλικ στο κουμπί **+** στις **Τιμές κατηγοριών**.</span><span class="sxs-lookup"><span data-stu-id="8d076-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="8d076-124">Στο παράθυρο διαλόγου **Τιμή κατηγορίας συναλλαγής**, συμπληρώστε τα στοιχεία και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="8d076-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8d076-125">Συνεχίστε προσθέτοντας τιμές κατηγοριών, ανάλογα με τις απαιτήσεις.</span><span class="sxs-lookup"><span data-stu-id="8d076-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="8d076-126">Μόλις τελειώσετε, επιλέξτε **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="8d076-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="8d076-127">Για να προσθέσετε στοιχεία τιμοκαταλόγου στον τιμοκατάλογο, κάντε κλικ στο κουμπί **+** στα **Στοιχεία τιμοκαταλόγου**.</span><span class="sxs-lookup"><span data-stu-id="8d076-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="8d076-128">Στο παράθυρο διαλόγου **Στοιχείο τιμοκαταλόγου**, συμπληρώστε τα στοιχεία και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="8d076-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8d076-129">Συνεχίστε προσθέτοντας στοιχεία τιμοκαταλόγου, ανάλογα με τις απαιτήσεις.</span><span class="sxs-lookup"><span data-stu-id="8d076-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="8d076-130">Μόλις τελειώσετε, επιλέξτε **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="8d076-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="8d076-131">Για να προσθέσετε σχέσεις περιφέρειας στον τιμοκατάλογο, κάντε κλικ στο κουμπί **+** στις **Σχέσεις περιφέρειας**.</span><span class="sxs-lookup"><span data-stu-id="8d076-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="8d076-132">Στο παράθυρο **Νέα σύνδεση**, συμπληρώστε τα στοιχεία και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="8d076-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="8d076-133">Συνεχίστε προσθέτοντας σχέσεις περιφερειών, ανάλογα με τις ανάγκες σας.</span><span class="sxs-lookup"><span data-stu-id="8d076-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="8d076-134">Μόλις τελειώσετε, επιλέξτε **Αποθήκευση** στην κάτω δεξιά γωνία της οθόνης.</span><span class="sxs-lookup"><span data-stu-id="8d076-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="8d076-135">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="8d076-135">See Also</span></span>  
 [<span data-ttu-id="8d076-136">Ρύθμιση παραμέτρων του Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="8d076-136">Configure Project Service Automation</span></span>](../psa/configure.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]