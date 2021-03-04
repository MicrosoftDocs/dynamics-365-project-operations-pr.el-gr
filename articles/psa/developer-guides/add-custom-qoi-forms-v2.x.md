---
title: Προσθήκη νέων φορμών προσαρμοσμένης οντότητας (Project Service Automation 2.x)
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο προσθήκης φορμών προσαρμοσμένων οντοτήτων για τις ευκαιρίες, τις προσφορές, τις παραγγελίες ή τα τιμολόγια στο Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 31986efed81892cc5722cb8f5e292cde14d8843d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144593"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="c8d08-103">Προσθήκη νέων φορμών προσαρμοσμένης οντότητας (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="c8d08-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="c8d08-104">Τύπος πεδίου</span><span class="sxs-lookup"><span data-stu-id="c8d08-104">Type field</span></span> 

<span data-ttu-id="c8d08-105">Το Dynamics 365 Project Service Automation βασίζεται στο πεδίο **Τύπος** (**msdyn\_ordertype**) στις οντότητες Ευκαιρία, Προσφορά, Παραγγελία και Τιμολόγιο για να διακρίνει αυτές τις εκδόσεις **βάσει εργασίας** αυτών των οντοτήτων από τις εκδόσεις **βάσει στοιχείου** και **βάσει υπηρεσίας**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="c8d08-106">Οι εκδόσεις που βασίζονται σε εργασία αυτών των οντοτήτων διεκπεραιώνονται από το PSA.</span><span class="sxs-lookup"><span data-stu-id="c8d08-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="c8d08-107">Η πολλή επιχειρηματική λογική από την πλευρά του προγράμματος-πελάτη και από την πλευρά του διακομιστή της λύσης εξαρτάται από το πεδίο **Τύπος**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="c8d08-108">Για αυτόν το λόγο, είναι σημαντικό να προετοιμαστεί το πεδίο με σωστή τιμή κατά τη δημιουργία των οντοτήτων.</span><span class="sxs-lookup"><span data-stu-id="c8d08-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="c8d08-109">Μια εσφαλμένη τιμή μπορεί να προκαλέσει εσφαλμένες συμπεριφορές και κάποια επιχειρηματική λογική ενδέχεται να μην εκτελεστεί σωστά.</span><span class="sxs-lookup"><span data-stu-id="c8d08-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="c8d08-110">Αυτόματη εναλλαγή φορμών</span><span class="sxs-lookup"><span data-stu-id="c8d08-110">Automatic form switching</span></span>

<span data-ttu-id="c8d08-111">Για να αποφύγετε την καταστροφή πιθανών δεδομένων και τις μη αναμενόμενες συμπεριφορές που προκαλούνται από εσφαλμένη προετοιμασία και επεξεργασία των καρτελών της οντότητας πωλήσεων, το PSA πλέον περιλαμβάνει λογική για την αυτόματη εναλλαγή φορμών στις έτοιμες φόρμες.</span><span class="sxs-lookup"><span data-stu-id="c8d08-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="c8d08-112">Αυτή η λογική πηγαίνει τους χρήστες στη σωστή φόρμα για εργασία με την έκδοση με βάση την εργασία ή με οποιονδήποτε άλλο τύπο οντότητας ευκαιρίας, προσφοράς, παραγγελίας ή τιμολογίου.</span><span class="sxs-lookup"><span data-stu-id="c8d08-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="c8d08-113">Όταν ένας χρήστης ανοίγει την έκδοση με βάση την εργασία μιας οντότητας ευκαιρίας, προσφοράς, παραγγελίας ή τιμολογίου, η φόρμα αλλάζει σε **Πληροφορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="c8d08-114">Η λογική αυτόματης εναλλαγής φορμών βασίζεται στην αντιστοίχιση μεταξύ της τιμής **formId** και του πεδίου **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="c8d08-115">Όλες οι έτοιμες φόρμες έχουν προστεθεί σε αυτήν την αντιστοίχιση.</span><span class="sxs-lookup"><span data-stu-id="c8d08-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="c8d08-116">Ωστόσο, οι προσαρμοσμένες φόρμες θα πρέπει να προστεθούν με μη αυτόματο τρόπο, για να υποδείξουν την έκδοση της οντότητας που πρόκειται να διαχειριστούν.</span><span class="sxs-lookup"><span data-stu-id="c8d08-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="c8d08-117">Αυτό βασίζεται στο πεδίο **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="c8d08-118">Εάν η εναλλαγή φορμών λείπει από την αντιστοίχιση, η λογική θα μεταπηδήσει στην έτοιμη φόρμα με βάση την τιμή που αποθηκεύεται στο πεδίο **msdyn\_ordertype** της οντότητας.</span><span class="sxs-lookup"><span data-stu-id="c8d08-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="c8d08-119">Προσθήκη προσαρμοσμένων φορμών και ενεργοποίηση της λογικής εναλλαγής φορμών</span><span class="sxs-lookup"><span data-stu-id="c8d08-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="c8d08-120">Το παρακάτω παράδειγμα δείχνει τον τρόπο προσθήκης μιας προσαρμοσμένης φόρμας, **Τα στοιχεία έργου μου** έτσι ώστε να λειτουργεί με ευκαιρίες βασισμένες στην εργασία.</span><span class="sxs-lookup"><span data-stu-id="c8d08-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="c8d08-121">Η ίδια διεργασία χρησιμοποιείται για την προσθήκη προσαρμοσμένων φορμών, έτσι ώστε να λειτουργούν με προσφορές, παραγγελίες και τιμολόγια.</span><span class="sxs-lookup"><span data-stu-id="c8d08-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="c8d08-122">Ακολουθήστε τα παρακάτω βήματα για να δημιουργήσετε μια προσαρμοσμένη έκδοση της φόρμας **Πληροφορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="c8d08-123">Στην οντότητα ευκαιρίας, ανοίξτε τη φόρμα **Πληροφορίες έργου** και αποθηκεύστε ένα αντίγραφο με το όνομα **Οι πληροφορίες έργου μου**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="c8d08-124">Ανοίξτε τη νέα φόρμα και, στη συνέχεια, στις ιδιότητες, βεβαιωθείτε ότι υπάρχουν οι δέσμες ενεργειών προετοιμασίας φορμών από τη φόρμα **Πληροφορίες έργου**.</span><span class="sxs-lookup"><span data-stu-id="c8d08-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="c8d08-125">Μην καταργήσετε τις δέσμες ενεργειών.</span><span class="sxs-lookup"><span data-stu-id="c8d08-125">Don't remove the scripts.</span></span> <span data-ttu-id="c8d08-126">Διαφορετικά, ορισμένα δεδομένα ενδεχομένως να μην αρχικοποιηθούν σωστά.</span><span class="sxs-lookup"><span data-stu-id="c8d08-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="c8d08-127">Βεβαιωθείτε ότι το πεδίο **Τύπος** (**msdyn\_ordertype**) υπάρχει στη φόρμα.</span><span class="sxs-lookup"><span data-stu-id="c8d08-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="c8d08-128">Μην καταργήσετε αυτό το πεδίο.</span><span class="sxs-lookup"><span data-stu-id="c8d08-128">Don't remove this field.</span></span> <span data-ttu-id="c8d08-129">Διαφορετικά, οι δέσμες ενεργειών προετοιμασίας θα αποτύχουν.</span><span class="sxs-lookup"><span data-stu-id="c8d08-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="c8d08-130">Βρείτε την τιμή **formId** της νέας φόρμας.</span><span class="sxs-lookup"><span data-stu-id="c8d08-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="c8d08-131">Μπορείτε να τη συμπληρώσετε με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="c8d08-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="c8d08-132">Κάντε εξαγωγή της φόρμας **Τα στοιχεία έργου μου** ως μέρος μιας μη διαχειριζόμενης λύσης και μετά αναζητήστε την τιμή **formId** στο αρχείο customization.xml της λύσης που έχει εξαχθεί.</span><span class="sxs-lookup"><span data-stu-id="c8d08-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="c8d08-133">Ανοίξτε τη φόρμα **Τα στοιχεία έργου μου** στο πρόγραμμα επεξεργασίας φορμών και, στη συνέχεια, αναζητήστε το καθολικά μοναδικό αναγνωριστικό (GUID) δίπλα στην παράμετρο **fromId** στην URL όπως φαίνεται στην παρακάτω απεικόνιση.</span><span class="sxs-lookup"><span data-stu-id="c8d08-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![Η τιμή formId της νέας φόρμας στο URL](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="c8d08-135">Δημιουργήστε μια αντιστοίχιση **msdyn\_ordertype** για την τιμή **formId** κάνοντας επεξεργασία του πόρου web msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js.</span><span class="sxs-lookup"><span data-stu-id="c8d08-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="c8d08-136">Καταργήστε τον κώδικα από τον πόρο και αντικαταστήστε τον με τον ακόλουθο κώδικα.</span><span class="sxs-lookup"><span data-stu-id="c8d08-136">Remove the code from the resource, and replace it with the following code.</span></span>

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. <span data-ttu-id="c8d08-137">Αποθηκεύστε και δημοσιεύστε τις προσαρμογές.</span><span class="sxs-lookup"><span data-stu-id="c8d08-137">Save and then publish the customizations.</span></span>
