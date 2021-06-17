---
title: Ενοποίηση διπλής εγγραφής Project Operations
description: Αυτό το θέμα παρέχει μια επισκόπηση της ενοποίησης διπλής εγγραφής Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998681"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="ee312-103">Επισκόπηση ενοποίησης διπλής εγγραφής Project Operations</span><span class="sxs-lookup"><span data-stu-id="ee312-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="ee312-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="ee312-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ee312-105">Το Project Operations χρησιμοποιεί [δυνατότητες διπλής εγγραφής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) για το συγχρονισμό δεδομένων μεταξύ Microsoft Dataverse και Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="ee312-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="ee312-106">Η εικόνα που ακολουθεί δείχνει τον τρόπο συγχρονισμού των δεδομένων στο πλαίσιο αυτής της ενοποίησης μεταξύ Dataverse και Οικονομικών.</span><span class="sxs-lookup"><span data-stu-id="ee312-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Επισκόπηση ροών δεδομένων Project Operations](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="ee312-108">Το Project Operations στο Dataverse παρέχει ένα σύγχρονο περιβάλλον εργασίας χρήστη (UI) και εύκολη επεκτασιμότητα χωρίς κώδικα/χαμηλό κώδικα, χρησιμοποιώντας τις δυνατότητες του Power Platform.</span><span class="sxs-lookup"><span data-stu-id="ee312-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="ee312-109">Οι διαχειριστές έργου, οι διαχειριστές πόρων, τα μέλη ομάδας έργου και άλλα άτομα προσκηνίου, εκτελούν τις δραστηριότητές τους στο Project Operations στο Dataverse.</span><span class="sxs-lookup"><span data-stu-id="ee312-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="ee312-110">Το Project Operations στα οικονομικά παρέχουν υποστήριξη για τη λογιστική έργων και την αναγνώριση των εσόδων.</span><span class="sxs-lookup"><span data-stu-id="ee312-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="ee312-111">Το Project Operations κάνει προσθήκες στο οικονομικό πλαίσιο των Οικονομικών για τον υπολογισμό του φόρου πωλήσεων, τις νομισματικές ισοτιμίες, τις αναφορές οικονομικών διαστάσεων και πολλά άλλα.</span><span class="sxs-lookup"><span data-stu-id="ee312-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="ee312-112">Οι εμπειρίες του Λογιστή έργου βασίζονται κυρίως στα Οικονομικά.</span><span class="sxs-lookup"><span data-stu-id="ee312-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="ee312-113">Η ενοποίηση του Project Operations αποτελείται από το παρακάτω στοιχείο ενοποίησης:</span><span class="sxs-lookup"><span data-stu-id="ee312-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="ee312-114">Ρύθμιση Project Operations και ρύθμιση παραμέτρων ενοποίησης δεδομένων</span><span class="sxs-lookup"><span data-stu-id="ee312-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="ee312-115">Εκτιμήσεις έργου και πραγματικές τιμές</span><span class="sxs-lookup"><span data-stu-id="ee312-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="ee312-116">Τιμολόγια έργου</span><span class="sxs-lookup"><span data-stu-id="ee312-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="ee312-117">Διαχείριση εξόδων</span><span class="sxs-lookup"><span data-stu-id="ee312-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="ee312-118">Τιμολόγιο προμηθευτή</span><span class="sxs-lookup"><span data-stu-id="ee312-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
