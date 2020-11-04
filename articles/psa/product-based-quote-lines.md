---
title: Γραμμές προσφοράς βάσει προϊόντων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις γραμμές προσφοράς βάσει προϊόντων.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
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
ms.openlocfilehash: 55a5b5041a494892e6d96bf24e1bc132a26521dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077096"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="03a0c-103">Γραμμές προσφοράς βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="03a0c-103">Product-based quote lines</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="03a0c-104">Μπορείτε να δημιουργήσετε γραμμές προσφοράς βάσει προϊόντων στο Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="03a0c-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="03a0c-105">Οι γραμμές προσφοράς που βασίζονται σε προϊόντα μπορούν να είναι "εγγεγραμμένες" γραμμές ή μπορούν να είναι στοιχεία από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="03a0c-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="03a0c-106">Κατάλογος προϊόντων</span><span class="sxs-lookup"><span data-stu-id="03a0c-106">Product catalog</span></span>

<span data-ttu-id="03a0c-107">Τα προϊόντα σε έναν κατάλογο προϊόντων Dynamics 365 έχουν μια προεπιλεγμένη μονάδα και μια ομάδα μονάδων.</span><span class="sxs-lookup"><span data-stu-id="03a0c-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="03a0c-108">Εάν πολλά προϊόντα χρησιμοποιούν από κοινού το ίδιο σύνολο χαρακτηριστικών, μπορείτε να δημιουργήσετε μια οικογένεια προϊόντων που έχει και αυτά τα χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="03a0c-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="03a0c-109">Όλα τα προϊόντα σε μια οικογένεια προϊόντων κληρονομούν το ίδιο σύνολο χαρακτηριστικών.</span><span class="sxs-lookup"><span data-stu-id="03a0c-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="03a0c-110">Για παράδειγμα, μια εταιρεία πουλά άδειες συνδρομής για διάφορες εφαρμογές λογισμικού.</span><span class="sxs-lookup"><span data-stu-id="03a0c-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="03a0c-111">Όλα τα συνδρομητικά λογισμικά έχουν τα εξής δύο χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="03a0c-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="03a0c-112">Αριθμός χρηστών</span><span class="sxs-lookup"><span data-stu-id="03a0c-112">Number of users</span></span> 
- <span data-ttu-id="03a0c-113">Διάρκεια συνδρομής (σε μήνες)</span><span class="sxs-lookup"><span data-stu-id="03a0c-113">Subscription duration (in months)</span></span>

<span data-ttu-id="03a0c-114">Ένας καλός τρόπος για να διατηρήσετε αυτόν τον τύπο καταλόγου είναι να δημιουργήσετε μια οικογένεια προϊόντων με όνομα **Συνδρομητικό λογισμικό** και αυτό έχει **Αριθμό χρηστών** και **Διάρκεια συνδρομής** ως χαρακτηριστικά.</span><span class="sxs-lookup"><span data-stu-id="03a0c-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software** , and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="03a0c-115">Στη συνέχεια, μπορείτε να προσθέσετε μεμονωμένα προϊόντα, όπως το **Dynamics 365 Sales** ή **Dynamics 365 Field Service** στην οικογένεια προϊόντων **Συνδρομητικό λογισμικό**.</span><span class="sxs-lookup"><span data-stu-id="03a0c-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="03a0c-116">Προσθήκη στοιχείων καταλόγου προϊόντων σε μια προσφορά έργου</span><span class="sxs-lookup"><span data-stu-id="03a0c-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="03a0c-117">Οι σελίδες "προσφορά έργου" και "σύμβαση έργου" έχουν ενότητες για δύο τύπους γραμμών: γραμμές βάσει έργου και γραμμές βασισμένες σε προϊόντα.</span><span class="sxs-lookup"><span data-stu-id="03a0c-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="03a0c-118">Για γραμμές βασισμένες σε προϊόντα, το Dynamics 365 χρησιμοποιείται για την προσθήκη στοιχείων από έναν κατάλογο προϊόντων σε μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="03a0c-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="03a0c-119">Η αναπτυσσόμενη λίστα στη γραμμή προσφοράς ή τη γραμμή σύμβασης έργου περιλαμβάνει όλα τα προϊόντα και τις μονάδες του τιμοκαταλόγου προϊόντος που επισυνάπτεται στην προσφορά ή τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="03a0c-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="03a0c-120">Μπορείτε, επίσης, να προσθέσετε προϊόντα που δεν αποτελούν μέρος του τιμοκαταλόγου προϊόντων της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="03a0c-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="03a0c-121">Επιπλέον, μπορείτε να επιλέξετε προϊόντα από άλλους τιμοκαταλόγους ή μπορείτε να επιλέξετε προϊόντα απευθείας από τον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="03a0c-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="03a0c-122">Όταν επιλέγετε προϊόντα απευθείας από έναν κατάλογο προϊόντων, ο προεπιλεγμένος τιμοκατάλογος αυτού του προϊόντος χρησιμοποιείται για την λήψη της τιμής πώλησης του προϊόντος.</span><span class="sxs-lookup"><span data-stu-id="03a0c-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="03a0c-123">Εάν δεν έχει οριστεί ένας προεπιλεγμένος τιμοκατάλογος, η τιμή έχει οριστεί σε 0 (μηδέν).</span><span class="sxs-lookup"><span data-stu-id="03a0c-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="03a0c-124">Εάν μια γραμμή προσφοράς βασίζεται σε έναν κατάλογο προϊόντων, μπορείτε να παρακάμψετε την τιμή πώλησης απευθείας στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="03a0c-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="03a0c-125">Λάβετε υπόψη σας ότι μια ουρά προσφοράς στο Dynamics 365 έχει πεδίο **Τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="03a0c-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="03a0c-126">Είναι διαθέσιμες δύο τιμές:</span><span class="sxs-lookup"><span data-stu-id="03a0c-126">Two values are available:</span></span>

- <span data-ttu-id="03a0c-127">Παράκαμψη τιμής</span><span class="sxs-lookup"><span data-stu-id="03a0c-127">Override pricing</span></span>  
- <span data-ttu-id="03a0c-128">Χρήση προεπιλογής</span><span class="sxs-lookup"><span data-stu-id="03a0c-128">Use default</span></span>

<span data-ttu-id="03a0c-129">Εάν ορίσετε αυτό το πεδίο σε **Παράκαμψη τιμολόγησης** , το Dynamics 365 δεν ορίζει μια προεπιλεγμένη τιμή.</span><span class="sxs-lookup"><span data-stu-id="03a0c-129">If you set this field to **Override pricing** , Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="03a0c-130">Πρέπει να εισάγετε μια τιμή για το προϊόν στη γραμμή προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="03a0c-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="03a0c-131">Εάν ορίσετε αυτό το πεδίο σε **Χρήση προεπιλογής** , το Dynamics 365 χρησιμοποιεί την προεπιλεγμένη τιμή πώλησης και κλειδώνει το πεδίο για την αποτροπή της επεξεργασίας.</span><span class="sxs-lookup"><span data-stu-id="03a0c-131">If you set this field to **Use default** , Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="03a0c-132">Μετά την εγκατάσταση του PSA, οι προεπιλεγμένοι τιμοκατάλογοι καταχωρούνται στις γραμμές με βάση το προϊόν σε μια προσφορά.</span><span class="sxs-lookup"><span data-stu-id="03a0c-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="03a0c-133">Το πεδίο **Τιμολόγηση** ορίζεται σε **Παράκαμψη τιμολόγησης** ώστε να παρακάμπτει την τιμολόγηση ώστε να μπορείτε να επεξεργαστείτε την προεπιλεγμένη τιμή στις γραμμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="03a0c-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![Ρύθμιση παράκαμψης τιμολόγησης](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="03a0c-135">Συντελεστές ποσότητας για τα προϊόντα</span><span class="sxs-lookup"><span data-stu-id="03a0c-135">Quantity factors for products</span></span>

<span data-ttu-id="03a0c-136">Το PSA χρησιμοποιεί συντελεστές ποσότητας για να υποστηρίξει την πώληση προϊόντων βασισμένων σε συνδρομή.</span><span class="sxs-lookup"><span data-stu-id="03a0c-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="03a0c-137">Για τα προϊόντα που βασίζονται σε συνδρομή, η ποσότητα στη γραμμή σύμβασης προσφοράς ή έργου εκφράζεται ως ο αριθμός των μηνών χρηστών.</span><span class="sxs-lookup"><span data-stu-id="03a0c-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="03a0c-138">Συνήθως, η τιμή του συνδρομητικού λογισμικού αποθηκεύεται στον κατάλογο ως τιμή ανά χρήστη ανά μήνα.</span><span class="sxs-lookup"><span data-stu-id="03a0c-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="03a0c-139">Ωστόσο, μπορείτε να χρησιμοποιήσετε άλλες περιγραφές ώρας αντί για αυτές.</span><span class="sxs-lookup"><span data-stu-id="03a0c-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="03a0c-140">Κατά τη διάρκεια της διαδικασίας πωλήσεων, η τιμή στη γραμμή προσφοράς είναι συνήθως η τιμή ανά χρήστη, ανά μήνα κατά τον οποίο διαπραγματεύτηκε και λαμβάνουν έκπτωση από τον αντιπρόσωπο πωλήσεων IT.</span><span class="sxs-lookup"><span data-stu-id="03a0c-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="03a0c-141">Κάθε συμφωνία έχει διαφορετικό αριθμό χρηστών και ένα διαφορετικό αριθμό μηνών συνδρομής.</span><span class="sxs-lookup"><span data-stu-id="03a0c-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="03a0c-142">Η ποσότητα που χρησιμοποιείται για τον υπολογισμό του ποσού της γραμμής προσφοράς είναι ένα προϊόν του πλήθους χρηστών και του αριθμού των μηνών συνδρομής.</span><span class="sxs-lookup"><span data-stu-id="03a0c-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="03a0c-143">Για την υποστήριξη αυτού του τύπου πώλησης, το PSA εισήγαγε την έννοια των ποσοτικών παραγόντων.</span><span class="sxs-lookup"><span data-stu-id="03a0c-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="03a0c-144">Οι συντελεστές ποσότητας εξαρτώνται από τα χαρακτηριστικά του προϊόντος στο Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="03a0c-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="03a0c-145">Όταν ρυθμίζετε τις παραμέτρους συγκεκριμένων ιδιοτήτων για ένα προϊόν, το PSA σάς δίνει τη δυνατότητα να επισημάνετε ένα υποσύνολο αυτών των ιδιοτήτων ή όλες τις ιδιότητες, ως συντελεστές ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="03a0c-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="03a0c-146">Το PSA επικυρώνει ότι μόνο οι αριθμητικές ιδιότητες ή οι ιδιότητες προϊόντος που έχουν έναν τύπο αριθμητικών δεδομένων επισημαίνονται ως συντελεστές ποσότητας.</span><span class="sxs-lookup"><span data-stu-id="03a0c-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="03a0c-147">Όταν ένα προϊόν για το οποίο έχουν ρυθμιστεί συντελεστές ποσότητας έχει προστεθεί σε μια γραμμή προσφοράς, το πεδίο **Ποσότητα** στη γραμμή προσφοράς μετατρέπεται σε πεδίο μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="03a0c-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="03a0c-148">Αφού εισάγετε τις τιμές για τις ιδιότητες προϊόντος που είναι συντελεστές ποσότητας, το PSA υπολογίζει την ποσότητα της ουράς προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="03a0c-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="03a0c-149">Για παράδειγμα, το Dynamics 365 μπορεί να έχει τις ακόλουθες ιδιότητες:</span><span class="sxs-lookup"><span data-stu-id="03a0c-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="03a0c-150">**Αριθμός χρηστών** - ο αριθμός των χρηστών</span><span class="sxs-lookup"><span data-stu-id="03a0c-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="03a0c-151">**Αριθμός μηνών** - ο αριθμός των μηνών συνδρομής</span><span class="sxs-lookup"><span data-stu-id="03a0c-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="03a0c-152">**SKU προϊόντος**</span><span class="sxs-lookup"><span data-stu-id="03a0c-152">**Product SKU**</span></span> 

<span data-ttu-id="03a0c-153">Οι ιδιότητες **Αριθμός χρηστών** και **Αριθμός μηνών** μπορούν να επισημανθούν ως συντελεστές ποσότητας με επεξεργασία των ιδιοτήτων της γραμμής προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="03a0c-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![Επισήμανση αριθμού χρηστών και μηνών ως παράγοντες ποιότητας](media/basic-guide-11.png)
 
