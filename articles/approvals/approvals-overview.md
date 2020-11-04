---
title: Επισκόπηση εγκρίσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με εγκρίσεις στο Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076776"
---
# <a name="approvals-overview"></a><span data-ttu-id="62f8f-103">Επισκόπηση εγκρίσεων</span><span class="sxs-lookup"><span data-stu-id="62f8f-103">Approvals overview</span></span>

<span data-ttu-id="62f8f-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="62f8f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="62f8f-105">Οι υποβολές χρόνου και εξόδων μετακινούνται μέσω μιας ροής εργασιών έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="62f8f-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="62f8f-106">Μετά την έγκριση των καταχωρήσεων, οι συναλλαγές καταγράφονται στις πραγματικές τιμές ή γίνεται κράτηση του χρόνου στο χρονοδιάγραμμα.</span><span class="sxs-lookup"><span data-stu-id="62f8f-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="62f8f-107">Ροή εργασιών εγκρίσεων</span><span class="sxs-lookup"><span data-stu-id="62f8f-107">Approvals workflow</span></span>
<span data-ttu-id="62f8f-108">Όταν δημιουργείτε και υποβάλλετε μια καταχώρηση χρόνου ή εξόδων, δημιουργείται μια εγγραφή έγκρισης.</span><span class="sxs-lookup"><span data-stu-id="62f8f-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="62f8f-109">Ο υπεύθυνος έγκρισης έργου ή ο διευθυντής σας ελέγχουν και εγκρίνουν την καταχώρισή σας.</span><span class="sxs-lookup"><span data-stu-id="62f8f-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="62f8f-110">Εάν η εγγραφή σχετίζεται με ένα έργο, όταν εγκριθεί, θα δημιουργηθούν οι πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="62f8f-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="62f8f-111">Με αυτόν τον τρόπο, το κόστος και η χρέωση πρέπει να παρακολουθούνται.</span><span class="sxs-lookup"><span data-stu-id="62f8f-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="62f8f-112">Έγκριση καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="62f8f-112">Approve an entry</span></span>
<span data-ttu-id="62f8f-113">Η φόρμα **Εγκρίσεις** σάς δίνει τη δυνατότητα να κάνετε εναλλαγή μεταξύ διαφορετικών προβολών ώστε να μπορείτε να προβάλλετε τους διαφορετικούς τύπους εγκρίσεων.</span><span class="sxs-lookup"><span data-stu-id="62f8f-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="62f8f-114">Μεταβείτε στη φόρμα **Εγκρίσεις** και επιλέξτε **Έξοδα** , **Ώρα** ή **Ανακλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-114">Go to the **Approvals** form and select **Expenses** , **Time** , or **Recalls**.</span></span>
2. <span data-ttu-id="62f8f-115">Εξετάστε κάθε έγκριση και επιλέξτε αυτές που θέλετε να εγκρίνετε.</span><span class="sxs-lookup"><span data-stu-id="62f8f-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="62f8f-116">Επιλέξτε **Έγκριση** για να εγκρίνετε τις επιλεγμένες καταχωρήσεις.</span><span class="sxs-lookup"><span data-stu-id="62f8f-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="62f8f-117">Το σύστημα θα επεξεργαστεί αυτές τις καταχωρήσεις και θα δημιουργήσει πραγματικές τιμές ή μια κράτηση.</span><span class="sxs-lookup"><span data-stu-id="62f8f-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="62f8f-118">Απόρριψη καταχώρησης</span><span class="sxs-lookup"><span data-stu-id="62f8f-118">Reject an entry</span></span>
<span data-ttu-id="62f8f-119">Ως υπεύθυνος έγκρισης έργου, μπορεί να χρειαστεί να στείλετε ξανά μια καταχώρηση σε ένα χρήστη για διόρθωση.</span><span class="sxs-lookup"><span data-stu-id="62f8f-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="62f8f-120">Μεταβείτε στη φόρμα **Εγκρίσεις** και επιλέξτε την καταχώρηση που θα απορρίψετε.</span><span class="sxs-lookup"><span data-stu-id="62f8f-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="62f8f-121">Επιλέξτε **Απόρριψη**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-121">Select **Reject**.</span></span>
3. <span data-ttu-id="62f8f-122">Προαιρετικό - Προσθέστε ένα σχόλιο στο παράθυρο διαλόγου **Σχόλια απόρριψης** για να ενημερώσετε το χρήστη γιατί απορρίφθηκε η καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="62f8f-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="62f8f-123">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-123">Select **OK**.</span></span> <span data-ttu-id="62f8f-124">Η εγγραφή θα επιστραφεί στο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="62f8f-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="62f8f-125">Ανάκληση καταχωρήσεων</span><span class="sxs-lookup"><span data-stu-id="62f8f-125">Recall entries</span></span>
<span data-ttu-id="62f8f-126">Σε κάποιο σημείο, μπορεί να χρειαστεί να ανακαλέσετε μια καταχώρηση που υποβλήθηκε.</span><span class="sxs-lookup"><span data-stu-id="62f8f-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="62f8f-127">Εάν η εγγραφή δεν έχει εγκριθεί, θα επιστραφεί αμέσως.</span><span class="sxs-lookup"><span data-stu-id="62f8f-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="62f8f-128">Μια εγκεκριμένη εγγραφή, ωστόσο, μπορεί να έχει σημαντική επίπτωση.</span><span class="sxs-lookup"><span data-stu-id="62f8f-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="62f8f-129">Ο υπεύθυνος έγκρισης έργου υποχρεούται να εγκρίνει την ανάκληση προκειμένου να αντιστρέψει τη συναλλαγή στις πραγματικές τιμές.</span><span class="sxs-lookup"><span data-stu-id="62f8f-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="62f8f-130">Καθορισμός υπεύθυνων έγκρισης έργου</span><span class="sxs-lookup"><span data-stu-id="62f8f-130">Specify Project approvers</span></span>
<span data-ttu-id="62f8f-131">Κάθε έργο έχει ορισμένα μέλη ομάδας έργου.</span><span class="sxs-lookup"><span data-stu-id="62f8f-131">Each project has a number of project team members.</span></span> <span data-ttu-id="62f8f-132">Μπορείτε να καθορίσετε τα μέλη της ομάδας που θα είναι επίσης υπεύθυνοι έγκρισης έργου.</span><span class="sxs-lookup"><span data-stu-id="62f8f-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="62f8f-133">Μεταβείτε στη φόρμα **Έργα** και ανοίξτε το έργο από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="62f8f-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="62f8f-134">Στην καρτέλα **Ομάδα** , επιλέξτε το μέλος της ομάδας που θα είναι υπεύθυνος έγκρισης έργου και, στη συνέχεια, κάντε κλικ στην επιλογή **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="62f8f-135">Ορίστε το πεδίο **Υπεύθυνος έγκρισης έργου** σε **Ναι**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="62f8f-136">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-136">Select **Save**.</span></span>
5. <span data-ttu-id="62f8f-137">Επαναλάβετε τα βήματα 2-4 για να προσθέσετε επιπλέον υπεύθυνους έγκρισης έργου.</span><span class="sxs-lookup"><span data-stu-id="62f8f-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="62f8f-138">Ρύθμιση παραμέτρων του διαχειριστή χρήστη</span><span class="sxs-lookup"><span data-stu-id="62f8f-138">Configure the user's manager</span></span>

1. <span data-ttu-id="62f8f-139">Μεταβείτε στην επιλογή **Ρυθμίσεις** > **Ασφάλεια** > **Χρήστες**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="62f8f-140">Επιλέξτε το χρήστη στον οποίο αναθέτετε έναν διευθυντή και στην περιοχή **Πληροφορίες οργανισμού** , επιλέξτε το διευθυντή από τη λίστα.</span><span class="sxs-lookup"><span data-stu-id="62f8f-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="62f8f-141">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="62f8f-141">Select **Save**.</span></span>

