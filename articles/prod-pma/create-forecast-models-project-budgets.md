---
title: Δημιουργία μοντέλων πρόβλεψης για προϋπολογισμούς έργων
description: Αυτό το θέμα περιγράφει τον τρόπο δημιουργίας ενός μοντέλου πρόβλεψης για τους υπόλοιπους προϋπολογισμούς.
author: Yowelle
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 3549b41fce72b44230ab27de081dade15a912266
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006286"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="bfd99-103">Δημιουργία μοντέλων πρόβλεψης για προϋπολογισμούς έργων</span><span class="sxs-lookup"><span data-stu-id="bfd99-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="bfd99-104">Αυτό το θέμα περιγράφει τον τρόπο δημιουργίας ενός μοντέλου πρόβλεψης για τους υπόλοιπους προϋπολογισμούς.</span><span class="sxs-lookup"><span data-stu-id="bfd99-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="bfd99-105">Ένα έργο που υπόκειται σε στοιχείο ελέγχου προϋπολογισμού χρησιμοποιεί δύο τύπους προϋπολογισμών: τον αρχικό και τον υπόλοιπο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="bfd99-106">Όταν δημιουργείτε έναν προϋπολογισμό έργου, πρέπει να καθορίσετε τα μοντέλα πρόβλεψης αρχικού και υπόλοιπου προϋπολογισμού που δημιουργήθηκαν στη σελίδα **Μοντέλα πρόβλεψης**.</span><span class="sxs-lookup"><span data-stu-id="bfd99-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="bfd99-107">Οι προϋπολογισμοί έργου με βάση τα καθορισμένα μοντέλα δημιουργούνται κατά την ολοκλήρωση του προϋπολογισμού έργου.</span><span class="sxs-lookup"><span data-stu-id="bfd99-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="bfd99-108">Ένα μοντέλο πρόβλεψης που χρησιμοποιείται για το στοιχείο ελέγχου προϋπολογισμού δεν μπορεί να έχει ένα δευτερεύον μοντέλο ή να χρησιμοποιείται ως δευτερεύον μοντέλο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="bfd99-109">Επιλέξτε **Διαχείριση έργου και λογιστική** >  **Ρύθμιση** > **Προβλέψεις**  > **Μοντέλα πρόβλεψης**.</span><span class="sxs-lookup"><span data-stu-id="bfd99-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="bfd99-110">Επιλέξτε **Δημιουργία** για να δημιουργήσετε ένα νέο μοντέλο πρόβλεψης και, στη συνέχεια, καταχωρίστε έναν αριθμό αναγνωριστικού μοντέλου και ένα όνομα για το νέο μοντέλο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="bfd99-111">Ορίστε την επιλογή **Διακόπηκε** σε **Ναι** για να αποτρέψετε την αλλαγή στις γραμμές πρόβλεψης για το μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="bfd99-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="bfd99-112">Εάν οι γραμμές πρόβλεψης με τις οποίες σχετίζεται το μοντέλο πρέπει να δημιουργήσουν προβλέψεις ταμειακών ροών στη γενική λογιστική, ορίστε το στοιχείο **Να συμπεριληφθεί σε προβλέψεις ταμειακών ροών** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="bfd99-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="bfd99-113">Για να χρησιμοποιήσετε την ημερομηνία έργου ως ημερομηνία τιμολόγησης, ορίστε την **Ημερομηνία τιμολογίου πρόβλεψης** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="bfd99-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="bfd99-114">Στο πεδίο **Τύπος προϋπολογισμού**, επιλέξτε έναν από τους ακόλουθους τύπους μοντέλου:</span><span class="sxs-lookup"><span data-stu-id="bfd99-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="bfd99-115">**Αρχικός προϋπολογισμός**: Χρησιμοποιήστε τα ποσά αρχικού προϋπολογισμού που δεσμεύτηκαν κατά τη δημιουργία και την έγκριση του αρχικού προϋπολογισμού.</span><span class="sxs-lookup"><span data-stu-id="bfd99-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="bfd99-116">**Υπολειπόμενος προϋπολογισμός**: Χρησιμοποιήστε τα υπόλοιπα ποσά προϋπολογισμού κατά τη διάρκεια ζωής του έργου.</span><span class="sxs-lookup"><span data-stu-id="bfd99-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="bfd99-117">Τα υπόλοιπα σε αυτό το μοντέλο πρόβλεψης μειώνονται από τις πραγματικές συναλλαγές και αυξάνονται ή μειώνονται κατά τις αναθεωρήσεις του προϋπολογισμού.</span><span class="sxs-lookup"><span data-stu-id="bfd99-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="bfd99-118">**Μεταφορά**: Χρησιμοποιήστε τα ποσά προϋπολογισμού μεταφοράς για το έργο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="bfd99-119">Η μεταφορά είναι μια προαιρετική διεργασία που μπορεί να εκτελεστεί για τη μεταφορά μη χρησιμοποιημένων ποσών προϋπολογισμού από ένα οικονομικό έτος σε ένα άλλο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="bfd99-120">Ορίστε τις ακόλουθες επιλογές όπως απαιτείται:</span><span class="sxs-lookup"><span data-stu-id="bfd99-120">Set the following options as required:</span></span>

   - <span data-ttu-id="bfd99-121">Ενεργοποιήστε την **Ημερομηνία τιμολογίου πρόβλεψης** για να χρησιμοποιήσετε την ημερομηνία έργου ως ημερομηνία τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="bfd99-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="bfd99-122">Ενεργοποιήστε την **Πρόβλεψη με WIP** για πρόβλεψη με βάση την εργασία σε εξέλιξη (WIP) και, στη συνέχεια, επιλέξτε τον τύπο WIP.</span><span class="sxs-lookup"><span data-stu-id="bfd99-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="bfd99-123">Μπορείτε να διατηρήσετε τον προεπιλεγμένο **τύπο προϋπολογισμού** ως **Κανένας** ή να εισαγάγετε ένα νέο τύπο.</span><span class="sxs-lookup"><span data-stu-id="bfd99-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="bfd99-124">Ο τύπος προϋπολογισμού δεν μπορεί να αλλάξει μετά την αλλαγή μιας καρτέλας.</span><span class="sxs-lookup"><span data-stu-id="bfd99-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="bfd99-125">Εάν αλλάξετε τον προεπιλεγμένο τύπο προϋπολογισμού, όλες οι άλλες επιλογές δεν θα είναι διαθέσιμες για ενημερώσεις και δεν θα μπορείτε να χρησιμοποιήσετε ξανά αυτό το μοντέλο πρόβλεψης.</span><span class="sxs-lookup"><span data-stu-id="bfd99-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]