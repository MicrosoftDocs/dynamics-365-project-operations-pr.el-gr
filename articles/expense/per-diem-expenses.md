---
title: Ημερήσιες δαπάνες
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τον τρόπο εργασίας με τις ημερήσιες δαπάνες.
author: suvaidya
ms.date: 03/18/2022
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.search.region: ''
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 0d2f95b677720726049d7d010e9738ad8c513802
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923188"
---
# <a name="per-diem-expenses"></a>Ημερήσιες δαπάνες

> [!IMPORTANT] 
> Οι λειτουργίες που περιγράφονται σε αυτό το άρθρο είναι διαθέσιμες στους στοχευμένους χρήστες ως μέρος μιας έκδοσης προεπισκόπησης.

Η ημερήσια πληρωμή είναι ένα σταθερό, προκαθορισμένό καθημερινό επίδομα που μια εταιρεία πληρώνει στους υπαλλήλους της για τη διαμονή (ξενοδοχεία), τη διατροφή και περιστασιακές δαπάνες που υφίσταται ο συγκεκριμένος υπάλληλος ενώ ταξιδεύει για την επαγγελματικούς λόγους. Η εταιρεία πληρώνει αυτό το επίδομα στους υπαλλήλους αντί να πληρώνει τα πραγματικά οδοιπορικά. Οι υπάλληλοι μπορούν να χρησιμοποιούν το ημερήσιο επίδομα **Περιστασιακά/Άλλα** για να καλύπτουν φιλοδωρήματα, υπηρεσίες δωματίου, υπηρεσίες καθαριστηρίου ή στεγνοκαθαριστηρίου για σημαντικές επαγγελματικές συναντήσεις. Η ημερήσια τιμή μπορεί να ποικίλει, ανάλογα με το εάν ο εργοδότης επιλέγει να επιλέξει να αποζημιώσει για το συνδυασμένο κόστος της διαμονής και της διατροφής, ή μόνο για το κόστος της διατροφής και των περιστασιακών εξόδων.

Οι τιμές ημερήσιας αποζημίωσης βασίζονται στην εποχή του χρόνου, στην τοποθεσία ταξιδίου ή και στα δύο. Κατά τη δημιουργία ενός κανόνα ημερήσιας χρέωσης, μπορείτε να καθορίσετε ότι ένα ποσοστό της ημερήσιας χρέωσης θα παρακρατείται στην περίπτωση που ένας υπάλληλος λάβει δωρεάν διατροφή ή υπηρεσίες. Επίσης, μπορείτε να ορίσετε έναν ελάχιστο αριθμό ωρών και ένα μέγιστο αριθμό ωρών που η ημερήσια χρέωση μπορεί να εφαρμοστεί στα οδοιπορικά ενός υπαλλήλου.

Η ημερήσια αποζημίωσης υπολογίζεται ως το συνολικό επίδομα που προσφέρεται ανά ημέρα μείον τη μείωση διατροφής (κόστος δωρεάν γευμάτων) που παρέχεται στον εργαζόμενο.

## <a name="configure-per-diems"></a>Ρύθμιση παραμέτρων ημερήσιων αποζημιώσεων

Για να ρυθμίσετε τις ημερήσιες δαπάνες, ακολουθήστε τα παρακάτω βήματα.

1. Μεταβείτε στη **Διαχείριση εξόδων** \> **Ρύθμιση** \> **Γενικά** \> **Παράμετροι διαχείρισης εξόδων**.
2. Στην καρτέλα **Ημερήσια αποζημίωση**, στο πεδίο **Υπολογισμός μείωσης διατροφής κατά** επιλέξτε τον τρόπο υπολογισμού των ημερήσιων αποζημιώσεων:

    - **Τύπος γεύματος ανά ταξίδι** – Υπολογίστε την ημερήσια αποζημίωση με βάση τον τύπο γεύματος που εισάγεται (πρωϊνό, μεσημεριανό ή βραδινό) και με βάση τη μείωση γεύματος που καθορίζεται για κάθε τύπο γεύματος για το ημερήσιο επίδομα όσο διαρκεί το ταξίδι.
    - **Τύπος γεύματος ανά ημέρα** – Υπολογίστε την ημερήσια αποζημίωση με βάση τον τύπο γεύματος που εισάγεται και με βάση τη μείωση γεύματος που καθορίζεται για κάθε τύπο γεύματος για το ημερήσιο επίδομα ανά ημέρα.
    - **Αριθμός γευμάτων ανά ημέρα** – Υπολογίστε την ημερήσια αποζημίωση με βάση τον αριθμό των φευμάτων που καταχωρούνται ανά ημέρα και με τη μείωση του αριθμού των γευμάτων που παρέχονται καθημερινά.

3. Μεταβείτε στη **Διαχείριση εξόδων** \> **Ρύθμιση** \> **Υπολογισμοί και κωδικοί** \> **Ημερήσιες τοποθεσίες**.
4. Προσθέστε τοποθεσίες όπου μπορούν να χρησιμοποιηθούν οι ημερήσιες αποζημιώσεις.
5. Για κάθε τοποθεσία που προσθέτετε, στην καρτέλα **Ημερήσιες αποζημιώσεις**, επιλέξτε τη χρέωση και τη νομισματική μονάδα ημερήσιας αποζημίωσης που ισχύουν μεταξύ συγκεκριμένων ημερομηνιών έναρξης και λήξης για τη διαμονή, τη διατροφή και άλλες δαπάνες. Για να ρυθμίσετε τις παραμέτρους των χρεώσεων και των νομισματικών μονάδων ημερήσιων αποζημιώσεων, μεταβείτε στην **Διαχείριση δαπανών**\>**Ρύθμιση**\>**Υπολογισμοί και κωδικοί**\>**Ημερήσιες αποζημιώσεις**.

## <a name="per-diems-in-the-reimagined-expense-interface"></a>Οι ημερήσιες αποζημιώσεις στη νέα διασύνδεση δαπανών

Η δυνατότητα ημερήσια αποζημίωσης υποστηρίζεται στον νέο χώρο εργασίας **Διαχείριση δαπανών** στο Microsoft Dynamics 365 Finance έκδο 10.0.25 και νεότερη.

Για ενεργοποίηση ημερήσιων αποζημιώσεων, ακολουθήστε αυτά τα βήματα.

1. Στον χώρο εργασίας **Διαχείριση δυνατοτήτων**, βρείτε και επιλέξτε τη δυνατότητα **Νέες αναφορές δαπανών** στη λίστα και, στη συνέχεια, επιλέξτε **Ενεργοποίηση τώρα**.
2. Βρείτε και επιλέξτε τη δυνατότητα **Ημερήσια αποζημίωση για νέα διασύνδεση αναφορών δαπανών** στη λίστα και, έπειτα, επιλέξτε **Ενεργοποίηση τώρα**.

## <a name="how-the-feature-works"></a>Πώς λειτουργεί η δυνατότητα

Σε αυτήν την ενότητα παρέχονται παραδείγματα για τρία σενάρια ρύθμισης παραμέτρων. Για κάθε παράδειγμα, το πεδίο **Υπολογισμός μείωσης διατροφής κατά** ορίζεται σε διαφορετική τιμή. Και στα τρία παραδείγματα, το συνολικό ποσό που είναι πληρωτέο είναι το ίδιο έως ότου εφαρμοστεί η μείωση της διατροφής. Μετά από αυτό το σημείο, το συνολικό πληρωτέο ποσό διαφέρει για κάθε παράδειγμα.

Για να δημιουργήσετε την ημερήσια δαπάνη που χρησιμοποιείται και για τα τρία παραδείγματα, ακολουθήστε τα παρακάτω βήματα.

1. Μεταβείτε στους **Χώρους εργασίας** \> **Διαχείριση δαπανών**.
2. Επιλέξτε **Νέα αναφορά δαπανών** ή επιλέξτε μια υπάρχουσα αναφορά δαπανών.
3. Προσθήκη νέας δαπάνης. Στο πεδίο **Κατηγορία**, επιλέξτε **Ημερήσια αποζημίωση**. Επιλέξτε την τοποθεσία και τις ημερομηνίες έναρξης και λήξης του ταξιδιού σας. Η ημερήσια αποζημίωσης διαμονή, διατροφή και περιστασιακά έξοδα (άλλες δαπάνες) υπολογίζεται με βάση το ημερήσιο επίδομα που έχει οριστεί για την επιλεγμένη τοποθεσία.

    Για παράδειγμα, επιλέγετε το **Redmond (Η.Π.Α.)** ως τοποθεσία. Το ημερήσιο επίδομα για τη συγκεκριμένη τοποθεσία είναι 150 δολάρια ΗΠΑ (150 δολάρια ΗΠΑ) για διαμονή, USD 75 για διατροφή και USD 5 για περιστασιακά έξοδα. Η ημερομηνία έναρξης είναι η 10 Ιανουαρίου και η ημερομηνία λήξης είναι η 14 Ιανουαρίου. Επομένως, η επιλεγμένη διάρκεια είναι πέντε ημέρες όταν η επιλεγμένη ρύθμιση παραμέτρων είναι ημέρες ημερολογίου με ώρα και η επιλεγμένη ώρα ξεκινά και λήγει στις 12:00 π.μ. κατά τις ημερομηνίες έναρξης και λήξης. Ακολουθούν οι υπολογισμοί:

    - Συνολικό πληρωτέο ποσό = 5 × (150 + 75 + 5) = 5 × 230 = USD 1.150
    - Τμήμα διατροφής και περιστασιακών εξόδων του συνολικού ποσού = 5 × (75 + 5) = USD 400

Σε περίπτωση που κατά τη διάρκεια του ταξιδιού παρέχονταν πρωινό, μεσημεριανό και δείπνο, αυτά τα στοιχεία πρέπει να δικαιολογηθούν ως μείωση διατροφής.

### <a name="example-1-per-diem-where-meal-reductions-are-based-on-meal-type-per-trip"></a>Παράδειγμα 1: Ημερήσια αποζημίωση όπου οι μειώσεις διατρφοής βασίζονται στον τύπο διατροφής ανά ταξίδι

Σε αυτό το παράδειγμα, η μείωση διατροφής είναι 30% για το πρωινό, 30% για το μεσημεριανό και 40% για το δείπνο. Στη σελίδα **Παράμετροι διαχείρισης δαπανών**, το πεδίο **Υπολογισμός μείωσης διατροφής κατά** ορίζεται σε **Τύπος διατροφής ανά ταξίδι**. Ακολουθούν οι υπολογισμοί σε περίπτωση που παρέχονται τρία πρωϊνά, δύο μεσημεριανά γεύματα και κανένα γεύμα στον εργαζόμενο:

- Μείωση διατροφής = (3 × \[75 × 30%\]) + (2 × \[75 × 30%\]) + 0 = (3 × 22,50) + (2 × 22,50) + 0 = 67,50 + 45 + 0 = USD 112,50
- Γεύματα και περιστασιακά έξοδα = 400 – 112,50 = USD 287,50
- Συνολικό ποσό πληρωτέο = Συνολικό επίδομα – Μείωση διατροφής = 1.150 – 112,50 = USD 1.037,50

![Τα ημερήσια έξοδα όπου η μείωση διατροφής βασίζενται στον τύπο διατροφής ανά ταξίδι.](media/1-meal-type-per-trip.png)

### <a name="example-2-per-diem-where-meal-reductions-are-based-on-meal-type-per-day"></a>Παράδειγμα 2: Ημερήσια αποζημίωση όπου οι μειώσεις διατρφοής βασίζονται στον τύπο διατροφής ανά ημέρα

Σε αυτό το παράδειγμα, η μείωση διατροφής είναι 30% για το πρωινό, 30% για το μεσημεριανό και 40% για το δείπνο. Στη σελίδα **Παράμετροι διαχείρισης δαπανών**, το πεδίο **Υπολογισμός μείωσης διατροφής κατά** ορίζεται σε **Τύπος διατροφής ανά ημέρα**. Σε αυτήν την περίπτωση, στο πλέγμα **Γεύματα** στο στο παράθυρο διαλόγου **Επεξεργασία δαπανών**, απαλείψτε τα πλαίσια ελέγχου για να υποδείξετε ποια γεύματα σας παρασχέθηκαν κατά τη διάρκεια του ταξιδιού σας.

Για παράδειγμα, ακολουθούν οι υπολογισμοί εάν για τις πρώτες τρεις ημέρες του ταξιδιού παρασχέθηκε πρωινό:

- Μείωση καθημερινής διατροφής για καθεμία από τις πρώτες τρεις ημέρες = 75 × 30% = USD 22,50
- Συνολική μείωση της τιμής = 3 × 22,50 = USD 67,50
- Διατροφή και περιστασιακά έξοδα για τις ημέρες 1 έως 3 = 75 – 22,50 = USD 57,50
- Συνολικός αριθμός διατροφής και περιστασιακών εξόδων = Άθροισμα της διατροφής και των περιστασιακών εξόδων σε πέντε ημέρες = 400 – 67,50 = USD 332,50
- Συνολικό ποσό πληρωτέο = Συνολικό ποσό – Μείωση διατροφής = 1.150 – 67,50 = USD 1.082,50

![Τα ημερήσια έξοδα όπου η μείωση διατροφής βασίζενται στον τύπο διατροφής ανά ημέρα.](media/2-meal-type-per-day.png)

### <a name="example-3-per-diem-where-meal-reductions-are-based-on-number-of-meals-per-day"></a>Παράδειγμα 3: Ημερήσια αποζημίωση όπου οι μειώσεις διατρφοής βασίζονται στον αριθμό των γευμάτων ανά ημέρα

Σε αυτό το παράδειγμα, η μείωση της διατροφής υπολογίζεται με βάση τον αριθμό των γευμάτων που παρασχέθηκαν ανά ημέρα (δηλαδή, το πεδίο **Υπολογισμός μείωσης διατροφής κατά** στη σελίδα **Παράμετροι διαχείρισης εξόδων** έχει οριστεί σε **Αριθμό γευμάτων ανα ημέρα**). Στο πλέγμα **Γεύματα** στο στο παράθυρο διαλόγου **Επεξεργασία δαπανών**, απαλείψτε τα πλαίσια ελέγχου για να υποδείξετε ποια γεύματα σας παρασχέθηκαν.
Σε αυτή την περίπτωση, η μείωση της διατρφοής βασίζεται μόνο στην # παρεχόμενων γευμάτων και όχι στον τύπο του γεύματος (πρωϊνό/μεσημεριανό/βραδινό).

Ακολουθούν οι υπολογισμοί για ημερήσιες αποζημιώσεις όταν το καθημερινό επίδομα είναι USD 150 για διαμονή, USD 75 για διατροφή και USD 5 για περιστασιακά έξοδα:

- **Συνολικό πληρωτέο ποσό** = 5 × (150 + 75 + 5) = 5 × 230 = USD 1.150
- **Ένα γεύμα:** Μείωση διατροφής = 20% = USD 15
- **Δύο γεύματα:** Μείωση διατροφής = 50% = USD 37,50
- **Τρία γεύματα:** Μείωση διατροφής = 100% = USD 75

Ακολουθούν οι υπολογισμοί για το **επίδομα διατροφής και περιστασιακά έξοδα**, που περιλαμβάνει USD 5 για περιστασιακά έξοδα:

- Ημέρα 1 - Παρέχονται δύο γεύματα = (75 – 37,50) + 5 = 37,50 + 5 = USD 42,50
- Ημέρα 2 - Παρέχονται δύο γεύματα = (75 – 37,50) + 5 = 37,50 + 5 = USD 42,50
- Ημέρα 3 - Παρέχεται ένα γεύμα = (75 – 15) + 5 = 60 + 5 = USD 65
- Ημέρα 4 - Δεν παρέχεται κανένα γεύμα = (75 – 0) + 5 = 75 + 5 = USD 80
- Ημέρα 5 - Παρέχονται τρία γεύματα = (75 – 75) + 5 = 0 + 5 = USD 5

- Συνολικά γεύματα και περιστασιακά γεύματα = Γεύματα και περιστασιακά γεύματα για την Ημέρα 1+ Ημέρα 2 +Ημέρα 3+Ημέρα 4+ Ημέρα 5 = USD 235
- Συνολική μείωση διατροφής = Μείωση διατροφής για την Ημέρα 1+ Ημέρα 2 +Ημέρα 3+Ημέρα 4+ Ημέρα 5= 37,5+ 37,5+ 15 + 0+ 75 = USD 165
- Συνολικό ποσό πληρωτέο = Συνολικό επίδομα – Συνολή μείωση διατροφής = USD 1.150 – USD 165 = USD 985

![Τα ημερήσια έξοδα όπου η μείωση διατροφής βασίζενται στον αριθμό γευμάτων ανά ημέρα.](media/3-number-of-meals-per-day.png)

> [!NOTE]
> Από την έκδοση Finance 10.0.23, εάν χρησιμοποιείτε το νέο περιβάλλον εργασίας δαπανών, δεν μπορείτε να δημιουργήσετε ημερήσιες δαπάνες με επικαλυπτόμενες ημερομηνίες. Εάν το επιχειρήσετε, θα εμφανιστεί ένα μήνυμα σφάλματος.