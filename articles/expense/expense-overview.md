---
title: Επισκόπηση εξόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη λειτουργία εξόδων στο Project Operations.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 6da831fef5dba060b8019d7689645405c7ebdbed
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076796"
---
# <a name="expense-home-page"></a><span data-ttu-id="60ade-103">Αρχική σελίδα εξόδων</span><span class="sxs-lookup"><span data-stu-id="60ade-103">Expense home page</span></span>

<span data-ttu-id="60ade-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="60ade-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="60ade-105">Το Dynamics 365 Project Operations υποστηρίζει τη δυνατότητα επεξεργασίας εξόδων.</span><span class="sxs-lookup"><span data-stu-id="60ade-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="60ade-106">Η επεξεργασία εξόδων πραγματοποιείται με ή χωρίς έργα χρησιμοποιώντας μια προσαρμόσιμη ροή εργασιών πολιτικών, κατηγοριών συναλλαγών και εγκρίσεων.</span><span class="sxs-lookup"><span data-stu-id="60ade-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="60ade-107">Στο Project Operations, υπάρχουν δύο υποστηριζόμενα μοντέλα ανάπτυξης για έξοδα:</span><span class="sxs-lookup"><span data-stu-id="60ade-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="60ade-108">**Πλήρης** : Είναι διαθέσιμη η πλήρης ανάπτυξη για τα **Σενάρια Project Operations βασισμένα σε πόρους/μη εφοδιασμένα** ή **Project Operations για σενάρια βασισμένα σε εντολές παραγωγής**.</span><span class="sxs-lookup"><span data-stu-id="60ade-108">**Full** : Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order based scenarios**.</span></span>
- <span data-ttu-id="60ade-109">**Βασική** : Η βασική ανάπτυξη είναι διαθέσιμη για τα **Σενάρια Project Operations βασισμένα σε πόρους/μη εφοδιασμένα** και **Ελαφριά ανάπτυξη – συμφωνία για προτιμολόγηση**.</span><span class="sxs-lookup"><span data-stu-id="60ade-109">**Basic** : Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="60ade-110">Πλήρης</span><span class="sxs-lookup"><span data-stu-id="60ade-110">Full</span></span> 
<span data-ttu-id="60ade-111">Η πλήρης ανάπτυξη δαπάνης παρέχει μια πλήρη εφαρμογή πολιτικής η οποία περιλαμβάνει τη δυνατότητα δημιουργίας πολιτικών, όπως:</span><span class="sxs-lookup"><span data-stu-id="60ade-111">Full Expense deployment provides a complete policy enforcement which includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="60ade-112">Όρια κατηγορίας εξόδων</span><span class="sxs-lookup"><span data-stu-id="60ade-112">Expense category limits</span></span>
  - <span data-ttu-id="60ade-113">Ταξίδια</span><span class="sxs-lookup"><span data-stu-id="60ade-113">Travel</span></span>
  - <span data-ttu-id="60ade-114">Ημερήσια αποζημίωση</span><span class="sxs-lookup"><span data-stu-id="60ade-114">Per diem</span></span>
  - <span data-ttu-id="60ade-115">Εισαγωγές πιστωτικής κάρτας</span><span class="sxs-lookup"><span data-stu-id="60ade-115">Credit card imports</span></span>
  - <span data-ttu-id="60ade-116">Λήψη οπτικής αναγνώρισης χαρακτήρων</span><span class="sxs-lookup"><span data-stu-id="60ade-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="60ade-117">Βασικό</span><span class="sxs-lookup"><span data-stu-id="60ade-117">Basic</span></span> 
<span data-ttu-id="60ade-118">Το σενάριο ανάπτυξης βασικών δαπανών σάς επιτρέπει να καταγράφετε μόνο τις βασικές δαπάνες σε σχέση με ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="60ade-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="60ade-119">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [Καταχώρηση εξόδων (ελαφριά)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="60ade-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="60ade-120">Προσδιορισμός της ανάπτυξης εξόδων</span><span class="sxs-lookup"><span data-stu-id="60ade-120">Determine your Expense deployment</span></span>
<span data-ttu-id="60ade-121">Για να διαπιστώσετε εάν εκτελείτε τη βασική ανάπτυξη διαχείρισης εξόδων, επαληθεύστε ότι η διεύθυνση URL διεύθυνσης τελειώνει σε **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="60ade-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 
