---
title: Κρατήσεις έναντι αναθέσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις διαφορές μεταξύ των κρατήσεων πόρων και των αναθέσεων πόρων.
author: ruhercul
ms.date: 01/08/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3c1a1003af0b23c4be44fefac0b3c4ea725f96b2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012766"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="fa328-103">Κρατήσεις έναντι αναθέσεων</span><span class="sxs-lookup"><span data-stu-id="fa328-103">Bookings vs assignments</span></span>

<span data-ttu-id="fa328-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="fa328-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fa328-105">Οι κρατήσεις είναι η εκχώρηση πόρων σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="fa328-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="fa328-106">Με τη χρήση κρατήσεων καταναλώνεται η παραγωγική ικανότητα του πόρου.</span><span class="sxs-lookup"><span data-stu-id="fa328-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="fa328-107">Οι κρατήσεις αντιπροσωπεύουν οργανωτικές έννοιες για τις ομάδες, ώστε να μπορούν να κατανοήσουν τον τρόπο με τον οποίο θα συμμετέχουν πόροι σε διάφορα έργα.</span><span class="sxs-lookup"><span data-stu-id="fa328-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="fa328-108">Το Dynamics 365 Project Operations θεωρεί τις κρατήσεις ως έννοια επιπέδου έργου.</span><span class="sxs-lookup"><span data-stu-id="fa328-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="fa328-109">Σε αντίθεση με τις κρατήσεις, οι αναθέσεις είναι η δέσμευση πόρων σε εργασίες έργου του χρονοδιαγράμματος έργου.</span><span class="sxs-lookup"><span data-stu-id="fa328-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="fa328-110">Οι πόροι μπορούν να έχουν όνομα ή να είναι γενικοί.</span><span class="sxs-lookup"><span data-stu-id="fa328-110">The resources can be named or generic.</span></span>  <span data-ttu-id="fa328-111">Όταν μια απαίτηση πόρου προκύπτει από τις αναθέσεις εργασιών έργου, το Project Operations χρησιμοποιεί την προσπάθεια για την ανάθεση πόρων για τη δημιουργία των λεπτομερειών απαίτησης πόρου.</span><span class="sxs-lookup"><span data-stu-id="fa328-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="fa328-112">Ωστόσο, το πεδίο για τις αναθέσεις πόρων δεν διατηρείται.</span><span class="sxs-lookup"><span data-stu-id="fa328-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="fa328-113">Οι ενημερώσεις για κρατήσεις που προκύπτουν από την απαίτηση πόρου δεν ενημερώνουν τυχόν αναθέσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="fa328-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="fa328-114">Συνήθως, το άθροισμα των κρατήσεων για έναν πόρο θα ισούται με το άθροισμα των αναθέσεων του πόρου σε μία ή πολλές εργασίες.</span><span class="sxs-lookup"><span data-stu-id="fa328-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="fa328-115">Ωστόσο, το Project Operations δεν επιβάλλει την εν λόγω συμφωνία.</span><span class="sxs-lookup"><span data-stu-id="fa328-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="fa328-116">Η προβολή **εναρμόνισης** εμφανίζει μια θέση του διευθυντή έργου όπου οι κρατήσεις και οι αναθέσεις ενός πόρου δεν συμφωνούν.</span><span class="sxs-lookup"><span data-stu-id="fa328-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]