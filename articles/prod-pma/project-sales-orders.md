---
title: Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας παραγγελιών πώλησης βάσει έργου για έργα χρόνου και υλικά έργα.
author: Yowelle
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
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 74a90ea0bdb8f760273c0f6b1c61bffcb70b6c8d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289054"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="a7334-103">Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα</span><span class="sxs-lookup"><span data-stu-id="a7334-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="a7334-104">Αυτό το θέμα περιγράφει τον τρόπο δημιουργίας μιας παραγγελίας πώλησης για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="a7334-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="a7334-105">Οι παραγγελίες πώλησης μπορούν να δημιουργηθούν μόνο για έργα τύπου **χρόνος και υλικό**.</span><span class="sxs-lookup"><span data-stu-id="a7334-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="a7334-106">Εάν ένα έργο χρόνου και υλικού έχει πολλαπλές προελεύσεις χρηματοδότησης στη σύμβαση έργου, πρέπει να ενεργοποιήσετε την παράμετρο **Να επιτρέπονται παραγγελίες πώλησης για έργα με πολλαπλές προελεύσεις χρηματοδότησης** στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="a7334-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="a7334-107">Η υποστήριξη για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης είναι διαθέσιμη ξεκινώντας από την έκδοση 10.0.2 της εφαρμογής ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="a7334-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="a7334-108">Η παράμετρος για την ενεργοποίηση της υποστήριξης για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης θα καταργηθεί στο κύμα κυκλοφορίας του Απριλίου 2020, μετά το οποίο θα έχει ενεργοποιηθεί πάντα η λειτουργικότητα.</span><span class="sxs-lookup"><span data-stu-id="a7334-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="a7334-109">Μπορείτε να δημιουργήσετε παραγγελίες πώλησης βάσει έργου με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="a7334-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="a7334-110">Μεταβείτε στο ίδιο το έργο.</span><span class="sxs-lookup"><span data-stu-id="a7334-110">Go to the project itself.</span></span> <span data-ttu-id="a7334-111">Στο παράθυρο ενεργειών, επιλέξτε **Διαχείριση > Εργασίες στοιχείων > Παραγγελία πώλησης**.</span><span class="sxs-lookup"><span data-stu-id="a7334-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="a7334-112">Οι πληροφορίες έργου προεπιλέγουν την παραγγελία πώλησης από το έργο.</span><span class="sxs-lookup"><span data-stu-id="a7334-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="a7334-113">Εάν η σύμβαση έργου έχει περισσότερες από μία πηγές χρηματοδότησης, θα πρέπει να επιλέξετε την προέλευση χρηματοδότησης για να ορίσετε τον πελάτη για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="a7334-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="a7334-114">Εάν υπάρχει μόνο μία προέλευση χρηματοδότησης για το έργο, ο πελάτης θα οριστεί αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="a7334-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="a7334-115">Μεταβείτε στη σελίδα **Όλες οι παραγγελίες πώλησης** και δημιουργήστε μια νέα παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="a7334-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="a7334-116">Θα πρέπει να επιλέξετε το έργο για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="a7334-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="a7334-117">Μετά την επιλογή του έργου, ο πελάτης θα οριστεί από την προέλευση χρηματοδότησης ή θα πρέπει να επιλέξετε τον πηγαίο κώδικα χρηματοδότησης εάν η σύμβαση έργου έχει πολλαπλές προελεύσεις χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="a7334-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]