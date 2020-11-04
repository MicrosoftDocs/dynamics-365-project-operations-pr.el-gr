---
title: Προβλέψεις και προϋπολογισμοί έργου
description: 'Το Microsoft Dynamics 365 Finance παρέχει δύο τρόπους για να διαχειριστείτε και να ελέγξετε τα έργα σας: προβλέψεις έργου και προϋπολογισμοί έργου.'
author: Yowelle
manager: AnnBe
ms.date: 10/25/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ForecastModel, ProjYearEndProcess
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23501
ms.assetid: 4e6d1384-19a2-4232-b3f3-d2590c218bd7
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f99c00effbb0678f1f55e5068a7128cbfb86f5ce
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077029"
---
# <a name="project-forecasts-and-budgets"></a><span data-ttu-id="5e3a3-103">Προβλέψεις και προϋπολογισμοί έργου</span><span class="sxs-lookup"><span data-stu-id="5e3a3-103">Project forecasts and budgets</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="5e3a3-104">Υπάρχουν δύο τρόποι για να διαχειριστείτε και να ελέγξετε τα έργα σας: προβλέψεις έργου και προϋπολογισμοί έργου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-104">There are two ways to manage and control your projects: project forecasts and project budgets.</span></span> 

<span data-ttu-id="5e3a3-105">Χρησιμοποιήστε την πρόβλεψη έργου εάν ο οργανισμός σας έχει μια λειτουργική προοπτική και αν εστιάζει στα έσοδα και το κόστος που προκύπτουν από συγκεκριμένες συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-105">Use project forecasting if your organization has an operational perspective, and if it focuses on revenues and costs that are derived from specific transactions.</span></span> <span data-ttu-id="5e3a3-106">Αν ο οργανισμός σας επικεντρώνεται περισσότερο σε οικονομικά ποσά, μπορείτε να χρησιμοποιήσετε τον προϋπολογισμό έργου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-106">Use project budgeting if your organization focuses more on the financial amounts.</span></span> 

<span data-ttu-id="5e3a3-107">Τόσο οι προβλέψεις έργου όσο και οι προϋπολογισμοί έργου χρησιμοποιούν μοντέλα πρόβλεψης για να κρατήσουν τα προβλεπόμενα ποσά συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-107">Both project forecasts and project budgets use forecast models to hold the projected transaction amounts.</span></span> 

<span data-ttu-id="5e3a3-108">Κάθε μέθοδος έχει τα πλεονεκτήματά της.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-108">Each method has its advantages.</span></span> <span data-ttu-id="5e3a3-109">Θα πρέπει να λάβετε υπόψη σας τα παρακάτω σημεία προτού επιλέξετε μια μέθοδο για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-109">You should consider the following points before you select a method for your organization.</span></span>

|   <span data-ttu-id="5e3a3-110">Μέθοδος εκχώρησης</span><span class="sxs-lookup"><span data-stu-id="5e3a3-110">Allocation method</span></span>       |           <span data-ttu-id="5e3a3-111">Πρόβλεψη έργου</span><span class="sxs-lookup"><span data-stu-id="5e3a3-111">Project forecasting</span></span>            |        <span data-ttu-id="5e3a3-112">Προϋπολογισμός έργου</span><span class="sxs-lookup"><span data-stu-id="5e3a3-112">Project budgeting</span></span>                           |
|---------------------------|------------------------------------------|----------------------------------------------------|
| <span data-ttu-id="5e3a3-113">**Ανάθεση περιόδου**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-113">**Period allocation**</span></span>     | <span data-ttu-id="5e3a3-114">δεν μπορείτε να εκχωρήσετε ρητά συναλλαγές σε μια οικονομική περίοδο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-114">You can't explicitly allocate transactions over a fiscal period.</span></span> <span data-ttu-id="5e3a3-115">Αντ' αυτού, η πρόβλεψη και ο έλεγχος της πρόβλεψης βασίζονται στη διάρκεια ζωής του έργου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-115">Instead, the forecast, and the control of the forecast, are based on the life of the project.</span></span> <span data-ttu-id="5e3a3-116">Επειδή οι προβλέψεις βασίζονται σε μια συγκεκριμένη ημερομηνία, θα πρέπει να συμπεράνετε την περίοδο από την ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-116">Because forecasts are based on a specific date, you must infer the period from the date.</span></span> | <span data-ttu-id="5e3a3-117">Μπορείτε να εκχωρήσετε συναλλαγές σε ένα ολόκληρο έργο ή σε μια οικονομική περίοδο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-117">You can allocate transactions over the whole project or a fiscal period.</span></span> <span data-ttu-id="5e3a3-118">Εάν αναθέσετε σε μια περίοδο, μπορείτε να μεταφέρετε μη χρησιμοποιηθέντα ποσά προς τα εμπρός στην επόμενη οικονομική περίοδο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-118">If you allocate over a period, you can carry unused amounts forward to the next fiscal period.</span></span> |
| <span data-ttu-id="5e3a3-119">**Προβολή συναλλαγών**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-119">**Viewing transactions**</span></span>  | <span data-ttu-id="5e3a3-120">Μπορείτε να προβάλετε τις συναλλαγές στις φόρμες πρόβλεψης, όπου μπορείτε να δείτε τις προβλέψεις για ολόκληρη την εταιρεία και για όλα τα έργα, ανεξάρτητα από την ιεραρχία.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-120">You can view transactions in the forecast forms, where you see the forecasts for the whole company and for all projects, regardless of the hierarchy.</span></span> <span data-ttu-id="5e3a3-121">Για να εστιάσετε σε ένα συγκεκριμένο έργο, πρέπει να φιλτράρετε τα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-121">To focus on a particular project, you must filter the data.</span></span>                                       | <span data-ttu-id="5e3a3-122">Μπορείτε να προβάλετε προϋπολογισμένες συναλλαγές για μία μόνο ιεραρχική δομή έργου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-122">You can view budgeted transactions for a single project hierarchy.</span></span> <span data-ttu-id="5e3a3-123">Για αυτόν το λόγο, μπορείτε να προβάλετε τις λεπτομέρειες της συναλλαγής για ένα γονικό έργο ή για τα δευτερεύοντα έργα του.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-123">Therefore, you can view transaction details for a parent project or its subprojects.</span></span>                 |
| <span data-ttu-id="5e3a3-124">**Μεταβλητές συναλλαγής**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-124">**Transaction variables**</span></span> | <span data-ttu-id="5e3a3-125">Όταν καταχωρείτε συναλλαγές πρόβλεψης, μπορείτε να χρησιμοποιήσετε κάθε χαρακτηριστικό που υπάρχει για μια πραγματική συναλλαγή.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-125">When you enter forecast transactions, you can use every attribute that exists for an actual transaction.</span></span> <span data-ttu-id="5e3a3-126">Με αυτόν τον τρόπο μπορείτε να κάνετε περισσότερες λεπτομέρειες στις προβλέψεις.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-126">This allows for greater detail in the forecast.</span></span> <span data-ttu-id="5e3a3-127">Για παράδειγμα, μπορείτε να καταχωρίσετε λεπτομέρειες για τις ιδιότητες "ποσότητες", "υπάλληλοι", "στοιχεία" ή "γραμμές".</span><span class="sxs-lookup"><span data-stu-id="5e3a3-127">For example, you can enter details for quantities, workers, items, or line properties.</span></span>         | <span data-ttu-id="5e3a3-128">Όταν καταχωρείτε λεπτομέρειες προϋπολογισμού, μπορείτε να χρησιμοποιήσετε μόνο ποσά, κατηγορίες και δραστηριότητες.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-128">When you enter budget details, you can use only amounts, categories, and activities.</span></span>                    |
| <span data-ttu-id="5e3a3-129">**Ασφάλεια**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-129">**Security**</span></span>              | <span data-ttu-id="5e3a3-130">Η πρόβλεψη βασίζεται στις συναλλαγές που καταχωρείτε στις φόρμες πρόβλεψης και δεν περιλαμβάνει μηχανισμό ελέγχου διεργασιών.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-130">Forecasting is based on transactions that you enter in the forecast forms and involves no process control mechanism.</span></span> <span data-ttu-id="5e3a3-131">Κάθε εργαζόμενος που έχει δικαιώματα για μια φόρμα πρόβλεψης μπορεί να αναθεωρήσει πληροφορίες χωρίς έγκριση.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-131">Any worker who has permissions for a forecast form can revise information without approval.</span></span>                                        | <span data-ttu-id="5e3a3-132">Ο προϋπολογισμός χρησιμοποιεί το σύστημα ροής εργασιών, το οποίο ενεργοποιεί τη διαχείριση αλλαγών και σας επιτρέπει να κρατήσετε ένα ιστορικό των αναθεωρήσεων.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-132">Budgeting uses the workflow system, which enables change management and lets you keep a history of the revisions.</span></span>         |
| <span data-ttu-id="5e3a3-133">**Τύποι οντότητας**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-133">**Entry types**</span></span>           | <span data-ttu-id="5e3a3-134">Οι εγγραφές συναλλαγών πρόβλεψης είναι βασισμένες στον αριθμό μονάδων και στις τιμές μονάδων κόστους και πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-134">Forecast transaction entries are based on the number of units, and on cost and sales unit prices.</span></span>  | <span data-ttu-id="5e3a3-135">Τα στοιχεία του προϋπολογισμού υπολογίζονται με βάση τα ποσά, τα οποία διαιρούνται μεταξύ κόστους και εσόδων.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-135">Budget details are based on amounts, which are split between costs and revenues.</span></span>                                          |
| <span data-ttu-id="5e3a3-136">**Μοντέλα πρόβλεψης**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-136">**Forecast models**</span></span>       | <span data-ttu-id="5e3a3-137">Επειδή κάθε πρόβλεψη πρέπει να συσχετιστεί με ένα μοντέλο, μπορείτε να δημιουργήσετε πολλαπλά μοντέλα προβλέψεων και επίσης να ρυθμίσετε υπομοντέλα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-137">Because each forecast must be associated with a model, you can create multiple forecast models and also set up submodels.</span></span>           | <span data-ttu-id="5e3a3-138">Ο προϋπολογισμός έργου περιορίζει τα μοντέλα πρόβλεψης που χρησιμοποιούνται για τον προϋπολογισμό.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-138">Project budgeting limits the forecast models that are used for budgeting.</span></span> <span data-ttu-id="5e3a3-139">Λιγότερα μοντέλα πρόβλεψης μπορούν να συμβάλουν στη βελτίωση της συνέπειας στις προβολές.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-139">Fewer forecast models can help increase consistency in projections.</span></span>                           |
| <span data-ttu-id="5e3a3-140">**Υπερβάσεις κόστους**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-140">**Cost overruns**</span></span>         | <span data-ttu-id="5e3a3-141">Μπορείτε να επιτρέψετε ή να απαγορεύσετε μόνο την είσοδο συναλλαγών που θα προκαλέσουν υπέρβαση του κόστους.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-141">You can only allow or disallow the entry of transactions that will cause a cost overrun.</span></span>   | <span data-ttu-id="5e3a3-142">Ο προϋπολογισμός έργου παρέχει πρόσθετες επιλογές ελέγχου για τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-142">Project budgeting provides additional control options for users.</span></span> <span data-ttu-id="5e3a3-143">Μπορείτε να επιτρέψετε προειδοποιήσεις και υπερβάσεις.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-143">You can allow warnings and overruns.</span></span>                    |
| <span data-ttu-id="5e3a3-144">**Στοιχείο ελέγχου**</span><span class="sxs-lookup"><span data-stu-id="5e3a3-144">**Control**</span></span>               | <span data-ttu-id="5e3a3-145">Το στοιχείο ελέγχου πρόβλεψης εκτελείται με τη χρήση της μείωσης πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-145">Forecast control is performed by using forecast reduction.</span></span> <span data-ttu-id="5e3a3-146">Τα πραγματικά ποσά αφαιρούνται από τα υπόλοιπα των συναλλαγών προβλέψεων χωρίς ίχνος ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-146">Actual amounts are subtracted from forecast transaction balances without any audit trail.</span></span> <span data-ttu-id="5e3a3-147">Αυτό μπορεί να καταστήσει δυσκολότερη την ανίχνευση του σημείου όπου πραγματοποιήθηκαν οι πραγματικές συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-147">This can make it more difficult to trace where the actual transactions occurred.</span></span>                   | <span data-ttu-id="5e3a3-148">Στο στοιχείο ελέγχου προϋπολογισμού έργου, τα πραγματικά ποσά αφαιρούνται από τα ποσά του υπόλοιπου προϋπολογισμού.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-148">In project budget control, actual amounts are subtracted from amounts in the remaining budget.</span></span> <span data-ttu-id="5e3a3-149">Αυτό επιτρέπει ένα σαφέστερο ίχνος ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-149">This allows for a clearer audit trail.</span></span>                                   |

## <a name="project-forecasts"></a><span data-ttu-id="5e3a3-150">Προβλέψεις έργου</span><span class="sxs-lookup"><span data-stu-id="5e3a3-150">Project forecasts</span></span>
<span data-ttu-id="5e3a3-151">Όταν χρησιμοποιείτε την πρόβλεψη έργου, μπορείτε να εισαγάγετε τις συναλλαγές πρόβλεψης σε φόρμες πρόβλεψης για κάθε τύπο συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-151">When you use project forecasting, you can enter forecast transactions in forecast forms for each transaction type.</span></span> <span data-ttu-id="5e3a3-152">Κάθε χαρακτηριστικό που είναι διαθέσιμο για μια πραγματική συναλλαγή μπορεί να χρησιμοποιηθεί για μια συναλλαγή πρόβλεψης — για παράδειγμα, κερδοφορία της σειράς, χαρακτηριστικά της ουράς, εργαζόμενοι ή περιγραφές.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-152">Every attribute that is available for an actual transaction can be used for a forecast transaction—for example, line profitability, line attributes, workers, or descriptions.</span></span> <span data-ttu-id="5e3a3-153">Επίσης, μπορείτε να προβάλετε τη διάρκεια μετά την οποία θα επιβαρυνθείτε με ένα κόστος που θα τιμολογήσετε σε έναν πελάτη.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-153">You can also project how long after you incur a cost you will invoice a customer.</span></span> 

<span data-ttu-id="5e3a3-154">Οι συναλλαγές προβλέψεων έργου βασίζονται σε μονάδες και ποσά.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-154">Project forecasting transactions are based on units and amounts.</span></span> 

<span data-ttu-id="5e3a3-155">Πρέπει να συσχετίσετε κάθε πρόβλεψη έργου με ένα μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-155">You must associate each project forecast with a forecast model.</span></span> <span data-ttu-id="5e3a3-156">Όταν καταχωρείτε μια συναλλαγή πρόβλεψης, προτείνεται αυτόματα ένα μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-156">When you enter a forecast transaction, a forecast model is automatically suggested.</span></span> <span data-ttu-id="5e3a3-157">Το μοντέλο πρόβλεψης λειτουργεί ως κοντέινερ για τις συναλλαγές πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-157">The forecast model acts as a container for the forecast transactions.</span></span> 

<span data-ttu-id="5e3a3-158">Μπορείτε να ορίσετε τα μοντέλα πρόβλεψης ως υπομοντέλα για ένα μοντέλο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-158">You can designate forecast models as submodels for a model.</span></span> <span data-ttu-id="5e3a3-159">Με αυτόν τον τρόπο μπορείτε να προβλέψετε την περιοχή, την χρονική περίοδο ή το τμήμα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-159">This lets you forecast by region, time period, or department.</span></span> <span data-ttu-id="5e3a3-160">Μπορείτε να αντιγράψετε τις συναλλαγές πρόβλεψης σε ένα μοντέλο για να δημιουργήσετε ένα νέο μοντέλο και μπορείτε επίσης να μεταφέρετε τις συναλλαγές στη γενική λογιστική.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-160">You can copy the forecast transactions in a model to create a new model, and you can also transfer the transactions to the general ledger.</span></span> <span data-ttu-id="5e3a3-161">Επειδή υπάρχει μια σχέση ένα προς ένα ανάμεσα σε μια πρόβλεψη και ένα μοντέλο, κάθε μοντέλο πρόβλεψης δημιουργεί έναν ξεχωριστό προϋπολογισμό για ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-161">Because there is a one-to-one relationship between a forecast and a model, each forecast model makes up a separate budget for a project.</span></span> 

<span data-ttu-id="5e3a3-162">Τα μοντέλα πρόβλεψης μπορούν να χρησιμοποιήσουν τη μείωση των προβλέψεων ως μηχανισμό ελέγχου για τα έργα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-162">Forecast models can use forecast reduction as the control mechanism for projects.</span></span> <span data-ttu-id="5e3a3-163">Στη μείωση πρόβλεψης, οι πραγματικές συναλλαγές μειώνουν τα υπόλοιπα των συναλλαγών πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-163">In forecast reduction, actual transactions reduce forecast transaction balances.</span></span> <span data-ttu-id="5e3a3-164">Ωστόσο, επειδή η μείωση των προβλέψεων εφαρμόζεται στο υψηλότερο έργο στην ιεραρχία, παρέχει μια περιορισμένη προβολή των αλλαγών στην πρόβλεψη.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-164">However, because forecast reduction is applied to the highest project in the hierarchy, it provides a limited view of changes in the forecast.</span></span> <span data-ttu-id="5e3a3-165">Για παράδειγμα, εάν ένας εργαζόμενος είναι συσχετισμένος με ένα δευτερεύον έργο, οι πραγματικές συναλλαγές για τον εργαζόμενο καταχωρούνται στο γονικό έργο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-165">For example, if a worker is associated with a subproject, the actual transactions for the worker are posted to the parent project.</span></span> <span data-ttu-id="5e3a3-166">Αυτό μπορεί να δυσκολέψει την παρακολούθηση των αλλαγών, επειδή δεν μπορείτε εύκολα να καθορίσετε τη συναλλαγή στην οποία το δευτερεύον έργο προκάλεσε μια μείωση στο ποσό πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-166">This can make it difficult to track changes, because you can't easily determine which transaction in which subproject caused a reduction to the forecast amount.</span></span> <span data-ttu-id="5e3a3-167">Ως εκ τούτου, είναι καλή ιδέα να δημιουργήσετε ένα αντίγραφο του μοντέλου πρόβλεψης για τη μείωση των προβλέψεων για χρήση.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-167">Therefore, it's a good idea to create a copy of a forecast model for forecast reduction to use.</span></span> <span data-ttu-id="5e3a3-168">Στη συνέχεια, μπορείτε να χρησιμοποιήσετε τις αναφορές για να προβάλετε τις αρχικές προβλέψεις.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-168">You can then use reports to view what was originally forecasted.</span></span> 

<span data-ttu-id="5e3a3-169">Μπορείτε να αναθεωρήσετε, να αντιγράψετε, να διαγράψετε ή να μεταφέρετε προβλέψεις έργου σε έναν προϋπολογισμό γενικής λογιστικής.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-169">You can revise, copy, delete, or transfer project forecasts to a general ledger budget.</span></span> <span data-ttu-id="5e3a3-170">Ωστόσο, δεν υπάρχει στοιχείο ελέγχου διεργασίας.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-170">However, there is no process control.</span></span> <span data-ttu-id="5e3a3-171">Κάθε εργαζόμενος που έχει δικαιώματα για μια φόρμα πρόβλεψης μπορεί να αναθεωρήσει πληροφορίες χωρίς έλεγχο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-171">Any worker who has permission for a forecast form can make revisions without review.</span></span>

-   <span data-ttu-id="5e3a3-172">**Αναθεώρηση** – Μπορείτε να αναθεωρήσετε μια συναλλαγή πρόβλεψης στις ίδιες φόρμες όπου πραγματοποιήθηκαν οι αρχικές καταχωρήσεις.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-172">**Revise** – You can revise a forecast transaction in the same forms where the original entries were made.</span></span>
-   <span data-ttu-id="5e3a3-173">**Αντιγραφή ή διαγραφή** – Όταν αντιγράφετε συναλλαγές πρόβλεψης, αντιγράφετε τις γραμμές συναλλαγής ενός μοντέλου πρόβλεψης σε ένα άλλο μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-173">**Copy or delete** – When you copy forecast transactions, you copy the transaction lines of one forecast model to another forecast model.</span></span> <span data-ttu-id="5e3a3-174">Όταν διαγράφετε μια πρόβλεψη, διαγράφετε τις συναλλαγές πρόβλεψης από ένα μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-174">When you delete a forecast, you delete the forecast transactions from a forecast model.</span></span> <span data-ttu-id="5e3a3-175">Για να περιορίσετε τις συναλλαγές πρόβλεψης που αντιγράφονται ή διαγράφονται, επιλέξτε συγκεκριμένους τύπους συναλλαγών και ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-175">To limit the forecast transactions that are copied or deleted, select specific transaction types and dates.</span></span> <span data-ttu-id="5e3a3-176">Με αυτόν τον τρόπο μπορείτε να αντιγράψετε ή να διαγράψετε μόνο συγκεκριμένα τμήματα μιας πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-176">This lets you copy or delete only specific parts of a forecast.</span></span>
-   <span data-ttu-id="5e3a3-177">**Μεταφορά** – Όταν μεταφέρετε μια πρόβλεψη έργου σε έναν προϋπολογισμό γενικής λογιστικής, μεταφέρετε τις συναλλαγές πρόβλεψης ενός μοντέλου πρόβλεψης σε έναν προϋπολογισμό γενικής λογιστικής.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-177">**Transfer** – When you transfer a project forecast to a general ledger budget, you transfer the forecast transactions of a forecast model to a general ledger budget.</span></span> <span data-ttu-id="5e3a3-178">Μπορείτε να αντικαταστήσετε όλες τις συναλλαγές που είχαν μεταβιβαστεί στον προϋπολογισμό γενικής λογιστικής στις οποίες μεταφέρετε την πρόβλεψη του έργου σας.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-178">You can overwrite any previously transferred transactions in the general ledger budget that you transfer your project forecast to.</span></span>

## <a name="project-budgets"></a><span data-ttu-id="5e3a3-179">Προϋπολογισμοί έργου</span><span class="sxs-lookup"><span data-stu-id="5e3a3-179">Project budgets</span></span>
<span data-ttu-id="5e3a3-180">Ο προϋπολογισμός έργου είναι μια απλούστερη μέθοδος από την πρόβλεψη, παρόλο που ενσωματώνει τα μοντέλα πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-180">Project budgeting is a simpler method than forecasting, although it does integrate with forecast models.</span></span> <span data-ttu-id="5e3a3-181">Χρησιμοποιεί μια φόρμα καταχώρησης για τις αρχικές λεπτομέρειες και τις αναθεωρήσεις του προϋπολογισμού και επιτρέπει προβολές που βασίζονται μόνο στο ποσό, την κατηγορία ή τη δραστηριότητα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-181">It uses a single entry form for original budget details and revisions, and allows for projections that are based only on amount, category, or activity.</span></span> 

<span data-ttu-id="5e3a3-182">Στον προϋπολογισμό έργου, όλοι οι αρχικοί προϋπολογισμοί και οι αναθεωρήσεις πρέπει να αποσταλούν σε μια ροή εργασιών έργου για έγκριση.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-182">In project budgeting, all original budgets and revisions must be sent to a project workflow for approval.</span></span> <span data-ttu-id="5e3a3-183">Οι ροές εργασιών σάς παρέχουν αυξημένο έλεγχο στη διεργασία και δημιουργούν μια καρτέλα ιστορικού αλλαγών.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-183">Workflows give you increased control over the process and create a change history record.</span></span> 

<span data-ttu-id="5e3a3-184">Ο προϋπολογισμός έργου μοιάζει με τον προϋπολογισμό γενικής λογιστικής, αλλά είναι ταχύτερη και πιο εύκολη η ρύθμισή του.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-184">Project budgeting resembles general ledger budgeting, but is faster and easier to set up.</span></span> <span data-ttu-id="5e3a3-185">Πολλές από τις επιλογές του προϋπολογισμού γενικής λογιστικής, όπως οι ακολουθίες αριθμών ή η νομισματική μονάδα, δεν χρειάζεται να οριστούν ξεχωριστά για τα έργα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-185">Many of the options in general ledger budgeting, such as number sequences or currency, do not have to be set up separately for projects.</span></span>

<span data-ttu-id="5e3a3-186">Οι προϋπολογισμοί έργου συσχετίζονται αυτόματα με δύο μοντέλα πρόβλεψης, ένα για τον αρχικό προϋπολογισμό και ένα για τον υπολειπόμενο προϋπολογισμό.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-186">Project budgets are automatically associated with two forecast models, one for original budget and one for remaining budget.</span></span> <span data-ttu-id="5e3a3-187">Ως εκ τούτου, οι αναφορές που βασίζονται σε μοντέλα πρόβλεψης μπορούν να χρησιμοποιήσουν δεδομένα προϋπολογισμού.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-187">Therefore, reports that are based on forecast models can use budget data.</span></span> <span data-ttu-id="5e3a3-188">Όταν ένα προϋπολογισμός έργου έχει δεσμευτεί, το σύστημα δημιουργεί συναλλαγές πρόβλεψης με βάση τα συσχετισμένα μοντέλα, τα οποία χρησιμοποιούνται για λόγους αναφοράς και ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-188">When a project budget is committed, the system creates forecast transactions based on the associated models, which are used for reporting and control purposes.</span></span>

## <a name="forecast-models"></a><span data-ttu-id="5e3a3-189">Μοντέλα πρόβλεψης</span><span class="sxs-lookup"><span data-stu-id="5e3a3-189">Forecast models</span></span>
<span data-ttu-id="5e3a3-190">Τα μοντέλα πρόβλεψης έχουν μια ιεραρχία ενός επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-190">Forecast models have a single-layer hierarchy.</span></span> <span data-ttu-id="5e3a3-191">Αυτό σημαίνει ότι μια πρόβλεψη έργου πρέπει να συσχετιστεί με ένα μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-191">This means that one project forecast must be associated with one forecast model.</span></span>

<span data-ttu-id="5e3a3-192">Εάν χρησιμοποιείτε την πρόβλεψη έργου, μπορείτε να αναγνωρίσετε μοντέλα ως υπομοντέλα.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-192">If you use project forecasting, you can identify models as submodels.</span></span> <span data-ttu-id="5e3a3-193">Στη συνέχεια μπορείτε να δημιουργήσετε προβλέψεις κατά τμήμα, χρονική περίοδο ή περιοχή.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-193">You can then create forecasts by department, time period, or region.</span></span> <span data-ttu-id="5e3a3-194">Για παράδειγμα, μπορείτε να δημιουργήσετε ένα μοντέλο πρόβλεψης για ένα έτος και, στη συνέχεια, να δημιουργήσετε υπομοντέλα για τις τοπικές προβλέψεις βορειοανατολικά, νοτιοανατολικά, βορειοδυτικά και νοτιοδυτικά που υποβάλουν οι τοπικοί φορείς.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-194">For example, you can create a forecast model for a year, and then create submodels for the Northeast, Southeast, Northwest, and Southwest regional forecasts that regional heads submit.</span></span> <span data-ttu-id="5e3a3-195">Επιλέγοντας διάφορες επιλογές στις διαθέσιμες αναφορές, μπορείτε να προβάλετε τις πληροφορίες κατά συνολική πρόβλεψη ή κατά υπομοντέλο.</span><span class="sxs-lookup"><span data-stu-id="5e3a3-195">By selecting different options in the available reports, you can view information by total forecast or by submodel.</span></span>


