---
title: Τιμοκατάλογοι προϊόντος
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τους τιμοκαταλόγους στην τιμολόγηση καταλόγου που χρησιμοποιούνται για προσφορές και συμβάσεις έργου.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3570aeb78804e9b267caa55a27e02d6c8df9a5c6
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898171"
---
# <a name="product-price-lists"></a>Τιμοκατάλογοι προϊόντος

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Οι τιμοκατάλογοι και οι οντότητες στοιχείων τιμοκαταλόγου υποστηρίζουν την τιμολόγηση καταλόγου προϊόντων. Ως επί το πλείστον, αυτή η λειτουργικότητα χρησιμοποιείται για γραμμές βασισμένες σε καταλόγους σε προσφορές έργου και συμβάσεις έργου.

Για τις γραμμές βάσει έργου, μια σύμβαση αντιπροσωπεύει τη συμφωνία αφού αυτή κερδηθεί. Επειδή η διαδικασία της διαπραγμάτευσης συνήθως προηγείται της νίκης, η τιμολόγηση που επισυνάπτεται στην προσφορά αντιγράφεται πάντα ως έχει σε ένα νέο τιμοκατάλογο και επισυνάπτεται στη σύμβαση. Αυτός ο νέος τιμοκατάλογος δεν μπορεί να αλλάξει εκτός του πεδίου της σύμβασης. Αυτός ο περιορισμός προστατεύει την κάρτα ποσοστού για την οποία έγινε διαπραγμάτευση από οποιεσδήποτε αλλαγές στις τιμές που πραγματοποιούνται στον κύριο τιμοκατάλογο.

Τα προϊόντα θα πρέπει να οριστούν έτσι, ώστε να έχουν προεπιλεγμένους τιμοκαταλόγους κόστους και τιμής στον κατάλογο προϊόντων. Χρησιμοποιήστε την τιμή καταλόγου, το τυπικό κόστος και το τρέχον κόστος για να ρυθμίσετε τις παραμέτρους του προεπιλεγμένου κόστους και τις τιμές καταλόγου. Οι προεπιλεγμένες τιμές λίστας χρησιμοποιούνται σε μια γραμμή προσφοράς ή μια γραμμή σύμβασης έργου μόνο όταν το σύστημα δεν μπορεί να βρει μια γραμμή τιμοκαταλόγου για αυτό το προϊόν στο τιμοκατάλογο προϊόντος για την προσφορά ή τη σύμβαση έργου.

Η τιμή κόστους των γραμμών καταλόγου προϊόντων μπορεί να αλλάξει μεταξύ προσφορών. Αυτή η δυνατότητα είναι σημαντική, επειδή αν δεν παρακολουθείτε με ακρίβεια το κόστος, δεν μπορείτε να καθορίσετε τα λειτουργικά κέρδη στις δεσμεύσεις του έργου. Από προεπιλογή, το τυπικό κόστος του προϊόντος χρησιμοποιείται ως τιμή κόστους. Ωστόσο, η τιμή του προεπιλεγμένου κόστους μπορεί να ενημερωθεί στη γραμμή προσφοράς, εάν υπάρχει διαφορετική τιμή κόστους για την εν λόγω προσφορά.

## <a name="price-list-items"></a>Στοιχεία τιμοκαταλόγου

Μπορείτε να προσθέσετε προϊόντα από έναν κατάλογο προϊόντων σε διαφορετικούς τιμοκαταλόγους. Οι γραμμές τιμοκαταλόγου για τα προϊόντα αναφέρονται πάντα σε μια συγκεκριμένη μονάδα. Η τιμολόγηση για ένα προϊόν σε στοιχεία τιμοκαταλόγου μπορεί να ρυθμιστεί ως ποσό νομίσματος. Εναλλακτικά, μπορεί να ρυθμιστεί ως συνάρτηση της τιμής λίστας, του τρέχοντος κόστους ή του τυπικού κόστους.

Το PSA υποστηρίζει διάφορες επιλογές στρογγυλοποίησης, όταν οι τιμές έχουν ρυθμιστεί ως συνάρτηση της τιμής τιμοκαταλόγου, του τυπικού κόστους ή του τρέχοντος κόστους. Εκτός από την αξιοποίηση πολλών μεθόδων τιμολόγησης και επιλογών στρογγυλοποίησης, μπορείτε να συσχετίσετε τις λίστες εκπτώσεων με τα στοιχεία τιμοκαταλόγου. 

Όταν δημιουργείτε έναν νέο προσαρμοσμένο τιμοκατάλογο για μια προσφορά επιλέγοντας **Δημιουργία προσαρμοσμένης τιμολόγησης** στη σελίδα **Προσφορά έργου**, δημιουργείται ένα αντίγραφο του τιμοκαταλόγου και το πεδίο **Οντότητα** στην επικεφαλίδα του νέου τιμοκαταλόγου έχει οριστεί σε **Οντότητα "Πωλήσεις"**. Το όνομα του νέου τιμοκαταλόγου επισυνάπτεται στο όνομα της προσφοράς και σε μια σήμανση χρόνου. Επίσης, μπορείτε να χρησιμοποιήσετε το όνομα του νέου τιμοκαταλόγου και το όνομα της προσφοράς σε προσαρμοσμένες ροές εργασιών για να ενεργοποιήσετε την πρόσθετη αναθεώρηση και τις εγκρίσεις για προσφορές που χρησιμοποιούν προσαρμοσμένη τιμολόγηση.

 
## <a name="default-product-price-list"></a>Προεπιλεγμένος τιμοκατάλογος προϊόντων
Κάθε καρτέλα πελάτη έχει ένα πεδίο **Προσαρμοσμένος τιμοκατάλογος** όπου μπορείτε να καθορίσετε έναν τιμοκατάλογο που να αντιστοιχεί στη νομισματική μονάδα του πελάτη. Μια προεπιλεγμένη τιμή δεν καταχωρείται αυτόματα σε αυτό το πεδίο. Όταν υπάρχει μια προσαρμοσμένη συμφωνία τιμολόγησης με ένα συγκεκριμένο πελάτη, μπορείτε να χρησιμοποιήσετε αυτό το πεδίο για να συσχετίσετε έναν τιμοκατάλογο με αυτόν τον πελάτη.

Οι οντότητες "ευκαιρία", "προσφορά" και "σύμβαση έργου" χρησιμοποιούν την ακόλουθη σειρά για να εισαγάγουν προεπιλεγμένους τιμοκαταλόγους προϊόντων. Η ίδια παραγγελία χρησιμοποιείται για τους τιμοκαταλόγους έργου.

1.  Προσφορά
2.  Ευκαιρία
3.  Πελάτης
4.  Καθολικές ρυθμίσεις 

Από προεπιλογή, το πεδίο **Προϊόν** στη γραμμή προσφοράς παραθέτει όλα τα ενεργά προϊόντα στο τιμοκατάλογο προϊόντος της προσφοράς. Εάν ένα προϊόν έχει αδρανοποιηθεί ή είναι προσχέδιο προϊόντος, δεν περιλαμβάνεται στη λίστα, ακόμα κι αν είναι στον τιμοκατάλογο. 

Οι γραμμές καταλόγου προϊόντων προστίθενται ως γραμμές τιμολογίου στο πρώτο τιμολόγιο που δημιουργείται για μια σύμβαση έργου. Σε ένα προσχέδιο τιμολογίου, οι εν λόγω γραμμές τιμολογίου είναι δυνατό να διαγραφούν. Σε αυτήν την περίπτωση, οι γραμμές θα εμφανιστούν σε ένα επόμενο τιμολόγιο μέχρι να τιμολογηθεί ή μέχρι να αποσταλεί το τιμολόγιο στον πελάτη. Δεν μπορείτε να τιμολογήσετε μια μερική ποσότητα μιας σειράς τιμολογίου προϊόντος. Όταν τιμολογούνται οι γραμμές προϊόντων από τη σύμβαση έργου, δημιουργούνται πραγματικές τιμές. Ωστόσο, αυτές οι πραγματικές τιμές δεν είναι συνδεδεμένες με τη σχετική οντότητα έργου. Με άλλα λόγια, οι γραμμές σύμβασης έργου που βασίζεται σε προϊόντα είναι ανεξάρτητες από οποιαδήποτε χρήση βάσει έργου. Δεν παρακολουθείται η υλική κατανάλωση σε έργα.