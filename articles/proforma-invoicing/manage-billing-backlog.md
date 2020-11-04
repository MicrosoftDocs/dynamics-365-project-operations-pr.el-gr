---
title: Διαχείριση της λίστας εκκρεμοτήτων χρέωσης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο προβολής και επεξεργασίας της λίστας εκκρεμοτήτων χρέωσης στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ec77f3911a460b96414a61bc44ea254f1b7da660
ms.sourcegitcommit: f8edff6422b82fdf2cea897faa6abb51e2c0c3c8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/21/2020
ms.locfileid: "4087930"
---
# <a name="manage-the-billing-backlog"></a><span data-ttu-id="1bafb-103">Διαχείριση της λίστας εκκρεμοτήτων χρέωσης</span><span class="sxs-lookup"><span data-stu-id="1bafb-103">Manage the billing backlog</span></span>

<span data-ttu-id="1bafb-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="1bafb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1bafb-105">Το Dynamics 365 Project Operations διαθέτει δύο αποκλειστικές προβολές που θα σας βοηθήσουν να εργαστείτε και να διαχειριστείτε τη λίστα εκκρεμοτήτων χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="1bafb-105">Dynamics 365 Project Operations has two dedicated views to help you work with and manage the billing backlog.</span></span> <span data-ttu-id="1bafb-106">Πρόκειται για τα **Ορόσημα με προκαθορισμένη τιμή** και τη **Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού**. Για να επιλέξετε μια προβολή, στην περιοχή **Πωλήσεις** του Project Operations, στη σελίδα περιήγησης αριστερά, επιλέξτε **Χρέωση**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-106">They are **Fixed Price Milestones** and **Time and Material Billing Backlog** To select a view, in the **Sales** area of Project Operations, on the left navigation page, select **Billing**.</span></span> <span data-ttu-id="1bafb-107">Οι συνδέσεις της λίστας εκκρεμοτήτων χρέωσης αποθηκεύονται εκεί.</span><span class="sxs-lookup"><span data-stu-id="1bafb-107">The billing backlog links are stored there.</span></span>

## <a name="fixed-price-milestones"></a><span data-ttu-id="1bafb-108">Ορόσημα σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="1bafb-108">Fixed Price Milestones</span></span>

<span data-ttu-id="1bafb-109">Αυτή η προβολή εμφανίζει όλα τα ορόσημα με προκαθορισμένη τιμή σε όλες τις γραμμές σύμβασης έργου στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="1bafb-109">This view lists all fixed price milestones across all of the project contract lines in the system.</span></span> <span data-ttu-id="1bafb-110">Τα μεμονωμένα ή πολλαπλά ορόσημα μπορούν να χαρακτηριστούν ως **Έτοιμο για τιμολόγηση** ή **Δεν είναι έτοιμο για τιμολόγηση** από αυτήν την προβολή.</span><span class="sxs-lookup"><span data-stu-id="1bafb-110">Single or multiple milestones can be marked as **Ready to Invoice** or **Not Ready to Invoice** from this view.</span></span> <span data-ttu-id="1bafb-111">Όταν επισημαίνετε ένα ορόσημο ως **Έτοιμο για τιμολόγηση** , το ορόσημο είναι διαθέσιμο για ένα προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="1bafb-111">When you mark a milestone as **Ready to Invoice** , the milestone becomes available for a draft invoice.</span></span>

<span data-ttu-id="1bafb-112">Όταν οι γραμμές σύμβασης πολλών πελατών έχουν μια μέθοδο χρέωσης σταθερής τιμής, δημιουργείται ένα ορόσημο για κάθε πελάτη της γραμμής σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="1bafb-112">When multi-customer contract lines have a fixed price billing method, one milestone is created for each customer on the contract line.</span></span> <span data-ttu-id="1bafb-113">Ο χρήστης δημιουργεί ένα ορόσημο και αυτό το ορόσημο διαιρείται στις καρτέλες πελάτης=συγκεκριμένες καρτέλες ορόσημου εσωτερικά, σύμφωνα με το ποσοστό διαίρεσης χρέωσης που έχει οριστεί για κάθε πελάτη στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="1bafb-113">The user creates a milestone and that milestone is split into customer=specific milestone records internally, according to the billing percentage split defined for each customer on the contract line.</span></span> <span data-ttu-id="1bafb-114">Στην προβολή **Ορόσημα σταθερής τιμής** , θα δείτε μεμονωμένες καρτέλες ορόσημων για τον συγκεκριμένο πελάτη.</span><span class="sxs-lookup"><span data-stu-id="1bafb-114">In the **Fixed Price Milestones** view, you will see individual customer-specific milestone records.</span></span> <span data-ttu-id="1bafb-115">Κάθε μία από αυτές τις καρτέλες με τα ορόσημα μπορεί να χαρακτηριστεί ως **Έτοιμο για τιμολόγηση** ξεχωριστά από αυτήν την προβολή.</span><span class="sxs-lookup"><span data-stu-id="1bafb-115">Each of these milestone records can be marked as **Ready to Invoice** separately from this view.</span></span> <span data-ttu-id="1bafb-116">Όταν μία ή περισσότερες διαιρέσεις ορόσημου επισημαίνεται ως **Έτοιμο για τιμολόγηση** , η κεφαλίδα μετακινείται σε κατάσταση **Σε εξέλιξη** από **Δεν έχει ξεκινήσει**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-116">When one or more of the related milestone splits are marked as **Ready to Invoice** , the header moves to a status of **In Progress** from **Not Started**.</span></span> <span data-ttu-id="1bafb-117">Όταν όλες οι διαιρέσεις ορόσημου έχουν τιμολογηθεί, η κεφαλίδα της κατάστασης του ορόσημου γίνεται **Ολοκληρώθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-117">When all of the milestone splits have been invoiced, the header milestone status becomes **Completed**.</span></span>

<span data-ttu-id="1bafb-118">Σε αυτήν την προβολή εμφανίζεται ένα ορόσημο σε ένα προσχέδιο τιμολόγιο με μια κατάσταση χρέωσης για το **Τιμολόγιο πελάτη που δημιουργήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-118">A milestone on a draft invoice is shown in this view with a billing status of **Customer Invoice Created**.</span></span> <span data-ttu-id="1bafb-119">Όταν επιβεβαιωθεί το προσχέδιο του τιμολογίου, η κατάσταση χρέωσης σε αυτήν την καρτέλα ενημερώνεται σε **Το τιμολόγιο καταχωρήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-119">When the draft invoice is confirmed, the billing status on this record is updated to **Invoice Posted**.</span></span> <span data-ttu-id="1bafb-120">Η ενημέρωση αυτής της τιμής κατάστασης με χρήση προσαρμοσμένου κώδικα δεν συνιστάται.</span><span class="sxs-lookup"><span data-stu-id="1bafb-120">Updating this status value by using custom code isn't recommended.</span></span> <span data-ttu-id="1bafb-121">Το Project Operations δεν θα λειτουργεί σωστά εάν αυτές οι τιμές κατάστασης ενημερωθούν με προσαρμοσμένο κώδικα.</span><span class="sxs-lookup"><span data-stu-id="1bafb-121">Project Operations won't function correctly if these status values are updated with custom code.</span></span>

## <a name="time-and-material-billing-backlog"></a><span data-ttu-id="1bafb-122">Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού</span><span class="sxs-lookup"><span data-stu-id="1bafb-122">Time and Material Billing Backlog</span></span>

<span data-ttu-id="1bafb-123">Αυτή η προβολή περιλαμβάνει όλες τις μη χρεωμένες πραγματικές πωλήσεις οι οποίες δεν έχουν τιμολογηθεί σε όλες τις συμβάσεις έργου στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="1bafb-123">This view lists all unbilled sales actuals that haven't been invoiced across all project contracts in the system.</span></span> <span data-ttu-id="1bafb-124">Οι μεμονωμένες ή οι πολλαπλές μη χρεωμένες πραγματικές πωλήσεις μπορούν να χαρακτηριστούν ως **Έτοιμο για τιμολόγηση** ή **Δεν είναι έτοιμο για τιμολόγηση** από αυτήν την προβολή.</span><span class="sxs-lookup"><span data-stu-id="1bafb-124">Single or multiple unbilled sales actuals can be marked as **Ready to Invoice** or **Not Ready to Invoice** from this view.</span></span> <span data-ttu-id="1bafb-125">Η σήμανση μιας μη χρεωμένης πραγματικής πώλησης ως **Έτοιμο για τιμολόγηση** καθιστά δυνατή την τοποθέτηση σε προσχέδιο τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="1bafb-125">Marking an unbilled sales actual as **Ready to Invoice** makes it available to be put on a draft invoice.</span></span>

<span data-ttu-id="1bafb-126">Οι μη χρεωμένες πραγματικές πωλήσεις με κατάσταση **Μη υπέρβαση** του **Απέτυχε** δεν είναι δυνατό να επισημανθούν ως **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-126">Unbilled sales actuals that have a **Not-to-Exceed** status of **Failed** can't be marked as **Ready to Invoice**.</span></span> <span data-ttu-id="1bafb-127">Εάν αυτές οι πραγματικές τιμές πρέπει να επισημαίνονται με αυτόν τον τρόπο, επαναφέρετε την κατάσταση άλλων πραγματικών στοιχείων στη γραμμή σύμβασης που έχουν δεσμευτεί και, στη συνέχεια, αξιολογήστε την κατάσταση **Μη υπέρβαση**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-127">If these actuals need to be marked as such, reset the status on other actuals on the contract line that are committed, and then evaluate the **Not-to-Exceed** status.</span></span>

<span data-ttu-id="1bafb-128">Στην περίπτωση γραμμών σύμβασης πολλών πελατών που έχουν μια μέθοδο χρέωσης χρόνου και υλικού, όταν γίνεται έγκριση χρόνου και εξόδων, δημιουργείται μια πραγματική μη χρεωμένη πώληση για κάθε πελάτη στη γραμμή σύμβασης, σύμφωνα με τη διαίρεση ποσοστού χρέωσης που έχει οριστεί για κάθε πελάτη στη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="1bafb-128">In the case of multi-customer contract lines that have a time and material billing method, when time and expenses are approved, an unbilled sales actual is created for each customer on the contract line according to the billing percentage split defined for each customer on the contract line.</span></span> <span data-ttu-id="1bafb-129">Στην προβολή **Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού** , θα δείτε αυτές τις μεμονωμένες μη χρεωμένες πραγματικές πωλήσεις για τον πελάτη.</span><span class="sxs-lookup"><span data-stu-id="1bafb-129">In the **Time and Material Billing Backlog** view, you'll see these individual customer-specific unbilled sales actuals.</span></span> <span data-ttu-id="1bafb-130">Κάθε μία από αυτές τις καρτέλες μη χρεωμένων πραγματικών πωλήσεων μπορεί να χαρακτηριστεί ως **Έτοιμο για τιμολόγηση** ξεχωριστά από αυτήν την προβολή.</span><span class="sxs-lookup"><span data-stu-id="1bafb-130">Each of these unbilled sales actual records can be marked as **Ready to Invoice** separately from this view.</span></span>

<span data-ttu-id="1bafb-131">Σε αυτήν την προβολή εμφανίζεται μια μη χρεωμένη πραγματική πώληση σε ένα προσχέδιο τιμολόγιο με μια **Κατάσταση χρέωσης** **Τιμολόγιο πελάτη που δημιουργήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-131">An unbilled sales actual on a draft invoice is shown in this view with a **Billing Status** of **Customer Invoice Created**.</span></span> <span data-ttu-id="1bafb-132">Όταν επιβεβαιωθεί το προσχέδιο του τιμολογίου, η κατάσταση χρέωσης σε αυτήν την καρτέλα ενημερώνεται σε **Το τιμολόγιο πελάτη καταχωρήθηκε**.</span><span class="sxs-lookup"><span data-stu-id="1bafb-132">When the draft invoice is confirmed, the billing status on this record is updated to **Customer Invoice Posted**.</span></span> <span data-ttu-id="1bafb-133">Η ενημέρωση αυτής της τιμής κατάστασης όταν είναι σε αυτήν την κατάσταση με χρήση προσαρμοσμένου κώδικα δεν συνιστάται.</span><span class="sxs-lookup"><span data-stu-id="1bafb-133">Updating this status value when it is in this state by using custom code isn't recommended.</span></span> <span data-ttu-id="1bafb-134">Το Project Operations δεν θα λειτουργεί σωστά εάν αυτές οι τιμές κατάστασης ενημερωθούν με προσαρμοσμένο κώδικα.</span><span class="sxs-lookup"><span data-stu-id="1bafb-134">Project Operations won't function correctly when these status values are updated with custom code.</span></span>