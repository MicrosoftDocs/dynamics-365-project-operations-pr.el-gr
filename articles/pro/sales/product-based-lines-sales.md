---
title: Γραμμές ευκαιρίας βάσει προϊόντων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με στοιχεία γραμμών ευκαιρίας βάσει προϊόντων στο Project Operations.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7865da682ae607f017bf59ce1ae1addc9fefa60b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994496"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="89076-103">Γραμμές ευκαιρίας βάσει προϊόντων - lite</span><span class="sxs-lookup"><span data-stu-id="89076-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="89076-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="89076-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="89076-105">Οι γραμμές ευκαιρίας που βασίζονται σε προϊόντα είναι στοιχεία γραμμής της ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="89076-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="89076-106">Αυτά τα διακριτά στοιχεία γραμμής βρίσκονται στο τελικό τιμολόγιο που παρέχεται στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="89076-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="89076-107">Το τιμολόγιο δεν περιλαμβάνει άλλες πρόσθετες υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="89076-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="89076-108">Οι συσχετισμένες δαπάνες και η κατανάλωση δεν παρακολουθούνται σε εργασίες οποιωνδήποτε σχετικών έργων.</span><span class="sxs-lookup"><span data-stu-id="89076-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="89076-109">Οι γραμμές βάσει προϊόντων μπορούν να είναι στοιχεία καταλόγου ή εγγεγραμμένων προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="89076-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="89076-110">Οι περισσότερες λειτουργίες στις γραμμές βάσει προϊόντων μιας ευκαιρίας ακολουθούν τη λειτουργικότητα που παρέχεται από την εφαρμογή Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="89076-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="89076-111">Για περισσότερες πληροφορίες σχετικά με τις γραμμές ευκαιριών που βασίζονται σε προϊόντα, ανατρέξτε στην ενότητα [Προσθήκη προϊόντων σε μια ευκαιρία](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="89076-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="89076-112">Ο **προϋπολογισμός πελάτη** είναι μια έννοια που αφορά ειδικά τις γραμμές ευκαιρίας βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="89076-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="89076-113">Το πεδίο **Προϋπολογισμός πελάτη** παρακολουθεί το ποσό που έχει πληρώσει ο πελάτης για το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="89076-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="89076-114">Όταν η μέθοδος εσόδων της σύνοψης ευκαιρίας **Υπολογίζεται από το σύστημα**, οι τιμές του προϋπολογισμού πελάτη στις γραμμές ευκαιρίας συνοψίζονται για τον υπολογισμό των εκτιμώμενων εσόδων.</span><span class="sxs-lookup"><span data-stu-id="89076-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]