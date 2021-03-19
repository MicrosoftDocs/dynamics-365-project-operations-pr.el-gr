---
title: Έργα εκτίμησης εσόδων σταθερής τιμής
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα έσοδα σταθερής τιμής σε έργα.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7cf4d7853f7fedaeeeba99bc589f39989b924423
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278913"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="92ba0-103">Έργα εκτίμησης εσόδων σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="92ba0-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="92ba0-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="92ba0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="92ba0-105">Όταν δημιουργείτε μια γραμμή σύμβασης έργου με τα παρακάτω χαρακτηριστικά στο Dynamics 365 Project Operations στο Microsoft Dataverse, το σύστημα δημιουργεί αυτόματα ένα έργο εκτίμησης εσόδων σταθερής τιμής.</span><span class="sxs-lookup"><span data-stu-id="92ba0-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="92ba0-106">Οι πληροφορίες σε αυτό το έργο βασίζονται στα εξής:</span><span class="sxs-lookup"><span data-stu-id="92ba0-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="92ba0-107">Μια μέθοδος χρέωσης σταθερής τιμής.</span><span class="sxs-lookup"><span data-stu-id="92ba0-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="92ba0-108">Ένα συσχετισμένο έργο.</span><span class="sxs-lookup"><span data-stu-id="92ba0-108">An associated project.</span></span>
  - <span data-ttu-id="92ba0-109">Τουλάχιστον ένα ορόσημο που καθορίζεται στην καρτέλα **Χρονοδιάγραμμα τιμολογίων** στη σελίδα **Γραμμή σύμβασης έργου**.</span><span class="sxs-lookup"><span data-stu-id="92ba0-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="92ba0-110">Επανεξέταση έρων εκτιμήσεων εσόδων σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="92ba0-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="92ba0-111">Για να εξετάσετε τα έργα εκτιμήσεων εσόδων σταθερής τιμής, ολοκληρώστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="92ba0-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="92ba0-112">Στο περιβάλλον του Dynamics 365 Finance, μεταβείτε στην επιλογή **Διαχείρησ έργων και λογιστική** > **Έργα** > **Έργα εκτίμησης εσόδων σταθερής τιμής**.</span><span class="sxs-lookup"><span data-stu-id="92ba0-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="92ba0-113">Επιλέξτε το έργο που θέλετε να προβάλετε και κάντε διπλό κλικ στο στοιχείο **Αναγνωριστικό έργου εκτίμησης** για να ανοίξετε την καρτέλα και να εξετάσετε τις λεπτομέρειες του έργου.</span><span class="sxs-lookup"><span data-stu-id="92ba0-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="92ba0-114">Αναπτύξτε την καρτέλα **Έργο**. Θα δείτε ένα έργο στο πλέγμα **Επιλεγμένα έργα**.</span><span class="sxs-lookup"><span data-stu-id="92ba0-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="92ba0-115">Το σύστημα το χρησιμοποιεί αυτό ως ως προεπιλεγμένο έργο, επειδή είναι το έργο που σχετίζεται με τη γραμμή σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="92ba0-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="92ba0-116">Για να αλλάξετε τη συσχέτιση, επιλέξτε πρόσθετα έργα και προσθέστε τα στο πλέγμα **Επιλεγμένα έργα**.</span><span class="sxs-lookup"><span data-stu-id="92ba0-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="92ba0-117">Εάν έχουν επιλεγεί πολλαπλά έργα σε αυτό το πλέγμα, οι εκτιμήσεις ολοκλήρωσης ποσοστού του έργου και εσόδων υπολογίζονται από κοινού για όλα τα επιλεγμένα έργα.</span><span class="sxs-lookup"><span data-stu-id="92ba0-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="92ba0-118">Το κόστος έργου, το προφίλ εσόδων, το πρότυπο κόστους και ο κωδικός περιόδου μπορούν να οριστούν με μη αυτόματο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="92ba0-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="92ba0-119">Εάν δεν έχουν οριστεί με μη αυτόματο τρόπο, οι προεπιλεγμένες τιμές στη διάρκεια του πρώτου υπολογισμού εκτίμησης για το έργο με τη χρήση των κανόνων που έχουν ρυθμιστεί για προφίλ κόστους και εσόδων έργου.</span><span class="sxs-lookup"><span data-stu-id="92ba0-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]