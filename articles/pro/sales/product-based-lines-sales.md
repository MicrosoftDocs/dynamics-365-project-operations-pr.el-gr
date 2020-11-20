---
title: Γραμμές ευκαιρίας βάσει προϊόντων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με στοιχεία γραμμών ευκαιρίας βάσει προϊόντων στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fd32bedb94cf36f706c112a845f342d9dde19805
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176326"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="b8c67-103">Γραμμές ευκαιρίας βάσει προϊόντων - lite</span><span class="sxs-lookup"><span data-stu-id="b8c67-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="b8c67-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="b8c67-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b8c67-105">Οι γραμμές ευκαιρίας που βασίζονται σε προϊόντα είναι στοιχεία γραμμής της ευκαιρίας.</span><span class="sxs-lookup"><span data-stu-id="b8c67-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="b8c67-106">Αυτές οι γραμμές παραδίδονται στον πελάτη ως διαφορετικά στοιχεία γραμμής στο τελικό τιμολόγιο χωρίς άλλες υπηρεσίες προστιθέμενης αξίας.</span><span class="sxs-lookup"><span data-stu-id="b8c67-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="b8c67-107">Οι συσχετισμένες δαπάνες και η κατανάλωση δεν παρακολουθούνται σε εργασίες οποιωνδήποτε σχετικών έργων.</span><span class="sxs-lookup"><span data-stu-id="b8c67-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="b8c67-108">Οι γραμμές βάσει προϊόντων μπορούν να είναι στοιχεία καταλόγου ή εγγεγραμμένων προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="b8c67-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="b8c67-109">Οι περισσότερες λειτουργίες στις γραμμές βάσει προϊόντων μιας ευκαιρίας ακολουθούν τη λειτουργικότητα που παρέχεται από την εφαρμογή Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="b8c67-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="b8c67-110">Για περισσότερες πληροφορίες σχετικά με τις γραμμές ευκαιριών που βασίζονται σε προϊόντα, ανατρέξτε στην ενότητα [Προσθήκη προϊόντων σε μια ευκαιρία](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="b8c67-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="b8c67-111">Μια έννοια σχετικά με τις γραμμές ευκαιριών βάσει προϊόντων που αφορά συγκεκριμένες ευκαιρίες βασισμένες σε έργα είναι ο **Προϋπολογισμός πελάτη**.</span><span class="sxs-lookup"><span data-stu-id="b8c67-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="b8c67-112">Χρησιμοποιήστε αυτό το πεδίο για να παρακολουθήσετε το ποσό που προτίθεται να καταβάλει ο πελάτης για το στοιχείο γραμμής.</span><span class="sxs-lookup"><span data-stu-id="b8c67-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="b8c67-113">Εάν η μέθοδος εσόδων της σύνοψης ευκαιριών έχει οριστεί σε **Υπολογίστηκε από το σύστημα**, οι τιμές προϋπολογισμού του πελάτη σε όλες τις γραμμές με βάση το προϊόν και τις γραμμές του έργου συνοψίζονται για τον υπολογισμό των εκτιμώμενων εσόδων.</span><span class="sxs-lookup"><span data-stu-id="b8c67-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
