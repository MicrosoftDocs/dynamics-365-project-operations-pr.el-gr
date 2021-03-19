---
title: Χρήση υπάρχοντος πεδίου στο Project Service ως διάσταση τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση των υπαρχόντων πεδίων Project Service ως διαστάσεις τιμολόγησης.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: ad03f5f7c1c9e93ca12a8c8d48ffbd2f80b1511f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281568"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="1c6f8-103">Χρήση υπάρχοντος πεδίου στο Project Service ως διάσταση τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="1c6f8-103">Use an existing field in Project Service as a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1c6f8-104">Το Project Service Automation (PSA) διαθέτει πολλά πεδία στην οντότητα **Πραγματικές τιμές** τα οποία μπορούν να χρησιμοποιηθούν ως διαστάσεις τιμολόγησης για τιμολόγηση βασισμένη σε πόρους στους οργανισμούς έργου.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="1c6f8-105">Για παράδειγμα, ένα συνηθισμένο πεδίο είναι ο **Πόρος με δυνατότητα κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="1c6f8-106">Οι μικρότερες εταιρείες με λιγότερους από 20-30 πόρους με δυνατότητα χρέωσης μπορεί να διαπιστώσουν ότι η ύπαρξη ποσοστού τιμολόγησης και κόστους για κάθε πόρο είναι μια απλούστερη προσέγγιση.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="1c6f8-107">Ωστόσο, καθώς το χρεώσιμο εργατικό δυναμικό μεγαλώνει, οι συγκεκριμένες τιμές θα μπορούσαν να γίνουν μη ρεαλιστικές για τη διατήρηση του κόστους πόρου και τα ποσοστά χρέωσης αρχίζουν να ποικίλλουν καθώς οι πόροι προωθούνται, αποκτούν περισσότερη εμπειρία ή αποκτούν διαφορετικά σύνολα δεξιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-107">However, as the billable workforce grows, specific rates could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill set.</span></span> <span data-ttu-id="1c6f8-108">Επειδή αυτή η προσέγγιση εξακολουθεί να ισχύει για εταιρείες συγκεκριμένου μεγέθους, ανατρέξτε στο θέμα [Χρησιμοποιήστε έναν πόρο με δυνατότητα κράτησης ως διάσταση τιμολόγησης](bookable-resource-pricing-dimension.md) για να κατανοήσετε τον τρόπο με τον οποίο ένα υπάρχον πεδίο Project Service μπορεί να χρησιμοποιηθεί ως διάσταση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-108">Because this approach still works for companies of a certain size, see [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="1c6f8-109">Ένα άλλο παράδειγμα είναι η κατηγορία των συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-109">Another example is that of transaction category.</span></span> <span data-ttu-id="1c6f8-110">Οι πελάτες και οι υπεύθυνοι υλοποίησης έχουν χρησιμοποιήσει την κατηγορία "συναλλαγή" στο PSA για να ταξινομήσουν την εργασία και να χρησιμοποιήσουν το πεδίο σε τιμή και κόστος με βάση την κατηγορία εργασίας.</span><span class="sxs-lookup"><span data-stu-id="1c6f8-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="1c6f8-111">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Χρήση της κατηγορίας συναλλαγών ως διάσταση τιμολόγησης](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="1c6f8-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]