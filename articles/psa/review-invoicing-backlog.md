---
title: Εξετάστε τις λίστες εκκρεμοτήτων τιμολόγησης για τα έργα και τις συμβάσεις έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ελέγχου του χρόνου, των εξόδων και των λιστών εκκρεμοτήτων προϊόντων, καθώς και τον τρόπο με τον οποίο μπορείτε να τα επισημάνετε ως έτοιμα για τιμολόγηση.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: eb6d942d61bf8b5d20afb75c88716132a596bcbd
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077125"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="04bc5-103">Εξετάστε τις λίστες εκκρεμοτήτων τιμολόγησης για τα έργα και τις συμβάσεις έργου</span><span class="sxs-lookup"><span data-stu-id="04bc5-103">Review the invoicing backlog on projects and project contracts</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="04bc5-104">Όταν μια συναλλαγή είναι έτοιμη να δημιουργήσει και να επεξεργαστεί ένα τιμολόγιο, η συναλλαγή θα πρέπει να είναι επισημασμένη ως **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="04bc5-105">Αυτό το θέμα περιγράφει τους τύπους των συναλλαγών που μπορούν να δημιουργηθούν.</span><span class="sxs-lookup"><span data-stu-id="04bc5-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="04bc5-106">Εξετάστε τον χρόνο και τη λίστα εκκρεμοτήτων χρέωσης υλικού</span><span class="sxs-lookup"><span data-stu-id="04bc5-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="04bc5-107">Όταν μια καταχώρηση χρόνου ή εξόδων υποβάλλεται και εγκρίνεται για ένα έργο, το PSA δημιουργεί ένα πραγματικό έργο.</span><span class="sxs-lookup"><span data-stu-id="04bc5-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="04bc5-108">Εάν ο συνδυασμός του έργου και της κλάσης συναλλαγής αντιστοιχίζονται σε μια γραμμή σύμβασης για ένα έργο χρόνου και υλικού, δημιουργούνται δύο πραγματικά στοιχεία κατά την έγκριση της καταχώρησης:</span><span class="sxs-lookup"><span data-stu-id="04bc5-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="04bc5-109">Πραγματικό κόστος</span><span class="sxs-lookup"><span data-stu-id="04bc5-109">Cost actual</span></span> 
- <span data-ttu-id="04bc5-110">Πραγματικές μη χρεώσιμες πωλήσεις</span><span class="sxs-lookup"><span data-stu-id="04bc5-110">Unbilled sales actual</span></span>

<span data-ttu-id="04bc5-111">Οι πραγματικές μη χρεώσιμες πωλήσεις αντιπροσωπεύουν τη λίστα εκκρεμοτήτων χρέωσης και η κατάσταση χρέωσής τους πρέπει να οριστεί σε **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="04bc5-112">Όταν δημιουργείται ένα τιμολόγιο έργου, οι πραγματικές μη χρεώσιμες πωλήσεις επισημαίνονται **Έτοιμο για τιμολόγηση** αντιγράφονται ως λεπτομέρειες για τη σειρά τιμολογίων.</span><span class="sxs-lookup"><span data-stu-id="04bc5-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="04bc5-113">Για να εξετάσετε τη λίστα εκκρεμοτήτων χρέωσης για χρόνο και υλικό, μεταβείτε στις **Πωλήσεις** \> **Χρέωση** \> **Λίστα εκκρεμοτήτων χρέωσης χρόνου και υλικού**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="04bc5-114">Επιλέξτε όλες τις πραγματικές μη χρεωμένες πωλήσεις που είναι έτοιμες για τιμολόγηση και, στη συνέχεια, επιλέξτε **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="04bc5-115">Η κατάσταση χρέωσης αυτών των πραγματικών τιμών αλλάζει σε **Έτοιμο προς τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![Λίστα εκκρεμοτήτων χρέωσης ώρας και υλικού](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="04bc5-117">Εξέταση λίστας εκκρεμοτήτων χρέωσης προϊόντος</span><span class="sxs-lookup"><span data-stu-id="04bc5-117">Review the product billing backlog</span></span>

<span data-ttu-id="04bc5-118">Στο PSA, όταν μια σύμβαση έργου έχει γραμμές σύμβασης βασισμένες σε προϊόντα, οι εν λόγω γραμμές λαμβάνονται υπόψη για τιμολόγηση κάθε φορά που δημιουργείται ένα τιμολόγιο για τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="04bc5-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="04bc5-119">Κάθε προϊόν που έχει γραμμές σύμβασης που έχουν επισημανθεί ως **Έτοιμο για τιμολόγηση** αντιγράφεται στο τιμολόγιο έργου ως γραμμές τιμολογίου έργου.</span><span class="sxs-lookup"><span data-stu-id="04bc5-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="04bc5-120">Για να εξετάσετε τη λίστα εκκρεμοτήτων χρέωσης για προϊόντα μεταβείτε στις **Πωλήσεις** \> **Χρέωση** \> **Λίστα εκκρεμοτήτων χρέωσης προϊόντων**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="04bc5-121">Επιλέξτε όλες τις γραμμές σύμβασης που βασίζονται σε προϊόντα που είναι έτοιμα για τιμολόγηση και, στη συνέχεια, επιλέξτε **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="04bc5-122">Η κατάσταση χρέωσης αυτών των γραμμών αλλάζει σε **Έτοιμο προς τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![Λίστα εκκρεμοτήτων χρέωσης προϊόντος](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="04bc5-124">Εξέταση ορόσημων χρέωσης σε συμβάσεις σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="04bc5-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="04bc5-125">Κάθε μια από τις γραμμές σύμβασης έργου που έχει μια μέθοδο χρέωσης προκαθορισμένης τιμής πρέπει να καθορίζει τα ορόσημα της σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="04bc5-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="04bc5-126">Αυτά τα ορόσημα σύμβασης μπορούν να τιμολογούνται μόνο εάν έχουν επισημανθεί ως **Έτοιμα για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="04bc5-127">Για να εξετάσετε τα ορόσημα χρέωσης, μεταβείτε στις **Πωλήσεις** \> **Χρέωση** \> **Ορόσημα σταθερής τιμής**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="04bc5-128">Επιλέξτε τα ορόσημα που είναι έτοιμα για τιμολόγηση και, στη συνέχεια, επιλέξτε **Έτοιμο για τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="04bc5-129">Η κατάσταση χρέωσης αυτών των ορόσημων αλλάζει σε **Έτοιμο προς τιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="04bc5-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![Ορόσημα σταθερής τιμής](media/FPBacklog.png)
