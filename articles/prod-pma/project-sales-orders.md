---
title: Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα
description: Αυτό το θέμα επεξηγεί τον τρόπο δημιουργίας παραγγελιών πώλησης βάσει έργου για έργα χρόνου και υλικά έργα.
author: Yowelle
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: dec9bc700d18f71ec7c9e976b38cb8cbb41f21b5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009661"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="f8223-103">Παραγγελίες πώλησης έργου για έργα χρόνου και υλικά έργα</span><span class="sxs-lookup"><span data-stu-id="f8223-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f8223-104">Αυτό το θέμα περιγράφει τον τρόπο δημιουργίας μιας παραγγελίας πώλησης για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="f8223-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="f8223-105">Οι παραγγελίες πώλησης μπορούν να δημιουργηθούν μόνο για έργα τύπου **χρόνος και υλικό**.</span><span class="sxs-lookup"><span data-stu-id="f8223-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="f8223-106">Εάν ένα έργο χρόνου και υλικού έχει πολλαπλές προελεύσεις χρηματοδότησης στη σύμβαση έργου, πρέπει να ενεργοποιήσετε την παράμετρο **Να επιτρέπονται παραγγελίες πώλησης για έργα με πολλαπλές προελεύσεις χρηματοδότησης** στη σελίδα **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="f8223-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="f8223-107">Η υποστήριξη για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης είναι διαθέσιμη ξεκινώντας από την έκδοση 10.0.2 της εφαρμογής ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="f8223-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="f8223-108">Η παράμετρος για την ενεργοποίηση της υποστήριξης για παραγγελίες πώλησης έργου με πολλαπλές πηγές χρηματοδότησης θα καταργηθεί στο κύμα κυκλοφορίας του Απριλίου 2020, μετά το οποίο θα έχει ενεργοποιηθεί πάντα η λειτουργικότητα.</span><span class="sxs-lookup"><span data-stu-id="f8223-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="f8223-109">Μπορείτε να δημιουργήσετε παραγγελίες πώλησης βάσει έργου με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="f8223-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="f8223-110">Μεταβείτε στο ίδιο το έργο.</span><span class="sxs-lookup"><span data-stu-id="f8223-110">Go to the project itself.</span></span> <span data-ttu-id="f8223-111">Στο παράθυρο ενεργειών, επιλέξτε **Διαχείριση > Εργασίες στοιχείων > Παραγγελία πώλησης**.</span><span class="sxs-lookup"><span data-stu-id="f8223-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="f8223-112">Οι πληροφορίες έργου προεπιλέγουν την παραγγελία πώλησης από το έργο.</span><span class="sxs-lookup"><span data-stu-id="f8223-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="f8223-113">Εάν η σύμβαση έργου έχει περισσότερες από μία πηγές χρηματοδότησης, θα πρέπει να επιλέξετε την προέλευση χρηματοδότησης για να ορίσετε τον πελάτη για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="f8223-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="f8223-114">Εάν υπάρχει μόνο μία προέλευση χρηματοδότησης για το έργο, ο πελάτης θα οριστεί αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="f8223-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="f8223-115">Μεταβείτε στη σελίδα **Όλες οι παραγγελίες πώλησης** και δημιουργήστε μια νέα παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="f8223-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="f8223-116">Θα πρέπει να επιλέξετε το έργο για την παραγγελία πώλησης.</span><span class="sxs-lookup"><span data-stu-id="f8223-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="f8223-117">Μετά την επιλογή του έργου, ο πελάτης θα οριστεί από την προέλευση χρηματοδότησης ή θα πρέπει να επιλέξετε τον πηγαίο κώδικα χρηματοδότησης εάν η σύμβαση έργου έχει πολλαπλές προελεύσεις χρηματοδότησης.</span><span class="sxs-lookup"><span data-stu-id="f8223-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]