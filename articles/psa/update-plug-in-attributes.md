---
title: Ενημέρωση χαρακτηριστικών προσθήκης για συμπερίληψη νέων διαστάσεων τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την ενημέρωση των χαρακτηριστικών προσθηκών για τις διαστάσεις τιμολόγησης.
author: Rumant
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: b0d50733340f277453f4ef5b52bdd3ee089449cd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012811"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="4efcd-103">Ενημέρωση χαρακτηριστικών προσθήκης για συμπερίληψη νέων διαστάσεων τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="4efcd-103">Update plug-in attributes to include new pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> <span data-ttu-id="4efcd-104">Εάν δεν χρησιμοποιείτε τις δυνατότητες δημιουργίας προσφοράς και συμβάσεων του Project Service Automation (PSA), μπορείτε να παραλείψετε αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="4efcd-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="4efcd-105">Αυτό το θέμα υποθέτει ότι έχετε ολοκληρώσει τις διαδικασίες στα θέματα [Δημιουργήστε προσαρμοσμένα πεδία και οντότητες](create-custom-fields-entities.md), [Προσθέτετε προσαρμοσμένα πεδία σε οντότητες ρύθμισης παραμέτρων τιμών και οντότητες συναλλαγής](field-references.md) και [Ρύθμιση παραμέτρων προσαρμοσμένων πεδίων ως διαστάσεις τιμολόγησης](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="4efcd-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="4efcd-106">Εάν δεν έχετε ολοκληρώσει αυτές τις διαδικασίες, επιστρέψτε και ολοκληρώστε τις και, στη συνέχεια, επιστρέψτε σε αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="4efcd-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="4efcd-107">Όταν δημιουργείται μια λεπτομέρεια γραμμής προσφοράς στη σελίδα **Γραμμή προσφοράς** για μια γραμμή προσφοράς έργου, το σύστημα δημιουργεί δύο γραμμές εκτίμησης στο παρασκήνιο -- μία γραμμή για την πλευρά του κόστους της εκτίμησης και μία για την πλευρά των πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="4efcd-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="4efcd-108">Αυτό είναι το ίδιο και για τις γραμμές σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="4efcd-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="4efcd-109">Όταν πραγματοποιείτε μια αλλαγή στην ποσότητα ή σε ένα πεδίο από την πλευρά του κόστους, αυτή η αλλαγή μεταβιβάζεται στην πλευρά "Πωλήσεις".</span><span class="sxs-lookup"><span data-stu-id="4efcd-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="4efcd-110">Αυτό είναι δυνατό λόγω των ακόλουθων προσθηκών που πρέπει να καταχωρηθούν μετά από μια αλλαγή στις διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="4efcd-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="4efcd-111">PreOperationContractLineDetailUpdate - Ενημερώσεις **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="4efcd-112">PreOperationQuoteLineDetailUpdate - Ενημερώσεις **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="4efcd-113">Τα παρακάτω βήματα σας εξηγούν τη διεργασία καταχώρησης των προσθηκών.</span><span class="sxs-lookup"><span data-stu-id="4efcd-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="4efcd-114">Ανοίξτε το **PluginRegistrationTool** και συνδέστε το με την online παρουσία σας.</span><span class="sxs-lookup"><span data-stu-id="4efcd-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="4efcd-115">Κάντε κλικ στην **Αναζήτηση** και αναζητήστε την προσθήκη για να ενημερωθείτε.</span><span class="sxs-lookup"><span data-stu-id="4efcd-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![Στιγμιότυπο οθόνης του δέντρου αναζήτησης](media/PRT-1.png)

3. <span data-ttu-id="4efcd-117">Μετά την εύρεση της προσθήκης, επιλέξτε την και, στη συνέχεια, πατήστε **Επιλογή στην κύρια φόρμα**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="4efcd-118">Επιλέξτε το βήμα της προσθήκης που θα ενημερωθεί, κάντε δεξί κλικ και, στη συνέχεια, επιλέξτε **Ενημέρωση**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![Στιγμιότυπο οθόνης της προσθήκης για ενημέρωση](media/PRT-2.png)
 
5. <span data-ttu-id="4efcd-120">Στο παράθυρο ενημέρωσης επιλέξτε τα αποσιωπητικά (**...**) στα χαρακτηριστικά φιλτραρίσματος.</span><span class="sxs-lookup"><span data-stu-id="4efcd-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![Στιγμιότυπο οθόνης των πληροφοριών υπάρχουσας ρύθμισης βημάτων ενημέρωσης](media/PRT-3.png)
 
6. <span data-ttu-id="4efcd-122">Επιλέξτε τα πλαίσια ελέγχου χαρακτηριστικών τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="4efcd-122">Select the pricing attribute check boxes.</span></span>

 ![Στιγμιότυπο οθόνης που εμφανίζει την επιλογή πλαισίου ελέγχου για χαρακτηριστικά τιμολόγησης](media/PRT-4.png)

7. <span data-ttu-id="4efcd-124">Κάντε κλικ στο **ΟΚ** για να κλείσετε τη σελίδα και επιλέξτε **Βήμα ενημέρωσης**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![Στιγμιότυπο οθόνης που δείχνει το κουμπί "Βήμα ενημέρωσης"](media/PRT-5.png)
 
8. <span data-ttu-id="4efcd-126">Επαναλάβετε αυτήν τη διεργασία για τη δεύτερη προσθήκη, **PreOperationQuoteLineDetail-Update of msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="4efcd-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="4efcd-127">Κλείστε το εργαλείο καταχώρισης προσθήκης.</span><span class="sxs-lookup"><span data-stu-id="4efcd-127">Close the plug-in registration tool.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]