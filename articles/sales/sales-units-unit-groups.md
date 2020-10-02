---
title: Μονάδες και ομάδες μονάδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας μονάδων και ομάδων μονάδων στο Dynamics 365 Project operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: ea5399368214a293ca7c10fabf21d82407b5c76f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898756"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="8c517-103">Μονάδες και ομάδες μονάδων</span><span class="sxs-lookup"><span data-stu-id="8c517-103">Units and unit groups</span></span>

<span data-ttu-id="8c517-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="8c517-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8c517-105">Οι μονάδες είναι οι ποσότητες ή οι μετρήσεις στις οποίες πωλείτε τα προϊόντα ή τις υπηρεσίες σας.</span><span class="sxs-lookup"><span data-stu-id="8c517-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="8c517-106">Για παράδειγμα, εάν πουλάτε προμήθειες κηπουρικής, μπορεί να πουλάτε σπόρους για σπορά σε πακέτα, κουτιά και παλέτες.</span><span class="sxs-lookup"><span data-stu-id="8c517-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="8c517-107">Μια ομάδα μονάδων είναι μια συλλογή από αυτές τις διαφορετικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="8c517-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="8c517-108">Για να ολοκληρώσετε τα βήματα σε αυτό το θέμα, βεβαιωθείτε ότι σας ανατεθεί ο ρόλος του Διαχειριστή συστήματος ή του Υπεύθυνου Sales Professional ή εάν έχετε ισοδύναμα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="8c517-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="8c517-109">Δημιουργία ομάδας μονάδων</span><span class="sxs-lookup"><span data-stu-id="8c517-109">Create a unit group</span></span>

1. <span data-ttu-id="8c517-110">Στον χάρτη τοποθεσίας, επιλέξτε **Μονάδες**.</span><span class="sxs-lookup"><span data-stu-id="8c517-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="8c517-111">Επιλέξτε **Δημιουργία** και στο παράθυρο διαλόγου **Δημιουργία ομάδας μονάδων**, πληκτρολογήστε το όνομα της μονάδας.</span><span class="sxs-lookup"><span data-stu-id="8c517-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="8c517-112">Στο πεδίο **Πρωτεύουσα μονάδα** πληκτρολογήστε τη ελάχιστη κοινή μονάδα μέτρησης στην οποία θα πωλείται το προϊόν.</span><span class="sxs-lookup"><span data-stu-id="8c517-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="8c517-113">Για παράδειγμα, μπορείτε να εισάγετε "τεμάχιο" ή "ουγγιά".</span><span class="sxs-lookup"><span data-stu-id="8c517-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="8c517-114">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="8c517-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="8c517-115">Προσθήκη μονάδων σε μια ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="8c517-115">Add units to a unit group</span></span>

1. <span data-ttu-id="8c517-116">Ανοίξτε μια ομάδα μονάδων και στην καρτέλα **Σχετικά**, επιλέξτε **Μονάδες**.</span><span class="sxs-lookup"><span data-stu-id="8c517-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="8c517-117">Θα δείτε ότι έχει ήδη προστεθεί η κύρια μονάδα.</span><span class="sxs-lookup"><span data-stu-id="8c517-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="8c517-118">Επιλέξτε **Προσθήκη νέας μονάδας** και στη σελίδα **Γρήγορη δημιουργία: μονάδα**, στο πεδίο **Όνομα**, καταγράψτε το όνομα της μονάδας.</span><span class="sxs-lookup"><span data-stu-id="8c517-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="8c517-119">Στο πεδίο **Ποσότητα**, καταγράψτε την ποσότητα που θα περιέχει η μονάδα.</span><span class="sxs-lookup"><span data-stu-id="8c517-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="8c517-120">Για παράδειγμα, εάν ένα κουτί περιέχει δύο τεμάχια, πληκτρολογήστε "2".</span><span class="sxs-lookup"><span data-stu-id="8c517-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="8c517-121">Στο πεδίο **Βασική μονάδα**, επιλέξτε μια βασική μονάδα για να καθορίσετε τη χαμηλότερη μονάδα μέτρησης για τη μονάδα.</span><span class="sxs-lookup"><span data-stu-id="8c517-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="8c517-122">Για παράδειγμα, μπορείτε να επιλέξετε "τεμάχιο".</span><span class="sxs-lookup"><span data-stu-id="8c517-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="8c517-123">Επιλέξτε **Αποθήκευση**:</span><span class="sxs-lookup"><span data-stu-id="8c517-123">Select **Save**:</span></span>
