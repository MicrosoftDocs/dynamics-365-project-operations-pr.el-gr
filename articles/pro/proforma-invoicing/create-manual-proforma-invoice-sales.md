---
title: Δημιουργία μη αυτόματου προτιμολογίου - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία ενός μη αυτόματου προτιμολογίου στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 104c2f3f7f0ca0682158d0f7fa0f50a4967e6dd0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274188"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="686ec-103">Δημιουργία μη αυτόματου προτιμολογίου - lite</span><span class="sxs-lookup"><span data-stu-id="686ec-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="686ec-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="686ec-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="686ec-105">Στα Dynamics 365 Project Operations, τα προτιμολόγια μπορούν να δημιουργηθούν με μη αυτόματο τρόπο, όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="686ec-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="686ec-106">Μπορείτε να δημιουργήσετε με μη αυτόματο τρόπο ένα προτιμολόγιο από τη σελίδα λίστας **Συμβάσεις έργου** ή από τη σελίδα λεπτομερειών **Σύμβαση έργου**.</span><span class="sxs-lookup"><span data-stu-id="686ec-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="686ec-107">Σελίδα λίστας συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="686ec-107">Project Contracts list page</span></span>

<span data-ttu-id="686ec-108">Από τη σελίδα λίστας **Συμβάσεις έργου**, επιλέξτε μία ή περισσότερες συμβάσεις έργου και δημιουργήστε τιμολόγια για όλες τις επιλεγμένες καρτέλες.</span><span class="sxs-lookup"><span data-stu-id="686ec-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="686ec-109">Το σύστημα ελέγχει για να διαπιστώσει ποια από τις επιλεγμένες συμβάσεις έργου έχει τη λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="686ec-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="686ec-110">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="686ec-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="686ec-111">Εάν μια σύμβαση έργου έχει πολλαπλούς πελάτες, μπορεί να έχει δημιουργηθεί ένα τιμολόγιο ανά πελάτη και πολλαπλά τιμολόγια ανά σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="686ec-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="686ec-112">Όλα τα τιμολόγια του έργου που δημιουργήθηκαν είναι διαθέσιμα στη σελίδα **Τιμολόγιο** στην ενότητα **Χρέωση** της περιοχής **Πωλήσεις**.</span><span class="sxs-lookup"><span data-stu-id="686ec-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="686ec-113">Σελίδα λεπτομερειών σύμβασης έργου</span><span class="sxs-lookup"><span data-stu-id="686ec-113">Project Contract details page</span></span>

<span data-ttu-id="686ec-114">Ένα προτιμολόγιο μπορεί επίσης να δημιουργηθεί από τη σελίδα λεπτομερειών **Σύμβαση έργου**.</span><span class="sxs-lookup"><span data-stu-id="686ec-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="686ec-115">Το σύστημα επαληθεύει ότι η σύμβαση έργου έχει μια λίστα εκκρεμοτήτων **Έτοιμο για τιμολόγηση** με ημερομηνία πριν από τη σημερινή ημερομηνία.</span><span class="sxs-lookup"><span data-stu-id="686ec-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="686ec-116">Από αυτές τις συμβάσεις, το σύστημα δημιουργεί προσχέδια προτιμολόγια με βάση τον αριθμό των πελατών σε κάθε γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="686ec-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="686ec-117">Όταν δημιουργείται ένα μεμονωμένο προτιμολόγιο, ανοίγει η σελίδα **Τιμολόγιο**.</span><span class="sxs-lookup"><span data-stu-id="686ec-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="686ec-118">Εάν δημιουργηθούν πολλά τιμολόγια για τη σύμβαση έργου, ανοίγει η σελίδα λίστας **Τιμολόγια** για να εμφανιστούν όλα τα τιμολόγια που έχουν δημιουργηθεί.</span><span class="sxs-lookup"><span data-stu-id="686ec-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]