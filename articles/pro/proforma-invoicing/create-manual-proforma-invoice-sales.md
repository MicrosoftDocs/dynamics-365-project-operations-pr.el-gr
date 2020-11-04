---
title: Δημιουργία μη αυτόματου προτιμολογίου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία ενός μη αυτόματου προτιμολογίου στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/20/2020
ms.locfileid: "4077145"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="01b83-103">Δημιουργία μη αυτόματου προτιμολογίου</span><span class="sxs-lookup"><span data-stu-id="01b83-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="01b83-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="01b83-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="01b83-105">Στο Dynamics 365 Project Operations, τα προτιμολόγια μπορούν να δημιουργηθούν με μη αυτόματο τρόπο, ανάλογα με τις ανάγκες.</span><span class="sxs-lookup"><span data-stu-id="01b83-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="01b83-106">Μπορείτε να δημιουργήσετε με μη αυτόματο τρόπο ένα προτιμολόγιο από τη σελίδα λίστας **Συμβάσεις έργου** ή από τη σελίδα λεπτομερειών **Σύμβαση έργου**.</span><span class="sxs-lookup"><span data-stu-id="01b83-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="01b83-107">Σελίδα λίστας συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="01b83-107">Project Contracts list page</span></span>

<span data-ttu-id="01b83-108">Από τη σελίδα λίστας **Συμβάσεις έργου** , επιλέξτε μία ή περισσότερες συμβάσεις έργου και δημιουργήστε τιμολόγια για όλες τις επιλεγμένες καρτέλες.</span><span class="sxs-lookup"><span data-stu-id="01b83-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="01b83-109">Το σύστημα ελέγχει για να διαπιστώσει ποια από τις επιλεγμένες συμβάσεις έργου έχει τη λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="01b83-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="01b83-110">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="01b83-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="01b83-111">Εάν μια σύμβαση έργου έχει πολλαπλούς πελάτες, μπορεί να έχει δημιουργηθεί ένα τιμολόγιο ανά πελάτη και πολλαπλά τιμολόγια ανά σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="01b83-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="01b83-112">Όλα τα τιμολόγια του έργου που δημιουργήθηκαν είναι διαθέσιμα στη σελίδα **Τιμολόγιο** στην ενότητα **Χρέωση** της περιοχής **Πωλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="01b83-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="01b83-113">Σελίδα λεπτομερειών σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="01b83-113">Project Contract details page</span></span>

<span data-ttu-id="01b83-114">Μπορείτε, επίσης, να δημιουργήσετε ένα προτιμολόγιο από τη σελίδα λεπτομερειών **Σύμβαση έργου** το οποίο δημιουργεί το τιμολόγιο για τη συγκεκριμένη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="01b83-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="01b83-115">Το σύστημα επβεβαιώνει ότι η σύμβαση έργου έχει μια λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="01b83-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="01b83-116">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια με βάση τον αριθμό των πελατών σε κάθε γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="01b83-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="01b83-117">Όταν δημιουργείται ένα μεμονωμένο προτιμολόγιο, ανοίγει η σελίδα **Τιμολόγιο**.</span><span class="sxs-lookup"><span data-stu-id="01b83-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="01b83-118">Εάν υπάρχουν πολλά τιμολόγια που έχουν δημιουργηθεί για τη συγκεκριμένη σύμβαση έργου, τότε η σελίδα λίστας **Τιμολόγια** ανοίγει για να εμφανιστούν όλα τα τιμολόγια που δημιουργήθηκαν.</span><span class="sxs-lookup"><span data-stu-id="01b83-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
