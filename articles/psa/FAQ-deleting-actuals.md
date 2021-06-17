---
title: Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το λόγο για τον οποίο δεν είναι δυνατή η διαγραφή καρτελών από την οντότητα πραγματικών τιμών.
author: JPBurrows
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
ms.openlocfilehash: 434be93cedb4772616b1e6d5cbe15fc715eed19a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993101"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="b9dc6-103">Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;</span><span class="sxs-lookup"><span data-stu-id="b9dc6-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b9dc6-104">Το Project Service Automation (PSA) δεν σας επιτρέπει να διαγράφετε πραγματικές τιμές επειδή χρησιμεύουν ως πηγή αλήθειας για συναλλαγές που έχουν οικονομικές επιπτώσεις σε συστήματα κατάντη, όπως η γενική λογιστική.</span><span class="sxs-lookup"><span data-stu-id="b9dc6-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="b9dc6-105">Εάν είναι δυνατή η διαγραφή των πραγματικών τιμών, η ακεραιότητα των συναλλαγών αναφοράς οικονομικών στοιχείων μπορεί να αμφισβητηθεί.</span><span class="sxs-lookup"><span data-stu-id="b9dc6-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="b9dc6-106">Για να δημιουργήσετε ένα ίχνος ελέγχου, οι πελάτες θα πρέπει να χρησιμοποιούν περιοδικά για τη δημιουργία αντιστάθμισης συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="b9dc6-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]