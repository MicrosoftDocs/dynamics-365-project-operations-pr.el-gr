---
title: Έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με την έρευνα για το Χρονοδιάγραμμα των δαπανών των Ομοσπονδιακών Επιχορηγήσεων.
author: velofog
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: johnmichalak
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: 00f9e97b9a6b3e8fe5e9cf9143e670612869b84c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916656"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a>Έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων

[!include [banner](../includes/banner.md)]

Σύμφωνα με την Εγκύκλιο Α-133 του Γραφείου Διαχείρισης και Προϋπολογισμού, οι εταιρείες που λαμβάνουν ομοσπονδιακή χρηματοδότηση υπόκεινται σε προϋποθέσεις ελέγχου, οι οποίες είναι επίσης γνωστές ως μεμονωμένοι έλεγχοι. Η διαδικασία ελέγχου χρησιμοποιείται για την αναφορά των εσόδων και των δαπανών των ομοσπονδιακών επιδοτήσεων σε επαναλαμβανόμενη βάση. Μέρος της αναφοράς μεμονωμένου ελέγχου περιλαμβάνει το Πρόγραμμα δαπανών ομοσπονδιακών βραβείων (SEFA).

Η έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων περιλαμβάνει τον τίτλο και τον αριθμό του Καταλόγου ομοσπονδιακών εγχώριων βοηθειών (CFDA), τον αριθμό επιδότησης, το έτος της επιδότησης, το όνομα της ομοσπονδιακής υπηρεσίας που παρέχει τα κεφάλαια και το όνομα της οντότητας διαβίβασης. Η έρευνα είναι για μια συγκεκριμένη περίοδο. Τυπικά, αυτή η περίοδος είναι η ίδια με την περίοδο οικονομικών δηλώσεων η οποία είναι ένα οικονομικό έτος.

Η έρευνα περιλαμβάνει τις επιδοτήσεις που έχουν ημερομηνίες προβολής στο επιλεγμένο εύρος ημερομηνιών. Η στήλη **Εταιρεία επιδότησης** της έρευνας δείχνει τον πελάτη της επιδότησης, ή, για μια επιδότηση διαβίβασης, την εταιρεία επιδότησης. Για μια επιδότηση διαβίβασης, η στήλη **Εταιρεία διαβίβασης** εμφανίζει τον πελάτη της επιδότησης. Αν η επιδότηση δεν είναι μια επιδότηση διαβίβασης, η στήλη **Εταιρεία διαβίβασης** είναι κενή.

## <a name="set-up-the-cfda-clusters"></a>Ρύθμιση συμπλεγμάτων CFDA

Πρέπει να δημιουργήσετε τα συμπλέγματα CFDA που μπορούν να συσχετιστούν με τους αριθμούς CFDA στην έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων.

1. Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική \> Ρύθμιση \> Επιδοτήσεις \> Συμπλέγματα του Καταλόγου ομοσπονδιακών εγχώριων βοηθειών**.
2. Επιλέξτε **Νέο** για να δημιουργήσετε ένα σύμπλεγμα CFDA.
3. Καταχωρήστε το όνομα του συμπλέγματος.
4. Επιλέξτε **Αποθήκευση** για να αποθηκευτούν οι αλλαγές σας.

## <a name="set-up-cfda-numbers"></a>Ρύθμιση CFDA αριθμών

Πρέπει να δημιουργήσετε αριθμούς CFDA που μπορούν να προστεθούν σε επιδοτήσεις και να συμπεριληφθούν στην έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων.

1. Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική \> Ρύθμιση \> Επιδοτήσεις \> Αριθμοί του Καταλόγου ομοσπονδιακών εγχώριων βοηθειών**.
2. Επιλέξτε **Νέος** για να δημιουργήσετε έναν αριθμό CFDA.
3. Στη στήλη **Αριθμός**, πληκτρολογήστε τον αριθμό CFDA.
4. Πατήστε το πλήκτρο **Tab**.
5. Στη στήλη **Περιγραφή**, πληκτρολογήστε τον τίτλο CFDA.
6. Πατήστε το πλήκτρο **Tab**.
7. Προαιρετικό: Στο πεδίο **Σύμπλεγμα προγραμμάτων**, προσθέστε το κατάλληλο σύμπλεγμα CFDA.
8. Επιλέξτε **Αποθήκευση** για να αποθηκευτούν οι αλλαγές σας.

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>Ορίστε επιδοτήσεις για αναφορά για την έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων

1. Μεταβείτε στη **Διαχείριση έργου και λογιστική \> Επιδοτήσεις \> Επιδοτήσεις** και επιλέξτε μια υπάρχουσα επιδότηση.
2. Στη συνοπτική καρτέλα **Ρύθμιση** στο πεδίο **Κατάλογος ομοσπονδιακών εγχώριων βοηθειών**, αναθέστε τον αριθμό CFDA. Ο αριθμός CFDA στην επιδότηση προσδιορίζει το σύμπλεγμα CFDA για αναφορά.
3. Στη συνοπτική καρτέλα **Πληροφορίες επικοινωνίας** καταχωρήστε τις πληροφορίες του χορηγού, ακολουθώντας τα παρακάτω βήματα:

    1. Στο πεδίο **Πελάτης επιδότησης**, καταχωρήστε τον πελάτη ο οποίος είναι υπεύθυνος για την επιδότηση. Για μια υπάρχουσα επιδότηση, αυτές οι πληροφορίες ενδέχεται να έχουν ήδη καταχωρηθεί.
    2. Δηλώστε εάν ο πελάτης της επιδότησης είναι ο χρηματοδότης. Εάν ο πελάτης της επιδότησης είναι ο χρηματοδότης, αφήστε το πλαίσιο ελέγχου **Διαβίβαση** απενεργοποιημένο. Εάν ένας άλλος πελάτης είναι ο χρηματοδότης και ο πελάτης επιδότησης είναι υπεύθυνος για τη δαπάνη και την παρακολούθηση των χρημάτων, επιλέξτε το πλαίσιο ελέγχου **Διαβίβαση**.

4. Εάν επιλέξατε το πλαίσιο ελέγχου **Διαβίβαση** στο προηγούμενο βήμα, στο πεδίο **Εταιρεία επιδότησης**, καταχωρήστε τον πελάτη που παρείχε την επιδότηση. Η εταιρεία επιδότησης και ο πελάτης επιδότησης δεν είναι δυνατό να είναι ο ίδιος πελάτης.

Ακολουθεί ένα παράδειγμα μιας επιδότησης διαβίβασης:

Η ομοσπονδιακή κυβέρνηση χρηματοδότησε ένα έργο υποδομής για μια πολιτεία. Η ομοσπονδιακή κυβέρνηση έδωσε τα χρήματα στην πολιτεία για να τα δαπανήσει. Σε αυτή την περίπτωση, η ομοσπονδιακή κυβέρνηση είναι η εταιρεία επιδότησης και η πολιτεία είναι ο πελάτης της επιδότησης.

> [!NOTE] 
> Όταν ενεργοποιείτε για πρώτη φορά τη δυνατότητα, οι αρχικοί αριθμοί CFDA θα καταχωρηθούν χρησιμοποιώντας τους υπάρχοντες αριθμούς στις επιδοτήσεις.

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a>Εξαίρεση των επιδοτήσεων από την αναφορά SEFA με βάση τον τύπο επιδότησης

1. Μεταβείτε στη **Διαχείριση έργου και λογιστική \> Ρύθμιση \> Επιδοτήσεις \> Τύποι επιδότησης**.
2. Στη συνοπτική καρτέλα **Προεπιλεγμένες πληροφορίες**, επιλέξτε το πλαίσιο ελέγχου **Εξαίρεση από Πρόγραμμα δαπανών ομοσπονδιακών βραβείων**.
3. Επιλέξτε **Αποθήκευση** για να αποθηκευτούν οι αλλαγές σας.

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>Εκτέλεση έρευνας Πρόγραμμα δαπανών ομοσπονδιακών βραβείων

1. Μεταβείτε στην επιλογή **Διαχείριση έργου και λογιστική \> Έρευνες και αναφορές \> Έρευνα επιδότησης \> Πρόγραμμα δαπανών ομοσπονδιακών βραβείων**.
2. Στην ενότητα **Παράμετροι**, ακολουθήστε τα εξής βήματα:

    1. Στο πεδίο **Διάστημα ημερομηνιών**, επιλέξτε τον κωδικό για το διάστημα ημερομηνιών. Εναλλακτικά, στα πεδία **Από την ημερομηνία** και **Έως την ημερομηνία**, καθορίστε το διάστημα ημερομηνιών.
    2. Προαιρετικά: Για να συμπεριλάβετε μόνο συναλλαγές που έχουν χρεωθεί ως έσοδα στην έρευνα, ορίστε την επιλογή **Να συμπεριληφθούν μόνο τα τιμολογημένα έσοδα** σε **Ναι**.

## <a name="columns"></a>Στήλες

Η έρευνα Πρόγραμμα δαπανών ομοσπονδιακών βραβείων περιλαμβάνει τις ακόλουθες στήλες:

- Όνομα συμπλέγματος Κατάλογος ομοσπονδιακών εγχώριων βοηθειών
- Εταιρεία επιδότησης
- Εταιρεία διαβίβασης
- Όνομα επιδότησης
- Αναγνωριστικό επιδότησης
- Αναγνωριστικό εφαρμογής επιδότησης
- Κατάλογος ομοσπονδιακών εγχώριων βοηθειών
- Αποδείξεις
- Δαπάνες


[!INCLUDE[footer-include](../includes/footer-banner.md)]