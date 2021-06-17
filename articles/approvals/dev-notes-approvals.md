---
title: Σημειώσεις προγραμματιστή για εγκρίσεις
description: Αυτό το θέμα παρέχει πρόσθετες πληροφορίες προγραμματιστή σχετικά με την εργασία με εγκρίσεις.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996791"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="3edeb-103">Σημειώσεις προγραμματιστή για εγκρίσεις</span><span class="sxs-lookup"><span data-stu-id="3edeb-103">Developer notes for Approvals</span></span>

<span data-ttu-id="3edeb-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="3edeb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3edeb-105">Το Dynamics 365 Project Operations περιλαμβάνει λογική επικύρωσης που διασφαλίζει τη σωστή μετάβαση καρτέλας μέσω των σταδίων έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="3edeb-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="3edeb-106">Οι σωστές μεταβάσεις καρτελών εξασφαλίζουν τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3edeb-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="3edeb-107">Όλες οι γραμμές υποστήριξης δημιουργούνται σε σχετιζόμενους πίνακες, όπως τα ημερολόγια και οι πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="3edeb-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="3edeb-108">Ο υπεύθυνος έγκρισης επισημαίνεται ως **Υπεύθυνος έγκρισης έργου** στο έργο πριν προχωρήσετε.</span><span class="sxs-lookup"><span data-stu-id="3edeb-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]