---
title: Κοστολόγηση γραμμών σύμβασης βάσει προϊόντων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7dfb9425174dddee52f9ee64f7a963e48a6bca70
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/20/2020
ms.locfileid: "4077147"
---
# <a name="costing-product-based-contract-lines"></a><span data-ttu-id="af023-103">Κοστολόγηση γραμμών σύμβασης βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="af023-103">Costing product-based contract lines</span></span>

<span data-ttu-id="af023-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="af023-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="af023-105">Οι γραμμές σύμβασης βασισμένες σε προϊόντα στο Dynamics 365 Project Operations περιλαμβάνουν το πεδίο **Τιμή κόστους** , το οποίο αποθηκεύει την τιμή κόστους του προϊόντος για τους υπολογισμούς κερδοφορίας κατάντη.</span><span class="sxs-lookup"><span data-stu-id="af023-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="af023-106">Όταν δημιουργείται μια γραμμή σύμβασης βάσει προϊόντων για ένα προϊόν καταλόγου, το κόστος της γραμμής προσφοράς βάσει προϊόντων είναι προεπιλεγμένο από το πεδίο **Τυπικό κόστος** στον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="af023-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="af023-107">Το πεδίο **Τυπικό κόστος** στον κατάλογο προϊόντων ορίζεται στη βασική νομισματική μονάδα του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="af023-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="af023-108">Όταν το κόστος μονάδας προεπιλέγεται στη γραμμή σύμβασης, μετατρέπεται σε νόμισμα πωλήσεων στη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="af023-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="af023-109">Κόστος μονάδας σε γραμμή σύμβασης βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="af023-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="af023-110">Ο σκοπός της ύπαρξης ενός κόστους μονάδας σε μια γραμμή σύμβασης βασισμένης σε προϊόντα είναι να επιτρέπεται διαφορετικό κόστος για ένα προϊόν για κάθε πώληση μονάδας.</span><span class="sxs-lookup"><span data-stu-id="af023-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="af023-111">Παρόλο που δεν είναι πάντα απαραίτητο, υπάρχουν ορισμένα σενάρια στα οποία το κόστος του προϊόντος μπορεί να έχει έκπτωση για τον πελάτη από τον προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="af023-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="af023-112">Σκεφτείτε το ακόλουθο σενάριο:</span><span class="sxs-lookup"><span data-stu-id="af023-112">Consider the following scenario:</span></span>

<span data-ttu-id="af023-113">Η Fabrikam Robotics εγκαθιστά ρομποτικούς βραχίονες στις γραμμές συναρμολόγησης της Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="af023-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="af023-114">Η Fabrikam παρέχει υπηρεσίες εγκατάστασης, αλλά οι ρομποτικοί βραχίονες παρέχονται από την Trey Research.</span><span class="sxs-lookup"><span data-stu-id="af023-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="af023-115">Εάν η εγκατάσταση των ρομποτικών βραχιόνων στη Adatum Corporation ανοίγει μια νέα βιομηχανία κάθετη για τους ρομποτικούς βραχίονες της Trey Research, τότε η Trey μπορεί να δώσει μια ειδική έκπτωση για την εν λόγω συμφωνία στη Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="af023-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="af023-116">Σε αυτήν την περίπτωση, η Fabrikam δημιουργεί μια γραμμή σύμβασης με βάση τα προϊόντα για ρομποτικούς βραχίονες και καταχωρίζει ένα κόστος ανά μονάδα για αυτήν τη σύμβαση, η οποία είναι διαφορετική από το τυπικό κόστος των ρομποτικών βραχιόνων από την Trey Research.</span><span class="sxs-lookup"><span data-stu-id="af023-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
