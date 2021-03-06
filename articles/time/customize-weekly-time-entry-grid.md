---
title: Επέκταση χρονικών καταχωρήσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο με τον οποίο οι προγραμματιστές έχουν τη δυνατότητα επέκτασης του στοιχείου ελέγχου καταχώρησης ώρας.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 93f411ad7c86beefcc35e7799a03987dacdcd62b
ms.sourcegitcommit: 5a29adce48133e09f051929e8544d6c2c93c025d
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/02/2020
ms.locfileid: "3930880"
---
# <a name="extending-time-entries"></a>Επέκταση χρονικών καταχωρήσεων

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Το Dynamics 365 Project Operations περιλαμβάνει ένα προσαρμοσμένο στοιχείο ελέγχου καταχώρησης χρόνου με δυνατότητα επέκτασης. Αυτό το στοιχείο ελέγχου περιλαμβάνει τις εξής δυνατότητες:

- Εισαγωγή ώρας οριζόντια κατά τη διάρκεια μιας εβδομάδας
- Σύνολα ανά ημέρα, γραμμή ή εβδομάδα
- Αντιγραφή γραμμών ή εβδομάδων
- Καταχώρηση ώρας ως ΩΩ: λλ ή ΩΩ. λλ (μετατρέπεται αυτόματα σε ΩΩ. ΩΩ)
- Εισαγωγή από αναθέσεις, κρατήσεις ή συναντήσεις

Η επέκταση καταχωρήσεων χρόνου είναι δυνατή σε δύο περιοχές:
- [Προσθήκη καταχωρήσεων προσαρμοσμένου χρόνου για δική σας χρήση](#add)
- [Προσαρμογή του στοιχείου ελέγχου εβδομαδιαίας χρονικής καταχώρησης](#customize)

## <a name="add-custom-time-entries-for-your-own-use"></a>Π<a name="add"></a>Προσθήκη καταχωρήσεων προσαρμοσμένου χρόνου για δική σας χρήση.

Οι καταχωρήσεις χρόνου είναι μια βασική οντότητα που έχει σχεδιαστεί για χρήση σε πολλαπλά σενάρια. Στο Κύμα 1 Απριλίου 2020, παρουσιάστηκε η βασική λύση TESA η οποία παρέχει μια οντότητα **Ρύθμιση** και έναν νέο ρόλο ασφαλείας **Χρήστης χρονικής καταχώρησης**. Συμπεριλήφθηκαν επίσης τα νέα πεδία, **msdyn_start** και **msdyn_end** τα οποία έχουν άμεση σχέση με το **msdyn_duration**. Η νέα οντότητα, ρόλος ασφαλείας και τα πεδία επιτρέπουν μια πιο ενοποιημένη προσέγγιση του χρόνου σε πολλαπλά προϊόντα.


### <a name="time-source-entity"></a>Οντότητα προέλευσης χρόνου
| Πεδίο | Περιγραφή | 
|-------|------------|
| Ονομασία  | Το όνομα της καταχώρησης του χρόνου προέλευσης που χρησιμοποιείται ως τιμή επιλογής κατά τη δημιουργία της καταχώρησης του χρόνου. |
| Προεπιλεγμένη προέλευση ώρας [προέλευση χρόνου: isdefault] | Από προεπιλογή, μόνο μία προέλευση χρόνου μπορεί να είναι σημειωμένη στην προεπιλεγμένη προέλευση ώρας. Αυτή η δυνατότητα επιτρέπει την εισαγωγή καταχωρήσεων σε προεπιλεγμένη προέλευση χρόνου, εάν δεν έχει καθοριστεί κάποιο. |
|Τύπος προέλευσης ώρας [προέλευση ώρας: sourcetype] | Ο τύπος προέλευσης είναι μια επιλογή (τύπος προέλευσης καταχώρησης χρόνου) που επιτρέπει τη συσχέτιση της προέλευσης ώρας με μια εφαρμογή. Πρόσθετες τιμές θα προστεθούν σε αυτό το σύνολο επιλογών καθώς προστίθενται πρόσθετες εφαρμογές. Λάβετε υπόψη ότι η Microsoft δεσμεύει τιμές μεγαλύτερες από 190.000.000.|


### <a name="time-entries-and-the-time-source-entity"></a>Καταχωρήσεις χρόνου και η οντότητα προέλευσης χρόνου
Κάθε φορά που η καταχώρηση συσχετίζεται με μια καρτέλα προέλευσης χρόνου. Αυτή η καρτέλα προσδιορίζει τον τρόπο και τις εφαρμογές που θα πρέπει να επεξεργαστούν την καταχώρηση του χρόνου.

Οι καταχωρήσεις χρόνου είναι πάντα ένα συνεχόμενο σύνολο χρόνου με έναρξη, λήξη και διάρκεια.

Η λογική θα ενημερώσει αυτόματα την καρτέλα της καταχώρησης χρόνου στις παρακάτω περιπτώσεις:

- Εάν παρέχονται δύο από τα τρία παρακάτω πεδία, το τρίτο υπολογίζεται αυτόματα 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- Τα πεδία **msdyn_start** και **msdyn_end** είναι ενημερωμένα από τη ζώνη ώρας.
- Οι καταχωρήσεις ώρας που δημιουργούνται με μόνο **msdyn_date** και **msdyn_duration** που καθορίζονται θα ξεκινούν τα μεσάνυχτα και τα **msdyn_start** και **msdyn_end** θα ενημερωθούν ανάλογα.

#### <a name="time-entry-types"></a>Τύποι χρονικής καταχώρησης

Οι καρτέλες καταχώρησης χρόνου έχουν έναν συσχετισμένο τύπο που καθορίζει τη συμπεριφορά στη ροή υποβολής για τη συσχετισμένη εφαρμογή.

|Ετικέτα | Τιμή|
|-----|-----|
|Σε διάλειμμα   |192,355,000|
|Ταξίδια | 192,355,001|
|Υπερωρία   | 192,354,320|
|Εργασία   | 192,350,000|
|Απουσία    | 192,350,001|
|Διακοπές   | 192,350,002|



## <a name="customize-the-weekly-time-entry-control"></a><a name="customize"></a>Προσαρμογή του στοιχείου ελέγχου εβδομαδιαίας χρονικής καταχώρησης
Οι προγραμματιστές μπορούν να προσθέσουν επιπλέον πεδία και αναζητήσεις σε άλλες οντότητες και να εφαρμόσουν προσαρμοσμένους επιχειρηματικούς κανόνες για την υποστήριξη των επιχειρηματικών τους σεναρίων.

### <a name="add-custom-fields-with-lookups-to-other-entities"></a>Προσθήκη προσαρμοσμένων πεδίων που έχουν αναζητήσεις σε άλλες οντότητες
Υπάρχουν τρία βασικά βήματα για την προσθήκη ενός προσαρμοσμένου πεδίου στο πλέγμα εβδομαδιαίας καταχώρησης ώρας.

- Προσθέστε το προσαρμοσμένο πεδίο στο παράθυρο διαλόγου "γρήγορη δημιουργία".
- Ρυθμίστε τις παραμέτρους του πλέγματος για εμφάνιση του προσαρμοσμένου πεδίου.
- Προσθέστε το προσαρμοσμένο πεδίο είτε στη ροή εργασιών επεξεργασίας γραμμής ή στη ροή εργασιών επεξεργασίας κελιού.

Πρέπει επίσης να βεβαιωθείτε ότι το νέο πεδίο έχει τις απαιτούμενες επικυρώσεις στη ροή εργασιών επεξεργασίας κελιού ή γραμμής. Στο πλαίσιο αυτού του βήματος, θα πρέπει να κλειδώσετε το πεδίο, με βάση την κατάσταση της καταχώρησης του χρόνου.

#### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Προσθέστε το προσαρμοσμένο πεδίο στο παράθυρο διαλόγου "γρήγορη δημιουργία"
Πρέπει να προσθέσετε το προσαρμοσμένο πεδίο στο παράθυρο διαλόγου **Γρήγορη δημιουργία χρονικής καταχώρισης**. Στη συνέχεια, οι χρήστες μπορούν να εισαγάγουν μια τιμή όταν προσθέτουν καταχωρήσεις χρόνου επιλέγοντας **Δημιουργία**.

#### <a name="configure-the-grid-to-show-the-custom-field"></a>Ρυθμίστε τις παραμέτρους του πλέγματος για εμφάνιση του προσαρμοσμένου πεδίου
Υπάρχουν δύο τρόποι για την προσθήκη ενός προσαρμοσμένου πεδίου στο πλέγμα εβδομαδιαίας καταχώρησης ώρας:

  - Προσαρμογή προβολής και προσθήκη προσαρμοσμένου πεδίου
  - Δημιουργία νέας προεπιλεγμένης χρονικής καταχώρησης 


**Προσαρμογή προβολής και προσθήκη προσαρμοσμένου πεδίου**

Μπορείτε να προσαρμόσετε την προβολή **Οι εβδομαδιαίες χρονικές καταχωρήσεις μου** και να προσθέσετε το προσαρμοσμένο πεδίο. Μπορείτε να επιλέξετε τη θέση και το μέγεθος του προσαρμοσμένου πεδίου στο πλέγμα κάνοντας επεξεργασία αυτών των ιδιοτήτων στην προβολή.

**Δημιουργία νέας προεπιλεγμένης χρονικής καταχώρησης** 

Αυτή η προβολή θα πρέπει να έχει πεδία **Περιγραφή** και **Εξωτερικά σχόλια** εκτός από τις στήλες που θέλετε να έχετε στο πλέγμα. 

1. Επιλέξτε τη θέση το μέγεθος και την προεπιλεγμένη σειρά ταξινόμησης του πλέγματος κάνοντας επεξεργασία αυτών των ιδιοτήτων στην προβολή. 
2. Ρυθμίστε τις παραμέτρους του προσαρμοσμένου στοιχείου ελέγχου για αυτήν την προβολή ώστε να είναι στοιχείο ελέγχου **Πλέγμα χρονικής καταχώρισης**. 
3. Προσθέστε αυτό το στοιχείο ελέγχου στην προβολή και επιλέξτε το για περιεχόμενο Web, τηλέφωνο και tablet. 
4. Ρυθμίστε τις παραμέτρους για το πλέγμα εβδομαδιαίων καταχωρήσεων χρόνου. Ορίστε το πεδίο **Ημερομηνία έναρξης** σε **msdyn_date**, ορίστε το πεδίο **Διάρκεια** σε **msdyn_duration** και ορίστε το πεδίο **Κατάσταση** σε **msdyn_entrystatus**. 
5. Για την προεπιλεγμένη προβολή, το πεδίο **Λίστα κατάστασης μόνο για ανάγνωση** έχει οριστεί σε **192350002,192350003,192350004**, το πεδίο **Ροή εργασίας επεξεργασίας σειράς** έχει οριστεί σε **msdyn_timeentryrowedit** και το πεδίο **Ροή εργασίας επεξεργασίας κελιού** έχει οριστεί σε **msdyn_timeentryedit**. 
6. Μπορείτε να προσαρμόσετε αυτά τα πεδία για την προσθήκη ή την κατάργηση κατάστασης μόνο για ανάγνωση ή για τη χρήση μιας διαφορετικής εμπειρίας βάσει εργασιών (TBX) για επεξεργασία γραμμής ή κελιού. Αυτά τα πεδία θα πρέπει να συνδεθούν σε μια στατική τιμή.


> [!NOTE] 
> Και οι δύο επιλογές θα αφαιρέσουν ένα έτοιμο φίλτρο στις οντότητες **Έργο** και **Εργασία έργου** έτσι ώστε να είναι ορατές όλες οι προβολές αναζήτησης για τις οντότητες. Εμφανίζονται μόνο οι σχετικές προβολές αναζήτησης.
Πρέπει να καθορίσετε την κατάλληλη ροή εργασιών για το προσαρμοσμένο πεδίο. Το πιο πιθανό είναι ότι, εάν προσθέσατε το πεδίο στο πλέγμα, θα πρέπει να μεταβείτε στη ροή εργασιών επεξεργασίας γραμμής που χρησιμοποιείται για πεδία που εφαρμόζονται σε όλες τις καταχωρήσεις χρονικής γραμμής. Εάν το προσαρμοσμένο πεδίο έχει μια μοναδική τιμή κάθε μέρα, όπως ένα προσαρμοσμένο πεδίο για την **Ώρα λήξης**λήξης, θα πρέπει να μεταβείτε στη ροή εργασιών επεξεργασίας κελιού.

Για να προσθέσετε το προσαρμοσμένο πεδίο σε μια ροή εργασιών, σύρετε ένα στοιχείο **Πεδίο** στην κατάλληλη θέση στη σελίδα και, στη συνέχεια, ορίστε τις ιδιότητές του. Ορίστε την ιδιότητα **Προέλευση** σε **Χρονική καταχώρηση** και ορίστε την ιδιότητα **Πεδίο δεδομένων** στο προσαρμοσμένο πεδίο. Η ιδιότητα **Πεδίο** καθορίζει τις εμφανιζόμενο όνομα στη σελίδα TBX. Επιλέξτε **Εφαρμογή** για να αποθηκεύσετε τις αλλαγές σας στο πεδίο και, στη συνέχεια, επιλέξτε **Ενημέρωση** για να αποθηκεύσετε τις αλλαγές σας στη σελίδα.

Για να χρησιμοποιήσετε μια νέα προσαρμοσμένη σελίδα TBX αντί για αυτό, δημιουργήστε μια νέα διεργασία. Ορίστε την κατηγορία σε **Ροή επιχειρηματικής διαδικασίας**, ορίστε την οντότητα σε **Χρονική καταχώριση** και ορίστε τον τύπο επιχειρηματικής διαδικασίας σε **Εκτέλεση διαδικασίας ως ροή εργασιών**. Στις **Ιδιότητες** η ιδιότητα **Όνομα σελίδας** πρέπει να οριστεί σε εμφανιζόμενο όνομα για τη σελίδα. Προσθέστε όλα τα σχετικά πεδία στη σελίδα TBX. Αποθηκεύστε και ενεργοποιήστε τη διεργασία και, στη συνέχεια, ενημερώστε την ιδιότητα προσαρμοσμένου στοιχείου ελέγχου για τη σχετική ροή εργασιών στην τιμή **Όνομα** της διεργασίας.

### <a name="add-new-option-set-values"></a>Προσθήκη νέων τιμών συνόλου επιλογών
Για να προσθέσετε τιμές συνόλου επιλογών σε ένα έτοιμο πεδίο, ανοίξτε τη σελίδα επεξεργασίας για το πεδίο και, στη συνέχεια, στην περιοχή **Τύπος**, επιλέξτε **Επεξεργασία** δίπλα στο σύνολο επιλογών. Στη συνέχεια, προσθέστε μια νέα επιλογή που έχει μια προσαρμοσμένη ετικέτα και ένα χρώμα. Εάν θέλετε να προσθέσετε μια νέα κατάσταση χρονικής καταχώρισης, το έτοιμο πεδίο ονομάζεται **Κατάσταση καταχώρισης** όχι **Κατάσταση**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Ορισμός μιας νέας κατάστασης καταχώρησης ώρας ως "μόνο για ανάγνωση"
Για να ορίσετε μια νέα κατάσταση καταχώρησης ώρας ως "μόνο για ανάγνωση", προσθέστε τη νέα τιμή καταχώρησης ώρας στην ιδιότητα **Λίστα κατάστασης μόνο για ανάγνωση**. Το επεξεργάσιμο τμήμα του πλέγματος καταχωρήσεων ώρας θα κλειδωθεί για γραμμές με τη νέα κατάσταση.
Στη συνέχεια, προσθέστε επιχειρηματικούς κανόνες για να κλειδώσετε όλα τα πεδία στις σελίδες TBX **Επεξεργασία σειράς χρονικής καταχώρησης** και **Επεξεργασία χρονικής καταχώρησης**. Μπορείτε να αποκτήσετε πρόσβαση στους επιχειρηματικούς κανόνες για αυτές τις σελίδες ανοίγοντας το πρόγραμμα επεξεργασίας ροή επιχειρηματικής διαδικασίας για τη σελίδα και στη συνέχεια επιλέγοντας **Επιχειρηματικοί κανόνες**. Μπορείτε να προσθέσετε τη νέα κατάσταση στη συνθήκη στους υπάρχοντες επιχειρηματικούς κανόνες ή μπορείτε να προσθέσετε έναν νέο επιχειρηματικό κανόνα για τη νέα κατάσταση.

### <a name="add-custom-validation-rules"></a>Προσθήκη προσαρμοσμένων κανόνων επικύρωσης
Υπάρχουν δύο τύποι κανόνων επικύρωσης, τους οποίους μπορείτε να προσθέσετε για την εμπειρία του πλέγματος εβδομαδιαίας καταχώρησης χρόνου:

- Επιχειρηματικοί κανόνες από την πλευρά του πελάτη που λειτουργούν σε παράθυρα διαλόγου γρήγορης δημιουργίας και σε TBX σελίδες.
- Επικυρώσεις για την προσθήκη στην πλευρά του διακομιστή που εφαρμόζονται σε όλες τις ενημερώσεις καταχώρησης ώρας.

#### <a name="business-rules"></a>Επιχειρησιακοί κανόνες
Χρησιμοποιήστε τους επιχειρηματικούς κανόνες για να κλειδώνετε και να ξεκλειδώνετε πεδία, να καταχωρείτε προεπιλεγμένες τιμές στα πεδία και να καθορίζετε επικυρώσεις που απαιτούν πληροφορίες μόνο από την καρτέλα τρέχουσας καταχώρησης ώρας. Μπορείτε να αποκτήσετε πρόσβαση στους επιχειρηματικούς κανόνες για μια σελίδα TBX ανοίγοντας το πρόγραμμα επεξεργασίας ροή επιχειρηματικής διαδικασίας για τη σελίδα και στη συνέχεια επιλέγοντας **Επιχειρηματικοί κανόνες**. Στη συνέχεια, μπορείτε να επεξεργαστείτε τους υπάρχοντες επιχειρηματικούς κανόνες ή να προσθέσετε έναν νέο επιχειρηματικό κανόνα. Για ακόμα πιο προσαρμοσμένες επικυρώσεις, μπορείτε να χρησιμοποιήσετε έναν επιχειρηματικό κανόνα για την εκτέλεση της JavaScript.

#### <a name="plug-in-validations"></a>Επικυρώσεις προσθηκών
Θα πρέπει να χρησιμοποιήσετε τις επικυρώσεις προσθηκών για οποιεσδήποτε επικυρώσεις που απαιτούν περισσότερο περιβάλλον από ό,τι είναι διαθέσιμο σε μία καρτέλα καταχώρησης χρόνου ή για τυχόν επικυρώσεις που θέλετε να εκτελεστούν σε ενσωματωμένες ενημερώσεις στο πλέγμα. Για να ολοκληρώσετε την επικύρωση, δημιουργήστε μια προσαρμοσμένη προσθήκη σχετικά με την οντότητα **Χρονική καταχώριση**.
