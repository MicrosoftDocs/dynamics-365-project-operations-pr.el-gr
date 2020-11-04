---
title: Δημιουργία και εφαρμογή όρων διατήρησης πληρωμής προμηθευτών
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης και διατήρησης των όρων διατήρησης για πληρωμές προμηθευτών.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077053"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="c78ea-103">Δημιουργία και εφαρμογή όρων διατήρησης πληρωμής προμηθευτών</span><span class="sxs-lookup"><span data-stu-id="c78ea-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="c78ea-104">Η ρύθμιση των όρων διατήρησης της πληρωμής από προμηθευτές για ένα έργο είναι χρήσιμη όταν ο οργανισμός σας θέλει να διατηρήσει μέρος των πληρωμών που πραγματοποιήθηκαν σε έναν πωλητή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="c78ea-105">Για παράδειγμα, όταν θέλετε να βάλετε σε αναμονή μια πληρωμή σε έναν πωλητή έως ότου τα προϊόντα που παραδόθηκαν να ανταποκρίνονται στις προσδοκίες σας.</span><span class="sxs-lookup"><span data-stu-id="c78ea-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="c78ea-106">Οι όροι διατήρησης πληρωμής προμηθευτών μπορούν να καθοριστούν όταν διαπραγματεύεστε μια σύμβαση προμηθευτών.</span><span class="sxs-lookup"><span data-stu-id="c78ea-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="c78ea-107">Δημιουργία όρων διατήρησης πληρωμής προμηθευτών</span><span class="sxs-lookup"><span data-stu-id="c78ea-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="c78ea-108">Μπορείτε να εισαγάγετε το ποσοστό της πληρωμής του πωλητή προς διατήρηση και το ποσοστό των προηγούμενων διατηρούμενων ποσών που θα αποδεσμευτούν.</span><span class="sxs-lookup"><span data-stu-id="c78ea-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="c78ea-109">Τα ποσά διατηρούνται αυτόματα σε τιμολόγια προμηθευτών έως ότου η σύμβαση φθάσει στην καθορισμένη κατάσταση ολοκλήρωσης.</span><span class="sxs-lookup"><span data-stu-id="c78ea-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="c78ea-110">Μετά τη ρύθμιση των όρων διατήρησης, μπορείτε να τους εφαρμόσετε σε οποιοδήποτε έργο για αυτόν τον πωλητή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="c78ea-111">Χρησιμοποιήστε τα παρακάτω βήματα για να δημιουργήσετε και να διατηρήσετε όρους διατήρησης για πληρωμές προμηθευτών.</span><span class="sxs-lookup"><span data-stu-id="c78ea-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="c78ea-112">Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική** > **Διατήρηση** > **Όροι διατήρησης πληρωμής προμηθευτών**.</span><span class="sxs-lookup"><span data-stu-id="c78ea-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="c78ea-113">Επιλέξτε **Δημιουργία** για να προσθέσετε ένα νέο όρο διατήρησης πωλητή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="c78ea-114">Η τιμή **Αναγνωριστικό κανόνα** για τον νέο όρο καταχωρείται αυτόματα.</span><span class="sxs-lookup"><span data-stu-id="c78ea-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="c78ea-115">Καταχωρίστε μια σύντομη περιγραφή στο πεδίο **Περιγραφή** και στη συνοπτική καρτέλα **Όροι** επιλέξτε **Προσθήκη γραμμής** για την εισαγωγή τιμών όρων για τα εξής:</span><span class="sxs-lookup"><span data-stu-id="c78ea-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="c78ea-116">**Ποσοστό παραδοθέντων μονάδων** : Καταχωρίστε ένα ποσοστό ολοκλήρωσης για τον όρο.</span><span class="sxs-lookup"><span data-stu-id="c78ea-116">**Percentage of units delivered** : Enter a percentage of completion for the term.</span></span> <span data-ttu-id="c78ea-117">Τα ποσά διατηρούνται αυτόματα σε τιμολόγια προμηθευτών έως ότου το στάδιο ολοκλήρωσης έργου ισούται με το καθορισμένο ποσοστό.</span><span class="sxs-lookup"><span data-stu-id="c78ea-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="c78ea-118">Για παράδειγμα, εάν καταχωρείτε 50.00, τα ποσά διατηρούνται μέχρι να ολοκληρωθεί το 50 τοις εκατό του έργου.</span><span class="sxs-lookup"><span data-stu-id="c78ea-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="c78ea-119">**Ποσοστό διατήρησης** : Καταχωρίστε ένα ποσοστό του ποσού του τιμολογίου του προμηθευτή που θα διατηρηθεί.</span><span class="sxs-lookup"><span data-stu-id="c78ea-119">**Percentage to retain** : Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="c78ea-120">Για παράδειγμα, εάν εισαγάγετε 10.00, τότε το 10% του ποσού σε ένα τιμολόγιο πωλητή διατηρείται μέχρι το έργο να φθάσει στο ποσοστό ολοκλήρωσης που έχει οριστεί στο πεδίο **Ποσοστό παραδοθέντων μονάδων**.</span><span class="sxs-lookup"><span data-stu-id="c78ea-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="c78ea-121">**Ποσοστό αποδέσμευσης** : Επιλέξτε **Προσθήκη γραμμής** για να καταχωρίσετε ένα ποσοστό από τα ποσά που διατηρήθηκαν προηγουμένως και πρόκειται να αποδεσμευτούν για το επιλεγμένο επίπεδο ολοκλήρωσης έργου.</span><span class="sxs-lookup"><span data-stu-id="c78ea-121">**Percentage to release** : Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="c78ea-122">Εάν έχετε περισσότερα από ένα ορόσημα για διαφορετικά επίπεδα ολοκλήρωσης έργου, καταχωρίστε μια ξεχωριστή γραμμή όρου διατήρησης προμηθευτών για κάθε κανόνα διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="c78ea-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="c78ea-123">Κάθε γραμμή μπορεί να προσδιορίζει ένα διαφορετικό ποσοστό διατήρησης και ένα διαφορετικό ποσοστό αποδέσμευσης για κάθε καθορισμένο επίπεδο ολοκλήρωσης έργου.</span><span class="sxs-lookup"><span data-stu-id="c78ea-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="c78ea-124">Μετά τη δημιουργία όρων διατήρησης προμηθευτή για έναν προμηθευτή, μπορείτε να εφαρμόσετε τους όρους σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="c78ea-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="c78ea-125">Εφαρμογή όρων διατήρησης προμηθευτή σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="c78ea-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="c78ea-126">Μεταβείτε στην ενότητα **Διαχείριση έργου και λογιστική** > **Έργα** > **Όλα τα έργα** και ανοίξτε ένα έργο από τη σελίδα λίστας έργων.</span><span class="sxs-lookup"><span data-stu-id="c78ea-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="c78ea-127">Στη συνοπτική καρτέλα **Συμφωνίες προμηθευτών** επιλέξτε **Προσθήκη γραμμής**.</span><span class="sxs-lookup"><span data-stu-id="c78ea-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="c78ea-128">Στο πεδίο **Κωδικός λογαριασμού** , επιλέξτε ένα από τα εξής:</span><span class="sxs-lookup"><span data-stu-id="c78ea-128">In the **Account code field** , select one of the following options:</span></span> 

   - <span data-ttu-id="c78ea-129">**Πίνακας** : Οι όροι διατήρησης προμηθευτή ισχύουν για έναν μόνο πωλητή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-129">**Table** : The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="c78ea-130">**Ομάδα** – Οι όροι διατήρησης προμηθευτή ισχύουν για όλους τους πωλητές σε μια ομάδα προμηθευτών.</span><span class="sxs-lookup"><span data-stu-id="c78ea-130">**Group** : The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="c78ea-131">**Όλοι** : Οι όροι διατήρησης προμηθευτή ισχύουν για όλους τους προμηθευτές.</span><span class="sxs-lookup"><span data-stu-id="c78ea-131">**All** : The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="c78ea-132">Στο πεδίο **Προμηθευτής/Ομάδα προμηθευτών** , επιλέξτε τον προμηθευτή ή την ομάδα προμηθευτών όπου εφαρμόζονται οι όροι διατήρησης του προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-132">In the **Vendor/Vendor group field** , select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="c78ea-133">Εάν επιλέξατε **Όλοι** στο προηγούμενο βήμα, αυτό το πεδίο δεν είναι διαθέσιμο.</span><span class="sxs-lookup"><span data-stu-id="c78ea-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="c78ea-134">Στο πεδίο **Όροι διατήρησης προμηθευτών** , επιλέξτε τους όρους διατήρησης που δημιουργήσατε στην προηγούμενη διαδικασία.</span><span class="sxs-lookup"><span data-stu-id="c78ea-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="c78ea-135">Σε περίπτωση που το έργο έχει επίσης ορίσει όρους πληρωμής κατά την πληρωμή (PWP) για τον προμηθευτή, εισαγάγετε το ποσοστό κατωφλίου για το έργο στο πεδίο **Ποσοστό κατωφλίου PWP**.</span><span class="sxs-lookup"><span data-stu-id="c78ea-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="c78ea-136">Οι όροι διατήρησης προμηθευτών εμφανίζονται επίσης στις παραγγελίες αγοράς που δημιουργείτε για τον πωλητή.</span><span class="sxs-lookup"><span data-stu-id="c78ea-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>
