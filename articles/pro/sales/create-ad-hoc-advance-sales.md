---
title: Δημιουργία μιας επί τούτου προπληρωμής σε μια σύμβαση - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία μιας προκαταβολής σε μια σύμβαση, ανάλογα με τις ανάγκες.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a6bf02c2e2ab2f3c696b1eab1b92a20272187bf5
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181362"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract---lite"></a><span data-ttu-id="20ecd-103">Δημιουργία μιας επί τούτου προπληρωμής σε μια σύμβαση - lite</span><span class="sxs-lookup"><span data-stu-id="20ecd-103">Creating an ad hoc advance on a contract - lite</span></span>

<span data-ttu-id="20ecd-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="20ecd-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="20ecd-105">Το Microsoft Dynamics 365 Project Operations υποστηρίζει σενάρια τιμολόγησης που περιλαμβάνουν προπληρωμές και προκαταβολές.</span><span class="sxs-lookup"><span data-stu-id="20ecd-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="20ecd-106">Η διεργασία για τη χρήση **προκαταβολών** στο **Project Operations** είναι παρόμοια με τις συμβάσεις **προπληρωμής**.</span><span class="sxs-lookup"><span data-stu-id="20ecd-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="20ecd-107">Ολοκληρώστε τα παρακάτω βήματα για να τιμολογήσετε τον πελάτη για μια προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="20ecd-108">Μεταβείτε στη σελίδα **Σύμβαση έργου** και, στη συνέχεια, επιλέξτε την καρτέλα **Προκαταβολές και προπληρωμές**.</span><span class="sxs-lookup"><span data-stu-id="20ecd-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="20ecd-109">Στο υποπλέγμα που περιλαμβάνει όλες τις προκαταβολές και τις προπληρωμές που έχουν καταγραφεί προηγουμένως, επιλέξτε **+ Νέα προπληρωμή σύμβασης έργου**.</span><span class="sxs-lookup"><span data-stu-id="20ecd-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="20ecd-110">Η φόρμα **Γρήγορη δημιουργία** ανοίγει για την καταχώρηση μιας προπληρωμής ή μιας προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="20ecd-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="20ecd-111">Στον παρακάτω πίνακα παρουσιάζονται τα πεδία για την καταγραφή μιας προκαταβολής και τα θέματα που πρέπει να λάβετε υπόψη σας καθώς δημιουργείτε νέα:</span><span class="sxs-lookup"><span data-stu-id="20ecd-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="20ecd-112">Πεδίο</span><span class="sxs-lookup"><span data-stu-id="20ecd-112">Field</span></span> | <span data-ttu-id="20ecd-113">Περιγραφή</span><span class="sxs-lookup"><span data-stu-id="20ecd-113">Description</span></span> | <span data-ttu-id="20ecd-114">Κατάντη επίπτωση</span><span class="sxs-lookup"><span data-stu-id="20ecd-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="20ecd-115">**Πελάτης σύμβασης έργου**</span><span class="sxs-lookup"><span data-stu-id="20ecd-115">**Project Contract Customer**</span></span> | <span data-ttu-id="20ecd-116">Αυτό το πεδίο δηλώνει ποιος πελάτης στη σύμβαση θα τιμολογηθεί για αυτήν την προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="20ecd-117">Εάν έχετε πολλούς πελάτες στη σύμβαση και θέλετε να τιμολογήσετε κάθε έναν από αυτούς για ένα συγκεκριμένο ποσό προπληρωμής ή προκαταβολής, δημιουργήστε μια προκαταβολή για κάθε πελάτη ξεχωριστά.</span><span class="sxs-lookup"><span data-stu-id="20ecd-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="20ecd-118">**Περιγραφή**</span><span class="sxs-lookup"><span data-stu-id="20ecd-118">**Description**</span></span> | <span data-ttu-id="20ecd-119">Η περιγραφή του σκοπού ή του χρόνου της προκαταβολής για τον προσδιορισμό αυτής της προκαταβολής.</span><span class="sxs-lookup"><span data-stu-id="20ecd-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="20ecd-120">Αυτή η περιγραφή εμφανίζεται στη γραμμή τιμολογίου για αυτήν την προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="20ecd-121">**Ποσό**</span><span class="sxs-lookup"><span data-stu-id="20ecd-121">**Amount**</span></span> | <span data-ttu-id="20ecd-122">Το ποσό για την προπληρωμή ή την προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="20ecd-123">Αυτό το ποσό εμφανίζεται στη γραμμή τιμολογίου για αυτήν την προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="20ecd-124">**Δεδομένα τιμολογίου**</span><span class="sxs-lookup"><span data-stu-id="20ecd-124">**Invoice Date**</span></span> | <span data-ttu-id="20ecd-125">Η ημερομηνία τιμολόγησης αυτής της προκαταβολής στον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="20ecd-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="20ecd-126">Αυτή είναι η ημερομηνία για τη διαδικασία αυτόματης δημιουργίας τιμολογίων για τη δημιουργία μιας γραμμής τιμολογίου για αυτήν την προκαταβολή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="20ecd-127">**Κατάσταση τιμολογίου**</span><span class="sxs-lookup"><span data-stu-id="20ecd-127">**Invoice Status**</span></span> | <span data-ttu-id="20ecd-128">Αυτή είναι μια ρύθμιση επιλογών που υποδεικνύει εάν αυτή η προκαταβολή προστίθεται σε προσχέδιο τιμολογίου για αυτόν τον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="20ecd-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="20ecd-129">Οι πιθανές τιμές είναι:</span><span class="sxs-lookup"><span data-stu-id="20ecd-129">The possible values are:</span></span></br><span data-ttu-id="20ecd-130">- **Ανέτοιμο για τιμολόγηση**</span><span class="sxs-lookup"><span data-stu-id="20ecd-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="20ecd-131">- **Έτοιμο για τιμολόγηση**</span><span class="sxs-lookup"><span data-stu-id="20ecd-131">- **Ready to invoice**</span></span> | <span data-ttu-id="20ecd-132">Όταν μια προκαταβολή ή προπληρωμή έχει σημανθεί ως **Έτοιμο για τιμολόγηση**, προστίθεται ως χρόνος γραμμής σε ένα προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="20ecd-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="20ecd-133">Μόνο μια πλήρως τιμολογημένη προκαταβολή μπορεί να χρησιμοποιηθεί για τη συμφωνία με το κόστος έργου για την επόμενη περίοδο τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="20ecd-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="20ecd-134">Επιλέξτε **Αποθήκευση και κλείσιμο** στο παράθυρο διαλόγου γρήγορης δημιουργία για να καταγράψετε την προκαταβολή ή την προπληρωμή.</span><span class="sxs-lookup"><span data-stu-id="20ecd-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>