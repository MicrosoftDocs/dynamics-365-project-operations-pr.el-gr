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
ms.openlocfilehash: 9c9e31dc6d4d5a8ad5cc568f2d7d673c8703936d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284853"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>Προσθήκη νέων φορμών προσαρμοσμένης οντότητας (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>Τύπος πεδίου 

Το Dynamics 365 Project Service Automation βασίζεται στο πεδίο **Τύπος** (**msdyn\_ordertype**) στις οντότητες Ευκαιρία, Προσφορά, Παραγγελία και Τιμολόγιο για να διακρίνει αυτές τις εκδόσεις **βάσει εργασίας** αυτών των οντοτήτων από τις εκδόσεις **βάσει στοιχείου** και **βάσει υπηρεσίας**. Οι εκδόσεις που βασίζονται σε εργασία αυτών των οντοτήτων διεκπεραιώνονται από το PSA. Η πολλή επιχειρηματική λογική από την πλευρά του προγράμματος-πελάτη και από την πλευρά του διακομιστή της λύσης εξαρτάται από το πεδίο **Τύπος**. Για αυτόν το λόγο, είναι σημαντικό να προετοιμαστεί το πεδίο με σωστή τιμή κατά τη δημιουργία των οντοτήτων. Μια εσφαλμένη τιμή μπορεί να προκαλέσει εσφαλμένες συμπεριφορές και κάποια επιχειρηματική λογική ενδέχεται να μην εκτελεστεί σωστά.

## <a name="automatic-form-switching"></a>Αυτόματη εναλλαγή φορμών

Για να αποφύγετε την καταστροφή πιθανών δεδομένων και τις μη αναμενόμενες συμπεριφορές που προκαλούνται από εσφαλμένη προετοιμασία και επεξεργασία των καρτελών της οντότητας πωλήσεων, το PSA πλέον περιλαμβάνει λογική για την αυτόματη εναλλαγή φορμών στις έτοιμες φόρμες. Αυτή η λογική πηγαίνει τους χρήστες στη σωστή φόρμα για εργασία με την έκδοση με βάση την εργασία ή με οποιονδήποτε άλλο τύπο οντότητας ευκαιρίας, προσφοράς, παραγγελίας ή τιμολογίου. Όταν ένας χρήστης ανοίγει την έκδοση με βάση την εργασία μιας οντότητας ευκαιρίας, προσφοράς, παραγγελίας ή τιμολογίου, η φόρμα αλλάζει σε **Πληροφορίες έργου**.

Η λογική αυτόματης εναλλαγής φορμών βασίζεται στην αντιστοίχιση μεταξύ της τιμής **formId** και του πεδίου **msdyn\_ordertype**. Όλες οι έτοιμες φόρμες έχουν προστεθεί σε αυτήν την αντιστοίχιση. Ωστόσο, οι προσαρμοσμένες φόρμες θα πρέπει να προστεθούν με μη αυτόματο τρόπο, για να υποδείξουν την έκδοση της οντότητας που πρόκειται να διαχειριστούν. Αυτό βασίζεται στο πεδίο **msdyn\_ordertype**. Εάν η εναλλαγή φορμών λείπει από την αντιστοίχιση, η λογική θα μεταπηδήσει στην έτοιμη φόρμα με βάση την τιμή που αποθηκεύεται στο πεδίο **msdyn\_ordertype** της οντότητας.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>Προσθήκη προσαρμοσμένων φορμών και ενεργοποίηση της λογικής εναλλαγής φορμών

Το παρακάτω παράδειγμα δείχνει τον τρόπο προσθήκης μιας προσαρμοσμένης φόρμας, **Τα στοιχεία έργου μου** έτσι ώστε να λειτουργεί με ευκαιρίες βασισμένες στην εργασία. Η ίδια διεργασία χρησιμοποιείται για την προσθήκη προσαρμοσμένων φορμών, έτσι ώστε να λειτουργούν με προσφορές, παραγγελίες και τιμολόγια.

Ακολουθήστε τα παρακάτω βήματα για να δημιουργήσετε μια προσαρμοσμένη έκδοση της φόρμας **Πληροφορίες έργου**.

1. Στην οντότητα ευκαιρίας, ανοίξτε τη φόρμα **Πληροφορίες έργου** και αποθηκεύστε ένα αντίγραφο με το όνομα **Οι πληροφορίες έργου μου**.
2. Ανοίξτε τη νέα φόρμα και, στη συνέχεια, στις ιδιότητες, βεβαιωθείτε ότι υπάρχουν οι δέσμες ενεργειών προετοιμασίας φορμών από τη φόρμα **Πληροφορίες έργου**. 

    > [!IMPORTANT]
    > Μην καταργήσετε τις δέσμες ενεργειών. Διαφορετικά, ορισμένα δεδομένα ενδεχομένως να μην αρχικοποιηθούν σωστά.

3. Βεβαιωθείτε ότι το πεδίο **Τύπος** (**msdyn\_ordertype**) υπάρχει στη φόρμα. 

    > [!IMPORTANT]
    > Μην καταργήσετε αυτό το πεδίο. Διαφορετικά, οι δέσμες ενεργειών προετοιμασίας θα αποτύχουν.

4. Βρείτε την τιμή **formId** της νέας φόρμας. Μπορείτε να τη συμπληρώσετε με δύο τρόπους:

    - Κάντε εξαγωγή της φόρμας **Τα στοιχεία έργου μου** ως μέρος μιας μη διαχειριζόμενης λύσης και μετά αναζητήστε την τιμή **formId** στο αρχείο customization.xml της λύσης που έχει εξαχθεί.
    - Ανοίξτε τη φόρμα **Τα στοιχεία έργου μου** στο πρόγραμμα επεξεργασίας φορμών και, στη συνέχεια, αναζητήστε το καθολικά μοναδικό αναγνωριστικό (GUID) δίπλα στην παράμετρο **fromId** στην URL όπως φαίνεται στην παρακάτω απεικόνιση.

    ![Η τιμή formId της νέας φόρμας στο URL](media/how-to-add-custom-forms-in-v2.0.png)

5. Δημιουργήστε μια αντιστοίχιση **msdyn\_ordertype** για την τιμή **formId** κάνοντας επεξεργασία του πόρου web msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js. Καταργήστε τον κώδικα από τον πόρο και αντικαταστήστε τον με τον ακόλουθο κώδικα.

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

6. Αποθηκεύστε και δημοσιεύστε τις προσαρμογές.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]