---
title: Ρύθμιση συντελεστών πωλήσεων και κόστους για τα προϊόντα καταλόγου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης των ποσοστών κόστους και πώλησης για στοιχεία στον κατάλογο προϊόντων.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 135b182af73bdab7a3520589431332ad059ec497
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176701"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="d2dbb-103">Ρύθμιση συντελεστών πωλήσεων και κόστους για τα προϊόντα καταλόγου - lite</span><span class="sxs-lookup"><span data-stu-id="d2dbb-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="d2dbb-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="d2dbb-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="d2dbb-105">Η ρύθμιση για τα στοιχεία καταλόγου προϊόντων στο Dynamics 365 Project Operations είναι η ίδια με αυτήν του Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="d2dbb-106">Επειδή τα προϊόντα δεν είναι δυνατό να υπολογιστούν ή να χρησιμοποιηθούν στο Project Operations, δεν χρειάζεται να ορίσετε τις τιμές καταλόγου προϊόντων σε τιμοκαταλόγους έργου για προσφορές και συμβάσεις.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="d2dbb-107">Οι τιμές καταλόγου προϊόντων πρέπει να οριστούν στο πεδίο **Τιμή προϊόντος** μιας προσφοράς, μιας σύμβασης ή ενός λογαριασμού.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="d2dbb-108">Μη ρυθμίζετε τις τιμές καταλόγου προϊόντων στους καταλόγους τιμών έργου για αυτές τις οντότητες.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="d2dbb-109">Οι τιμοκατάλογοι έργου αφορούν αποκλειστικά το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="d2dbb-110">Υπάρχει επιχειρηματική λογική που αφορά συγκεκριμένες εφαρμογές, η οποία αντιγράφει τους τιμοκαταλόγους από μια προσφορά σε μια σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="d2dbb-111">Το αποτέλεσα είναι ένας τιμοκατάλογος έργου συγκεκριμένη σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="d2dbb-112">Η λειτουργία αντιγραφής μπορεί να καθυστερήσει τη διεργασία κέρδους προσφοράς, εάν ο τιμοκατάλογος έργου στην προσφορά γίνει πολύ μεγάλος.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="d2dbb-113">Οι τιμοκατάλογοι προϊόντων δεν αντιγράφονται για τη δημιουργία προσαρμοσμένων λιστών τιμών σε συμβάσεις.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="d2dbb-114">Αυτό σημαίνει ότι οι τιμοκατάλογοι προϊόντων δεν επηρεάζουν την απόδοση της διαδικασίας κέρδους προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="d2dbb-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
