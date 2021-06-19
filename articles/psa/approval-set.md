---
title: Σύνολα έγκρισης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το σύνολο έγκρισης, τις αιτήσεις και τα υποσύνολα αυτών των λειτουργιών.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116871"
---
# <a name="approval-sets"></a><span data-ttu-id="16da6-103">Σύνολα έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="16da6-104">Η "Έγκριση" ορίζει τις αιτήσεις έγκρισης ομάδας σε μικρότερα υποσύνολα λειτουργιών.</span><span class="sxs-lookup"><span data-stu-id="16da6-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="16da6-105">Αυτή η ομαδοποίηση επιτρέπει την επεξεργασία των εγκρίσεων με τη σειρά κατά Έργο και επιτρέπει την επανάληψη και την ακολουθία.</span><span class="sxs-lookup"><span data-stu-id="16da6-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="16da6-106">Η ομαδοποίηση βελτιώνει την αξιοπιστία και την ανιχνευσιμότητα της επεξεργασίας έγκρισης για έγκριση μεγάλων όγκων.</span><span class="sxs-lookup"><span data-stu-id="16da6-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="16da6-107">Τα σύνολα έγκρισης δηλώνουν τη συνολική κατάσταση επεξεργασίας των σχετικών καρτελών τους.</span><span class="sxs-lookup"><span data-stu-id="16da6-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="16da6-108">Όταν γίνεται επεξεργασία μιας καρτέλας έγκρισης με χρήση ενός συνόλου έγκρισης, η καρτέλα μετακινείται από την καρτέλα **Υποβλήθηκε** σε **εγκρίθηκε** και δεν θα γίνει σύνδεση από το σύνολο έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="16da6-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="16da6-109">Εάν μια καρτέλα αποτύχει όταν υποβληθεί για έγκριση, η καρτέλα παραμένει σε κατάσταση **Υποβλήθηκε** και το σύνολο έγκρισης επισημαίνεται ως αποτυχημένο.</span><span class="sxs-lookup"><span data-stu-id="16da6-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="16da6-110">Το σύνολο έγκρισης καταγράφει το μήνυμα σφάλματος της αποτυχίας.</span><span class="sxs-lookup"><span data-stu-id="16da6-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="16da6-111">Επεξεργασία εγκρίσεων και συνόλων έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="16da6-112">Οι εγκρίσεις που βρίσκονται στην ουρά για επεξεργασία είναι ορατές στην προβολή **Επεξεργασία εγκρίσεων**.</span><span class="sxs-lookup"><span data-stu-id="16da6-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="16da6-113">Το σύστημα προσπαθεί να επεξεργαστεί όλες τις καταχωρήσεις ασύγχρονα, συμπεριλαμβανομένης της επανάληψης μιας έγκρισης σε περίπτωση που οι προηγούμενες προσπάθειες απέτυχαν.</span><span class="sxs-lookup"><span data-stu-id="16da6-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="16da6-114">Το πεδίο **Διάρκεια ζωής συνόλου έγκρισης** καταγράφει τον αριθμό των προσπαθειών επεξεργασίας του συνόλου προτού επισημανθεί ως αποτυχημένο.</span><span class="sxs-lookup"><span data-stu-id="16da6-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="16da6-115">Αποτυχημένες εγκρίσεις και σύνολα έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="16da6-116">Η προβολή **Αποτυχημένες εγκρίσεις** παραθέτει όλες τις εγκρίσεις που απαιτούν παρέμβαση χρήστη.</span><span class="sxs-lookup"><span data-stu-id="16da6-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="16da6-117">Ανοίξτε τα σχετικά αρχεία καταγραφής του συνόλου έγκρισης για να προσδιορίσετε την αιτία της αποτυχίας.</span><span class="sxs-lookup"><span data-stu-id="16da6-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="16da6-118">Επιλέγοντας **Επανάληψη** προστίθεται στο πλήθος διάρκειας ζωής του συνόλου έγκρισης, η έγκριση μετακινεί την έγκριση ξανά σε κατάσταση **Επεξεργασία** και επιχειρεί να επεξεργαστεί τις υπόλοιπες καρτέλες.</span><span class="sxs-lookup"><span data-stu-id="16da6-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="16da6-119">Ρύθμιση παραμέτρων συνόλων έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="16da6-120">Ενεργοποίηση της δυνατότητας συνόλων έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="16da6-121">Πριν ενεργοποιήσετε τη δυνατότητα "Σύνολα έγκρισης", βεβαιωθείτε ότι δεν υπάρχουν εγκρίσεις προς το παρόν προς επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="16da6-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="16da6-122">Μεταβείτε στη σελίδα **Παράμετροι έργου** και επιλέξτε **Στοιχείο ελέγχου δυνατότητας** > **Ενεργοποίηση σύγχρονων εγκρίσεων**.</span><span class="sxs-lookup"><span data-stu-id="16da6-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="16da6-123">Απενεργοποίηση της δυνατότητας συνόλων έγκρισης</span><span class="sxs-lookup"><span data-stu-id="16da6-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="16da6-124">Πριν απενεργοποιήσετε τη δυνατότητα "Σύνολα έγκρισης", βεβαιωθείτε ότι δεν υπάρχουν εγκρίσεις προς το παρόν προς επεξεργασία.</span><span class="sxs-lookup"><span data-stu-id="16da6-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="16da6-125">Μεταβείτε στη σελίδα **Παράμετροι έργου** και επιλέξτε **Στοιχείο ελέγχου δυνατότητας** > **Απενεργοποίηση σύγχρονων εγκρίσεων**.</span><span class="sxs-lookup"><span data-stu-id="16da6-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="16da6-126">Ρύθμιση παραμέτων του ασύγχρονου ορίου</span><span class="sxs-lookup"><span data-stu-id="16da6-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="16da6-127">Όταν δημιουργούνται σύνολα έγκρισης, η επεξεργασία μετακινείται στο παρασκήνιο όταν ο επιλεγμένος αριθμός καρτελών για έγκριση υπερβαίνει το επιλεγμένο όριο.</span><span class="sxs-lookup"><span data-stu-id="16da6-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="16da6-128">Χρησιμοποιήστε το πεδίο **Ασύγχρονη τιμή κατωφλίου** για να ρυθμίσετε πότε η επεξεργασία έγκρισης θα πρέπει να εκτελείται ταυτόχρονα ή ασύγχρονα.</span><span class="sxs-lookup"><span data-stu-id="16da6-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="16da6-129">Οι έγκυρες τιμές είναι:</span><span class="sxs-lookup"><span data-stu-id="16da6-129">Valid values are:</span></span>

  - <span data-ttu-id="16da6-130">Μηδέν: η επεξεργασία όλων των αιτήσεων πρέπει να γίνεται ασύγχρονα.</span><span class="sxs-lookup"><span data-stu-id="16da6-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="16da6-131">Αριθμοί μεγαλύτεροι από μηδέν: η επεξεργασία των εγκρίσεων γίνεται ασύγχρονα μόνο όταν ο αριθμός έγκρισης που έχει υποβληθεί υπερβαίνει αυτήν την τιμή.</span><span class="sxs-lookup"><span data-stu-id="16da6-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
