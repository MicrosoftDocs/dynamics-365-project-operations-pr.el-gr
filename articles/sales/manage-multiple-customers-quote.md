---
title: Διαχείριση πολλών πελατών σε προσφορές έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία σε προσφορές με πολλούς πελάτες που θα χρηματοδοτήσουν το έργο.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8b1d9284c063e34e34ec6525072a1f8f860116b6
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908170"
---
# <a name="manage-multiple-customers-on-project-quotes"></a>Διαχείριση πολλών πελατών σε προσφορές έργου

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Οι προσφορές έργου υποστηρίζουν το σενάριο όπου η πρόταση περιλαμβάνει πολλούς πελάτες οι οποίοι θα χρηματοδοτήσουν τη συμφωνία. Η καρτέλα **Σύνοψη** της προσφοράς έχει το πεδίο **Πιθανός πελάτης** που προσδιορίζει τον κύριο πελάτη της συμφωνίας. Είναι δυνατή η ρύθμιση άλλων πελατών για τη συμφωνία στην καρτέλα **Πελάτες** της προσφοράς έργου.

Όλοι οι πελάτες προσφοράς στην καρτέλα **Πελάτες** της προεπιλεγμένης προσφοράς έργου ως πελάτες γραμμής προσφοράς σε οποιεσδήποτε **νέες** γραμμές προσφοράς βάσει έργου που δημιουργήθηκαν για την προσφορά. Οποιεσδήποτε υπάρχουσες γραμμές προσφοράς βάσει έργου δεν θα μεταβιβαστούν στις νέες καρτέλες πελατών προσφοράς που δημιουργήθηκαν μετά από αυτές.

Οι πελάτες προσφοράς και οι πελάτες της γραμμής προσφοράς μπορούν να προστεθούν, να ενημερωθούν ή να διαγραφούν οποιαδήποτε στιγμή προτού κερδηθεί η προσφορά. Ένας έγκυρος πελάτης στην προσφορά έργου πρέπει να οριστεί ως πελάτης στην εταιρεία στην ιδιοκτήτρια εταιρεία ή στη νομική οντότητα στη σελίδα **Πελάτες**. Οι νομικές οντότητες έχουν ρυθμιστεί στη μονάδα **Διαχείριση έργου και λογιστική** του Dynamics 365 Project Operations και είναι διαθέσιμες ως εταιρείες στις μονάδες **Πωλήσεις έργου και παράδοση** του Project Operations.

## <a name="concept-of-a-primary-customer"></a>Έννοια ενός κύριου πελάτη

Ο πελάτης που βρίσκεται στην καρτέλα **Σύνοψη** της προσφοράς έργου ως πιθανός πελάτης είναι ο κύριος πελάτης της προσφοράς. Όταν προσπαθείτε να διαγράψετε τον κύριο πελάτη από τη λίστα "πελάτες" με την προσφορά, θα δείτε ένα σφάλμα όπου δεν είναι δυνατή η διαγραφή μιας κύριας καρτέλας πελάτη σε μια προσφορά.

Ο κύριος πελάτης δεν πρέπει να ενημερώνεται από τη λίστα πελατών της προσφοράς. Ωστόσο, μπορείτε να επηρεάσετε τον κύριο πελάτη με την αλλαγή του πιθανού πελάτη στην καρτέλα **Σύνοψη** της προσφοράς. Όταν αυτό το πεδίο ενημερωθεί στη **Σύνοψη προσφοράς**, ο νέος πιθανός πελάτης που επιλέξατε προστίθεται ως νέος πελάτης προσφοράς με τη σημαία **Κύριος**. Ο παλαιός πιθανός πελάτης θα εξακολουθεί να είναι πελάτης της προσφοράς.

## <a name="create-update-or-delete-a-quote-customer-record"></a>Δημιουργία, ενημέρωση ή διαγραφή καρτέλας πελάτη προσφοράς

Ένας πελάτης προσφοράς μπορεί να δημιουργηθεί, να ενημερωθεί ή να διαγραφεί από την καρτέλα **Πελάτες προσφοράς** στη σελίδα **Προσφορά**. Τα πεδία που παρατίθενται στον παρακάτω πίνακα βρίσκονται στην καρτέλα πελάτη προσφοράς μιας προσφοράς έργου.

| **Πεδίο** | **Θέση** | **Συνάφεια, σκοπός και καθοδήγηση** | **Κατάντη επίπτωση** |
| --- | --- | --- | --- |
| Λογαριασμ. | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Παραθέτει όλους τους ενεργούς λογαριασμούς. Αυτό το πεδίο είναι κλειδωμένο μετά τη δημιουργία της καρτέλας. Εάν θέλετε να την ενημερώσετε, διαγράψτε την καρτέλα και δημιουργήστε την ξανά. Εάν έχετε καταγράψει πραγματικές τιμές ή εάν η καρτέλα του πελάτη προσφοράς είναι πρωτεύων πελάτης, θα σας επιτραπεί να διαγράψετε την καρτέλα. | Οι πελάτες προσφοράς αντιγράφονται ως πελάτες της σειράς προσφοράς όταν δημιουργείται μια ουρά προσφοράς. Οι πελάτες προσφοράς αντιγράφονται επίσης στους πελάτες της σύμβασης έργου όταν κερδίζεται μια προσφορά. |
| Ποσοστό διαίρεσης χρέωσης | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Αντιπροσωπεύει το ποσοστό κάθε συναλλαγής που δεν έχει τιμολογηθεί και η οποία θα αποδοθεί σε αυτόν τον πελάτη προσφοράς. | Αντιγράφονται στις νέες γραμμές προσφοράς και στους πελάτες συμβάσεων έργου. |
| Όνομα επαφής χρέωσης | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Αυτό είναι ένα πεδίο κειμένου και πρέπει να χρησιμοποιηθεί για τον προσδιορισμό του υπευθύνου επικοινωνίας με το τιμολόγιο για αυτόν τον πελάτη. Αυτές οι προεπιλογές έχουν προεπιλεγεί από την καρτέλα "σχετικός λογαριασμός" | Αντιγράφεται σε πελάτες της σύμβασης έργου όταν μια προσφορά κερδηθεί και με τη σειρά στο πεδίο "Τιμολόγηση με όνομα σύμβασης" στο τιμολόγιο που δημιουργείται για αυτόν τον πελάτη. |
| Όνομα χρέωσης | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Αυτό είναι ένα πεδίο κειμένου και πρέπει να χρησιμοποιηθεί για τον προσδιορισμό του υπευθύνου επικοινωνίας με το τιμολόγιο για αυτόν τον πελάτη. | Αντιγράφεται σε πελάτες της σύμβασης έργου όταν μια προσφορά κερδηθεί και με τη σειρά στο πεδίο **Τιμολόγηση με όνομα σύμβασης** στο τιμολόγιο που δημιουργείται για αυτόν τον πελάτη. |
| Όροι πληρωμής | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Πρόκειται για ένα σύνολο επιλογών με τιμές που είναι προεπιλεγμένες από την καρτέλα του σχετικού λογαριασμού. | Αντιγράφεται σε πελάτες της σύμβασης έργου όταν μια προσφορά κερδηθεί και με τη σειρά στο πεδίο **Τιμολόγηση με όνομα σύμβασης** στο τιμολόγιο που δημιουργείται για αυτόν τον πελάτη. |
| Είναι στρογγυλοποίηση | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Υποδεικνύει εάν αυτός ο πελάτης είναι προεπιλεγμένος πελάτης στρογγυλοποίησης για αυτήν τη συμφωνία. | Αντιγράφονται στους πελάτες της σύμβασης έργου όταν κερδίζεται μια προσφορά. |
| Εταιρεία-κάτοχος | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Η νομική οντότητα στην οποία αυτός ο πελάτης έχει ρυθμιστεί στη μονάδα **Διαχείριση έργου και λογιστική**. Αυτό το πεδίο είναι μόνο για ανάγνωση και ορίζεται στην εταιρεία στην οποία ανήκει η ίδια η προσφορά. Η λίστα των πελατών που θα προστεθούν στο πεδίο **Λογαριασμός** έχει ήδη φιλτραριστεί στη λίστα από την εταιρεία που έχει την κυριότητα στη μονάδα **Διαχείριση έργου και λογιστική** του Project Operations. | Η εταιρεία που έχει την κυριότητα ταυτίζεται με την έννοια της νομικής οντότητας στη μονάδα **Διαχείρισης έργου και λογιστικής** του Project Operations. Όλες οι δαπάνες και τα έσοδα που προκύπτουν από αυτό το έργο υπολογίζονται στη γενική λογιστική της εταιρείας που έχει την κυριότητα. |
| Όριο που δεν πρέπει να υπερβαίνεται | Επεξεργάσιμο πλέγμα στην καρτέλα **Πελάτες προσφοράς** στις φόρμες **Κύρια** κα **Γρήγορη δημιουργία** για έναν πελάτη προσφοράς. | Υποδεικνύει εάν υπάρχει όριο ή ανώτατο όριο διαπραγματεύσεων στο συνολικό ποσό που θα τιμολογηθεί σε αυτόν τον πελάτη για αυτήν τη δέσμευση. | Αντιγράφονται στους πελάτες της σύμβασης έργου όταν κερδίζεται μια προσφορά. |

## <a name="editing-billing-split-percentages"></a>Επεξεργασία ποσοστών διαίρεσης χρέωσης

Μπορείτε να επεξεργαστείτε τα ποσοστά διαίρεσης χρέωσης χρησιμοποιώντας την εμπειρία επεξεργασίας πλέγματος σε γραμμή. Όταν τα ποσοστά διαίρεσης χρέωσης δεν είναι συνολικά 100%, θα εμφανιστεί ένα σφάλμα. Αφού ενημερώσετε τα ποσοστά διαίρεσης χρέωσης, ανανεώστε τη σελίδα για να καταργήσετε το σφάλμα.

Μπορείτε, επίσης, να δοκιμάσετε να επιλέξετε **Ομοιόμορφη διανομή** στο υποπλέγμα των πελατών προσφοράς. Αυτή η ενέργεια εκχωρεί διαιρέσεις χρέωσης σε όλους τους πελάτες προσφοράς. Εάν υπάρχει συντελεστής στρογγυλοποίησης, ο οποίος θα προστεθεί στον πελάτη στρογγυλοποίησης. Ένας από τους πελάτες προσφοράς επισημαίνεται πάντα ως πελάτης στρογγυλοποίησης. αυτό σημαίνει ότι η καρτέλα του πελάτη προσφοράς έχει τη σημαία **Στρογγυλοποίηση** ορισμένη σε **Ναι**. Κατά κανόνα, αυτός είναι ο κύριος πελάτης της προσφοράς, αλλά είναι δυνατή η αλλαγή του.