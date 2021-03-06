---
title: Γραμμές προσφοράς βάσει έργου (Pro)
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση γραμμών προσφοράς βάσει έργου για την εργασία έργου. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908167"
---
# <a name="project-based-quote-lines-pro"></a>Γραμμές προσφοράς βάσει έργου (Pro)

_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_

Οι γραμμές προσφοράς βάσει έργου έχουν σχεδιαστεί για να σας βοηθήσουν να υπολογίσετε τις εργασίες του έργου σε μια δέσμευση. Η δομή μιας σειράς προσφοράς βάσει έργου επεκτείνεται για εκτιμήσεις του έργου με τις ακόλουθες έννοιες:

- Μέθοδος χρέωσης
- Αντιστοίχιση έργου και εργασιών
- Κατηγορίες συναλλαγής που περιλαμβάνονται
- Όριο που δεν πρέπει να υπερβαίνεται
- Ρύθμιση χρέωσης
- Υπολογισμός με χρήση λεπτομερειών της γραμμής προσφοράς
- Πελάτες γραμμής προσφοράς

Στον ακόλουθο πίνακα παρέχονται πληροφορίες σχετικά με τα πεδία στην καρτέλα **Γενικά** της γραμμής προσφοράς βάσει έργου. Αυτά τα πεδία βοηθούν στη δημιουργία μιας αναλυτικής εκτίμησης για την εργασία του έργου.

| **Πεδίο** | **Συνάφεια, σκοπός και καθοδήγηση** | **Κατάντη επίπτωση** |
| --- | --- | --- |
| Ονομασία | Το όνομα της γραμμής προσφοράς που θα σας βοηθήσει να προσδιορίσετε το διακριτό στοιχείο της προσφοράς που εκτιμάται. | Αντιγράφονται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Μέθοδος χρέωσης | Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας. Αυτό το πεδίο περιλαμβάνει τα δύο κύρια συμβαλλόμενα μοντέλα που υποστηρίζονται από το Dynamics 365 Project Operations:</br>- Προκαθορισμένη τιμή</br>- Χρόνος και υλικό.| Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Project | Χρησιμοποιήστε αυτό το προαιρετικό πεδίο για να προσδιορίσετε το έργο που θα χρησιμοποιηθεί για την παροχή της εργασίας σε αυτήν τη δέσμευση. Όταν ένα έργο αντιστοιχίζεται σε μια γραμμή προσφοράς, βοηθάει με τη ρύθμιση των χρεώσιμων εργασιών και επίσης με την εισαγωγή μιας εκτίμησης βάσει έργου στη γραμμή προσφοράς ως λεπτομέρειες της προσφοράς. Όταν ένα έργο δεν έχει αντιστοιχιστεί σε μια γραμμή προσφοράς βάσει έργου, η εκτίμηση θα πρέπει να δημιουργηθεί με μη αυτόματο τρόπο, δημιουργώντας κάθε λεπτομέρεια της ουράς προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά.|
| Εργασίες που περιλαμβάνονται | Υποδεικνύει εάν αυτή η γραμμή προσφοράς χρησιμοποιείται για όλες ή ορισμένες από τις εργασίες έργου του επιλεγμένου έργου. Το πεδίο αυτό έχει τις ακόλουθες πιθανές τιμές:</br>- Όλες οι εργασίες έργου</br>- Επιλεγμένες εργασίες έργου μόνο</br>Μια κενή τιμή σε αυτό το πεδίο ισοδυναμεί με την επιλογή **Όλες οι εργασίες έργου**. | Όταν επιλέξετε **Μόνο επιλεγμένες εργασίες έργου**, στη συνέχεια, στη σελίδα έργου, η καρτέλα **Ρύθμιση χρέωσης εργασιών** σάς δίνει τη δυνατότητα να επιλέξετε συγκεκριμένες εργασίες για να τις συσχετίσετε με αυτήν τη γραμμή προσφοράς. Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Συμπερίληψη χρόνου | Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι συναλλαγές χρόνου ή το κόστος εργασίας για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Όχι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Ναι** υποδεικνύει ότι οι συναλλαγές χρόνου ή το κόστος εργασίας θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Συμπερίληψη εξόδου | Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν τα κόστη δαπανών για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Όχι** υποδεικνύει ότι το κόστος δαπάνης δεν θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Ναι** υποδεικνύει ότι το κόστος δαπάνης θα συμπεριληφθεί στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Συμπερίληψη χρέωσης | Μια σημαία **Ναι**/**Όχι** υποδεικνύει εάν οι χρεώσεις για το επιλεγμένο έργο θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Όχι** υποδεικνύει ότι οι χρεώσεις δεν θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. Μια τιμή **Ναι** υποδεικνύει ότι οι χρεώσεις θα συμπεριληφθούν στην εκτίμηση σε αυτήν τη γραμμή προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Ποσό προσφοράς | Αυτό είναι το ποσό που θα προσφερθεί στον πελάτη για όλες τις εργασίες που προβάλλονται σε αυτήν τη γραμμή προσφοράς βάσει έργου. Σε μια προσφορά που δημιουργήθηκε από μια ευκαιρία, αυτή η τιμή αντιγράφεται από το πεδίο **Προϋπολογισμός πελάτη** στη γραμμή ευκαιρίας. Όταν η γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό στις λεπτομέρειες της γραμμής προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Εκτιμώμενος φόρος | Πρόκειται για ένα επεξεργάσιμο πεδίο, για να προσθέτει ο χρήστης το εκτιμώμενο ποσό του φόρου στη γραμμή προσφοράς. Όταν μια γραμμή προσφοράς βάσει έργου έχει λεπτομέρειες σχετικά γραμμής, αυτό το πεδίο είναι κλειδωμένο για επεξεργασία και συνοψίζεται από το ποσό φόρου στις λεπτομέρειες της γραμμής προσφοράς. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Ποσό προσφοράς μετά από φόρο | Αυτό το πεδίο είναι το ποσό γραμμής προσφοράς μετά τη φορολογία και είναι μόνο για ανάγνωση. Το ποσό σε αυτό το πεδίο υπολογίζεται ως εξής *Ποσό προσφοράς + Φόρος*. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Όριο που δεν πρέπει να υπερβαίνεται | Αυτό το πεδίο είναι επεξεργάσιμο και είναι διαθέσιμο μόνο σε γραμμές προσφοράς βάσει έργου που έχουν μια μέθοδο χρέωσης **Χρόνος και Υλικό**. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |
| Προϋπολογισμός πελάτη | Αυτό το πεδίο είναι επεξεργάσιμο και αντιγράφεται από το αντίστοιχο πεδίο στη γραμμή ευκαιρίας αν η προσφορά δημιουργήθηκε από μια ευκαιρία. | Αυτή η τιμή πεδίου αντιγράφεται στη γραμμή σύμβασης έργου που δημιουργείται από αυτήν τη γραμμή προσφοράς όταν κερδίζεται η προσφορά. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Κανόνες επικύρωσης για πεδία στην καρτέλα "Γενικά" των γραμμών προσφοράς βάσει έργου

**Κανόνας 1**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, το έργο περιλαμβάνεται στη γραμμή προσφοράς.

**Κανόνας 2**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** είναι κενό ή εάν έχει οριστεί σε **Όλες οι εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν μόνο σε μια γραμμή προσφοράς βάσει έργου μιας προσφοράς.

**Κανόνας 3**: Εάν το πεδίο **Εργασίες που περιλαμβάνονται** έχει οριστεί σε **Μόνο επιλεγμένες εργασίες έργου**, ένα έργο και μια συγκεκριμένη κλάση συναλλαγής μπορούν να συμπεριληφθούν σε πολλές γραμμές προσφοράς βάσει έργου μιας προσφοράς.

**Κανόνας 4**: Εάν μια ευκαιρία έχει πολλές προσφορές, μπορεί να υπάρχουν γραμμές προσφοράς από διαφορετικές προσφορές, οι οποίες να αναφέρονται σε όλες τις αναφορές στο ίδιο έργο και να περιλαμβάνουν την ίδια κλάση συναλλαγής.

**Κανόνας 5**: Εάν οι προσφορές δεν ανήκουν στην ίδια ευκαιρία, δεν είναι δυνατό να συμπεριλάβουν την ίδια κλάση έργου και συναλλαγής.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>Ευκαιρία</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Προσφορά</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Γραμμή προσφοράς</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="90" valign="top">
                <p>
                    <strong>Εργασίες που περιλαμβάνονται</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Συμπερίληψη χρόνου</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Συμπερίληψη εξόδου</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Συμπερίληψη</strong>
                </p>
                <p>
                    <strong>Χρέωση</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>Έγκυρο/ Μη έγκυρο</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>Αιτία</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Μη έγκυρο </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Παραβίαση του Κανόνα #2. Ο χρόνος, η δαπάνη και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Μη έγκυρο </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Παραβίαση του Κανόνα #2. Ο χρόνος και οι χρεώσεις για το έργο P1 περιλαμβάνονται στις γραμμές προσφοράς QL1 και QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Έγκυρα </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
Ο χρόνος και οι χρεώσεις του έργου P1 περιλαμβάνονται στο QL1.
Η δαπάνη στο έργο P1 περιλαμβάνεται στο QL2.
Δεν υπάρχει επικάλυψη σε αυτό που περιλαμβάνεται σε κάθε ουρά προσφοράς και είναι έγκυρη.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Επιλεγμένες εργασίες μόνο </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Μη έγκυρο </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Παραβίαση του Κανόνα #2 παραπάνω </p>
                <p>
Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.
                </p>
                <p>
Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για το σύνολο του έργου P1 και συμπίπτει με τα στοιχεία που περιλαμβάνονται στο Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Επιλεγμένες εργασίες μόνο </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Έγκυρα </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Σύμφωνα με τον Κανόνα #3 παραπάνω, </p>
                <p>
Το Q1 περιλαμβάνει χρόνο, έξοδα και χρεώσεις σε ένα υποσύνολο εργασιών στο έργο P1.
                </p>
                <p>
Το QL2 περιλαμβάνει χρόνο, έξοδα και χρεώσεις για ένα υποσύνολο εργασιών στο έργο P1.
                </p>
                <p>
Η μόνη πρόσθετη επικύρωση είναι για το υποσύνολο των εργασιών στο QL1 που είναι διαφορετικές από το υποσύνολο των εργασιών στο QL2. Με αυτόν τον τρόπο εξασφαλίζεται ότι δεν υπάρχουν επικαλύψεις. Αυτό γίνεται από το σύστημα όταν σχετίζονται οι εργασίες.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Επιλεγμένες εργασίες μόνο </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Όλες οι εργασίες έργου ή κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" valign="top">
                <p>
Έγκυρα </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Με βάση τον κανόνα #5, το Q1 και το Q2 είναι δύο προσφορές με την ίδια ευκαιρία, ώστε να μπορούν να εκτιμηθούν και τα δύο για τα ίδια στοιχεία ενός έργου.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ2 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Όλες οι εργασίες έργου ή κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Όλες οι εργασίες έργου ή κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" valign="top">
                <p>
Έγκυρα </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
Με βάση τον κανόνα #4, το Q1 και το Q2 είναι δύο προσφορές σε διαφορετικές ευκαιρίες και δεν μπορούν να εκτιμηθούν για τα ίδια στοιχεία του ίδιου έργου.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
Τ1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
Π1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Όλες οι εργασίες έργου ή κενό </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="48" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="42" valign="top">
                <p>
Ναι </p>
            </td>
            <td width="54" valign="top">
                <p>
Μη έγκυρο </p>
            </td>
        </tr>
    </tbody>
</table>

