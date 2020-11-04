---
title: Διεταιρικά έξοδα
description: Ένας εργαζόμενος που απασχολείται σε μια νομική οντότητα ή σε έναν οργανισμό μπορεί να εκτελέσει εργασία για μια άλλη νομική οντότητα στον ίδιο οργανισμό. Σε αυτήν την περίπτωση, μπορείτε να χρησιμοποιήσετε τη δυνατότητα διεταιρικών εξόδων για να αναθέσετε τα έξοδα του εργαζομένου στη νομική οντότητα για την οποία εκτελέστηκε η εργασία.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077067"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="24fe9-104">Διεταιρικά έξοδα</span><span class="sxs-lookup"><span data-stu-id="24fe9-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="24fe9-105">Ένας εργαζόμενος που απασχολείται σε μια νομική οντότητα ή σε έναν οργανισμό μπορεί να εκτελέσει εργασία για μια άλλη νομική οντότητα στον ίδιο οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="24fe9-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="24fe9-106">Σε αυτήν την περίπτωση, μπορείτε να χρησιμοποιήσετε τη δυνατότητα διεταιρικών εξόδων για να αναθέσετε τα έξοδα του εργαζομένου στη νομική οντότητα για την οποία εκτελέστηκε η εργασία.</span><span class="sxs-lookup"><span data-stu-id="24fe9-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="24fe9-107">Η νομική οντότητα που απασχολεί τον εργαζόμενο ονομάζεται νομική οντότητα δανεισμού.</span><span class="sxs-lookup"><span data-stu-id="24fe9-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="24fe9-108">Η νομική οντότητα για την οποία ο εργαζόμενος επιβαρύνεται με έξοδα ονομάζεται δανειζόμενη νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="24fe9-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="24fe9-109">Για να μπορεί ένας εργαζόμενος να δημιουργήσει και να υποβάλει έξοδα για εργασία που εκτελείται για μια διαφορετική νομική οντότητα, στη νομική οντότητα δανεισμού", στη σελίδα **Παράμετροι διαχείρισης εξόδων** , επιλέξτε **Να επιτρέπονται οι γραμμές διεταιρικών εξόδων**.</span><span class="sxs-lookup"><span data-stu-id="24fe9-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="24fe9-110">Καταχώρηση φόρου για διεταιρικές δαπάνες</span><span class="sxs-lookup"><span data-stu-id="24fe9-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="24fe9-111">Εάν θέλετε να χρησιμοποιήσετε ομάδες φόρων που σχετίζονται με τη νομική οντότητα δανεισμού (προέλευση) αντί για τη δανειζόμενη νομική οντότητα (προορισμός)" στην αναφορά εξόδων σας, θα πρέπει να ρυθμίσετε τις παραμέτρους αυτές στη ρύθμιση φόρου πωλήσεων γενικής λογιστικής.</span><span class="sxs-lookup"><span data-stu-id="24fe9-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="24fe9-112">Όταν η παράμετρος γενικής λογιστικής, η **Νομική οντότητα για καταχώρηση διεταιρικών φόρων** έχει οριστεί σε **Προέλευση** και το στοιχείο **Εφαρμογή κανόνων φορολόγησης φόρων πωλήσεων** έχει οριστεί σε **Όχι** , θα χρησιμοποιηθεί ο συνδυασμός φόρων για τη νομική οντότητα δανεισμού.</span><span class="sxs-lookup"><span data-stu-id="24fe9-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="24fe9-113">Όταν η ίδια παράμετρος έχει οριστεί σε **Προορισμός** , θα χρησιμοποιηθεί ο συνδυασμός φόρων για τη δανειζόμενη νομική οντότητα.</span><span class="sxs-lookup"><span data-stu-id="24fe9-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="24fe9-114">Για νομικές οντότητες στις Ηνωμένες Πολιτείες, όταν η παράμετρος έχει οριστεί σε **Προέλευση** , το πεδίο **Εισπρακτέος φόρος πωλήσεων** πρέπει επίσης να έχει ρυθμιστεί στη νέα σελίδα **Ομάδες καταχώρησης καθολικού**.</span><span class="sxs-lookup"><span data-stu-id="24fe9-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="24fe9-115">Ο μηχανισμός λογιστικής θα χρησιμοποιήσει τις πληροφορίες από αυτό το πεδίο για τη συσχετισμένη με τον φόρο λογιστική καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="24fe9-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="24fe9-116">Η συμπεριφορά συμβαδίζει με τις γραμμές εξόδων που έχουν καταχωρηθεί με ή χωρίς έργο.</span><span class="sxs-lookup"><span data-stu-id="24fe9-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
