---
title: Προεπιλογές οικονομικής διάστασης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης των προεπιλογών οικονομικής διάστασης.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0a76447bb1a81a7157fccc0cd58eddd1eb5995de
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950129"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="8ee50-103">Προεπιλογές οικονομικής διάστασης</span><span class="sxs-lookup"><span data-stu-id="8ee50-103">Financial dimension defaults</span></span>

<span data-ttu-id="8ee50-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="8ee50-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="8ee50-105">Το Dynamics 365 Project Operations χρησιμοποιεί το πλαίσιο [οικονομικές διαστάσεις](/dynamics365/finance/general-ledger/financial-dimensions) στο Dynamics 365 Finance για να παράσχει πρόσθετες δεδομενικές πληροφορίες σχετικά με το δευτερεύον καθολικό του έργου και τις συναλλαγές του γενικού καθολικού.</span><span class="sxs-lookup"><span data-stu-id="8ee50-105">Dynamics 365 Project Operations uses the [Financial dimensions](/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="8ee50-106">Οι προεπιλεγμένες οικονομικές διαστάσεις μπορούν να οριστούν σε έναν πελάτη, σε μια προέλευση χρηματοδότησης έργου, σε ορόσημο, σε μια ουρά σύμβασης έργου ή σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="8ee50-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="8ee50-107">Ορισμός προεπιλεγμένων οικονομικών διαστάσεων για έναν πελάτη</span><span class="sxs-lookup"><span data-stu-id="8ee50-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="8ee50-108">Οι προεπιλογές διάστασης πελατών καθορίζονται στο Finance.</span><span class="sxs-lookup"><span data-stu-id="8ee50-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="8ee50-109">Ολοκληρώστε τα παρακάτω βήματα για να ορίσετε προεπιλογές διάστασης.</span><span class="sxs-lookup"><span data-stu-id="8ee50-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="8ee50-110">Μεταβείτε στους **Εισπρακτέους λογαριασμούς** > **Πελάτες** > **Όλοι οι πελάτες**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="8ee50-111">Στη σελίδα **Πελάτες**, στην καρτέλα **Οικονομικές διαστάσεις**, ορίστε τις τιμές οικονομικής διάστασης για συγκεκριμένο πελάτη.</span><span class="sxs-lookup"><span data-stu-id="8ee50-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="8ee50-112">Ορισμός προεπιλεγμένων οικονομικών διαστάσεων για συμβάσεις έργου</span><span class="sxs-lookup"><span data-stu-id="8ee50-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="8ee50-113">Οι συμβάσεις έργου δημιουργούνται και διατηρούνται στο Common Data Service (CDS).</span><span class="sxs-lookup"><span data-stu-id="8ee50-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="8ee50-114">Τα χαρακτηριστικά λογιστικής για τις συμβάσεις έργου ορίζονται στη μονάδα **Διαχείριση έργου και λογιστική** στο Finance.</span><span class="sxs-lookup"><span data-stu-id="8ee50-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="8ee50-115">Καθορισμός οικονομικών διαστάσεων για μια προέλευση χρηματοδότησης έργου</span><span class="sxs-lookup"><span data-stu-id="8ee50-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="8ee50-116">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** > **Έργα** > **Συμβάσεις έργου**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="8ee50-117">Επιλέξτε την καρτέλα που θέλετε να ενημερώσετε και, στην καρτέλα **Σύμβαση έργου** επιλέξτε **Εμφάνιση προεπιλεγμένης λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="8ee50-118">Αναπτύξτε τις **Σχετικές πληροφορίες** και επιλέξτε την καρτέλα **Πηγές χρηματοδότησης**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="8ee50-119">Ορίστε τις προεπιλογές οικονομικής διάστασης.</span><span class="sxs-lookup"><span data-stu-id="8ee50-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="8ee50-120">Σημειώστε ότι οι προεπιλεγμένες οικονομικές διαστάσεις από το λογαριασμό του πελάτη.</span><span class="sxs-lookup"><span data-stu-id="8ee50-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="8ee50-121">Καθορισμός οικονομικών διαστάσεων για μια γραμμή σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="8ee50-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="8ee50-122">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** > **Έργα** > **Συμβάσεις έργου**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="8ee50-123">Επιλέξτε την καρτέλα που θέλετε να ενημερώσετε και, στην καρτέλα **Σύμβαση έργου** επιλέξτε **Εμφάνιση προεπιλεγμένης λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="8ee50-124">Αναπτύξτε τις **Σχετικές πληροφορίες** και επιλέξτε την καρτέλα **Γραμμές σύμβασης**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="8ee50-125">Ορίστε τις προεπιλογές οικονομικής διάστασης.</span><span class="sxs-lookup"><span data-stu-id="8ee50-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="8ee50-126">Οι προεπιλογές οικονομικής διάστασης εφαρμόζονται και μπορούν να χρησιμοποιηθούν μόνο με γραμμές σύμβασης προκαθορισμένης τιμής (ορόσημο).</span><span class="sxs-lookup"><span data-stu-id="8ee50-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="8ee50-127">Αυτές οι προεπιλογές χρησιμοποιούνται σε σχετικές συναλλαγές μέσω του έργου και σε γραμμές τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="8ee50-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="8ee50-128">Ορισμός προεπιλεγμένων οικονομικών διαστάσεων για έργα</span><span class="sxs-lookup"><span data-stu-id="8ee50-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="8ee50-129">Τα έργα δημιουργούνται και διατηρούνται στο CDS.</span><span class="sxs-lookup"><span data-stu-id="8ee50-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="8ee50-130">Τα χαρακτηριστικά λογιστικής για έργα ορίζονται στη μονάδα **Διαχείριση έργου και λογιστική** στο Finance.</span><span class="sxs-lookup"><span data-stu-id="8ee50-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="8ee50-131">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** > **Έργα** > **Όλα τα έργα**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="8ee50-132">Επιλέξτε την καρτέλα που θέλετε να ενημερώσετε και, στην καρτέλα **Έργο** επιλέξτε **Εμφάνιση προεπιλεγμένης λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="8ee50-133">Αναπτύξτε τις **Σχετικές πληροφορίες** και επιλέξτε την καρτέλα **Ρυθμίσεις παραμέτρων**.</span><span class="sxs-lookup"><span data-stu-id="8ee50-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="8ee50-134">Ορίστε τις προεπιλογές οικονομικής διάστασης.</span><span class="sxs-lookup"><span data-stu-id="8ee50-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="8ee50-135">Σημειώστε ότι οι προεπιλεγμένες οικονομικές διαστάσεις από το λογαριασμό του πελάτη.</span><span class="sxs-lookup"><span data-stu-id="8ee50-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="8ee50-136">Εάν το έργο σχετίζεται με μια γραμμή σύμβασης με πολλούς πελάτες σύμβασης έργου, ο κύριος πελάτης χρησιμοποιείται για τις προεπιλεγμένες οικονομικές διαστάσεις.</span><span class="sxs-lookup"><span data-stu-id="8ee50-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="8ee50-137">Οι προεπιλεγμένες οικονομικές διαστάσεις του έργου χρησιμοποιούνται για τον ορισμό προεπιλογών γραμμής ημερολογίου για συναλλαγές χρόνου, εξόδων και χρέωσης στο **Ημερολόγιο ενοποίησης εργασιών έργου** και σε σχετικές γραμμές τιμολογίου έργου.</span><span class="sxs-lookup"><span data-stu-id="8ee50-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]