---
title: Εκτιμήσεις εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον ορισμό ή τον υπολογισμό των εξόδων βάσει έργου.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2afe4ff2f84fc5426c409e6314da73b11a4de281
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076838"
---
# <a name="expense-estimates"></a><span data-ttu-id="5b6ce-103">Εκτιμήσεις εξόδων</span><span class="sxs-lookup"><span data-stu-id="5b6ce-103">Expense estimates</span></span>
<span data-ttu-id="5b6ce-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="5b6ce-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5b6ce-105">Μαζί με τον καθορισμό εκτιμήσεων βάσει πόρων, το Dynamics 365 Project Operations επιτρέπει στους διαχειριστές έργου να καθορίσουν τα έξοδα βάσει έργου για κάθε έργο.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="5b6ce-106">Κάθε στοιχείο εξόδων μπορεί να συσχετιστεί με μια συγκεκριμένη εργασία έργου ή κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="5b6ce-107">Οι κατηγορίες δαπανών καθορίζονται συνήθως σε επίπεδο οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="5b6ce-108">Η τιμολόγηση για κάθε κατηγορία εξόδων καθορίζεται συνήθως στην ακόλουθη ιεραρχία:</span><span class="sxs-lookup"><span data-stu-id="5b6ce-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="5b6ce-109">Εταιρεία</span><span class="sxs-lookup"><span data-stu-id="5b6ce-109">Organization</span></span>
- <span data-ttu-id="5b6ce-110">Πελάτης</span><span class="sxs-lookup"><span data-stu-id="5b6ce-110">Customer</span></span>
- <span data-ttu-id="5b6ce-111">Προσφορά/σύμβαση</span><span class="sxs-lookup"><span data-stu-id="5b6ce-111">Quote/contract</span></span>

<span data-ttu-id="5b6ce-112">Ολοκληρώστε τα παρακάτω βήματα για να προβάλετε, να προσθέσετε ή να διαγράψετε μια δαπάνη έργου.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="5b6ce-113">Μεταβείτε στα **Έργα** και επιλέξτε το έργο στο οποίο θέλετε να εργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-113">Go to **Projects** , and select the project you want to work on.</span></span>
2. <span data-ttu-id="5b6ce-114">Επιλέξτε τη σελίδα **Εκτιμήσεις έργου** και προβάλετε τη λίστα των εξόδων έργου.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="5b6ce-115">Επιλέξτε **Νέα δαπάνη** για να προσθέσετε μια δαπάνη.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="5b6ce-116">Εναλλακτικά, επιλέξτε μια δαπάνη για διαγραφή και, στη συνέχεια, επιλέξτε **Διαγραφή δαπάνης**.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="5b6ce-117">Για κάθε στοιχείο γραμμή εξόδων ορίζονται τα παρακάτω χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="5b6ce-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="5b6ce-118">**Κατηγορία** : οι συνηθισμένες ομαδοποιήσεις που χρησιμοποιούνται για την περιγραφή όλων των εξόδων που πραγματοποιήθηκαν σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-118">**Category** : The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="5b6ce-119">**Ημερομηνία έναρξης** : η ημερομηνία κατά την οποία αναμένεται να πραγματοποιηθεί η δαπάνη.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-119">**Start Date** : The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="5b6ce-120">**Ποσότητα** : ο εκτιμώμενος αριθμός των στοιχείων εξόδων για μια συγκεκριμένη κατηγορία.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-120">**Quantity** : The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="5b6ce-121">**Τιμή κόστους μονάδας** : η τιμή μονάδας που χρησιμοποιήθηκε για τον υπολογισμό του κόστους της δαπάνης.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-121">**Unit Cost Price** : The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="5b6ce-122">**Τιμή πώλησης μονάδας** : Η τιμή μονάδας που χρησιμοποιήθηκε για τον υπολογισμό των τιμών πώλησης της δαπάνης.</span><span class="sxs-lookup"><span data-stu-id="5b6ce-122">**Unit Sales Price** : The unit price used to calculate the sale prices of the expense.</span></span>

