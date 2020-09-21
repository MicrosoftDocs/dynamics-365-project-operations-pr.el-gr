---
title: Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας παραγγελιών πώλησης βάσει έργου για έργα χρόνου και υλικά έργα.
author: KimANelson
manager: AnnBe
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 05ab0cf6-318c-42de-ba56-3e662283497e
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 446c73e9491b1892847caf7e843c802292107ef9
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751550"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="50737-103">Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα</span><span class="sxs-lookup"><span data-stu-id="50737-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]
[!include[banner](../includes/preview-banner.md)]

<span data-ttu-id="50737-104">Αυτό το θέμα περιγράφει τον τρόπο δημιουργίας μιας παραγγελίας πώλησης για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="50737-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="50737-105">Οι παραγγελίες πώλησης μπορούν να δημιουργηθούν μόνο για έργα τύπου **χρόνος και υλικό**.</span><span class="sxs-lookup"><span data-stu-id="50737-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="50737-106">Εάν ένα έργο χρόνου και υλικού έχει πολλαπλές προελεύσεις χρηματοδότησης στη σύμβαση έργου, πρέπει να ενεργοποιήσετε την παράμετρο **Να επιτρέπονται παραγγελίες πώλησης για έργα με πολλαπλές προελεύσεις χρηματοδότησης** στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="50737-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="50737-107">Η υποστήριξη για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης είναι διαθέσιμη ξεκινώντας από την έκδοση 10.0.2 της εφαρμογής ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="50737-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="50737-108">Η παράμετρος για την ενεργοποίηση της υποστήριξης για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης θα καταργηθεί στο κύμα κυκλοφορίας του Απριλίου 2020, μετά το οποίο θα έχει ενεργοποιηθεί πάντα η λειτουργικότητα.</span><span class="sxs-lookup"><span data-stu-id="50737-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="50737-109">Μπορείτε να δημιουργήσετε παραγγελίες πώλησης βάσει έργου με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="50737-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="50737-110">Μεταβείτε στο ίδιο το έργο.</span><span class="sxs-lookup"><span data-stu-id="50737-110">Go to the project itself.</span></span> <span data-ttu-id="50737-111">Στο παράθυρο ενεργειών, επιλέξτε **Διαχείριση > Εργασίες στοιχείων > Παραγγελία πώλησης**.</span><span class="sxs-lookup"><span data-stu-id="50737-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="50737-112">Οι πληροφορίες έργου προεπιλέγουν την παραγγελία πώλησης από το έργο.</span><span class="sxs-lookup"><span data-stu-id="50737-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="50737-113">Εάν η σύμβαση έργου έχει περισσότερες από μία πηγές χρηματοδότησης, θα πρέπει να επιλέξετε την προέλευση χρηματοδότησης για να ορίσετε τον πελάτη για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="50737-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="50737-114">Εάν υπάρχει μόνο μία προέλευση χρηματοδότησης για το έργο, ο πελάτης θα οριστεί αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="50737-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="50737-115">Μεταβείτε στη σελίδα **Όλες οι παραγγελίες πώλησης** και δημιουργήστε μια νέα παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="50737-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="50737-116">Θα πρέπει να επιλέξετε το έργο για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="50737-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="50737-117">Μετά την επιλογή του έργου, ο πελάτης θα οριστεί από την προέλευση χρηματοδότησης ή θα πρέπει να επιλέξετε τον πηγαίο κώδικα χρηματοδότησης εάν η σύμβαση έργου έχει πολλαπλές προελεύσεις χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="50737-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>

