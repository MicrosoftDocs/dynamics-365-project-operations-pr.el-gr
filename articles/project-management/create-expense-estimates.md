---
title: Εκτιμήσεις εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον ορισμό ή τον υπολογισμό των εξόδων βάσει έργου.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287058"
---
# <a name="expense-estimates"></a><span data-ttu-id="7784b-103">Εκτιμήσεις εξόδων</span><span class="sxs-lookup"><span data-stu-id="7784b-103">Expense estimates</span></span>
<span data-ttu-id="7784b-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="7784b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7784b-105">Μαζί με τον καθορισμό εκτιμήσεων βάσει πόρων, το Dynamics 365 Project Operations επιτρέπει στους διαχειριστές έργων να ορίζουν εμπειρίες βάσει έργου για κάθε έργο.</span><span class="sxs-lookup"><span data-stu-id="7784b-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="7784b-106">Κάθε στοιχείο εξόδων μπορεί να συσχετιστεί με μια συγκεκριμένη εργασία έργου ή κατηγορία εξόδων.</span><span class="sxs-lookup"><span data-stu-id="7784b-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="7784b-107">Οι κατηγορίες δαπανών καθορίζονται συνήθως σε επίπεδο οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="7784b-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="7784b-108">Η τιμολόγηση για κάθε κατηγορία εξόδων καθορίζεται συνήθως στην ακόλουθη ιεραρχία:</span><span class="sxs-lookup"><span data-stu-id="7784b-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="7784b-109">Εταιρεία</span><span class="sxs-lookup"><span data-stu-id="7784b-109">Organization</span></span>
- <span data-ttu-id="7784b-110">Πελάτης</span><span class="sxs-lookup"><span data-stu-id="7784b-110">Customer</span></span>
- <span data-ttu-id="7784b-111">Προσφορά/σύμβαση</span><span class="sxs-lookup"><span data-stu-id="7784b-111">Quote/contract</span></span>

<span data-ttu-id="7784b-112">Ολοκληρώστε τα παρακάτω βήματα για να προβάλετε, να προσθέσετε ή να διαγράψετε μια δαπάνη έργου.</span><span class="sxs-lookup"><span data-stu-id="7784b-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="7784b-113">Μεταβείτε στα **Έργα** και επιλέξτε το έργο στο οποίο θέλετε να εργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="7784b-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="7784b-114">Επιλέξτε τη σελίδα **Εκτιμήσεις έργου** και προβάλετε τη λίστα των εξόδων έργου.</span><span class="sxs-lookup"><span data-stu-id="7784b-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="7784b-115">Επιλέξτε **Νέα δαπάνη** για να προσθέσετε μια δαπάνη.</span><span class="sxs-lookup"><span data-stu-id="7784b-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="7784b-116">Εναλλακτικά, επιλέξτε μια δαπάνη για διαγραφή και, στη συνέχεια, επιλέξτε **Διαγραφή δαπάνης**.</span><span class="sxs-lookup"><span data-stu-id="7784b-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="7784b-117">Για κάθε στοιχείο γραμμή εξόδων ορίζονται τα παρακάτω χαρακτηριστικά:</span><span class="sxs-lookup"><span data-stu-id="7784b-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="7784b-118">**Κατηγορία**: οι συνηθισμένες ομαδοποιήσεις που χρησιμοποιούνται για την περιγραφή όλων των εξόδων που πραγματοποιήθηκαν σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="7784b-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="7784b-119">**Ημερομηνία έναρξης**: η ημερομηνία κατά την οποία αναμένεται να πραγματοποιηθεί η δαπάνη.</span><span class="sxs-lookup"><span data-stu-id="7784b-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="7784b-120">**Ποσότητα**: ο εκτιμώμενος αριθμός των στοιχείων εξόδων για μια συγκεκριμένη κατηγορία.</span><span class="sxs-lookup"><span data-stu-id="7784b-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="7784b-121">**Τιμή κόστους μονάδας**: η τιμή μονάδας που χρησιμοποιήθηκε για τον υπολογισμό του κόστους της δαπάνης.</span><span class="sxs-lookup"><span data-stu-id="7784b-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="7784b-122">**Τιμή πώλησης μονάδας**: Η τιμή μονάδας που χρησιμοποιήθηκε για τον υπολογισμό των τιμών πώλησης της δαπάνης.</span><span class="sxs-lookup"><span data-stu-id="7784b-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]