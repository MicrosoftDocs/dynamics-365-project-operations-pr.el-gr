---
title: Ενημέρωση χαρακτηριστικών προσθήκης με νέες διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ενημέρωσης των χαρακτηριστικών προσθηκών για τις διαστάσεις τιμολόγησης.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7999c003a0cf670d586ebf4445901e106fbee39f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274683"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="9cc7d-103">Ενημέρωση χαρακτηριστικών προσθήκης με νέες διαστάσεις τιμολόγησης</span><span class="sxs-lookup"><span data-stu-id="9cc7d-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="9cc7d-104">Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ενημέρωσης των χαρακτηριστικών προσθηκών για τις διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="9cc7d-105">Αυτό το θέμα ισχύει μόνο για τις δυνατότητες προσφοράς και σύμβασης στο Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cc7d-106">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="9cc7d-106">Prerequisites</span></span>
<span data-ttu-id="9cc7d-107">Πριν ολοκληρώσετε τα βήματα σε αυτό το θέμα, θα πρέπει να έχετε ολοκληρώσει τις διαδικασίες στα ακόλουθα θέματα:</span><span class="sxs-lookup"><span data-stu-id="9cc7d-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="9cc7d-108">Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων</span><span class="sxs-lookup"><span data-stu-id="9cc7d-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="9cc7d-109">Προσθήκη προσαρμοσμένων πεδίων σε ρύθμιση τιμών και οντότητες συναλλαγών </span><span class="sxs-lookup"><span data-stu-id="9cc7d-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="9cc7d-110">[Ρύθμιση προσαρμοσμένων πεδίων ως διαστάσεις τιμολόγησης ](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7d-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="9cc7d-111">Εάν δεν έχετε ολοκληρώσει αυτές τις διαδικασίες, ολοκληρώστε τις και, στη συνέχεια, επιστρέψτε σε αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="9cc7d-112">Δήλωση προσθήκης</span><span class="sxs-lookup"><span data-stu-id="9cc7d-112">Register a plug-in</span></span>
<span data-ttu-id="9cc7d-113">Όταν δημιουργείται μια λεπτομέρεια γραμμής προσφοράς στη σελίδα **Γραμμή προσφοράς** για μια γραμμή προσφοράς έργου, το σύστημα δημιουργεί δύο γραμμές εκτίμησης.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="9cc7d-114">Η μία γραμμή είναι για την πλευρά του κόστους της εκτίμησης και η άλλη γραμμή για τις πωλήσεις στο πλάι.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="9cc7d-115">Αυτό είναι το ίδιο και για τις γραμμές σύμβασης έργου.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="9cc7d-116">Όταν πραγματοποιείτε μια αλλαγή στην ποσότητα ή σε ένα πεδίο από την πλευρά του κόστους, αυτή η αλλαγή γίνετια επίσης στην πλευρά «Πωλήσεις».</span><span class="sxs-lookup"><span data-stu-id="9cc7d-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="9cc7d-117">Αυτό είναι δυνατό επειδή οι προσθήκες PreOperation στις οντότητες λεπτομερειών Quotelinedetail και contractline συνδέουν συγκεκριμένα χαρακτηριστικά στη σχέση κόστους με την πλευρά πωλήσεων της συναλλαγής.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="9cc7d-118">Εάν χρειάζεστε αλλαγές που πραγματοποιήθηκαν στις τιμές των διαστάσεων τιμολόγησης από την πλευρά των πωλήσεων, ώστε να γίνουν και από την πλευρά του κόστους, πρέπει να γίνει εκ νέου εγγραφή των ακόλουθων επεκτάσεων μετά από την πραγματοποίηση αλλαγών σε μια διάσταση τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="9cc7d-119">Αυτά είναι οι προσθήκες για ενημέρωση και εκ νέου καταχώρηση:</span><span class="sxs-lookup"><span data-stu-id="9cc7d-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="9cc7d-120">PreOperationContractLineDetailUpdate - **Ενημέρωση msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="9cc7d-121">PreOperationQuoteLineDetailUpdate - **Ενημερώσεις msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="9cc7d-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="9cc7d-122">Ολοκληρώστε τα παρακάτω βήματα για να ενημερώσετε και να καταχωρήσετε εκ νέου τις προσθήκες.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="9cc7d-123">Ανοίξτε το **PluginRegistrationTool** και συνδεθείτε στο περιβάλλον Project Operations του Dataverse.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="9cc7d-124">Επιλέξτε **Αναζήτηση** και πληκτρολογήστε τα πρώτα γράμματα της προσθήκης που θα ενημερωθεί.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="9cc7d-125">Μετά την εύρεση της προσθήκης, επιλέξτε την και, στη συνέχεια, επιλέξτε **Επιλογή στην κύρια φόρμα**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="9cc7d-126">Επιλέξτε το βήμα **Ενημέρωση msdyn_orderlinetransaction**, κάντε δεξί κλικ κι, έπειτα, επιλέξτε **Ενημέρωση**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="9cc7d-127">Στο σελίδα του παραθύρου διαλόγου **Ενημέρωση**, επιλέξτε τα αποσιωπητικά (**...**) στα χαρακτηριστικά φιλτραρίσματος.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="9cc7d-128">Ανοίγει το παράθυρο φιλτραρίσματος χαρακτηριστικών και παρέχεται μια λίστα με όλα τα χαρακτηριστικά της οντότητας και τις διαστάσεις τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="9cc7d-129">Επιλέξτε τα πλαίσια ελέγχου για τα χαρακτηριστικά διάστασης τιμολόγησης.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="9cc7d-130">Επιλέξτε **ΟΚ** για να κλείσετε τη σελίδα και επιλέξτε **Βήμα ενημέρωσης**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="9cc7d-131">Επαναλάβετε τα βήματα 2-7 για τη δεύτερη προσθήκη **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="9cc7d-132">Για αυτήν την προσθήκη, χρειάζεται να ενημερώσετε το βήμα **Ενημέρωση msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="9cc7d-133">Κλείστε το **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="9cc7d-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]