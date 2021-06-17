---
title: Διεταιρικά έξοδα
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο χρήσης των ενδοεταιρικών δαπανών για την ανάθεση των δαπανών ενός εργαζόμενου στη νομική οντότητα για την οποία εκτελέστηκε η εργασία.
author: ShylaThompson
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d2cdba8d5368a8b26bf4d98226bda76a58261cf0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005071"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="635a9-103">Διεταιρικά έξοδα</span><span class="sxs-lookup"><span data-stu-id="635a9-103">Intercompany expenses</span></span>

<span data-ttu-id="635a9-104">Ένας εργαζόμενος που απασχολείται σε μια νομική οντότητα ή σε έναν οργανισμό μπορεί να εκτελέσει εργασία για μια άλλη νομική οντότητα στον ίδιο οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="635a9-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="635a9-105">Μπορείτε να χρησιμοποιήσετε τις διεταιρικές δαπάνες για να αναθέσετε τα δαπάνες του εργαζόμενου στη νομική οντότητα για την οποία εκτελέστηκε η εργασία.</span><span class="sxs-lookup"><span data-stu-id="635a9-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="635a9-106">Η νομική οντότητα που απασχολεί τον εργαζόμενο ονομάζεται νομική οντότητα δανεισμού.</span><span class="sxs-lookup"><span data-stu-id="635a9-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="635a9-107">Η νομική οντότητα για την οποία ο εργαζόμενος επιβαρύνεται με έξοδα ονομάζεται δανειζόμενη νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="635a9-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="635a9-108">Για να μπορεί ένας εργαζόμενος να δημιουργήσει και να υποβάλει διεταιρικές δαπάνες, πρέπει να ενεργοποιήσετε τις γραμμές διεταιρικών δαπανών.</span><span class="sxs-lookup"><span data-stu-id="635a9-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="635a9-109">Στη νομική οντότητα που έχει τη δυνατότητα δανείων, στη σελίδα **Παράμετροι διαχείρισης δαπανών**, επιλέξτε **Να επιτρέπονται οι γραμμές διαεταιρικών δαπανών**.</span><span class="sxs-lookup"><span data-stu-id="635a9-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="635a9-110">Καταχώρηση φόρου για διεταιρικές δαπάνες</span><span class="sxs-lookup"><span data-stu-id="635a9-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="635a9-111">Για να μπορείτε να χρησιμοποιήσετε τις φορολογικές ομάδες που σχετίζονται με τη νομική οντότητα δανείων (προέλευση) αντί της νομικής οντότητας του δανείου (προορισμός) στην αναφορά εξόδων σας, πρέπει να ενεργοποιήσετε τη λειτουργικότητα στην εγκατάσταση του φόρου πωλήσεων γενικού καθολικού.</span><span class="sxs-lookup"><span data-stu-id="635a9-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="635a9-112">Όταν η παράμετρος **Νομική οντότητα για διεταιρική καταχώριση φόρων** έχει οριστεί σε **Προέλευση** και η **Εφαρμογή κανόνων φορολόγησης φόρου πωλήσεων** έχει οριστεί σε **Όχι**, χρησιμοποιείται ο συνδυασμός φόρου για τη νομική οντότητα δανείων.</span><span class="sxs-lookup"><span data-stu-id="635a9-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="635a9-113">Όταν η ίδια παράμετρος έχει οριστεί σε **Προορισμός**, θα χρησιμοποιηθεί ο συνδυασμός φόρων για τη δανειζόμενη νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="635a9-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="635a9-114">Για νομικές οντότητες στις Ηνωμένες Πολιτείες, όταν η παράμετρος έχει οριστεί σε **Προέλευση**, το πεδίο **Εισπρακτέος φόρος πωλήσεων** πρέπει επίσης να έχει ρυθμιστεί στη νέα σελίδα **Ομάδες καταχώρησης καθολικού**.</span><span class="sxs-lookup"><span data-stu-id="635a9-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="635a9-115">Ο μηχανισμός λογιστικής θα χρησιμοποιήσει τις πληροφορίες από αυτό το πεδίο για τη συσχετισμένη με τον φόρο λογιστική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="635a9-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="635a9-116">Η συμπεριφορά συμβαδίζει με τις γραμμές εξόδων που έχουν καταχωρηθεί με ή χωρίς έργο.</span><span class="sxs-lookup"><span data-stu-id="635a9-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  


[!INCLUDE[footer-include](../includes/footer-banner.md)]