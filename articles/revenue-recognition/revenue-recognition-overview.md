---
title: Επισκόπηση αναγνώρισης εσόδων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναγνώριση εσόδων στο Project Operations.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f5f962572c6ec0298d2d91d33f83e4120a498a6f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013756"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="a5fe4-103">Επισκόπηση αναγνώρισης εσόδων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-103">Revenue recognition overview</span></span>

<span data-ttu-id="a5fe4-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="a5fe4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a5fe4-105">Στο Dynamics 365 Project Operations, οι αρχές αναγνώρισης εσόδων ποικίλλουν ανάλογα με την επιλεγμένη μέθοδο χρέωσης για ένα έργο ή τμήμα του έργου.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="a5fe4-106">Αυτό το θέμα παρέχει πληροφορίες σχετικά με την αναγνώριση εσόδων στο Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="a5fe4-107">Οι συναλλαγές υπολογίζονται ψρησιμοποιώντας μέθοδο χρέωσης χρόνου και υλικών</span><span class="sxs-lookup"><span data-stu-id="a5fe4-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="a5fe4-108">Η αναγνώριση κόστους και εσόδων συνδέονται.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="a5fe4-109">Το κόστος συναλλαγής και οι μη χρεωμένες πωλήσεις καταχωρούνται χρησιμοποιώντας το [ημερολόγιο ενοποίησης Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="a5fe4-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="a5fe4-110">Το προφίλ κόστους και εσόδων έργου προσδιορίζει εάν οι μη χρεωμένες συναλλαγές πωλήσεων καταχωρούνται στο γενικό καθολικό.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="a5fe4-111">Εάν έχει επιλεγεί το **Δεδουλευμένα έσοδα**, το σύστημα χρησιμοποιεί τους λογαριασμούς **τιμή πωλήσεων WIP** και την **τιμή πωλήσεων δεδουλευμένων εσόδων** κατά την καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="a5fe4-112">Ακολουθεί ένα παράδειγμα αυτής της μεθόδου.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="a5fe4-113">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="a5fe4-113">Transaction type</span></span> | <span data-ttu-id="a5fe4-114">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-114">Debit/Credit</span></span> | <span data-ttu-id="a5fe4-115">Ποσό</span><span class="sxs-lookup"><span data-stu-id="a5fe4-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="a5fe4-116">Τιμή πωλήσεων WIP</span><span class="sxs-lookup"><span data-stu-id="a5fe4-116">WIP Sales value</span></span> | <span data-ttu-id="a5fe4-117">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-117">Debit</span></span> | <span data-ttu-id="a5fe4-118">100</span><span class="sxs-lookup"><span data-stu-id="a5fe4-118">100</span></span> |
  | <span data-ttu-id="a5fe4-119">Τιμή πωλήσεων συσσωρευμένων εσόδων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-119">Accrued revenue sales value</span></span> | <span data-ttu-id="a5fe4-120">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-120">Credit</span></span> | <span data-ttu-id="a5fe4-121">100</span><span class="sxs-lookup"><span data-stu-id="a5fe4-121">100</span></span> |

- <span data-ttu-id="a5fe4-122">Τα έσοδα αναγνωρίζονται κατά την τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="a5fe4-123">Το σύστημα χρησιμοποιεί τον λογαριασμό **Τιμολογημένα έσοδα** κατά την καταχώρηση.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="a5fe4-124">Ακολουθεί ένα παράδειγμα αυτής της μεθόδου.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="a5fe4-125">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="a5fe4-125">Transaction type</span></span> | <span data-ttu-id="a5fe4-126">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-126">Debit/Credit</span></span> | <span data-ttu-id="a5fe4-127">Ποσό</span><span class="sxs-lookup"><span data-stu-id="a5fe4-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="a5fe4-128">Υπόλοιπο πελάτη</span><span class="sxs-lookup"><span data-stu-id="a5fe4-128">Customer balance</span></span> | <span data-ttu-id="a5fe4-129">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-129">Debit</span></span> | <span data-ttu-id="a5fe4-130">120</span><span class="sxs-lookup"><span data-stu-id="a5fe4-130">120</span></span> |
  | <span data-ttu-id="a5fe4-131">Πληρωτέος φόρος πωλήσεων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-131">Sales tax payable</span></span> | <span data-ttu-id="a5fe4-132">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-132">Credit</span></span> | <span data-ttu-id="a5fe4-133">20</span><span class="sxs-lookup"><span data-stu-id="a5fe4-133">20</span></span> |
  | <span data-ttu-id="a5fe4-134">Τιμολογημένα έσοδα</span><span class="sxs-lookup"><span data-stu-id="a5fe4-134">Invoiced Revenue</span></span> | <span data-ttu-id="a5fe4-135">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-135">Credit</span></span> | <span data-ttu-id="a5fe4-136">100</span><span class="sxs-lookup"><span data-stu-id="a5fe4-136">100</span></span> |

- <span data-ttu-id="a5fe4-137">Εάν τα έσοδα έχουν συγκεντρωθεί όταν καταχωρούνται οι πωλήσεις που δεν έχουν τιμολογηθεί, το σύστημα θα αντιλογίσει τα δεδουλευμένα έσοδα στην τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="a5fe4-138">Τύπος συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="a5fe4-138">Transaction type</span></span> | <span data-ttu-id="a5fe4-139">Χρέωση/Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-139">Debit/Credit</span></span> | <span data-ttu-id="a5fe4-140">Ποσό</span><span class="sxs-lookup"><span data-stu-id="a5fe4-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="a5fe4-141">Τιμή πωλήσεων WIP</span><span class="sxs-lookup"><span data-stu-id="a5fe4-141">WIP Sales value</span></span> | <span data-ttu-id="a5fe4-142">Πίστωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-142">Credit</span></span> | <span data-ttu-id="a5fe4-143">100</span><span class="sxs-lookup"><span data-stu-id="a5fe4-143">100</span></span> |
  | <span data-ttu-id="a5fe4-144">Τιμή πωλήσεων συσσωρευμένων εσόδων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-144">Accrued revenue sales value</span></span> | <span data-ttu-id="a5fe4-145">Χρέωση</span><span class="sxs-lookup"><span data-stu-id="a5fe4-145">Debit</span></span> | <span data-ttu-id="a5fe4-146">100</span><span class="sxs-lookup"><span data-stu-id="a5fe4-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="a5fe4-147">Οι συναλλαγές υπολογίζονται χρησιμοποιώντας τη μέθοδο χρέωσης σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="a5fe4-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="a5fe4-148">Η αναγνώριση κόστους και εσόδων είναι ξεχωριστή.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="a5fe4-149">Το κόστος συναλλαγής καταχωρείται χρησιμοποιώντας το [ημερολόγιο ενοποίησης Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="a5fe4-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="a5fe4-150">Οι συναλλαγές μη χρεωμένων πωλήσεων δεν δημιουργούνται.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="a5fe4-151">Τα έσοδα μπορούν να αναγνωριστούν κατά την τιμολόγηση, εάν το προφίλ κόστους και εσόδων του έργου έχουν **Αρχή που χρησιμοποιείται για τους υπολογισμούς ολοκλήρωσης έργου** που έχουν οριστεί σε **Όχι WIP**.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="a5fe4-152">Χρησιμοποιήστε αυτήν τη μέθοδο μόνο για βραχυπρόθεσμα, απλά έργα.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="a5fe4-153">Τα έσοδα μπορούν να αναγνωριστούν με τη χρήση εκτιμήσεων εσόδων σταθερής τιμής, είτε με τη μέθοδο **Ολοκληρωμένη σύμβαση** είτε με τη μέθοδο **Αναγνώριση εσόδων ποσοστού ολοκλήρωσης**.</span><span class="sxs-lookup"><span data-stu-id="a5fe4-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="a5fe4-154">Πρόσθετοι πόροι</span><span class="sxs-lookup"><span data-stu-id="a5fe4-154">Additional resources</span></span>
[<span data-ttu-id="a5fe4-155">Άρθρο για τη Ρύθμιση παραμέτρων λογιστικής για χρεώσιμα έργα</span><span class="sxs-lookup"><span data-stu-id="a5fe4-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="a5fe4-156">Έργα εκτίμησης εσόδων σταθερής τιμής</span><span class="sxs-lookup"><span data-stu-id="a5fe4-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="a5fe4-157">Διαχείριση εκτιμήσεων εσόδων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="a5fe4-158">Κόστος ολοκλήρωσης μεθόδων</span><span class="sxs-lookup"><span data-stu-id="a5fe4-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]