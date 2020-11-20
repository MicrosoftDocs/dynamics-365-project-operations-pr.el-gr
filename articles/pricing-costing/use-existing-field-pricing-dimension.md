---
title: Πεδία Project Operations Ρύθμιση ως διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση των πεδίων ως διαστάσεις τιμολόγησης στο Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: 59367b35f15f806b109f606e912edc487d9e7685
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119238"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="ccf1a-103">Πεδία Project Operations Ρύθμιση ως διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="ccf1a-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="ccf1a-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="ccf1a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ccf1a-105">Η οντότητα **Πραγματικές τιμές** έχει πολλά πεδία που μπορούν να χρησιμοποιηθούν ως διαστάσεις τιμολόγησης για τιμολόγηση βασισμένη σε πόρους.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="ccf1a-106">Για παράδειγμα, ένα συνηθισμένο πεδίο είναι ο **Πόρος με δυνατότητα κράτησης**.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="ccf1a-107">Οι μικρότερες εταιρείες με λιγότερους από 20-30 πόρους με δυνατότητα χρέωσης μπορεί να διαπιστώσουν ότι η ύπαρξη ποσοστού τιμολόγησης και κόστους για κάθε πόρο είναι μια απλούστερη προσέγγιση.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="ccf1a-108">Ωστόσο, καθώς το χρεώσιμο εργατικό δυναμικό αναπτύσσεται, οι τιμές για συγκεκριμένους πόρους ενδέχεται να μην είναι ρεαλιστικό να παραμείνουν ως έχουν.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="ccf1a-109">Το κόστος πόρων και οι χρεώσεις λογαριασμών αρχίζουν να ποικίλλουν καθώς οι πόροι προωθούνται, κερδίζουν περισσότερη εμπειρία ή αποκτούν ένα διαφορετικό σύνολο δεξιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="ccf1a-110">Ένα άλλο παράδειγμα είναι η κατηγορία των συναλλαγών.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-110">Another example is that of transaction category.</span></span> <span data-ttu-id="ccf1a-111">Οι πελάτες και οι υπεύθυνοι υλοποίησης έχουν χρησιμοποιήσει την κατηγορία συναλλαγής για να ταξινομήσουν την εργασία και να χρησιμοποιήσουν το πεδίο σε τιμή και κόστος με βάση την κατηγορία εργασίας.</span><span class="sxs-lookup"><span data-stu-id="ccf1a-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
