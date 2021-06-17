---
title: Επισκόπηση γραμμών προσφοράς βάσει προϊόντων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με γραμμές σύμβασης βάσει προϊόντος.
author: rumant
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5cc3a97194e01b14de054a93a6268c1f0c24bc25
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994451"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="a2b78-103">Επισκόπηση γραμμών προσφοράς βάσει προϊόντων - lite</span><span class="sxs-lookup"><span data-stu-id="a2b78-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="a2b78-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="a2b78-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a2b78-105">Μπορείτε να δημιουργήσετε γραμμές προσφοράς βάσει προϊόντων στο Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a2b78-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="a2b78-106">Οι γραμμές προσφοράς που βασίζονται σε προϊόντα μπορούν να προστεθούν μη αυτόματα ή να είναι στοιχεία από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="a2b78-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="a2b78-107">Κατάλογος προϊόντων</span><span class="sxs-lookup"><span data-stu-id="a2b78-107">Product catalog</span></span>

<span data-ttu-id="a2b78-108">Κάθε προϊόν στον κατάλογο προϊόντων έχει μια προεπιλεγμένη μονάδα και μια ομάδα μονάδων.</span><span class="sxs-lookup"><span data-stu-id="a2b78-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="a2b78-109">Εάν πολλά προϊόντα χρησιμοποιούν από κοινού το ίδιο σύνολο χαρακτηριστικών, μπορείτε να δημιουργήσετε μια οικογένεια προϊόντων που έχει και αυτά τα χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="a2b78-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="a2b78-110">Για παράδειγμα, μια εταιρεία πουλά άδειες συνδρομής για διάφορες εφαρμογές λογισμικού.</span><span class="sxs-lookup"><span data-stu-id="a2b78-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="a2b78-111">Όλα τα συνδρομητικά λογισμικά έχουν τα εξής δύο χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="a2b78-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="a2b78-112">Αριθμός χρηστών</span><span class="sxs-lookup"><span data-stu-id="a2b78-112">Number of users</span></span>
- <span data-ttu-id="a2b78-113">Μια διάρκεια συνδρομής σε μήνες</span><span class="sxs-lookup"><span data-stu-id="a2b78-113">A subscription duration measured in months</span></span>

<span data-ttu-id="a2b78-114">Για να διατηρήσετε αυτόν τον τύπο καταλόγου είναι να δημιουργήσετε μια οικογένεια προϊόντων με όνομα **Συνδρομητικό λογισμικό** και αυτό έχει αριθμό χρηστών και διάρκεια συνδρομής ως χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="a2b78-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="a2b78-115">Στη συνέχεια, μπορείτε να προσθέσετε μεμονωμένα προϊόντα στην οικογένεια προϊόντων **Συνδρομητικό λογισμικό**.</span><span class="sxs-lookup"><span data-stu-id="a2b78-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="a2b78-116">Προσθήκη στοιχείων καταλόγου προϊόντων σε μια προσφορά έργου</span><span class="sxs-lookup"><span data-stu-id="a2b78-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="a2b78-117">Οι σελίδες **Προσφορά έργου** και **Σύμβαση έργου** έχουν ενότητες για γραμμές βάσει έργου και γραμμές βασισμένες σε προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="a2b78-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="a2b78-118">Για γραμμές βάσει προϊόντων, η αναπτυσσόμενη λίστα στη γραμμή προσφοράς ή τη γραμμή σύμβασης έργου περιλαμβάνει όλα τα προϊόντα και τις μονάδες του τιμοκαταλόγου προϊόντος.</span><span class="sxs-lookup"><span data-stu-id="a2b78-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="a2b78-119">Μπορείτε, επίσης, να προσθέσετε προϊόντα που δεν αποτελούν μέρος του τιμοκαταλόγου προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="a2b78-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="a2b78-120">Επιπλέον, μπορείτε να επιλέξετε προϊόντα από άλλους τιμοκαταλόγους ή μπορείτε να επιλέξετε προϊόντα απευθείας από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="a2b78-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="a2b78-121">Όταν επιλέγετε προϊόντα απευθείας από έναν κατάλογο προϊόντων, ο προεπιλεγμένος τιμοκατάλογος αυτού του προϊόντος χρησιμοποιείται για την λήψη της τιμής πώλησης του προϊόντος.</span><span class="sxs-lookup"><span data-stu-id="a2b78-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="a2b78-122">Εάν δεν έχει οριστεί ένας προεπιλεγμένος τιμοκατάλογος, η τιμή έχει οριστεί σε 0 (μηδέν).</span><span class="sxs-lookup"><span data-stu-id="a2b78-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="a2b78-123">Όταν μια γραμμή προσφοράς βασίζεται σε έναν κατάλογο προϊόντων, μπορείτε να παρακάμψετε την τιμή πώλησης απευθείας στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="a2b78-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="a2b78-124">Μια γραμμή προσφοράς στο πεδίο **Τιμολόγηση** με δύο διαθέσιμες τιμές:</span><span class="sxs-lookup"><span data-stu-id="a2b78-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="a2b78-125">**Παράκαμψη τιμολόγησης**</span><span class="sxs-lookup"><span data-stu-id="a2b78-125">**Override Pricing**</span></span>
- <span data-ttu-id="a2b78-126">**Χρήση προεπιλογής**</span><span class="sxs-lookup"><span data-stu-id="a2b78-126">**Use Default**</span></span>

<span data-ttu-id="a2b78-127">Εάν επιλέξετε **Παράκαμψη τιμολόγησης**, η προεπιλεγμένη τιμή δεν έχει οριστεί.</span><span class="sxs-lookup"><span data-stu-id="a2b78-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="a2b78-128">Πρέπει να εισάγετε μια τιμή για το προϊόν στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="a2b78-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="a2b78-129">Εάν επιλέξετε **Χρήση προεπιλογής**, χρησιμοποιείται η προεπιλεγμένη τιμή πώλησης και το πεδίο είναι κλειδωμένο για επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="a2b78-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="a2b78-130">Οι προεπιλεγμένοι τιμοκατάλογοι καταχωρούνται στις γραμμές με βάση το προϊόν σε μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="a2b78-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="a2b78-131">Το πεδίο **Τιμολόγηση** ορίζεται σε **Παράκαμψη τιμολόγησης** ώστε να παρακάμπτει την τιμολόγηση ώστε να μπορείτε να επεξεργαστείτε την προεπιλεγμένη τιμή στις γραμμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="a2b78-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="a2b78-132">Πρόκειται για μια παράκαμψη συγκεκριμένα για το Project Operations στη συμπεριφορά γραμμών βάσει προϊόντων στο Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="a2b78-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]