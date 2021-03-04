---
title: Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το λόγο για τον οποίο δεν είναι δυνατή η διαγραφή καρτελών από την οντότητα πραγματικών τιμών.
author: JPBurrows
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 36cd241c7c7a2ff6ae018c94d691bc95d1f0c912
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148958"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="9e193-103">Γιατί δεν μπορώ να διαγράψω καρτέλες από την οντότητα πραγματικών τιμών;</span><span class="sxs-lookup"><span data-stu-id="9e193-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9e193-104">Το Project Service Automation (PSA) δεν σας επιτρέπει να διαγράφετε πραγματικές τιμές επειδή χρησιμεύουν ως πηγή αλήθειας για συναλλαγές που έχουν οικονομικές επιπτώσεις σε συστήματα κατάντη, όπως η γενική λογιστική.</span><span class="sxs-lookup"><span data-stu-id="9e193-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="9e193-105">Εάν είναι δυνατή η διαγραφή των πραγματικών τιμών, η ακεραιότητα των συναλλαγών αναφοράς οικονομικών στοιχείων μπορεί να αμφισβητηθεί.</span><span class="sxs-lookup"><span data-stu-id="9e193-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="9e193-106">Για να δημιουργήσετε ένα ίχνος ελέγχου, οι πελάτες θα πρέπει να χρησιμοποιούν περιοδικά για τη δημιουργία αντιστάθμισης συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="9e193-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

