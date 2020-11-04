---
title: Λήψη στοιχείων σχετικά με την παραγγελία αγοράς από απαίτηση στοιχείου
description: Αυτό το θέμα επεξηγεί τον τρόπο λήψης στοιχείων σε μια παραγγελία αγοράς από μια απαίτηση στοιχείου.
author: Yowelle
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a5b3622458da957ed150311f6ea75d5f1444d5f1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077083"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="03eb7-103">Λήψη στοιχείων σχετικά με την παραγγελία αγοράς από απαίτηση στοιχείου</span><span class="sxs-lookup"><span data-stu-id="03eb7-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="03eb7-104">Αυτό το θέμα επεξηγεί τον τρόπο λήψης στοιχείων σε μια παραγγελία αγοράς από μια απαίτηση στοιχείου.</span><span class="sxs-lookup"><span data-stu-id="03eb7-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="03eb7-105">Με τη χρήση μιας απαίτησης στοιχείου αντί για μια συναλλαγή είδους, μπορείτε να προγραμματίσετε την παράδοση μόλις πριν από την πραγματική χρήση του στοιχείου, να δημιουργήσετε μια παραγγελία αγοράς, να συμπεριλάβετε το στοιχείο στο πλαίσιο της εμπορικής συμφωνίας και να συμπεριλάβετε την απαίτηση για ένα στοιχείο στον προγραμματισμό παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="03eb7-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="03eb7-106">Αυτή η εργασία χρησιμοποιεί το σύνολο δεδομένων USSI.</span><span class="sxs-lookup"><span data-stu-id="03eb7-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="03eb7-107">Στο παράθυρο περιήγησης, μεταβείτε στις **Λειτουργικές μονάδες > Διαχείριση έργου και λογιστική > Έργα > Όλα τα έργα**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="03eb7-108">Στη λίστα, επιλέξτε τη σύνδεση στην επιθυμητή γραμμή.</span><span class="sxs-lookup"><span data-stu-id="03eb7-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="03eb7-109">Στο παράθυρο ενεργειών, επιλέξτε **Σχεδιασμός**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="03eb7-110">Επιλέξτε **Απαιτήσεις στοιχείου**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="03eb7-111">Επιλέξτε **Νέα**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-111">Select **New**.</span></span>
6. <span data-ttu-id="03eb7-112">Στη νέα γραμμή, καταχωρίστε ή επιλέξτε μια τιμή στο πεδίο **Αριθμός στοιχείου**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="03eb7-113">Στο πεδίο **Ποσότητα** , καταχωρίστε έναν αριθμό.</span><span class="sxs-lookup"><span data-stu-id="03eb7-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="03eb7-114">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-114">Select **Save**.</span></span>
9. <span data-ttu-id="03eb7-115">Στο παράθυρο ενεργειών, επιλέξτε **Διαχείριση**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="03eb7-116">Επιλέξτε **Λειτουργίες**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-116">Select **Functions**.</span></span>
11. <span data-ttu-id="03eb7-117">Επιλέξτε **Δημιουργία παραγγελίας αγοράς**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="03eb7-118">Επιλέξτε το πλαίσιο ελέγχου **Συμπερίληψη όλων**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="03eb7-119">Στο πεδίο **Λογαριασμός πωλητή** , καταχωρίστε ή επιλέξτε μια τιμή.</span><span class="sxs-lookup"><span data-stu-id="03eb7-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="03eb7-120">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-120">Select **OK**.</span></span>
15. <span data-ttu-id="03eb7-121">Στο παράθυρο περιήγησης, μεταβείτε στις **Λειτουργικές μονάδες > Πληρωτέοι λογαριασμοί > Παραγγελίες αγοράς > Όλες οι παραγγελίες αγοράς**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="03eb7-122">Στη λίστα, επιλέξτε τη σύνδεση στην επιθυμητή γραμμή.</span><span class="sxs-lookup"><span data-stu-id="03eb7-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="03eb7-123">Στο παράθυρο ενεργειών, επιλέξτε **Αγορά**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="03eb7-124">Επιλέξτε **Επιβεβαίωση**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="03eb7-125">Στο παράθυρο ενεργειών, επιλέξτε **Λήψη**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="03eb7-126">Επιλέξτε **Απόδειξη προϊόντος**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="03eb7-127">Στο πεδίο **Απόδειξη προϊόντος** , πληκτρολογήστε μια τιμή.</span><span class="sxs-lookup"><span data-stu-id="03eb7-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="03eb7-128">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="03eb7-128">Select **OK**.</span></span>

