---
title: Κατανόηση κατάστασης έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κατάσταση που εκχωρείται σε έργα στο Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc5bc174518e46b32cf88ea7231bb2df10fde292
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127293"
---
# <a name="understand-project-status"></a><span data-ttu-id="02ba8-103">Κατανόηση κατάστασης έργου</span><span class="sxs-lookup"><span data-stu-id="02ba8-103">Understand project status</span></span>

<span data-ttu-id="02ba8-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="02ba8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="02ba8-105">Η ενότητα **Κατάσταση** στη σελίδα **Οντότητα έργου** παρέχει μια σύνοψη της εύρυθμης λειτουργίας του έργου βάσει του κόστους και της προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="02ba8-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="02ba8-106">Πεδία σύνοψης κατάστασης</span><span class="sxs-lookup"><span data-stu-id="02ba8-106">Status summary fields</span></span>

- <span data-ttu-id="02ba8-107">Το πεδίο **Συνολική κατάσταση έργου** είναι ένα επεξεργάσιμο πεδίο που εμφανίζει τη συνολική κατάσταση του έργου.</span><span class="sxs-lookup"><span data-stu-id="02ba8-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="02ba8-108">Αυτό το πεδίο χρησιμοποιεί χρωματική κωδικοποίηση, όπως πράσινο, κίτρινο και κόκκινο, για να υποδείξει αυξημένο κίνδυνο.</span><span class="sxs-lookup"><span data-stu-id="02ba8-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="02ba8-109">Το πεδίο **Σχόλια** επιτρέπει στο διαχειριστή έργου να εισαγάγει συγκεκριμένα σχόλια σχετικά με την κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="02ba8-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="02ba8-110">Δεν είναι δυνατή η επεξεργασία του πεδίου **Η κατάσταση ενημερώθηκε στις**.</span><span class="sxs-lookup"><span data-stu-id="02ba8-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="02ba8-111">Η τιμή σε αυτό το πεδίο είναι μια σήμανση χρόνου που υποδεικνύει την ημερομηνία τελευταίας ενημέρωσης της κατάστασης.</span><span class="sxs-lookup"><span data-stu-id="02ba8-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="02ba8-112">Τα πεδία **Απόδοση χρονοδιαγράμματος** και **Απόδοση κόστους** καθορίζονται από το πλέγμα παρακολούθησης.</span><span class="sxs-lookup"><span data-stu-id="02ba8-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="02ba8-113">Όταν η διακύμανση χρονοδιαγράμματος και κόστους για τον ριζικό κόμβο στην προβολή **Παρακολούθηση προσπάθειας** είναι θετική, μπορείτε να ενημερώσετε αυτά τα πεδία σε **Μπροστά**.</span><span class="sxs-lookup"><span data-stu-id="02ba8-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="02ba8-114">Όταν το χρονοδιάγραμμα και η διακύμανση κόστους του ριζικού κόμβου είναι αρνητικά, μπορείτε να τα ορίσετε σε **Πίσω**.</span><span class="sxs-lookup"><span data-stu-id="02ba8-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
