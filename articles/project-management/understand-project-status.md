---
title: Κατανόηση κατάστασης έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κατάσταση που έχει ανατεθεί σε έργα στο Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ad8c012b93bc65595dca33df1770562916c557e0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993416"
---
# <a name="understand-project-status"></a><span data-ttu-id="46b4f-103">Κατανόηση κατάστασης έργου</span><span class="sxs-lookup"><span data-stu-id="46b4f-103">Understand project status</span></span>

<span data-ttu-id="46b4f-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="46b4f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="46b4f-105">Η ενότητα **Κατάσταση** στη σελίδα **Οντότητα έργου** παρέχει μια σύνοψη της εύρυθμης λειτουργίας του έργου βάσει του κόστους και της προσπάθειας.</span><span class="sxs-lookup"><span data-stu-id="46b4f-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="46b4f-106">Πεδία σύνοψης κατάστασης</span><span class="sxs-lookup"><span data-stu-id="46b4f-106">Status summary fields</span></span>

- <span data-ttu-id="46b4f-107">Το πεδίο **Συνολική κατάσταση έργου** είναι ένα επεξεργάσιμο πεδίο που εμφανίζει τη συνολική κατάσταση του έργου.</span><span class="sxs-lookup"><span data-stu-id="46b4f-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="46b4f-108">Αυτό το πεδίο χρησιμοποιεί χρωματική κωδικοποίηση, όπως πράσινο, κίτρινο και κόκκινο, για να υποδείξει αυξημένο κίνδυνο.</span><span class="sxs-lookup"><span data-stu-id="46b4f-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="46b4f-109">Το πεδίο **Σχόλια** επιτρέπει στο διαχειριστή έργου να εισαγάγει συγκεκριμένα σχόλια σχετικά με την κατάσταση.</span><span class="sxs-lookup"><span data-stu-id="46b4f-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="46b4f-110">Δεν είναι δυνατή η επεξεργασία του πεδίου **Η κατάσταση ενημερώθηκε στις**.</span><span class="sxs-lookup"><span data-stu-id="46b4f-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="46b4f-111">Η τιμή σε αυτό το πεδίο είναι μια σήμανση χρόνου που υποδεικνύει την ημερομηνία τελευταίας ενημέρωσης της κατάστασης.</span><span class="sxs-lookup"><span data-stu-id="46b4f-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="46b4f-112">Τα πεδία **Απόδοση χρονοδιαγράμματος** και **Απόδοση κόστους** καθορίζονται από το πλέγμα παρακολούθησης.</span><span class="sxs-lookup"><span data-stu-id="46b4f-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="46b4f-113">Όταν η διακύμανση χρονοδιαγράμματος και κόστους για τον ριζικό κόμβο στην προβολή **Παρακολούθηση προσπάθειας** είναι θετική, μπορείτε να ενημερώσετε αυτά τα πεδία σε **Μπροστά**.</span><span class="sxs-lookup"><span data-stu-id="46b4f-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="46b4f-114">Όταν το χρονοδιάγραμμα και η διακύμανση κόστους του ριζικού κόμβου είναι αρνητικά, μπορείτε να τα ορίσετε σε **Πίσω**.</span><span class="sxs-lookup"><span data-stu-id="46b4f-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]