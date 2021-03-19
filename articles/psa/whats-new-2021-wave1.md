---
title: Τι νέο υπάρχει ή τι άλλαξε στο Project Service Automation κύμα πρώιμης πρόσβασης 1 2021, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες για το Project Service Automation κύμα πρώιμης πρόσβασης 1 2021, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2021
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
ms.openlocfilehash: d99906b11b0189fc8227accd68bd0457f6baa42c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281163"
---
# <a name="whats-new-or-changed-in-project-service-automation-early-access-wave-1-2021-v3"></a><span data-ttu-id="3daaf-103">Τι νέο υπάρχει ή τι άλλαξε στο Project Service Automation κύμα πρώιμης πρόσβασης 1 2021, V3</span><span class="sxs-lookup"><span data-stu-id="3daaf-103">What's new or changed in Project Service Automation Early Access Wave 1 2021, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

## <a name="project-service-automation-early-access-wave-1-2021-v3"></a><span data-ttu-id="3daaf-104">Project Service Automation κύμα πρώιμης πρόσβασης 1 2021, V3</span><span class="sxs-lookup"><span data-stu-id="3daaf-104">Project Service Automation Early Access Wave 1 2021, V3</span></span>

<span data-ttu-id="3daaf-105">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="3daaf-105">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="3daaf-106">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="3daaf-106">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="3daaf-107">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="3daaf-107">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="3daaf-108">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="3daaf-108">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="3daaf-109">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="3daaf-109">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="3daaf-110">Αυτό το θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι νέες ή έχουν αλλάξει για το Project Service Automation κύμα πρώιμης πρόσβασης 1 2021, V3.</span><span class="sxs-lookup"><span data-stu-id="3daaf-110">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Early Access Wave 1 2021.</span></span> <span data-ttu-id="3daaf-111">Αυτή η έκδοση έχει αριθμό δομής V3.10.49.3 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Φεβρουάριο 2021.</span><span class="sxs-lookup"><span data-stu-id="3daaf-111">This version has a build number of V3.10.49.3 and is generally available through a self-update in February 2021.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="3daaf-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="3daaf-112">Bug fixes</span></span>

<span data-ttu-id="3daaf-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="3daaf-113">**Time and Expense**</span></span>

<span data-ttu-id="3daaf-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="3daaf-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="3daaf-115">Οι ημερομηνίες λήξης συμπληρώνονται αυτόματα όταν δημιουργείται μια καταχώρηση χρόνου, εάν η διάρκεια είναι null.</span><span class="sxs-lookup"><span data-stu-id="3daaf-115">End dates auto-populate when a time entry is created if the duration is null.</span></span>
- <span data-ttu-id="3daaf-116">Οι χρήστες μπορούν να αλλάξουν την εργασία σε μια καταχώρηση ώρας που έχει εγκριθεί ή υποβληθεί.</span><span class="sxs-lookup"><span data-stu-id="3daaf-116">Users can change the task on a time entry that has been approved or submitted.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]