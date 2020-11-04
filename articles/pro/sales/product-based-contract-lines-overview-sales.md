---
title: Επισκόπηση γραμμών σύμβασης βάσει προϊόντων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις γραμμές σύμβασης βάσει προϊόντων.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 794a80b0dd6b8717b43e712b96b9ac077517c226
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076843"
---
# <a name="product-based-contract-lines-overview"></a><span data-ttu-id="791ed-103">Επισκόπηση γραμμών σύμβασης βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="791ed-103">Product-based contract lines overview</span></span>

<span data-ttu-id="791ed-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="791ed-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="791ed-105">Μπορείτε να δημιουργήσετε γραμμές σύμβασης βασισμένες σε προϊόντα στο Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="791ed-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="791ed-106">Οι γραμμές σύμβασης που βασίζονται σε προϊόντα μπορούν να μη αυτόματα δημιουργημένες γραμμές ή μπορούν να είναι στοιχεία από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="791ed-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="791ed-107">Κατάλογος προϊόντων</span><span class="sxs-lookup"><span data-stu-id="791ed-107">Product catalog</span></span>

<span data-ttu-id="791ed-108">Τα προϊόντα σε έναν κατάλογο προϊόντων έχουν μια προεπιλεγμένη μονάδα και μια ομάδα μονάδων.</span><span class="sxs-lookup"><span data-stu-id="791ed-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="791ed-109">Εάν πολλά προϊόντα χρησιμοποιούν από κοινού το ίδιο σύνολο χαρακτηριστικών, μπορείτε να δημιουργήσετε μια οικογένεια προϊόντων που έχει και αυτά τα χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="791ed-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="791ed-110">Όλα τα προϊόντα σε μια οικογένεια προϊόντων κληρονομούν το ίδιο σύνολο χαρακτηριστικών.</span><span class="sxs-lookup"><span data-stu-id="791ed-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="791ed-111">Για παράδειγμα, μια εταιρεία πουλά άδειες συνδρομής για διάφορες εφαρμογές λογισμικού.</span><span class="sxs-lookup"><span data-stu-id="791ed-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="791ed-112">Όλα τα συνδρομητικά λογισμικά έχουν τα εξής δύο χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="791ed-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="791ed-113">Αριθμός χρηστών</span><span class="sxs-lookup"><span data-stu-id="791ed-113">Number of users</span></span>
- <span data-ttu-id="791ed-114">Διάρκεια συνδρομής (σε μήνες)</span><span class="sxs-lookup"><span data-stu-id="791ed-114">Subscription duration (in months)</span></span>

<span data-ttu-id="791ed-115">Για να διατηρήσετε αυτόν τον τύπο καταλόγου, δημιουργήστε μια οικογένεια προϊόντων με όνομα **Λογισμικό συνδρομής**.</span><span class="sxs-lookup"><span data-stu-id="791ed-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="791ed-116">Προσθέστε τα χαρακτηριστικά, τον **Αριθμό χρηστών** και τη **Διάρκεια συνδρομής** στην οικογένεια προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="791ed-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="791ed-117">Στη συνέχεια, προσθέστε μεμονωμένα προϊόντα στην οικογένεια προϊόντων **Λογισμικό συνδρομής**.</span><span class="sxs-lookup"><span data-stu-id="791ed-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="791ed-118">Προσθήκη στοιχείων καταλόγου προϊόντων σε μια σύμβαση έργου</span><span class="sxs-lookup"><span data-stu-id="791ed-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="791ed-119">Οι συμβάσεις έργου έχουν ενότητες για δύο τύπους γραμμών: γραμμές βάσει έργου και γραμμές βασισμένες σε προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="791ed-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="791ed-120">Οι γραμμές βάσει προϊόντων περιλαμβάνουν όλα τα προϊόντα και τις μονάδες που περιλαμβάνονται στον τιμοκατάλογο προϊόντων της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="791ed-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="791ed-121">Τα προϊόντα που δεν αποτελούν μέρος του τιμοκαταλόγου προϊόντων της σύμβασης μπορούν να προστεθούν.</span><span class="sxs-lookup"><span data-stu-id="791ed-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="791ed-122">Μπορείτε να επιλέξετε προϊόντα από άλλους τιμοκαταλόγους ή απευθείας από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="791ed-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="791ed-123">Όταν επιλέγετε προϊόντα απευθείας από έναν κατάλογο προϊόντων, ο προεπιλεγμένος τιμοκατάλογος αυτού του προϊόντος χρησιμοποιείται για την λήψη της τιμής πώλησης του προϊόντος.</span><span class="sxs-lookup"><span data-stu-id="791ed-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="791ed-124">Εάν δεν έχει οριστεί ένας προεπιλεγμένος τιμοκατάλογος, η τιμή έχει οριστεί σε 0 (μηδέν).</span><span class="sxs-lookup"><span data-stu-id="791ed-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="791ed-125">Εάν μια γραμμή σύμβασης βασίζεται σε έναν κατάλογο προϊόντων, μπορείτε να παρακάμψετε την τιμή πώλησης απευθείας στη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="791ed-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="791ed-126">Μια γραμμή σύμβασης περιλαμβάνει το πεδίο **Τιμολόγηση** με τις δύο τιμές:</span><span class="sxs-lookup"><span data-stu-id="791ed-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="791ed-127">**Παράκαμψη τιμής**</span><span class="sxs-lookup"><span data-stu-id="791ed-127">**Override pricing**</span></span>
- <span data-ttu-id="791ed-128">**Χρήση προεπιλογής**</span><span class="sxs-lookup"><span data-stu-id="791ed-128">**Use default**</span></span>

<span data-ttu-id="791ed-129">Εάν ορίσετε το πεδίο **Τιμολόγηση** σε **Παράκαμψη τιμολόγησης** , η προεπιλεγμένη τιμή δεν ορίζεται.</span><span class="sxs-lookup"><span data-stu-id="791ed-129">If you set the **Pricing** field to **Override pricing** , the default price isn't set.</span></span> <span data-ttu-id="791ed-130">Καταχωρήστε μια τιμή για το προϊόν στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="791ed-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="791ed-131">Εάν ορίσετε το πεδίο σε **Χρήση προεπιλεγμένου** , χρησιμοποιείται η προεπιλεγμένη τιμή πώλησης και δεν είναι δυνατή η επεξεργασία του πεδίου.</span><span class="sxs-lookup"><span data-stu-id="791ed-131">If you set the field to **Use default** , the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="791ed-132">Μετά την εγκατάσταση του Project Operations, οι προεπιλεγμένοι τιμοκατάλογοι καταχωρούνται στις γραμμές με βάση το προϊόν σε μια σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="791ed-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="791ed-133">Το πεδίο **Τιμολόγηση** ορίζεται σε **Παράκαμψη τιμολόγησης** ώστε να παρακάμπτει την τιμολόγηση ώστε να μπορείτε να επεξεργαστείτε την προεπιλεγμένη τιμή στις γραμμές σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="791ed-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="791ed-134">Πρόκειται για μια συγκεκριμένη παράκαμψη Project Operations σε συμπεριφορά γραμμών βάσει προϊόντων στο Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="791ed-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>
