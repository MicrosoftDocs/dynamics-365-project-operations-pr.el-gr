---
title: Δημιουργία μη αυτόματου προτιμολογίου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία ενός μη αυτόματου προτιμολογίου στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 87ef090454b2a7ab997e7c21d8d10badc31c8235
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176386"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="e31ab-103">Δημιουργία μη αυτόματου προτιμολογίου - lite</span><span class="sxs-lookup"><span data-stu-id="e31ab-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="e31ab-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="e31ab-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e31ab-105">Στο Dynamics 365 Project Operations, τα προτιμολόγια μπορούν να δημιουργηθούν με μη αυτόματο τρόπο, ανάλογα με τις ανάγκες.</span><span class="sxs-lookup"><span data-stu-id="e31ab-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="e31ab-106">Μπορείτε να δημιουργήσετε με μη αυτόματο τρόπο ένα προτιμολόγιο από τη σελίδα λίστας **Συμβάσεις έργου** ή από τη σελίδα λεπτομερειών **Σύμβαση έργου**.</span><span class="sxs-lookup"><span data-stu-id="e31ab-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="e31ab-107">Σελίδα λίστας συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="e31ab-107">Project Contracts list page</span></span>

<span data-ttu-id="e31ab-108">Από τη σελίδα λίστας **Συμβάσεις έργου**, επιλέξτε μία ή περισσότερες συμβάσεις έργου και δημιουργήστε τιμολόγια για όλες τις επιλεγμένες καρτέλες.</span><span class="sxs-lookup"><span data-stu-id="e31ab-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="e31ab-109">Το σύστημα ελέγχει για να διαπιστώσει ποια από τις επιλεγμένες συμβάσεις έργου έχει τη λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="e31ab-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="e31ab-110">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="e31ab-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="e31ab-111">Εάν μια σύμβαση έργου έχει πολλαπλούς πελάτες, μπορεί να έχει δημιουργηθεί ένα τιμολόγιο ανά πελάτη και πολλαπλά τιμολόγια ανά σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e31ab-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="e31ab-112">Όλα τα τιμολόγια του έργου που δημιουργήθηκαν είναι διαθέσιμα στη σελίδα **Τιμολόγιο** στην ενότητα **Χρέωση** της περιοχής **Πωλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="e31ab-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="e31ab-113">Σελίδα λεπτομερειών σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="e31ab-113">Project Contract details page</span></span>

<span data-ttu-id="e31ab-114">Μπορείτε, επίσης, να δημιουργήσετε ένα προτιμολόγιο από τη σελίδα λεπτομερειών **Σύμβαση έργου** το οποίο δημιουργεί το τιμολόγιο για τη συγκεκριμένη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="e31ab-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="e31ab-115">Το σύστημα επβεβαιώνει ότι η σύμβαση έργου έχει μια λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="e31ab-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="e31ab-116">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια με βάση τον αριθμό των πελατών σε κάθε γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="e31ab-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="e31ab-117">Όταν δημιουργείται ένα μεμονωμένο προτιμολόγιο, ανοίγει η σελίδα **Τιμολόγιο**.</span><span class="sxs-lookup"><span data-stu-id="e31ab-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="e31ab-118">Εάν υπάρχουν πολλά τιμολόγια που έχουν δημιουργηθεί για τη συγκεκριμένη σύμβαση έργου, τότε η σελίδα λίστας **Τιμολόγια** ανοίγει για να εμφανιστούν όλα τα τιμολόγια που δημιουργήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="e31ab-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
