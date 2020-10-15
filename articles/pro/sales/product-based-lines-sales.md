---
title: Γραμμές ευκαιρίας βάσει προϊόντων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με στοιχεία γραμμών ευκαιρίας βάσει προϊόντων στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896236"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="732d6-103">Γραμμές ευκαιρίας βάσει προϊόντων</span><span class="sxs-lookup"><span data-stu-id="732d6-103">Product-based opportunity lines</span></span>

<span data-ttu-id="732d6-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="732d6-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="732d6-105">Οι γραμμές ευκαιρίας που βασίζονται σε προϊόντα είναι στοιχεία γραμμής της ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="732d6-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="732d6-106">Αυτές οι γραμμές παραδίδονται στον πελάτη ως διαφορετικά στοιχεία γραμμής στο τελικό τιμολόγιο χωρίς άλλες υπηρεσίες προστιθέμενης αξίας.</span><span class="sxs-lookup"><span data-stu-id="732d6-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="732d6-107">Οι συσχετισμένες δαπάνες και η κατανάλωση δεν παρακολουθούνται σε εργασίες οποιωνδήποτε σχετικών έργων.</span><span class="sxs-lookup"><span data-stu-id="732d6-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="732d6-108">Οι γραμμές βάσει προϊόντων μπορούν να είναι στοιχεία καταλόγου ή εγγεγραμμένων προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="732d6-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="732d6-109">Οι περισσότερες λειτουργίες στις γραμμές βάσει προϊόντων μιας ευκαιρίας ακολουθούν τη λειτουργικότητα που παρέχεται από την εφαρμογή Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="732d6-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="732d6-110">Για περισσότερες πληροφορίες σχετικά με τις γραμμές ευκαιριών που βασίζονται σε προϊόντα, ανατρέξτε στην ενότητα [Προσθήκη προϊόντων σε μια ευκαιρία](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="732d6-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="732d6-111">Μια έννοια σχετικά με τις γραμμές ευκαιριών βάσει προϊόντων που αφορά συγκεκριμένες ευκαιρίες βασισμένες σε έργα είναι ο **Προϋπολογισμός πελάτη**.</span><span class="sxs-lookup"><span data-stu-id="732d6-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="732d6-112">Χρησιμοποιήστε αυτό το πεδίο για να παρακολουθήσετε το ποσό που προτίθεται να καταβάλει ο πελάτης για το στοιχείο γραμμής.</span><span class="sxs-lookup"><span data-stu-id="732d6-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="732d6-113">Εάν η μέθοδος εσόδων της σύνοψης ευκαιριών έχει οριστεί σε **Υπολογίστηκε από το σύστημα**, οι τιμές προϋπολογισμού του πελάτη σε όλες τις γραμμές με βάση το προϊόν και τις γραμμές του έργου συνοψίζονται για τον υπολογισμό των εκτιμώμενων εσόδων.</span><span class="sxs-lookup"><span data-stu-id="732d6-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
