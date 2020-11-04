---
title: Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το λόγο για τον οποίο δεν είναι δυνατή η διαγραφή καρτελών από την οντότητα πραγματικών τιμών.
author: JPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: f47e7ccd46642dc6129fbb3beac3c9490160d046
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077042"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="460fb-103">Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;</span><span class="sxs-lookup"><span data-stu-id="460fb-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="460fb-104">Το Project Service Automation (PSA) δεν σας επιτρέπει να διαγράφετε πραγματικές τιμές επειδή χρησιμεύουν ως πηγή αλήθειας για συναλλαγές που έχουν οικονομικές επιπτώσεις σε συστήματα κατάντη, όπως η γενική λογιστική.</span><span class="sxs-lookup"><span data-stu-id="460fb-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="460fb-105">Εάν είναι δυνατή η διαγραφή των πραγματικών τιμών, η ακεραιότητα των συναλλαγών αναφοράς οικονομικών στοιχείων μπορεί να αμφισβητηθεί.</span><span class="sxs-lookup"><span data-stu-id="460fb-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="460fb-106">Για να δημιουργήσετε ένα ίχνος ελέγχου, οι πελάτες θα πρέπει να χρησιμοποιούν περιοδικά για τη δημιουργία αντιστάθμισης συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="460fb-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

