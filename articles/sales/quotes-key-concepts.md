---
title: Προσφορές - Βασικές έννοιες
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις προσφορές έργου και τις προσφορές πωλήσεων που είναι διαθέσιμες στο Project Operations (Λειτουργίες έργου).
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
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: b252f6e02d0809c352d3665731ec5e02e4e9a73f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898442"
---
# <a name="quotes---key-concepts"></a>Προσφορές - Βασικές έννοιες

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Στο Dynamics 365 Project Operations, υπάρχουν δύο τύποι προσφορών, έργου και πωλήσεων. Οι δύο τύποι προσφορών στα εξής:

- **Πλέγματα για στοιχεία γραμμής**: Σε μια προσφορά πώλησης, υπάρχει μόνο ένα πλέγμα για τα στοιχεία γραμμών. Σε μια προσφορά έργου υπάρχουν δύο πλέγματα για τα στοιχεία γραμμών. Το ένα πλέγμα είναι για τις γραμμές έργου και το άλλο για τις γραμμές προϊόντων.
- **Ενεργοποίηση και αναθεωρήσεις**: Οι προσφορές πωλήσεων υποστηρίζουν ενεργοποίηση και αναθεωρήσεις. Αυτές οι διεργασίες δεν υποστηρίζονται σε μια προσφορά έργου.
- **Συνημμένες παραγγελίες**: Μπορείτε να επισυνάψετε πολλαπλές παραγγελίες σε μια προσφορά πώλησης. Μπορείτε να επισυνάψετε μόνο μία σύμβαση έργου σε μια προσφορά έργου.
- **Νικήτρια προσφορά**: Όταν κερδίζετε μια προσφορά πωλήσεων, η σχετική ευκαιρία μπορεί να παραμείνει ανοιχτή. Μετά τη νίκη μιας προσφοράς έργου, κλείνει η σχετική ευκαιρία.
- **Πεδία και έννοιες**: Μια προσφορά πώλησης δεν περιλαμβάνει ορισμένα πεδία και έννοιες που περιλαμβάνονται σε μια προσφορά έργου. Τα πεδία περιλαμβάνουν **Μονάδα συμβάσεων**, **Υπεύθυνος λογαριασμών** και **Όνομα επαφής χρέωσης**.  
- **Τύπος**: Οι προσφορές πωλήσεων και οι προσφορές έργου προσδιορίζονται επίσης από το πεδίο βάσει σύνολο επιλογών, το **Τύπος**. Για μια προσφορά πώλησης, αυτό το πεδίο έχει την τιμή **Βάσει στοιχείου**. Για μια προσφορά έργου, έχει την τιμή **Βάσει εργασίας**.

Αυτό το θέμα επικεντρώνεται στις λεπτομέρειες των προσφορών έργου.

Μια προσφορά έργου στο Project Operations μπορεί να έχει πολλαπλά στοιχεία γραμμής ή γραμμές προσφοράς. Στην πραγματικότητα, μια προσφορά έργου έχει δύο πλέγματα για τα στοιχεία γραμμών. Το ένα πλέγμα είναι για γραμμές βάσει έργου που επιτρέπουν τη λεπτομερή εκτίμηση. Το άλλο πλέγμα αφορά γραμμές βασισμένες σε προϊόντα που χρησιμοποιούν μια απλή τιμή μονάδας και προσέγγιση βασισμένη σε ποσότητες.

- **Βάσει έργου**: Το ποσό προσφοράς καθορίζεται αφού υπολογίσετε την εργασία που απαιτείται. Μπορείτε να υπολογίσετε την εργασία σε υψηλό επίπεδο, απευθείας ως λεπτομέρειες γραμμής που βρίσκεται κάτω από κάθε γραμμή προσφοράς ή βάσει εκτιμήσεων από το μηδέν, χρησιμοποιώντας ένα έργο και ένα σχέδιο έργου. Οι γραμμές προσφοράς βάσει έργου εντοπίζονται μόνο σε προσφορές βασισμένες σε έργα που δημιουργούνται με τη χρήση του Project Operations. Αυτός ο τύπος γραμμής προσφοράς είναι μια προσαρμοσμένη φόρμα των γραμμών εγγεγραμμένης προσφοράς που είναι διαθέσιμες στο Microsoft Dynamics 365 Sales.

- **Με βάση τα προϊόντα**: Το ποσό προσφοράς καθορίζεται με βάση την ποσότητα των μονάδων που πωλούνται και της μοναδιαίας τιμής πώλησης. Το προϊόν σε μια γραμμή με βάση τα προϊόντα μπορεί να προέλθει από έναν κατάλογο προϊόντων στο Sales ή μπορεί να είναι ένα προϊόν που καθορίζετε εσείς. Αυτός ο τύπος προσφοράς είναι επίσης διαθέσιμος σε προσφορές βασισμένες σε έργα που δημιουργούνται με τη χρήση του Project Operations.

Το ποσό μιας προσφοράς είναι το σύνολο σε όλες τις γραμμές που βασίζονται σε προϊόντα και στις γραμμές βάσει έργου.

> [!NOTE]
> Οι προσφορές και οι γραμμές προσφοράς δεν είναι απαραίτητες στο Project Operations. Μπορείτε να εκκινήσετε τη διεργασία έργου με μια σύμβαση έργου (πωληθέν έργο). Ωστόσο, απαιτείται πάντα μια ευκαιρία, ανεξάρτητα από το εάν ξεκινάτε με μια προσφορά ή μια σύμβαση έργου.

## <a name="project-based-quote-lines"></a>Γραμμές προσφοράς βάσει έργου

Μια γραμμή προσφοράς βάσει έργου στο Project Operations έχει τις παρακάτω μεθόδους χρέωσης:

- Χρόνος και υλικό
- Σταθερή τιμή

### <a name="time-and-material"></a>Χρόνος και υλικό

Η μέθοδος χρέωσης του χρόνου και του υλικού βασίζεται στην κατανάλωση. Όταν επιλέγετε αυτήν τη μέθοδο χρέωσης, ο πελάτης τιμολογείται καθώς το έργο επιβαρύνεται με κόστος. Τα τιμολόγια δημιουργούνται σε μια περιοδική συχνότητα βάσει ημερομηνιών. Κατά τη διάρκεια της διαδικασίας πωλήσεων, η τιμή που αναφέρεται σε ένα στοιχείο χρόνου και υλικού δίνει μόνο μια εκτίμηση του τελικού κόστους για τον πελάτη. Ο προμηθευτής δεν δεσμεύεται για την ολοκλήρωση του έργου στην ακριβή τιμή προσφοράς. Τα στοιχεία χρόνου και υλικού αυξάνουν τον κίνδυνο του πελάτη. Οι πελάτες μπορεί να θέλουν να διαπραγματευτούν πρόσθετες ρήτρες μη υπέρβασης για την ελαχιστοποίηση του κινδύνου. Το Project Operations δεν υποστηρίζει τη ρύθμιση ρητρών μη υπέρβασης.

### <a name="fixed-price"></a>Σταθερή τιμή

Στη μέθοδο χρέωσης σταθερής τιμής, ένας προμηθευτής δεσμεύεται να παραδώσει το έργο με σταθερό κόστος για τον πελάτη. Ο πελάτης χρεώνεται με την τιμή της προσφοράς της γραμμής προσφοράς σταθερής τιμής, ανεξάρτητα από το κόστος που υπέχει ο προμηθευτής για να παραδώσει τη γραμμή προσφοράς. Η τιμή της γραμμής προσφοράς προκαθορισμένης τιμής χρεώνεται με έναν από τους ακόλουθους τρόπους: 

- Ως εφάπαξ ποσό στην αρχή ή στο τέλος του έργου ή όταν επιτυγχάνεται ένα ορόσημο έργου. 
- Σε μια συχνότητα με βάση την ημερομηνία των ίσων δόσεων της σταθερής τιμής στη γραμμή προσφοράς. Αυτές οι δόσεις είναι γνωστές ως περιοδικά ορόσημα.
- Σε δόσεις που έχουν μια χρηματική τιμή που ευθυγραμμίζεται με την πρόοδο της εργασίας ή με συγκεκριμένα ορόσημα που επιτυγχάνονται στο έργο. Σε αυτήν την περίπτωση, η τιμή κάθε δόσης μπορεί να διαφέρει, αλλά όλες πρέπει να προσθέτουν έως τη σταθερή τιμή στη γραμμή προσφοράς.

Το Project Operations υποστηρίζει και τους τρεις τύπους χρονοδιαγραμμάτων τιμολογίων για τις γραμμές προσφοράς σταθερών τιμών.

## <a name="transaction-classification"></a>Ταξινόμηση συναλλαγής

Οι επαγγελματικοί οργανισμοί εξυπηρέτησης συνήθως κάνουν προσφορά και τιμολογούν τους πελάτες τους με βάση την ταξινόμηση του κόστους. Το κόστος αντιπροσωπεύεται από τις ακόλουθες ταξινομήσεις συναλλαγής:

- **Χρόνος**: Αυτή η ταξινόμηση αντιπροσωπεύει το κόστος εργασίας ή το χρόνο ανθρώπινου δυναμικού σε ένα έργο.
- **Έξοδο**: Αυτή η ταξινόμηση αντιπροσωπεύει όλα τα άλλα είδη δαπανών σε ένα έργο. Επειδή οι δαπάνες μπορεί να είναι ευρέως ταξινομημένες, οι περισσότεροι οργανισμοί δημιουργούν υποκατηγορίες, όπως ταξίδι, ενοικιάσεις αυτοκινήτων, ξενοδοχεία ή αναλώσιμα γραφείου.
- **Τέλος**: Αυτή η ταξινόμηση αντιπροσωπεύει διάφορες επιβαρύνσεις, πρόστιμα και άλλα στοιχεία που επιβαρύνουν τον πελάτη. 
- **Φόρος**: Αυτή η ταξινόμηση αντιπροσωπεύει τα ποσά φόρων που προσθέτουν οι χρήστες όσο εισάγουν έξοδα.
- **Συναλλαγή υλικών**: Αυτή η ταξινόμηση αντιπροσωπεύει τα πραγματικά στοιχεία από τις γραμμές προϊόντων σε ένα επιβεβαιωμένο τιμολόγιο έργου.
- **Ορόσημο**: Αυτή η ταξινόμηση χρησιμοποιείται από τη λογική χρέωσης σταθερών τιμών.

Μία ή περισσότερες ταξινομήσεις συναλλαγών συσχετίζονται με κάθε γραμμή προσφοράς. Μετά τη νίκη μιας προσφοράς, η αντιστοίχιση μεταξύ ταξινόμησης και προσφοράς συναλλαγής μεταβιβάζεται στη γραμμή σύμβασης.
  
Για παράδειγμα, μια προσφορά μπορεί να περιέχει τις εξής δύο γραμμές προσφοράς: 

- Συμβουλευτικές εργασίες που χρησιμοποιούν μια μέθοδο χρέωσης χρόνου και υλικού, όπου ισχύουν ταξινομήσεις συναλλαγής χρόνου και τέλους. Για παράδειγμα, όλες οι συναλλαγές χρόνου και τέλους για το παράδειγμα **Εφαρμογή Dynamics AX** τιμολογούνται στον πελάτη με βάση την ώρα και το υλικό που χρησιμοποιούνται. 
- Σχετικά έξοδα ταξιδίου που χρησιμοποιούν μια μέθοδο χρέωσης προκαθορισμένης τιμής. Για παράδειγμα, όλα τα έξοδα ταξιδίου για το παράδειγμα **Εφαρμογή Dynamics AX** τιμολογούνται σε μια σταθερή νομισματική αξία.

> [!NOTE]
> Ο συνδυασμός των ταξινομήσεων έργου και συναλλαγής των στοιχείων **Χρόνος**, **Έξοδα** και **Τέλη** που σχετίζονται με μια γραμμή προσφοράς ή μια γραμμή σύμβασης πρέπει να είναι μοναδικός. Εάν ο ίδιος συνδυασμός της κλάσης έργου και συναλλαγής είναι συσχετισμένος με περισσότερες από μία γραμμές σύμβασης ή γραμμές προσφοράς, το Project Operations δεν θα λειτουργεί σωστά.

## <a name="billing-types"></a>Τύποι χρέωσης

Το πεδίο **Τύπος χρέωσης** καθορίζει την έννοια της χρέωσης. Πρόκειται για μια σύνολο επιλογών που έχει τις ακόλουθες πιθανές τιμές:

- **Χρεώσιμο**: Το κόστος που συσσωρεύεται από αυτόν το ρόλο/κατηγορία είναι ένα άμεσο κόστος που καθοδηγεί την εκτέλεση του έργου και ο πελάτης θα πληρώσει για αυτήν την εργασία. Η πληρωμή μπορεί να αντιμετωπιστεί ως συμφωνία χρόνου και υλικού ή προκαθορισμένης τιμής. Ωστόσο, ο εργαζόμενος που αφιερώνει αυτήν τη φορά τον χρόνο θα λάβει την αντίστοιχη διαπίστευση για τη χρεώσιμη χρήση που χρησιμοποιεί.
- **Μη χρεώσιμο**: Το κόστος που συσσωρεύεται από αυτόν το ρόλο/κατηγορία είναι ένα άμεσο κόστος που καθοδηγεί την εκτέλεση του έργου ακόμα και αν ο πελάτης δεν θα πληρώσει για αυτήν την εργασία. Ο εργαζόμενος που αφιερώνει αυτήν τη φορά χρόνο δεν θα πιστωθεί με χρήση χρέωσης για αυτό το άτομο.
- **Δωρεάν**: Το κόστος που συσσωρεύεται από αυτόν το ρόλο/κατηγορία είναι ένα άμεσο κόστος που καθοδηγεί την εκτέλεση του έργου και ο πελάτης αναγνωρίζει αυτό το γεγονός. Ο εργαζόμενος που αφιερώνει αυτήν τη φορά χρόνο θα πιστωθεί με χρήση χρέωσης για αυτό το άτομο. Ωστόσο, αυτό το κόστος δεν χρεώνεται στον πελάτη.
- **Μη διαθέσιμο**: Τα κόστη που επιβαρύνουν τα εσωτερικά έργα που δεν απαιτούν παρακολούθηση εσόδων παρακολουθούνται με χρήση αυτής της επιλογής.

## <a name="invoice-schedule"></a>Χρονοδιάγραμμα τιμολογίων

Το χρονοδιάγραμμα τιμολόγησης είναι μια σειρά ημερομηνιών κατά την τιμολόγηση για ένα έργο που προκύπτει. Μπορείτε, προαιρετικά, να δημιουργήσετε ένα χρονοδιάγραμμα τιμολογίου σε μια γραμμή προσφοράς. Κάθε γραμμή προσφοράς μπορεί να έχει το δικό της χρονοδιάγραμμα τιμολόγησης. Για να δημιουργήσετε ένα χρονοδιάγραμμα τιμολόγησης, πρέπει να παράσχετε τις παρακάτω τιμές χαρακτηριστικών:

- Μια ημερομηνία έναρξης χρέωσης 
- Μια ημερομηνία παράδοσης που αναπαριστά την ημερομηνία λήξης της χρέωσης στο έργο
- Μια συχνότητα τιμολογίων

Αυτές τις τρεις τιμές χαρακτηριστικών χρησιμοποιούνται για να δημιουργηθεί ένα κατά προσέγγιση σύνολο ημερομηνιών για τη δημιουργία τιμολόγησης.

## <a name="invoice-frequency"></a>Συχνότητα τιμολογίων

Η συχνότητα τιμολόγησης είναι μια οντότητα που αποθηκεύει τιμές χαρακτηριστικών που βοηθούν στην έκφραση της συχνότητας δημιουργίας τιμολογίων. Τα παρακάτω χαρακτηριστικά εκφράζουν ή ορίζουν την οντότητα συχνότητας τιμολογίου:

- **Περίοδος**: Υποστηρίζονται οι μηνιαίες, δεκαπενθήμερες και εβδομαδιαίες περίοδοι. 
- **Εκτελέσεις ανά περίοδο**: Για εβδομαδιαίες και δεκαπενθήμερες περιόδους, μπορείτε να ορίσετε μόνο μία εκτέλεση ανά περίοδο. Για μηνιαίες περιόδους, μπορείτε να ορίσετε μεταξύ μίας και τεσσάρων εκτελέσεων ανά περίοδο. 
- **Ημέρες εκτέλεσης**: Οι ημέρες κατά τις οποίες πρέπει να εκτελεστεί η τιμολόγηση. Μπορείτε να ρυθμίσετε αυτό το χαρακτηριστικό με δύο τρόπους:
  - **Καθημερινές**: Για παράδειγμα, μπορείτε να καθορίσετε την εκτέλεση της τιμολόγησης κάθε Δευτέρα ή κάθε δεύτερη Δευτέρα. Οι πελάτες που πρέπει να ορίσουν την τιμολόγηση για εκτέλεση σε μια εργάσιμη ημέρα μπορεί να προτιμούν τέτοιου είδους ρυθμίσεις παραμέτρων. 
  - **Ημερολογιακές ημέρες**: Για παράδειγμα, μπορείτε να προσδιορίσετε ότι η τιμολόγηση εκτελείται την έβδομη και την εικοστή πρώτη ημέρα κάθε μήνα. Ορισμένοι οργανισμοί ενδέχεται να προτιμούν τέτοιου είδους ρυθμίσεις παραμέτρων, επειδή βοηθούν στο να είναι εγγυημένο ότι η τιμολόγηση εκτελείται σε ένα σταθερό χρονοδιάγραμμα κάθε μήνα.
  
### <a name="invoice-schedule-for-a-fixed-price-quote-line"></a>Χρονοδιάγραμμα τιμολόγησης για μια γραμμές προσφοράς σταθερής τιμής

Για μια γραμμή προσφοράς σταθερής τιμής, μπορείτε να χρησιμοποιήσετε το πλέγμα **Χρονοδιάγραμμα τιμολόγησης** για να δημιουργήσετε ορόσημα χρέωσης τα οποία ισούνται με την τιμή της γραμμής προσφοράς.

- Για να δημιουργήσετε ορόσημα χρέωσης που είναι ισότιμα διαιρεμένα, επιλέξτε μια συχνότητα τιμολόγησης, καταγράψτε την ημερομηνία έναρξης χρέωσης στη γραμμή προσφοράς και επιλέξτε **Ζητούμενη ημερομηνία ολοκλήρωσης** στην ενότητα **Σύνοψη** της επικεφαλίδας προσφοράς. Στη συνέχεια επιλέξτε **Δημιουργία περιοδικών ορόσημων** για τη δημιουργία ισότιμων διαχωριστικών ορόσημων με βάση την επιλεγμένη συχνότητα τιμολογίου. 
- Για να δημιουργήσετε ένα ορόσημο χρέωσης εφάπαξ, δημιουργήστε ένα ορόσημο και, στη συνέχεια, καταγράψτε την τιμή της γραμμής προσφοράς ως το ποσό του ορόσημου.
- Για να δημιουργήσετε ορόσημα χρέωσης τα οποία βασίζονται σε συγκεκριμένες εργασίες του σχεδίου έργου, δημιουργήστε ένα ορόσημο και αντιστοιχίστε το στο στοιχείο χρονοδιαγράμματος του έργου, στο περιβάλλον εργασίας χρήστη ορόσημων χρέωσης.
