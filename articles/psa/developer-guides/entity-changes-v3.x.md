---
title: Αλλαγές οντότητας, στοιχείου ελέγχου και περιβάλλοντος εργασίας χρήστη (Project Service Automation 3.x)
description: Αυτό το άρθρο περιγράφει τις αλλαγές για το Microsoft Dynamics Project Service Automation 3.x.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 8f54d263666c4fb999464f98c0138fc008dbbbd2
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926868"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>Αλλαγές οντότητας, στοιχείου ελέγχου και περιβάλλοντος εργασίας χρήστη (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


Με την κυκλοφορία του Microsoft Dynamics Project Service Automation 3.x., έχουν γίνει πολλές αλλαγές στις οντότητες, τα στοιχεία ελέγχου, τις προβολές και το περιβάλλον εργασίας χρήστη. Αυτό το άρθρο παρέχει σημαντικές πληροφορίες σχετικά με αυτές τις σημαντικές αλλαγές.

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>Θυγατρικές-γονικές σχέσεις για έγγραφο πωλήσεων, γραμμές εγγράφου πωλήσεων, οντότητες λεπτομερειών γραμμής εγγράφου πωλήσεων
Σε εκδόσεις του Dynamics 365 Project Service Automation (PSA) που κυκλοφόρησαν πριν την έκδοση 3.0, ορισμένες από τις σχέσεις μεταξύ εγγράφων πωλήσεων, γραμμών εγγράφου πωλήσεων και οντοτήτων λεπτομερειών γραμμής εγγράφου πωλήσεων εφαρμόστηκαν μέσω πεδίων συμβολοσειράς που θα διατηρήσουν μια αναπαράσταση συμβολοσειράς του GUID της σχετικής οντότητας. Αυτό οφειλόταν σε περιορισμούς πλατφόρμας που απαίτησαν σημαντικό προσαρμοσμένο κώδικα στον διακομιστή και τις πλευρές του προγράμματος-πελάτη της λύσης ώστε αυτές οι σχέσεις να λειτουργούν παρόμοια με τις τυπικές σχέσεις οντότητας Dynamics CRM και να κάνουν τα πεδία συμβολοσειράς να ενεργούν ως πεδία αναζήτησης.

Το PSA 3.0 έχει ενημερωθεί για την αξιοποίηση των νέων σχέσεων οντότητας μεταξύ των οντοτήτων εγγράφου πωλήσεων και γραμμών εγγράφου.

Επειδή τα πεδία αναζήτησης μπορούν τώρα να χρησιμοποιηθούν για να υποδείξουν αναφορές σε οντότητες, τα πεδία που κράτησαν την τιμή συμβολοσειράς του GUID της σχετικής οντότητας σε προηγούμενες εκδόσεις δεν είναι πλέον απαραίτητα και επομένως έχουν καταργηθεί. Επίσης, ο προσαρμοσμένος κώδικας του προγράμματος-πελάτη και του διακομιστή που χειρίζεται τις σχέσεις που ορίζονται από τα πεδία συμβολοσειρών παλαιού τύπου έχουν επίσης καταργηθεί.

### <a name="entity-schema-changes"></a>Αλλαγές σχήματος οντότητας
Ο ακόλουθος πίνακας παρέχει μια λίστα "ένα προς ένα" των πεδίων συμβολοσειράς που δεν χρησιμοποιούνται και των νέων πεδίων αναζήτησης για τις οντότητες. 

 Οντότητα |   Πεδίο που δεν χρησιμοποιείται (συμβολοσειρά) | Νέο πεδίο (αναζήτηση)
--- | --- | ---
invoicedetail (Γραμμή τιμολογίου) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (Πραγματικά) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (χρονοδιάγραμμα τιμολογίου γραμμής σύμβασης έργου) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (ορόσημο γραμμής σύμβασης έργου) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (γεγονός) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (λεπτομέρεια γραμμής τιμολογίου) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (γραμμή τιμολογίου) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (κατηγορία πόρων γραμμής σύμβασης έργου) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (λεπτομέρεια γραμμής σύμβασης έργου) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (κατηγορία συναλλαγής γραμμής σύμβασης έργου) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (ταξινόμηση συναλλαγής γραμμής σύμβασης έργου) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (χρονοδιάγραμμα τιμολογίου γραμμής προσφοράς) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (κατηγορία πόρου γραμμής προσφοράς) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (ορόσημο γραμμής προσφοράς) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (λεπτομέρεια γραμμής προσφοράς) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (κατηγορία συναλλαγών γραμμής προσφοράς) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (Ταξινόμηση συναλλαγής γραμμής προσφοράς) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (Γραμμή παραγγελίας) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>Μη προσαρμοσμένες προβολές και στοιχεία ελέγχου που έχουν απορριφθεί
Οι παρακάτω προσαρμοσμένες προβολές και τα στοιχεία ελέγχου και τα σχετικά χειροποίητα αντικείμενα έχουν καταργηθεί.

- Προβολή χρέωσης.
- Προσαρμοσμένα στοιχεία ελέγχου πλέγματος για εμφάνιση λεπτομερειών στη σελίδα **Πληροφορίες προσφοράς** για τη γραμμή προσφοράς.
- Προσαρμοσμένα στοιχεία ελέγχου πλέγματος για εμφάνιση λεπτομερειών γραμμής σύμβασης έργου στη σελίδα **Πληροφορίες προσφοράς** για τη γραμμή παραγγελίας πώλησης.

> [!NOTE]
> Για την πλήρη λίστα των πόρων που δεν χρησιμοποιούνται δείτε [Πόροι web που δεν χρησιμοποιούνται στο Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>Λειτουργική μονάδα εφαρμογής Ενοποιημένο περιβάλλον εργασίας
Με την εισαγωγή λειτουργικών μονάδων εφαρμογής Ενοποιημένο περιβάλλον εργασίας (UCI), οι καταχωρήσεις του χάρτη τοποθεσίας PSA έχουν καταργηθεί από το σύστημα.  
Οι λειτουργίες που σχετίζονται με την εναλλαγή φορμών για την ευκαιρία, την προσφορά, την παραγγελία, το τιμολόγιο δεν είναι πλέον απαραίτητα επειδή η λειτουργική μονάδα εφαρμογής UCI περιλαμβάνει μόνο τις εκδόσεις PSA των φορμών.  

Οι ακόλουθοι πόροι Web έχουν καταργηθεί:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> Για την πλήρη λίστα των πόρων που δεν χρησιμοποιούνται δείτε [Πόροι web που δεν χρησιμοποιούνται στο Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md).




[!INCLUDE[footer-include](../../includes/footer-banner.md)]
