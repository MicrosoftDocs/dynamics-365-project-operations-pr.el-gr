---
title: Τύποι περιόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης τύπων περιόδου για εκτιμήσεις εσόδων.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 107cecbc1dabdf13147d847bf1816f44cc2703c5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287283"
---
# <a name="period-types"></a><span data-ttu-id="27db7-103">Τύποι περιόδων</span><span class="sxs-lookup"><span data-stu-id="27db7-103">Period types</span></span>

<span data-ttu-id="27db7-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="27db7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="27db7-105">Ένας τύπος περιόδου καθορίζει τη συχνότητα με την οποία εκτιμάται το έσοδο σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="27db7-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="27db7-106">Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης τύπων περιόδου για εκτιμήσεις εσόδων.</span><span class="sxs-lookup"><span data-stu-id="27db7-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="27db7-107">Δημιουργία και εργασία με τύπους περιόδοων</span><span class="sxs-lookup"><span data-stu-id="27db7-107">Create and work with period types</span></span>
<span data-ttu-id="27db7-108">Για να δημιουργήσετε και να εργαστείτε με τύπους περιόδου, ολοκληρώστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="27db7-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="27db7-109">Στο περιβάλλον Dynamics 365 Finance, μεταβείτε στο **Διαχείριση έργου και λογιστική** > **Ρύθμιση** > **Εκτιμήσεις** > **Τύποι περιόδου**.</span><span class="sxs-lookup"><span data-stu-id="27db7-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="27db7-110">Επιλέξτε **Νέο** για να δημιουργήσετε νέο τύπο περιόδου.</span><span class="sxs-lookup"><span data-stu-id="27db7-110">Select **New** to create new period type.</span></span> <span data-ttu-id="27db7-111">Εισαγάγετε ένα όνομα και μια περιγραφή.</span><span class="sxs-lookup"><span data-stu-id="27db7-111">Enter a name and description.</span></span>
3. <span data-ttu-id="27db7-112">Στο πεδίο **Συχνότητα**, επιλέξτε μια τιμή:</span><span class="sxs-lookup"><span data-stu-id="27db7-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="27db7-113">Εάν επιλέξτε **Εβδομάδα**, **Ανά δύο εβδομάδες**, **Ανά δεκαπενθήμερο**, **Μήνας**, **Ημέρα**, **Τρίμηνο** ή **Έτος**, το ημερολόγιο θα χρησιμοποιείται για την παραγωγή περιόδων.</span><span class="sxs-lookup"><span data-stu-id="27db7-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="27db7-114">Εάν επιλέξετε **Περίοδο καθολικού**, οι περιόδοι καθολικού από τη ρύθμιση παραμέτρων γενικού καθολικού θα χρησιμοποιηθούν για τη δημιουργία περιόδων.</span><span class="sxs-lookup"><span data-stu-id="27db7-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="27db7-115">Εάν επιλέξετε **Απεριόριστα**, μπορείτε να καθορίσετε προσαρμοσμένες περιόδους.</span><span class="sxs-lookup"><span data-stu-id="27db7-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="27db7-116">Επιλέξτε την καρτέλα τύπου περιόδου και, στη συνέχεια, επιλέξτε **Δημιουργία περιόδων** για τη δημιουργία περιόδων για τον τύπο περιόδου.</span><span class="sxs-lookup"><span data-stu-id="27db7-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="27db7-117">Σύμφωνα με τη συχνότητα περιόδου που επιλέξατε, μπορεί να έχετε την επιλογή να καθορίσετε μια ημερομηνία έναρξης ή τον αριθμό των περιόδων που θα δημιουργηθούν.</span><span class="sxs-lookup"><span data-stu-id="27db7-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="27db7-118">Επιλέξτε **Περίοδοι** για την αναθεώρηση των περιόδων που δημιουργούνται.</span><span class="sxs-lookup"><span data-stu-id="27db7-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]