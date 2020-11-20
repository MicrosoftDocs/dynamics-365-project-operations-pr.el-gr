---
title: Κοστολόγηση γραμμών προσφοράς βάσει προϊόντων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εφαρμογή μιας τιμής κόστους σε μια γραμμή προσφοράς βάσει προϊόντων.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d21ab159294cac66ffeb8abcf0943b4babd7b360
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118923"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="7e032-103">Κοστολόγηση γραμμών προσφοράς βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="7e032-103">Costing product-based quote lines</span></span>

<span data-ttu-id="7e032-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="7e032-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="7e032-105">Οι γραμμές προσφοράς βάσει προϊόντων στο Dynamics 365 Project Operations έχουν επίσης ένα πεδίο **Τιμή κόστους**.</span><span class="sxs-lookup"><span data-stu-id="7e032-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="7e032-106">Αυτό το πεδίο χρησιμοποιείται για την παρακολούθηση της τιμής κόστους για το προϊόν στη γραμμή προσφοράς και για τους υπολογισμούς κατάντη κερδοφορίας.</span><span class="sxs-lookup"><span data-stu-id="7e032-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="7e032-107">Όταν δημιουργείται μια γραμμή προσφοράς βασισμένης σε προϊόντα για ένα προϊόν καταλόγου, το κόστος της γραμμής προσφοράς με βάση τα προϊόντα είναι προεπιλεγμένο από το πεδίο **Τυπικό κόστος** στον κατάλογο προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="7e032-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="7e032-108">Το πεδίο "τυπικό κόστος" στον κατάλογο προϊόντων ορίζεται στη βασική νομισματική μονάδα του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="7e032-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="7e032-109">Το προεπιλεγμένο κόστος μονάδας στη γραμμή προσφοράς με βάση τα προϊόντα μετατρέπεται στη νομισματική μονάδα πώλησης της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="7e032-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="7e032-110">Κόστος μονάδας σε γραμμή προσφοράς βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="7e032-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="7e032-111">Ο σκοπός της ύπαρξης ενός κόστους μονάδας σε μια γραμμή προσφοράς βασισμένης σε προϊόντα είναι να επιτρέπεται διαφορετικό κόστος για ένα προϊόν για κάθε πώληση.</span><span class="sxs-lookup"><span data-stu-id="7e032-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="7e032-112">Αυτό δεν είναι ένα τυπικό σενάριο, αλλά μερικές φορές το κόστος του προϊόντος μπορεί να έχει έκπτωση από τον προμηθευτή, ανάλογα με τον πελάτη της τελικής πώλησης.</span><span class="sxs-lookup"><span data-stu-id="7e032-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="7e032-113">Για παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="7e032-113">For example:</span></span>

<span data-ttu-id="7e032-114">Η Fabrikam Robotics εγκαθιστά ρομποτικούς βραχίονες στις γραμμές συναρμολόγησης της A Datum Corporation.</span><span class="sxs-lookup"><span data-stu-id="7e032-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="7e032-115">Η Fabrikam παρέχει υπηρεσίες εγκατάστασης, αλλά οι ρομποτικοί βραχίονες παρέχονται από την Trey robotics.</span><span class="sxs-lookup"><span data-stu-id="7e032-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="7e032-116">Εάν η εγκατάσταση των ρομποτικών βραχιόνων στη A Datum Corporation ανοίγει μια νέα βιομηχανία κάθετη για τους ρομποτικούς βραχίονες της Trey, τότε η Trey μπορεί να δώσει μια ειδική έκπτωση για την εν λόγω συμφωνία στη Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="7e032-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="7e032-117">Σε αυτήν την περίπτωση, η Fabrikam θα δημιουργήσει μια γραμμή προσφοράς βασισμένη σε προϊόντα για ρομποτικούς βραχίονες και θα εισαγάγει ένα ειδικό κόστος ανά μονάδα για αυτήν την προσφορά.</span><span class="sxs-lookup"><span data-stu-id="7e032-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="7e032-118">Αυτό το κόστος διαφέρει από το τυπικό κόστος των ρομποτικών βραχιόνων της Trey.</span><span class="sxs-lookup"><span data-stu-id="7e032-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
