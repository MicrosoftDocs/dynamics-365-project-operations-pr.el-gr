---
title: Ενημέρωση εκτίμησης κατά την ολοκλήρωση
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την ενημέρωση της προβολής της προσπάθειας σε ένα έργο.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 59d04869839cebd6e197f94f2ada8ab12c495c3b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127203"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="29929-103">Ενημέρωση εκτίμησης κατά την ολοκλήρωση</span><span class="sxs-lookup"><span data-stu-id="29929-103">Update estimate at completion</span></span>

<span data-ttu-id="29929-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="29929-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="29929-105">Είναι σύνηθες για έναν υπεύθυνο έργου να αναθεωρεί τις αρχικές εκτιμήσεις σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="29929-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="29929-106">Οι εκ νέου προβολές των προβολών έργου είναι η αντίληψη του υπεύθυνου έργου για τις προβλέψεις, δεδομένης της τρέχουσας κατάστασης ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="29929-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="29929-107">Δεν συνιστούμε οι υπεύθυνοι έργου να αλλάξουν τους αριθμούς βασικής γραμμής επειδή η βασική γραμμή του έργου είναι η καθορισμένη προέλευση της αλήθειας για τις εκτιμήσεις χρονοδιαγράμματος και κόστους του έργου με τις οποίες έχουν συμφωνήσει όλοι οι ενδιαφερόμενοι στο έργο.</span><span class="sxs-lookup"><span data-stu-id="29929-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="29929-108">Υπάρχουν δύο τρόποι με τους οποίους ένας υπεύθυνος έργου μπορεί να επαναλάβει την προσπάθεια έργου στις εργασίες:</span><span class="sxs-lookup"><span data-stu-id="29929-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="29929-109">Παράκαμψη της προεπιλεγμένης εκτίμησης προς ολοκλήρωση (ETC) με μια νέα εκτίμηση της πραγματικής εναπομένουσας προσπάθειας για την εργασία.</span><span class="sxs-lookup"><span data-stu-id="29929-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="29929-110">Παράκαμψη του προεπιλεγμένου ποσοστού προόδου με μια νέα εκτίμηση της πραγματικής προόδου της εργασίας.</span><span class="sxs-lookup"><span data-stu-id="29929-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="29929-111">Κάθε μία από αυτές τις προσεγγίσεις προκαλεί έναν εκ νέου υπολογισμό του ETC, της εκτίμησης κατά την ολοκλήρωση (ΕΚΟ) και της ποσοστιαίας προόδου της εργασίας και της διακύμανσης προβαλλόμενης προσπάθειας σε μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="29929-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="29929-112">Υπολογίζονται εκ νέου το ποσοστό ΕΚΟ, ETC και προόδου στις εργασίες σύνοψης και παράγεται μια νέα προβολή της διακύμανσης της προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="29929-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
