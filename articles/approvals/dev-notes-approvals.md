---
title: Σημειώσεις προγραμματιστή για εγκρίσεις
description: Αυτό το θέμα παρέχει πρόσθετες πληροφορίες προγραμματιστή σχετικά με την εργασία με εγκρίσεις.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483948"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="12fb7-103">Σημειώσεις προγραμματιστή για εγκρίσεις</span><span class="sxs-lookup"><span data-stu-id="12fb7-103">Developer notes for Approvals</span></span>

<span data-ttu-id="12fb7-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="12fb7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="12fb7-105">Το Dynamics 365 Project Operations περιλαμβάνει λογική επικύρωσης που διασφαλίζει τη σωστή μετάβαση καρτέλας μέσω των σταδίων έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="12fb7-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="12fb7-106">Οι σωστές μεταβάσεις καρτελών εξασφαλίζουν τα εξής:</span><span class="sxs-lookup"><span data-stu-id="12fb7-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="12fb7-107">Όλες οι γραμμές υποστήριξης δημιουργούνται σε σχετιζόμενους πίνακες, όπως τα ημερολόγια και οι πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="12fb7-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="12fb7-108">Ο υπεύθυνος έγκρισης επισημαίνεται ως **Υπεύθυνος έγκρισης έργου** στο έργο πριν προχωρήσετε.</span><span class="sxs-lookup"><span data-stu-id="12fb7-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>
