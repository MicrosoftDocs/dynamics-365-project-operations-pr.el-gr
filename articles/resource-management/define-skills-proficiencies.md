---
title: Ορισμός δεξιοτήτων και επαρκειών
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη ρύθμιση των μοντέλων επάρκειας για την αξιολόγηση πόρων.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d1ef50a3aa297ef439b54d37de629414ca66c820
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279678"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="23db7-103">Ορισμός δεξιοτήτων και επαρκειών</span><span class="sxs-lookup"><span data-stu-id="23db7-103">Define skills and proficiencies</span></span>

<span data-ttu-id="23db7-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="23db7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="23db7-105">Οι δεξιότητες είναι χαρακτηριστικά πόρου τα οποία είναι κοινόχρηστα στο Dynamics 365 Project Operations και αν υπάρχουν στο Dynamics 365 Field Service.</span><span class="sxs-lookup"><span data-stu-id="23db7-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="23db7-106">Για να διατηρήσετε το αρχείο φύλαξης δεξιοτήτων στο Project Operations, μεταβείτε στα στοιχεία **Πόροι** \> **Δεξιότητες πόρων**.</span><span class="sxs-lookup"><span data-stu-id="23db7-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="23db7-107">Χρήση μοντέλων επάρκειας για την αξιολόγηση πόρων</span><span class="sxs-lookup"><span data-stu-id="23db7-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="23db7-108">Οι δεξιότητες για τους πόρους εκτιμάται από τα μοντέλα επάρκειας.</span><span class="sxs-lookup"><span data-stu-id="23db7-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="23db7-109">Οι μεμονωμένες αξιολογήσεις βρίσκονται σε ένα μοντέλο επάρκειας.</span><span class="sxs-lookup"><span data-stu-id="23db7-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="23db7-110">Για να δημιουργήσετε ένα μοντέλο επάρκειας, μεταβείτε στα στοιχεία **Πόροι** \> **Μοντέλα επάρκειας** και μετά **Νέο**.</span><span class="sxs-lookup"><span data-stu-id="23db7-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="23db7-111">Στο νέο μοντέλο αξιολόγησης, καθορίστε την ελάχιστη τιμή αξιολόγησης, τη μέγιστη τιμή αξιολόγησης και την οντότητα που αξιολογείται.</span><span class="sxs-lookup"><span data-stu-id="23db7-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="23db7-112">Στο υποπλέγμα **Τιμές αξιολόγησης** μπορείτε να καθορίσετε τις διαφορετικές τιμές αξιολόγησης, από την ελάχιστη έως τη μέγιστη.</span><span class="sxs-lookup"><span data-stu-id="23db7-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="23db7-113">Αυτές οι τιμές αξιολόγησης εμφανίζονται στα φίλτρα **"Απαιτήσεις πόρου**, **Πίνακας χρονοδιαγράμματος** και **Βοηθός χρονοδιαγράμματος**.</span><span class="sxs-lookup"><span data-stu-id="23db7-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]