---
title: Προσθήκη απαιτούμενων προσαρμοσμένων πεδίων για ρύθμιση τιμών και οντότητες συναλλαγών
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το πώς μπορείτε να προσθέσετε απαιτούμενες αναφορές προσαρμοσμένων πεδίων σε οντότητες και σε φόρμες και προβολές.
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
ms.openlocfilehash: a27bfe881fdb6431941fa860d279e3e7b526f623
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898306"
---
# <a name="add-required-custom-fields-to-price-setup-and-transactional-entities"></a>Προσθήκη απαιτούμενων προσαρμοσμένων πεδίων για ρύθμιση τιμών και οντότητες συναλλαγών

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Αυτό το θέμα υποθέτει ότι έχετε ολοκληρώσει τις διαδικασίες στο θέμα, [Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων που θα χρησιμοποιηθούν ως διαστάσεις τιμολόγησης](create-custom-fields-entities-pricing-dimensions.md). Εάν δεν έχετε ολοκληρώσει αυτές τις διαδικασίες, επιστρέψτε και ολοκληρώστε τις και, στη συνέχεια, επιστρέψτε σε αυτό το θέμα. 

Σε αυτό το θέμα, οι διαδικασίες θα σας δείξουν πώς να προσθέσετε τις απαιτούμενες αναφορές προσαρμοσμένων πεδίων σε οντότητες και στα στοιχεία περιβάλλοντος εργασίας χρήστη (UI), όπως φόρμες και προβολές.

## <a name="add-custom-pricing-dimension-fields"></a>Προσθήκη προσαρμοσμένων πεδίων διαστάσεων τιμολόγησης 
Αφού δημιουργηθούν τα προσαρμοσμένα πεδία και οι οντότητες, το επόμενο βήμα είναι να ενημερωθεί η ρύθμιση τιμών και οι οντότητες συναλλαγών σχετικά με τυχόν προσαρμοσμένες οντότητες ή σύνολα επιλογών με τη δημιουργία πεδίων αναφοράς. Ανάλογα με το αν η λίστα με τις διαστάσεις τιμολόγησης περιλαμβάνει διαστάσεις συνόλου επιλογών ή διαστάσεις οντότητας ή και τα δύο, ακολουθήστε μόνο τα βήματα στις **Προσαρμοσμένες διαστάσεις τιμολόγησης βάσει συνόλου επιλογών** ή **Προσαρμοσμένες διαστάσεις τιμολόγησης βάσει οντότητας** ή και τα δύο αντίστοιχα.

### <a name="option-set-based-custom-pricing-dimensions"></a>Προσαρμοσμένες διαστάσεις τιμολόγησης βάσει συνόλου επιλογών
Όταν μια προσαρμοσμένη διάσταση τιμολόγησης είναι βασισμένη στο σύνολο επιλογών, προσθέστε την ως πεδίο σε βασικές οντότητες. Στην παρακάτω διαδικασία, τα στοιχεία **Τοποθεσία εργασίας πόρου** και **Ώρες εργασίας πόρου** χρησιμοποιούνται ως διαστάσεις τιμολόγησης βάσει συνόλου επιλογών. Πρέπει πρώτα να προστεθούν ως πεδία στις οντότητες τιμολόγησης, **Τιμή ρόλου** και **Αύξηση τιμής ρόλου**.

1. Στις λειτουργίες έργου, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**. 
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Τιμή ρόλου**.
3. Αναπτύξτε την οντότητα **Τιμή ρόλου** και επιλέξτε **Πεδία**.
4. Επιλέξτε **Δημιουργία** για να δημιουργήσετε ένα νέο πεδίο με το όνομα **Τοποθεσία εργασίας πόρου** και επιλέξτε **Σύνολο επιλογών** ως τύπο πεδίου. 
5. Επιλέξτε **Χρήση υπάρχοντος συνόλου επιλογών**, επιλέξτε το σύνολο επιλογών **Τοποθεσία εργασίας πόρου** και μετά επιλέξτε **Αποθήκευση**.
6. Επαναλάβετε τα βήματα 1-5 για να προσθέσετε αυτό το πεδίο στην οντότητα **Αύξηση τιμής ρόλου**. 
7. Επαναλάβετε τα βήματα 1-5 για το σύνολο επιλογών **Ώρες εργασίας πόρου**.

> [!IMPORTANT]
> Όταν προσθέτετε ένα πεδίο σε περισσότερες από μία οντότητες, χρησιμοποιήστε το ίδιο όνομα πεδίου σε όλες τις οντότητες. 

Στις φάσεις πωλήσεων και εκτίμησης για ένα έργο, οι εκτιμήσεις της προσπάθειας εργασίας που απαιτείται για την ολοκλήρωση της εργασίας **Τοπική** και **Επιτόπια** στις **Κανονικές ώρες** και τις **Υπερωρίες** χρησιμοποιούνται για να υπολογίστε την τιμή της προσφοράς/έργου. Τα πεδία **Τοποθεσία εργασίας πόρου** και **Ώρες εργασίας πόρου** θα προστεθούν στις οντότητες εκτίμησης **Λεπτομέρεια γραμμής προσφοράς**, **Λεπτομέρεια γραμμής σύμβασης**, **Μέλος ομάδας έργου** και **Γραμμή εκτίμησης**.

1. Στις λειτουργίες έργου, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**. 
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Λεπτομέρεια γραμμής σύμβασης**.
3. Αναπτύξτε την οντότητα **Λεπτομέρεια γραμμής προσφοράς** και επιλέξτε **Πεδία**.
4. Επιλέξτε **Δημιουργία** για να δημιουργήσετε ένα νέο πεδίο με το όνομα **Τοποθεσία εργασίας πόρου** και επιλέξτε τύπο πεδίου το **Σύνολο επιλογών**. 
5. Επιλέξτε **Χρήση υπάρχοντος συνόλου επιλογών**, και **Τοποθεσία εργασίας πόρου** και μετά επιλέξτε **Αποθήκευση**.
6. Επαναλάβετε τα βήματα 1-5 για να προσθέσετε αυτό το πεδίο στις οντότητες **Λεπτομέρεια γραμμής σύμβασης έργου**, **Μέλος ομάδας έργου,** και **Γραμμή εκτίμησης**.
7. Επαναλάβετε τα βήματα 1-6 για το σύνολο επιλογών **Ώρες εργασίας πόρου**. 

Για παράδοση και τιμολόγηση, οι ολοκληρωμένες εργασίες πρέπει να τιμολογούνται με ακρίβεια, προκειμένου να επιλέξουν εάν είναι **Τοπική** ή **Επιτόπου**και εάν ολοκληρώθηκαν κατά τις **Κανονικές ώρες** ή τις **Υπερωρίες** στις πραγματικές τιμές του έργου. Τα πεδία **Τοποθεσία εργασίας πόρου** και **Ώρες εργασίας πόρου** θα πρέπει να προστεθούν στις οντότητες **Χρονική καταχώριση**, **Πραγματικές τιμές**, **Λεπτομέρεια γραμμής τιμολογίου** και **Γραμμή ημερολογίου**.

1. Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Χρονική καταχώριση**.
3. Αναπτύξτε την οντότητα **Λεπτομέρεια γραμμής προσφοράς** και επιλέξτε **Πεδία**.
4. Επιλέξτε **Δημιουργία** για να δημιουργήσετε ένα νέο πεδίο με το όνομα **Τοποθεσία εργασίας πόρου** και επιλέξτε **Σύνολο επιλογών** ως τύπο πεδίου. 
5. Επιλέξτε **Χρήση υπάρχοντος συνόλου επιλογών**, επιλέξτε το σύνολο επιλογών **Τοποθεσία εργασίας πόρου** και μετά επιλέξτε **Αποθήκευση**.
6. Επαναλάβετε τα βήματα 1-5 για να προσθέσετε αυτό το πεδίο στις οντότητες **Πραγματικές τιμές**, **Λεπτομέρεια γραμμής τιμολογίου** και **Γραμμή ημερολογίου**.
7. Επαναλάβετε τα βήματα 1-6 για το σύνολο επιλογών **Ώρες εργασίας πόρου**. 

Με αυτήν την ενέργεια ολοκληρώνονται οι αλλαγές σχήματος που απαιτούνται για τις προσαρμοσμένες διαστάσεις που βασίζονται στο σύνολο επιλογών.

## <a name="entity-based-custom-pricing-dimensions"></a>Προσαρμοσμένες διαστάσεις τιμολόγησης βάσει οντοτήτων

Όταν η προσαρμοσμένη διάσταση τιμολόγησης είναι μια οντότητα, θα προσθέσετε 1: N σχέσεις μεταξύ της οντότητας διάστασης και των κύριων οντοτήτων. Χρησιμοποιώντας το παράδειγμα του τυπικού τίτλου από τα ανωτέρω, είναι λογικό να αναμένετε ότι κάθε εργαζόμενος έχει αντιστοιχιστεί σε έναν τυπικό τίτλο. Ως εκ τούτου, θα χρειαστείτε μια σχέση 1: N από τον τυπικό τίτλο έως τον πόρο με δυνατότητα κράτησης ή μια σχέση N:1 εάν δημιουργήθηκε από έναν πόρο με δυνατότητα κράτησης σε έναν τυπικό τίτλο.

1. Στις λειτουργίες έργου, επιλέξτε **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**. 
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Τυπικός τίτλος**.
3. Αναπτύξτε την οντότητα **Τυπικός τίτλος** και επιλέξτε **Σχέσεις 1:N**.
4. Επιλέξτε **Δημιουργία** για να δημιουργήσετε μια νέα σχέση 1:Ν με το όνομα **Τυπικός τίτλος σε πόρο με δυνατότητα κράτησης**. Πληκτρολογήστε τις απαιτούμενες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.

Επίσης, θα πρέπει να προστεθεί ο τυπικός τίτλος στις οντότητες τιμολόγησης **Τιμή ρόλου** και **Αύξηση τιμή ρόλου**. Αυτό ολοκληρώνεται επίσης με τη χρήση σχέσεων 1:N μεταξύ των οντοτήτων **Τυπικός τίτλος** και **Τιμή ρόλου** και **Τυπικός τίτλος** και **Αύξηση τιμής ρόλου**.

1. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Τυπικός τίτλος**.
2. Αναπτύξτε την οντότητα **Τυπικός τίτλος** και επιλέξτε **Σχέσεις 1:N**.
3. Επιλέξτε **Δημιουργία** για να δημιουργήσετε μια νέα σχέση 1:Ν με το όνομα **Τυπικός τίτλος σε τιμή ρόλου**. Πληκτρολογήστε τις απαιτούμενες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.
4. Επαναλάβετε τα βήματα 1-4 για να δημιουργήσετε 1:N σχέσεις μεταξύ των οντοτήτων **Τυπικός τίτλος** και **Αύξηση τιμής ρόλου**.

Στις φάσεις πωλήσεων και εκτίμησης για το έργο, για την τιμή της προσφοράς/έργου, απαιτούνται εκτιμήσεις της προσπάθειας εργασίας για κάθε τυπικό τίτλο. Αυτό σημαίνει ότι 1:N σχέσεις από τον τυπικό τίτλο σε κάθε μία από αυτές τις οντότητες εκτίμησης είναι απαραίτητες: 

- **Λεπτομέρεια γραμμής προσφοράς**
- **Λεπτομέρεια γραμμής σύμβασης έργου**
- **Μέλος ομάδας έργου**
- **Γραμμή εκτίμησης**

5. Επαναλάβετε τα βήματα 1-5 για να δημιουργήσετε 1:N σχέσεις από τα στοιχεία **Τυπικός τίτλος** σε **Λεπτομέρεια γραμμής προσφοράς**, **Λεπτομέρεια γραμμής σύμβασης έργου**, **Μέλος ομάδας έργου** και **Γραμμή εκτίμησης**.

  Στις φάσεις παράδοσης και τιμολόγησης, η εργασία που ολοκληρώνεται από κάθε τυπικό τίτλο πρέπει να διατιμάται με ακρίβεια στις πραγματικές τιμές του έργου. Αυτό σημαίνει ότι πρέπει να υπάρχουν 1:N σχέσεις από οντότητες **Τυπικός τίτλος** σε **Χρονική καταχώριση**, **Πραγματικές τιμές**, **Λεπτομέρεια γραμμής τιμολογίου** και **Γραμμή ημερολογίου**.

6. Επαναλάβετε τα βήματα 1 - 6 για να δημιουργήσετε 1:N σχέσεις από οντότητες **Τυπικός τίτλος** σε **Χρονική καταχώριση**, **Πραγματικές τιμές**, **Λεπτομέρεια γραμμής τιμολογίου** και **Γραμμή ημερολογίου**.

### <a name="set-up-dimension-value-defaulting-using-the-mappings-features-of-the-platform"></a>Ορισμός προεπιλεγμένης τιμής διάστασης χρησιμοποιώντας τις δυνατότητες αντιστοίχισης της πλατφόρμας
Για τη χρονική καταχώριση, θα ήταν χρήσιμο το σύστημα να έχει τον προεπιλεγμένο τυπικό τίτλο κατά τη χρονική καταχώρηση από τον πόρο με δυνατότητα κράτησης που καταγράφει την καταχώρηση του χρόνου. Χρησιμοποιήστε τα παρακάτω βήματα για να προσθέσετε αντιστοιχίσεις πεδίων στη σχέση 1:N από **Πόρος με δυνατότητα κράτησης** σε **Χρονική καταχώριση**.

1. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες > Τυπικός τίτλος**.
2. Αναπτύξτε την οντότητα **Τυπικός τίτλος** και επιλέξτε **Σχέσεις 1:N**.
3. Κάντε διπλό κλικ στο στοιχείο **Πόρος με δυνατότητα κράτησης σε χρονική καταχώριση**. Στη σελίδα **Σχέση**, επιλέξτε **Χρήση αντιστοιχίσεων πεδίων**. 
4. Επιλέξτε **Δημιουργία** για να δημιουργήσετε μια νέα αντιστοίχιση πεδίου μεταξύ του πεδίου **Τυπικός τίτλος** στην οντότητα **Πόρος με δυνατότητα κράτησης** στο πεδίο αναφοράς **Τυπικός τίτλος** στην οντότητα **Χρονική καταχώριση**. 

Με αυτήν την ενέργεια ολοκληρώνονται οι αλλαγές σχήματος που απαιτούνται για τις προσαρμοσμένες διαστάσεις που βασίζονται σε οντότητα.

##  <a name="add-custom-fields-to-forms-views-and-business-rules"></a>Προσθήκη προσαρμοσμένων πεδίων σε φόρμες, προβολές και επιχειρηματικούς κανόνες

Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές σχήματος, το επόμενο βήμα είναι να καταστήσετε τα πεδία ορατά στο περιβάλλον εργασίας χρήστη προσθέτοντας τα πεδία στις φόρμες και τις προβολές.

1. Ανοίξτε τη φόρμα ή την προβολή. Στο δεξιό παράθυρο περιήγησης, επιλέξτε το πεδίο και σύρετέ το στον καμβά φόρμας. 
2. Εάν επεξεργάζεστε μια προβολή, χρησιμοποιήστε το δεξιό παράθυρο περιήγησης, επιλέξτε την επιλογή **Προσθήκη πεδίων** και στο παράθυρο διαλόγου **Λίστα πεδίων**, επιλέξτε τα πεδία που χρειάζεστε και επιλέξτε **ΟΚ**.

Ο παρακάτω πίνακας παρέχει μια αναλυτική λίστα με τις έτοιμες φόρμες και προβολές οι οποίες παρατίθενται ανά οντότητα και οι οποίες θα πρέπει να ενημερωθούν με τα νέα πεδία. Εάν υπάρχουν πρόσθετες προβολές ή φόρμες στις προσαρμογές σας σε αυτές τις οντότητες, προσθέστε και αυτά τα νέα πεδία.

| Entity        | Φόρμες που χρειάζονται το νέο πεδίο   |Προβολές που χρειάζονται το νέο πεδίο      |
| ------------------------------|---------------------------------|----------------------------------|
|  Τιμή ρόλου|• Πληροφορίες |• Ενεργές τιμές κατηγοριών πόρων<br> • Συσχετισμένη προβολή τιμής κατηγορίας πόρου|
|  Αύξηση τιμής ρόλου|• Πληροφορίες|• Ενεργή αύξηση τιμής ρόλου<br>• Συσχετισμένη προβολή αύξησης τιμής ρόλου|
|  Λεπτομέρεια γραμμής προσφοράς|• Πληροφορίες έργου<br>• Γρήγορη δημιουργία έργου|• Ενεργή λεπτομέρεια γραμμής προσφοράς<br>• Συνδυασμένες λεπτομέρειες γραμμής προσφοράς<br>• Συσχετισμένη προβολή λεπτομέρειας γραμμής προσφοράς|
|  Λεπτομέρεια γραμμής σύμβασης έργου|• Πληροφορίες έργου<br>• Γρήγορη δημιουργία έργου|• Συνδυασμένες λεπτομέρειες γραμμής σύμβασης<br>• Ενεργές λεπτομέρειες γραμμής σύμβασης<br>• Συσχετισμένη προβολή λεπτομερειών γραμμής σύμβασης|
|  Μέλος ομάδας έργου|• Πληροφορίες<br>• Νέα φόρμα|• Ενεργά μέλη ομάδων έργων<br>• Μέλη ομάδας έργου<br>• Συσχετισμένη προβολή μελών ομάδων έργων|
|  Χρονική καταχώρηση|• Πληροφορίες<br>• Δημιουργία χρονικής καταχώρησης|• Οι χρονικές καταχωρήσεις μου κατά ημέρα<br>• Οι χρονικές καταχωρήσεις μου για αυτήν την εβδομάδα<br>• Χρονικές καταχωρήσεις για έγκριση|
|  Γραμμή ημερολογίου|• Πληροφορίες<br>• Γρήγορη δημιουργία|• Ενεργές γραμμές ημερολογίων<br>• Συσχετισμένη προβολή γραμμής ημερολογίου|
|  Λεπτομέρεια γραμμής τιμολογίου|• Πληροφορίες<br>• Γρήγορη δημιουργία|• Ενεργές λεπτομέρειες γραμμής τιμολογίου<br>• Χρεώσιμες συναλλαγές τιμολογίου<br>• Δωρεάν συναλλαγές τιμολογίου<br>• Συσχετισμένη προβολή λεπτομερειών γραμμής τιμολογίου<br>• Μη χρεώσιμη συναλλαγή τιμολογίου|
|  Πραγματικό|• Πληροφορίες<br>• Ενεργές πραγματικές τιμές|• Πραγματική συσχετισμένη προβολή|

Επίσης, τα προσαρμοσμένα πεδία μπορεί να πρέπει να προστεθούν σε επιχειρηματικούς κανόνες, ανάλογα με τα στοιχεία που έχετε ορίσει. Ένα έτοιμο παράδειγμα είναι για τον επιχειρηματικό κανόνα **Επεξεργασιμότητα χρονικής καταχώρησης με βάση την κατάσταση**. Αυτός ο κανόνας καθορίζει ποια πεδία πρέπει να κλειδωθούν όταν η χρονική καταχώρηση δεν είναι σε κατάσταση επεξεργασίας, όπως **Εγκρίθηκε**. Προσθέστε πεδία σε αυτόν τον επιχειρηματικό κανόνα, έτσι ώστε τα πεδία να κλειδώνονται για επεξεργασία όταν η χρονική καταχώρηση είναι σε κατάσταση διαφορετική από **Προσχέδιο** ή **Επιστράφηκε**.
