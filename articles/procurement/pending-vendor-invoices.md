---
title: Αγορά υλικών μη διαθέσιμων σε απόθεμα χρησιμοποιώντας εκκρεμές τιμολόγιο προμηθευτή
description: Αυτό θέμα εξηγεί τον τρόπο καταγραφής των εκκρεμών τιμολογίων προμηθευτή.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993793"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="99ff5-103">Αγορά υλικών μη διαθέσιμων σε απόθεμα χρησιμοποιώντας εκκρεμές τιμολόγιο προμηθευτή</span><span class="sxs-lookup"><span data-stu-id="99ff5-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="99ff5-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="99ff5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="99ff5-105">Καθώς μια εταιρεία προμηθεύεται μη διαθέσιμα σε απόθεμα υλικά για ένα έργο, το κόστος μπορεί να καταγραφεί αμέσως έναντι του έργου.</span><span class="sxs-lookup"><span data-stu-id="99ff5-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="99ff5-106">Για παράδειγμα, η Contoso Robotics US πραγματοποιεί έργο ανανέωσης εξοπλισμού και χρειάζεται άδειες χρήσης λογισμικού.</span><span class="sxs-lookup"><span data-stu-id="99ff5-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="99ff5-107">Αυτές οι άδειες χρήσης προμηθεύονται από έναν τρίτο προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="99ff5-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="99ff5-108">Χρησιμοποιώντας το Dynamics 365 Finance, ο υπάλληλος πληρωτέων λογαριασμών καταγραφει ένα έγγραφο τιμολογίου εκκρεμούς προμηθευτή και εκχωρεί τις δαπάνες άδειας χρήσης απευθείας στο έργο ανανέωσης εξοπλισμού.</span><span class="sxs-lookup"><span data-stu-id="99ff5-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="99ff5-109">Προτού χρησιμοποιήσετε τη λειτουργικότητα που περιγράφεται σε αυτό το θέμα, εξετάστε και εφαρμόστε τις απαιτούμενες ρυθμίσεις παραμέτρων.</span><span class="sxs-lookup"><span data-stu-id="99ff5-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="99ff5-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση υλικών που δεν είναι σε απόθεμα και εκκρεμών τιμολογίων προμηθευτή](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="99ff5-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="99ff5-111">Καταχώρηση ενός εκκρεμούς τιμολογίου προμηθευτή που σχετίζεται με ένα έργο</span><span class="sxs-lookup"><span data-stu-id="99ff5-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="99ff5-112">Τα εκκρεμή τιμολόγια προμηθευτών μπορούν να καταγράφονται στη σελίδα **Εκκρεμή τιμολόγια προμηθευτών** (**Πληρωτέοι λογαριασμοί** >  **Τιμολόγια** > **Εκκρεμή τιμολόγια προμηθευτή**).</span><span class="sxs-lookup"><span data-stu-id="99ff5-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="99ff5-113">Ολοκληρώστε τα παρακάτω βήματα για να καταχωρήσετε ένα εκκρεμές τιμολόγιο πωλητή που σχετίζεται με ένα έργο:</span><span class="sxs-lookup"><span data-stu-id="99ff5-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="99ff5-114">Μεταβείτε στην επιλογή **πληρωτέοι λογαριασμοί** > **τιμολόγια** και επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="99ff5-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="99ff5-115">Στο πεδίο **Λογαριασμός τιμολογίου**, επιλέξτε έναν προμηθευτή και στο πεδίο **Αριθμός**, εισαγάγετε το αναγνωριστικό τιμολογίου προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="99ff5-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="99ff5-116">Προσθέστε μια γραμμή στο τιμολόγιο του προμηθευτή και στο πεδίο **Αριθμός στοιχείου**, επιλέξτε το μη διαθέσιμο σε απόθεμα στοιχείο που έχει αγοραστεί από τον προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="99ff5-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="99ff5-117">Οι γραμμές τιμολογίου προμηθευτή που βασίζονται σε κατηγορία προμήθειας δεν είναι δυνατό να καταχωρημένες για το έργο.</span><span class="sxs-lookup"><span data-stu-id="99ff5-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="99ff5-118">Προσθέστε την ποσότητα που αγοράστηκε.</span><span class="sxs-lookup"><span data-stu-id="99ff5-118">Add the quantity purchased.</span></span> <span data-ttu-id="99ff5-119">Το σύστημα θα συμπληρώνει την τιμή μονάδας με βάση τη διαμόρφωση της τιμής του μη διαθέσιμου σε απόθεμα στοιχείου.</span><span class="sxs-lookup"><span data-stu-id="99ff5-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="99ff5-120">Επαληθεύστε το συνολικό ποσό και άλλες απαιτούμενες λεπτομέρειες στη γραμμή.</span><span class="sxs-lookup"><span data-stu-id="99ff5-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="99ff5-121">Στις λεπτομέρειες γραμμής, στην καρτέλα **Έργο**, επιλέξτε το αναγνωριστικό του έργου στο οποίο θα καταγραφεί αυτό το στοιχείο.</span><span class="sxs-lookup"><span data-stu-id="99ff5-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="99ff5-122">Προαιρετικά, επιλέξτε τον αριθμό δραστηριότητας και ενημερώστε την ιδιότητα κατηγορίας έργου και γραμμής.</span><span class="sxs-lookup"><span data-stu-id="99ff5-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="99ff5-123">Καταχωρήστε το εκκρεμές τιμολόγιο προμηθευτή.</span><span class="sxs-lookup"><span data-stu-id="99ff5-123">Post pending vendor invoice.</span></span> <span data-ttu-id="99ff5-124">Όταν καταχωρείται το τιμολόγιο, το σύστημα καταγράφει:</span><span class="sxs-lookup"><span data-stu-id="99ff5-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="99ff5-125">Το υπόλοιπο ποσό του προμηθευτήυπόλοιπο.</span><span class="sxs-lookup"><span data-stu-id="99ff5-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="99ff5-126">Το ποσό φόρου πωλήσεων.</span><span class="sxs-lookup"><span data-stu-id="99ff5-126">The sales tax amount.</span></span>
    - <span data-ttu-id="99ff5-127">Το κόστος για το έργο καταγράφεται στο λογαριασμό ενοποίησης της προμήθειας.</span><span class="sxs-lookup"><span data-stu-id="99ff5-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="99ff5-128">Η πραγματική συναλλαγή έργου στο Dataverse.</span><span class="sxs-lookup"><span data-stu-id="99ff5-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="99ff5-129">Η επεξεργασία αυτής της συναλλαγής πραγματοποιείται περαιτέρω με χρήση του [Ημερολογίου ενοποίησης Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="99ff5-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="99ff5-130">Η καταχώρηση αυτού του ημερολογίου μετακινεί το ποσό από το λογαριασμό ενοποίησης προμήθειας στο λογαριασμό κόστους έργου.</span><span class="sxs-lookup"><span data-stu-id="99ff5-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
