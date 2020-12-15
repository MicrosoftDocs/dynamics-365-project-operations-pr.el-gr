---
title: Επισκόπηση αναγνώρισης εσόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναγνώριση εσόδων στο Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6844f4c5d4cda8a6a901b0302448f70f4c597f5d
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531434"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="7dbb1-103">Επισκόπηση αναγνώρισης εσόδων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-103">Revenue recognition overview</span></span>

<span data-ttu-id="7dbb1-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="7dbb1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="7dbb1-105">Στο Dynamics 365 Project Operations, οι αρχές αναγνώρισης εσόδων ποικίλλουν ανάλογα με την επιλεγμένη μέθοδο χρέωσης για ένα έργο ή τμήμα του έργου.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="7dbb1-106">Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναγνώριση εσόδων στο Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="7dbb1-107">Οι συναλλαγές υπολογίζονται ψρησιμοποιώντας μέθοδο χρέωσης χρόνου και υλικών</span><span class="sxs-lookup"><span data-stu-id="7dbb1-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="7dbb1-108">Η αναγνώριση κόστους και εσόδων συνδέονται.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="7dbb1-109">Το κόστος συναλλαγής και οι μη χρεωμένες πωλήσεις καταχωρούνται χρησιμοποιώντας το [ημερολόγιο ενοποίησης Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="7dbb1-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="7dbb1-110">Το προφίλ κόστους και εσόδων έργου προσδιορίζει εάν οι μη χρεωμένες συναλλαγές πωλήσεων καταχωρούνται στο γενικό καθολικό.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="7dbb1-111">Εάν έχει επιλεγεί το **Δεδουλευμένα έσοδα**, το σύστημα χρησιμοποιεί τους λογαριασμούς **τιμή πωλήσεων WIP** και την **τιμή πωλήσεων δεδουλευμένων εσόδων** κατά την καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="7dbb1-112">Ακολουθεί ένα παράδειγμα αυτής της μεθόδου.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="7dbb1-113">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="7dbb1-113">Transaction type</span></span> | <span data-ttu-id="7dbb1-114">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-114">Debit/Credit</span></span> | <span data-ttu-id="7dbb1-115">Ποσό</span><span class="sxs-lookup"><span data-stu-id="7dbb1-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="7dbb1-116">Τιμή πωλήσεων WIP</span><span class="sxs-lookup"><span data-stu-id="7dbb1-116">WIP Sales value</span></span> | <span data-ttu-id="7dbb1-117">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-117">Debit</span></span> | <span data-ttu-id="7dbb1-118">100</span><span class="sxs-lookup"><span data-stu-id="7dbb1-118">100</span></span> |
  | <span data-ttu-id="7dbb1-119">Τιμή πωλήσεων συσσωρευμένων εσόδων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-119">Accrued revenue sales value</span></span> | <span data-ttu-id="7dbb1-120">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-120">Credit</span></span> | <span data-ttu-id="7dbb1-121">100</span><span class="sxs-lookup"><span data-stu-id="7dbb1-121">100</span></span> |

- <span data-ttu-id="7dbb1-122">Τα έσοδα αναγνωρίζονται κατά την τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="7dbb1-123">Το σύστημα χρησιμοποιεί τον λογαριασμό **Τιμολογημένα έσοδα** κατά την καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="7dbb1-124">Ακολουθεί ένα παράδειγμα αυτής της μεθόδου.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="7dbb1-125">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="7dbb1-125">Transaction type</span></span> | <span data-ttu-id="7dbb1-126">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-126">Debit/Credit</span></span> | <span data-ttu-id="7dbb1-127">Ποσό</span><span class="sxs-lookup"><span data-stu-id="7dbb1-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="7dbb1-128">Υπόλοιπο πελάτη</span><span class="sxs-lookup"><span data-stu-id="7dbb1-128">Customer balance</span></span> | <span data-ttu-id="7dbb1-129">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-129">Debit</span></span> | <span data-ttu-id="7dbb1-130">120</span><span class="sxs-lookup"><span data-stu-id="7dbb1-130">120</span></span> |
  | <span data-ttu-id="7dbb1-131">Πληρωτέος φόρος πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-131">Sales tax payable</span></span> | <span data-ttu-id="7dbb1-132">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-132">Credit</span></span> | <span data-ttu-id="7dbb1-133">20</span><span class="sxs-lookup"><span data-stu-id="7dbb1-133">20</span></span> |
  | <span data-ttu-id="7dbb1-134">Τιμολογημένα έσοδα</span><span class="sxs-lookup"><span data-stu-id="7dbb1-134">Invoiced Revenue</span></span> | <span data-ttu-id="7dbb1-135">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-135">Credit</span></span> | <span data-ttu-id="7dbb1-136">100</span><span class="sxs-lookup"><span data-stu-id="7dbb1-136">100</span></span> |

- <span data-ttu-id="7dbb1-137">Εάν τα έσοδα έχουν συγκεντρωθεί όταν καταχωρούνται οι πωλήσεις που δεν έχουν τιμολογηθεί, το σύστημα θα αντιλογίσει τα δεδουλευμένα έσοδα στην τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="7dbb1-138">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="7dbb1-138">Transaction type</span></span> | <span data-ttu-id="7dbb1-139">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-139">Debit/Credit</span></span> | <span data-ttu-id="7dbb1-140">Ποσό</span><span class="sxs-lookup"><span data-stu-id="7dbb1-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="7dbb1-141">Τιμή πωλήσεων WIP</span><span class="sxs-lookup"><span data-stu-id="7dbb1-141">WIP Sales value</span></span> | <span data-ttu-id="7dbb1-142">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-142">Credit</span></span> | <span data-ttu-id="7dbb1-143">100</span><span class="sxs-lookup"><span data-stu-id="7dbb1-143">100</span></span> |
  | <span data-ttu-id="7dbb1-144">Τιμή πωλήσεων συσσωρευμένων εσόδων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-144">Accrued revenue sales value</span></span> | <span data-ttu-id="7dbb1-145">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="7dbb1-145">Debit</span></span> | <span data-ttu-id="7dbb1-146">100</span><span class="sxs-lookup"><span data-stu-id="7dbb1-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="7dbb1-147">Οι συναλλαγές υπολογίζονται χρησιμοποιώντας τη μέθοδο χρέωσης σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="7dbb1-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="7dbb1-148">Η αναγνώριση κόστους και εσόδων είναι ξεχωριστή.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="7dbb1-149">Το κόστος συναλλαγής καταχωρείται χρησιμοποιώντας το [ημερολόγιο ενοποίησης Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="7dbb1-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="7dbb1-150">Οι συναλλαγές μη χρεωμένων πωλήσεων δεν δημιουργούνται.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="7dbb1-151">Τα έσοδα μπορούν να αναγνωριστούν κατά την τιμολόγηση, εάν το προφίλ κόστους και εσόδων του έργου έχουν **Αρχή που χρησιμοποιείται για τους υπολογισμούς ολοκλήρωσης έργου** που έχουν οριστεί σε **Όχι WIP**.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="7dbb1-152">Χρησιμοποιήστε αυτήν τη μέθοδο μόνο για βραχυπρόθεσμα, απλά έργα.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="7dbb1-153">Τα έσοδα μπορούν να αναγνωριστούν με τη χρήση εκτιμήσεων εσόδων σταθερής τιμής, είτε με τη μέθοδο **Ολοκληρωμένη σύμβαση** είτε με τη μέθοδο **Αναγνώριση εσόδων ποσοστού ολοκλήρωσης**.</span><span class="sxs-lookup"><span data-stu-id="7dbb1-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="7dbb1-154">Πρόσθετοι πόροι</span><span class="sxs-lookup"><span data-stu-id="7dbb1-154">Additional resources</span></span>
[<span data-ttu-id="7dbb1-155">Άρθρο για τη Ρύθμιση παραμέτρων λογιστικής για χρεώσιμα έργα</span><span class="sxs-lookup"><span data-stu-id="7dbb1-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="7dbb1-156">Έργα εκτίμησης εσόδων σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="7dbb1-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="7dbb1-157">Διαχείριση εκτιμήσεων εσόδων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="7dbb1-158">Κόστος ολοκλήρωσης μεθόδων</span><span class="sxs-lookup"><span data-stu-id="7dbb1-158">Cost to complete methods</span></span>](cost-complete-methods.md)
