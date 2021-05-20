---
title: Γραμμές ευκαιρίας βάσει προϊόντων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με στοιχεία γραμμών ευκαιρίας βάσει προϊόντων στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f7dfabd068e180c7122ede0f79aaebfe220250a1
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949544"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="14895-103">Γραμμές ευκαιρίας βάσει προϊόντων - lite</span><span class="sxs-lookup"><span data-stu-id="14895-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="14895-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="14895-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="14895-105">Οι γραμμές ευκαιρίας που βασίζονται σε προϊόντα είναι στοιχεία γραμμής της ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="14895-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="14895-106">Αυτά τα διακριτά στοιχεία γραμμής βρίσκονται στο τελικό τιμολόγιο που παρέχεται στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="14895-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="14895-107">Το τιμολόγιο δεν περιλαμβάνει άλλες πρόσθετες υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="14895-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="14895-108">Οι συσχετισμένες δαπάνες και η κατανάλωση δεν παρακολουθούνται σε εργασίες οποιωνδήποτε σχετικών έργων.</span><span class="sxs-lookup"><span data-stu-id="14895-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="14895-109">Οι γραμμές βάσει προϊόντων μπορούν να είναι στοιχεία καταλόγου ή εγγεγραμμένων προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="14895-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="14895-110">Οι περισσότερες λειτουργίες στις γραμμές βάσει προϊόντων μιας ευκαιρίας ακολουθούν τη λειτουργικότητα που παρέχεται από την εφαρμογή Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="14895-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="14895-111">Για περισσότερες πληροφορίες σχετικά με τις γραμμές ευκαιριών που βασίζονται σε προϊόντα, ανατρέξτε στην ενότητα [Προσθήκη προϊόντων σε μια ευκαιρία](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="14895-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="14895-112">Ο **προϋπολογισμός πελάτη** είναι μια έννοια που αφορά ειδικά τις γραμμές ευκαιρίας βάσει έργου.</span><span class="sxs-lookup"><span data-stu-id="14895-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="14895-113">Το πεδίο **Προϋπολογισμός πελάτη** παρακολουθεί το ποσό που έχει πληρώσει ο πελάτης για το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="14895-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="14895-114">Όταν η μέθοδος εσόδων της σύνοψης ευκαιρίας **Υπολογίζεται από το σύστημα**, οι τιμές του προϋπολογισμού πελάτη στις γραμμές ευκαιρίας συνοψίζονται για τον υπολογισμό των εκτιμώμενων εσόδων.</span><span class="sxs-lookup"><span data-stu-id="14895-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]