---
title: Ρύθμιση παραμέτρων λογιστικής για εσωτερικά έργα
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης των πρακτικών λογιστικής για εσωτερικά έργα στο Project Operations.
author: sigitac
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ad8b974ef75cb0a4e43af0aa254cec1bbcab154a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012856"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="49560-103">Ρύθμιση παραμέτρων λογιστικής για εσωτερικά έργα</span><span class="sxs-lookup"><span data-stu-id="49560-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="49560-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="49560-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="49560-105">Τα εσωτερικά έργα επιτρέπουν στις εταιρείες να παρακολουθούν το κόστος που σχετίζεται με δραστηριότητες που δεν χρεώνονται σε έναν πελάτη.</span><span class="sxs-lookup"><span data-stu-id="49560-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="49560-106">Παραδείγματα εσωτερικών έργων είναι τα εξής:</span><span class="sxs-lookup"><span data-stu-id="49560-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="49560-107">Η ανάπτυξη ενός προϊόντος, για παράδειγμα, μιας εφαρμογής για κινητές συσκευές και η παρακολούθηση του κόστους που σχετίζεται με την ανάπτυξη.</span><span class="sxs-lookup"><span data-stu-id="49560-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="49560-108">Η διαχείριση χρόνου και εξόδων πριν από την πώληση.</span><span class="sxs-lookup"><span data-stu-id="49560-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="49560-109">Αυτό το εσωτερικό έργο προπώλησης μπορεί να μετατραπεί αργότερα σε ένα χρεώσιμο έργο εάν κερδηθεί η προσφορά.</span><span class="sxs-lookup"><span data-stu-id="49560-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="49560-110">Οποιοδήποτε έργο δεν συσχετίζεται με μια σύμβαση στο Dynamics 365 Project Operations αντιμετωπίζεται ως εσωτερικό.</span><span class="sxs-lookup"><span data-stu-id="49560-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="49560-111">Τα προφίλ κόστους έργου και εσόδων δεν χρησιμοποιούντα για να καθορίσουν τους κανόνες λογιστικής για το έργο.</span><span class="sxs-lookup"><span data-stu-id="49560-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="49560-112">Το κόστος εσωτερικού έργου καταχωρείται πάντα με τη χρήση των αρχών κέρδους και ζημίας.</span><span class="sxs-lookup"><span data-stu-id="49560-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="49560-113">Οι λογαριασμοί καθολικών για καταχωρήσεις καθορίζονται στη σελίδα **Ρύθμιση παραμέτρων καταχώρισης καθολικών**.</span><span class="sxs-lookup"><span data-stu-id="49560-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="49560-114">Οι συναλλαγές χρόνου καταχωρούνται με χρέωση του λογαριασμού **Κόστος** και πίστωση του λογαριασμού **Εκχώρηση μισθοδοσίας**.</span><span class="sxs-lookup"><span data-stu-id="49560-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="49560-115">Οι συναλλαγές εξόδων καταχωρούνται με χρέωση του λογαριασμού **Κόστος** και πίστωση του λογαριασμού **Λογαριασμός αντιστάθμισης για έξοδα**.</span><span class="sxs-lookup"><span data-stu-id="49560-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>
- <span data-ttu-id="49560-116">Οι συναλλαγές στοιχείων καταχωρούνται χρεώνοντας τον λογαριασμό **Κόστος** και πιστώνοντας τον λογαριασμό **Κόστος - Στοιχείο**.</span><span class="sxs-lookup"><span data-stu-id="49560-116">Item transactions are posted by debiting the **Cost** account and crediting the **Cost - Item** account.</span></span>

<span data-ttu-id="49560-117">Μετά την καταχώρηση των συναλλαγών στο έργο, εάν το έργο σχετίζεται με μια σύμβαση έργου, το σύστημα αντιστρέφει όλες τις συσσωρευμένες συναλλαγές και δημιουργεί νέες χρεώσιμες συναλλαγές.</span><span class="sxs-lookup"><span data-stu-id="49560-117">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="49560-118">Οι χρεώσιμες συναλλαγές ακολουθούν τους κανόνες λογιστικής που καθορίζονται στο αντίστοιχο προφίλ κόστους και εσόδων του έργου.</span><span class="sxs-lookup"><span data-stu-id="49560-118">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
