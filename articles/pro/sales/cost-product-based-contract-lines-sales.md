---
title: Κοστολόγηση γραμμών σύμβασης βάσει προϊόντων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a81c972f36179621f0547c24fc53d294485f638c
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764459"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="c946c-103">Κοστολόγηση γραμμών σύμβασης βάσει προϊόντων - lite</span><span class="sxs-lookup"><span data-stu-id="c946c-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="c946c-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="c946c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c946c-105">Οι γραμμές σύμβασης βάσει προϊόντων στο Dynamics 365 Project Operations περιλαμβάνουν το πεδίο **Τιμή κόστους** το οποίο αποθηκεύει την τιμή κόστους του προϊόντος για υπολογισμούς της κατάντη κερδοφορίας.</span><span class="sxs-lookup"><span data-stu-id="c946c-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="c946c-106">Όταν δημιουργείται μια γραμμή σύμβασης βάσει προϊόντος για ένα προϊόν καταλόγου, το κόστος της γραμμής ορίζεται από το πεδίο **Τυπικό κόστος** του καταλόγου προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="c946c-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="c946c-107">Το πεδίο **Τυπικό κόστος** στον κατάλογο προϊόντων ορίζεται στη βασική νομισματική μονάδα του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="c946c-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="c946c-108">Όταν το κόστος μονάδας προεπιλέγεται στη γραμμή σύμβασης, μετατρέπεται σε νόμισμα πωλήσεων στη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="c946c-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="c946c-109">Κόστος μονάδας σε γραμμή σύμβασης βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="c946c-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="c946c-110">Ο σκοπός της ύπαρξης ενός κόστους μονάδας σε μια γραμμή σύμβασης βασισμένης σε προϊόντα είναι να επιτρέπεται διαφορετικό κόστος για ένα προϊόν για κάθε πώληση μονάδας.</span><span class="sxs-lookup"><span data-stu-id="c946c-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="c946c-111">Παρόλο που δεν είναι πάντα απαραίτητο, υπάρχουν ορισμένα σενάρια στα οποία το κόστος του προϊόντος μπορεί να έχει έκπτωση για τον πελάτη από τον προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="c946c-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="c946c-112">Σκεφτείτε το ακόλουθο σενάριο:</span><span class="sxs-lookup"><span data-stu-id="c946c-112">Consider the following scenario:</span></span>

<span data-ttu-id="c946c-113">Η Fabrikam Robotics εγκαθιστά ρομποτικούς βραχίονες στις γραμμές συναρμολόγησης της Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="c946c-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="c946c-114">Η Fabrikam παρέχει υπηρεσίες εγκατάστασης αλλά οι ρομποτικοί βραχίονες είναι της Trey Research.</span><span class="sxs-lookup"><span data-stu-id="c946c-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="c946c-115">Εάν η εγκατάσταση των ρομποτικών βραχιόνων στη Adatum Corporation ανοίγει μια νέα βιομηχανία κάθετη για τους ρομποτικούς βραχίονες της Trey Research, τότε η Trey μπορεί να δώσει μια ειδική έκπτωση για την εν λόγω συμφωνία στη Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="c946c-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="c946c-116">Σε αυτή την περίπτωση, η Fabrikam δημιουργεί μια γραμμή σύμβασης βασισμένης σε προϊόν για ρομποτικούς βραχίονες.</span><span class="sxs-lookup"><span data-stu-id="c946c-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="c946c-117">Καταχωρείται μια τιμή ανά κόστος μονάδας για αυτήν τη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="c946c-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="c946c-118">Το κόστος είναι διαφορετικό από το κόστος της έρευνας στην Trey Research.</span><span class="sxs-lookup"><span data-stu-id="c946c-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>
