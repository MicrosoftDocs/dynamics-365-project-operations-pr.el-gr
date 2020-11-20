---
title: Διαχείριση συμβάσεων έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την προβολή συμβάσεων βάσει έργου.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441fbc378a423334f45bc65658811ef238515393
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177331"
---
# <a name="manage-project-contracts"></a><span data-ttu-id="f7f15-103">Διαχείριση συμβάσεων έργου</span><span class="sxs-lookup"><span data-stu-id="f7f15-103">Manage project contracts</span></span>

<span data-ttu-id="f7f15-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="f7f15-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f7f15-105">Οι συμβάσεις έργου στο Dynamics 365 Project Operations καταγράφουν και διαχειρίζονται τις συμβατικά συμφωνημένες δεσμεύσεις και τις λεπτομέρειες χρέωσης ενός έργου.</span><span class="sxs-lookup"><span data-stu-id="f7f15-105">Project contracts in Dynamics 365 Project Operations capture and manage the contractually agreed on commitments and billing details of a project.</span></span> <span data-ttu-id="f7f15-106">Η δομή μιας σύμβασης έργου στο Project Operations έχει σχεδιαστεί ανάλογα με την εργασία βάσει έργου και περιλαμβάνει τα ακόλουθα στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="f7f15-106">The structure of a project contract in Project Operations is tailored to project-based work with the following components:</span></span>

- <span data-ttu-id="f7f15-107">Γραμμές σύμβασης που προσδιορίζουν τα διακριτά στοιχεία του έργου που θα παρουσιαστούν ως στοιχεία υψηλού επιπέδου σε ένα τιμολόγιο έργου.</span><span class="sxs-lookup"><span data-stu-id="f7f15-107">Contract lines that identify the discrete components of work that will be presented as high-level components on a project invoice.</span></span>
- <span data-ttu-id="f7f15-108">Λεπτομέρειες της γραμμής σύμβασης που προσδιορίζουν και εκτιμούν την εργασία για κάθε στοιχείο ή γραμμή σύμβασης υψηλού επιπέδου.</span><span class="sxs-lookup"><span data-stu-id="f7f15-108">Contract line details that identify and estimate the work for each high-level component or contract line.</span></span> <span data-ttu-id="f7f15-109">Η εκτίμηση περιλαμβάνει το χρονοδιάγραμμα και τις οικονομικές πτυχές για την εργασία που συνδέεται με τη γραμμή σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="f7f15-109">The estimate includes the schedule and the financial aspects for the work tied to the contract line.</span></span>
- <span data-ttu-id="f7f15-110">Τα συμβατικά μοντέλα και τα φορολογήσιμα στοιχεία καθορίζονται για κάθε γραμμή σύμβασης που περιέχει τη συμφωνία χρέωσης για κάθε γραμμή σύμβασης και τη συνολική σύμβαση.</span><span class="sxs-lookup"><span data-stu-id="f7f15-110">Contracting models and chargeable components are set up for each contract line that holds the billing arrangement for each contract line and the overall contract.</span></span>

## <a name="view-all-project-based-contracts"></a><span data-ttu-id="f7f15-111">Προβολή όλων των συμβάσεων βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="f7f15-111">View all project-based contracts</span></span>

<span data-ttu-id="f7f15-112">Μπορείτε να δείτε μια λίστα όλων των συμβάσεων έργου στη σελίδα λίστας **Συμβάσεις**.</span><span class="sxs-lookup"><span data-stu-id="f7f15-112">A list of all project contracts can be seen on the **Contracts** list page.</span></span> 

1. <span data-ttu-id="f7f15-113">Μεταβείτε στις **Πωλήσεις** > **Συμβάσεις**.</span><span class="sxs-lookup"><span data-stu-id="f7f15-113">Go to **Sales** > **Contracts**.</span></span> <span data-ttu-id="f7f15-114">Εμφανίζεται μια λίστα με όλες τις συμβάσεις έργου που έχετε στο σύστημα.</span><span class="sxs-lookup"><span data-stu-id="f7f15-114">A list of all your project Contracts in the system are shown.</span></span> 
2. <span data-ttu-id="f7f15-115">Επιλέξτε την **Εναλλαγή προβολής** (το αναπτυσσόμενο βέλος δίπλα στο όνομα της προβολής) για να επιλέξετε άλλες φιλτραρισμένες προβολές.</span><span class="sxs-lookup"><span data-stu-id="f7f15-115">Select the **View switcher** (the drop-down arrow next to the name of the view) to select other filtered views.</span></span> <span data-ttu-id="f7f15-116">Μπορείτε να δημιουργήσετε τις δικές σας προβολές με προσαρμοσμένα κριτήρια φιλτραρίσματος.</span><span class="sxs-lookup"><span data-stu-id="f7f15-116">You can create your own views with custom filter criteria.</span></span>

<span data-ttu-id="f7f15-117">Οι συμβάσεις μπορούν να δημιουργηθούν ή να διαγραφούν από αυτήν τη σελίδα λίστας ή τις σελίδες λεπτομερειών.</span><span class="sxs-lookup"><span data-stu-id="f7f15-117">Contracts can be created or deleted from this list page or detail pages.</span></span>
