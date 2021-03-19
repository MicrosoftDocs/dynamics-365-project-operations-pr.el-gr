---
title: Ρύθμιση συντελεστών πωλήσεων και κόστους για τα προϊόντα καταλόγου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης των ποσοστών κόστους και πώλησης για στοιχεία στον κατάλογο προϊόντων.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0941c549cc38f0938a5819e8cb6ca9912f14790
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274458"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="a3f5c-103">Ρύθμιση συντελεστών πωλήσεων και κόστους για τα προϊόντα καταλόγου - lite</span><span class="sxs-lookup"><span data-stu-id="a3f5c-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="a3f5c-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="a3f5c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="a3f5c-105">Ο καθορισμός τιμολόγησης για τα στοιχεία τιμοκαταλόγου στο Dynamics 365 Project Operations είναι ίδιος με το Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="a3f5c-106">Στο Project Operations, τα προϊόντα δεν μπορούν να υπολογιστούν ή να χρησιμοποιηθούν σε έργα, επομένως οι τιμές του καταλόγου προϊόντων δεν χρειάζεται να ορίζεται σε τιμοκαταλόγους έργου για προσφορές και συμβάσεις.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="a3f5c-107">Χρησιμοποιήστε το πεδίο **Τιμή προϊόντος** για μια προσφορά, μια σύμβαση ή έναν λογαριασμό για να ορίσετε τις τιμές του καταλόγου προϊόντων.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="a3f5c-108">Μην ορίσετε τιμές καταλόγου προϊόντων στους τιμοκαταλόγους έργου.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="a3f5c-109">Οι τιμοκατάλογοι έργου αφορούν αποκλειστικά το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="a3f5c-110">Η επιχειρηματική λογική ειδικά για μια εφαρμογή αντιγράφει τους τιμοκαταλόγους από μια προσφορά σε μια σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="a3f5c-111">Το αποτέλεσα είναι ένας τιμοκατάλογος έργου συγκεκριμένη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="a3f5c-112">Η λειτουργία αντιγραφής μπορεί να καθυστερήσει τη διεργασία κέρδους προσφοράς, εάν ο τιμοκατάλογος έργου στην προσφορά γίνει πολύ μεγάλος.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="a3f5c-113">Οι τιμοκατάλογοι προϊόντων δεν αντιγράφονται για τη δημιουργία προσαρμοσμένων λιστών τιμών σε συμβάσεις.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="a3f5c-114">Επειδή δεν υπάρχει αντιγραφή, η απόδοση της διεργασίας προσφοράς δεν επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="a3f5c-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]