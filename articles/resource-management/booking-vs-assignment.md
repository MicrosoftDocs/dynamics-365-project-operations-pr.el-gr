---
title: Κρατήσεις έναντι αναθέσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις διαφορές μεταξύ των κρατήσεων πόρων και των αναθέσεων πόρων.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076765"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="985d1-103">Κρατήσεις έναντι αναθέσεων</span><span class="sxs-lookup"><span data-stu-id="985d1-103">Bookings vs assignments</span></span>

<span data-ttu-id="985d1-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="985d1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="985d1-105">Οι κρατήσεις είναι η εκχώρηση πόρων σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="985d1-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="985d1-106">Με τη χρήση κρατήσεων καταναλώνεται η παραγωγική ικανότητα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="985d1-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="985d1-107">Οι αναθέσεις είναι η ανάθεση πόρων σε εργασίες έργου του χρονοδιαγράμματος έργου.</span><span class="sxs-lookup"><span data-stu-id="985d1-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="985d1-108">Οι πόροι μπορεί να είναι είτε πραγματικοί είτε γενικοί.</span><span class="sxs-lookup"><span data-stu-id="985d1-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="985d1-109">Ιδανικά, για πραγματικούς πόρους, οι κρατήσεις και οι αναθέσεις πρέπει να συμφωνούν, επειδή δεν διαφέρουν.</span><span class="sxs-lookup"><span data-stu-id="985d1-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="985d1-110">Ωστόσο, το Microsoft Dynamics Project Operations δεν επιβάλλει την εν λόγω συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="985d1-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="985d1-111">Η προβολή **Εναρμόνιση** εμφανίζει μια θέση του διευθυντή έργου όπου οι κρατήσεις και οι αναθέσεις ενός πόρου δεν συμφωνούν.</span><span class="sxs-lookup"><span data-stu-id="985d1-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>