---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 29.5 Hotfix, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες για το Project Service Automation V3, έκδοση ενημέρωσης 29.5 Hotfix, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/26/2021
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
ms.openlocfilehash: d5050945c4ab7c1da61b07ec08bed20f32e166b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999176"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-295-v3"></a><span data-ttu-id="85b6d-103">Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 29.5, V3</span><span class="sxs-lookup"><span data-stu-id="85b6d-103">What's new or changed in Project Service Automation Update Release 29.5, V3</span></span>

<span data-ttu-id="85b6d-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="85b6d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="85b6d-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="85b6d-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="85b6d-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="85b6d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="85b6d-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="85b6d-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="85b6d-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="85b6d-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="85b6d-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 29.5.</span><span class="sxs-lookup"><span data-stu-id="85b6d-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.5.</span></span> <span data-ttu-id="85b6d-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.47.150 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Ιανουάριο του 2021.</span><span class="sxs-lookup"><span data-stu-id="85b6d-110">This version has a build number of V3.10.47.150 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-295"></a><span data-ttu-id="85b6d-111">Έκδοση κυκλοφορίας 29.5</span><span class="sxs-lookup"><span data-stu-id="85b6d-111">Update Release 29.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="85b6d-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="85b6d-112">Bug fixes</span></span>


<span data-ttu-id="85b6d-113">**Πωλήσεις**</span><span class="sxs-lookup"><span data-stu-id="85b6d-113">**Sales**</span></span>

<span data-ttu-id="85b6d-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="85b6d-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="85b6d-115">Σημειώνεται μια πιθανή μηδενική εξαίρεση αναφοράς στο **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** όταν κλείνετε μια προσφορά ως κερδισμένη και η προσφορά δεν έχει τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="85b6d-115">A possible null reference exception occurs in **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** when you close a quote as won and the quote has no price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
