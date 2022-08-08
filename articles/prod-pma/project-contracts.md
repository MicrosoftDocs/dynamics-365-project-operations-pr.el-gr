---
title: Συμβάσεις έργων
description: Αυτό το άρθρο παρέχει παραδείγματα των συμβάσεων έργων που μπορείτε να δημιουργήσετε για διάφορους τύπους έργων και πηγών χρηματοδότησης και πώς μπορείτε να διαχειριστείτε τις συμβάσεις και να τιμολογήσετε τους πελάτες του έργου.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: johnmichalak
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 14ff17bb070a44d8f3962e08f67d4c95bd8a26f9
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919646"
---
# <a name="project-contracts"></a>Συμβάσεις έργων

[!include [banner](../includes/banner.md)]

Αυτό το άρθρο παρέχει παραδείγματα των συμβάσεων έργων που μπορείτε να δημιουργήσετε για διάφορους τύπους έργων και πηγών χρηματοδότησης και πώς μπορείτε να διαχειριστείτε τις συμβάσεις και να τιμολογήσετε τους πελάτες του έργου.

Ο τύπος του έργου που δημιουργείτε για μια σύμβαση έργου καθορίζει τη μέθοδο που χρησιμοποιείται για την τιμολόγηση των πελατών του έργου. Μπορείτε να αλλάξετε μια σύμβαση έργου και το σχετικό έργο, αλλά δεν μπορείτε να αλλάξετε τον τύπο έργου. 

Χρησιμοποιώντας μια σύμβαση έργου, μπορείτε να τιμολογήσετε ταυτόχρονα ένα ή περισσότερα έργα. Επίσης, η σύμβαση έργου συμβάλλει στη διασφάλιση μιας συνεπούς διαδικασίας τιμολόγησης για κάθε δευτερεύον έργο σε μια δομή έργου. 

Κάθε έργο που θα τιμολογηθεί πρέπει να συσχετιστεί με μια σύμβαση έργου. Οι ρυθμίσεις για μια σύμβαση έργου εφαρμόζονται σε όλα τα έργα και τα δευτερεύοντα έργα που σχετίζονται με τη συγκεκριμένη σύμβαση έργου. 

Μια σύμβαση έργου μπορεί να καθορίσει μία ή περισσότερες πηγές χρηματοδότησης. Για αυτόν το λόγο, μπορείτε να διαιρέσετε τη χρέωση ανάμεσα σε πολλούς χρηματοδότες, να ορίσετε όρια χρηματοδότησης έτσι ώστε οι προελεύσεις χρηματοδότησης να μην χρεώνονται περισσότερο από ένα συγκεκριμένο ποσό και να ρυθμίσετε τις παραμέτρους των κανόνων χρηματοδότησης για τη χρέωση των δαπανών.

## <a name="funding-for-project-contracts"></a>Χρηματοδότηση συμβάσεων έργου
Ορισμένες συμβάσεις έργου ορίζουν ότι πολλαπλά μέρη μοιράζονται την ευθύνη για τη χρηματοδότηση του κόστους του έργου. Ακολουθούν μερικά παραδείγματα:

-   Ένας μεγάλος πελάτης που έχει πολλαπλά τμήματα απαιτεί τη διαίρεση μιας χρηματοδότησης έργου με διαίρεση.
-   Η εταιρεία σας συμμερίζεται το κόστος ενός μεγάλου έργου με εξωτερικό οργανισμό.
-   Ένα οδικό έργο συγχρηματοδοτείται από δύο δήμους.
-   Ένα έργο κατασκευής γέφυρας χρηματοδοτείται από μια κρατική επιδότηση και μια ιδιωτική εταιρεία.

Στο Dynamics 365 Finance, μπορείτε να διαιρέσετε τη χρέωση για μία συναλλαγή ή ένα ολόκληρο έργο σε πολλούς πελάτες, επιχορηγήσεις ή οργανισμούς. 

Σε έργα που έχουν πολλαπλούς χρηματοδότες, όλα τα μέρη που συνεισφέρουν στη χρηματοδότηση ενός προηγμένου χρηματοδοτικού έργου ονομάζονται πηγές χρηματοδότησης. Αφού ένας πελάτης, ένας οργανισμός ή μια επιδότηση ορίζεται ως προέλευση χρηματοδότησης, μπορεί να ανατεθεί σε έναν ή περισσότερους κανόνες χρηματοδότησης. Οι κανόνες χρηματοδότησης περιέχουν τα κριτήρια που καθορίζουν τον τρόπο με τον οποίο οι χρεώσεις εκχωρούνται στις διάφορες πηγές χρηματοδότησης ενός έργου. 

Επειδή τα στοιχεία που έχουν απομείνει, όπως αυτά που εμφανίζονται στις αιτήσεις αγοράς και τις παραγγελίες αγοράς, δεν είναι δυνατό να διαχωριστούν, το ποσό του κόστους δεν μπορεί να χωριστεί μεταξύ πολλών προελεύσεων χρηματοδότησης κατά τη στιγμή της διανομής. Επομένως, η τιμή προέλευσης χρηματοδότησης παραμένει 0 (μηδέν) έως ότου καταχωρηθεί το ζήτημα αποθέματος. Όταν καταχωρείται το ζήτημα του αποθέματος, το ποσό του κόστους κατανέμεται σύμφωνα με τους κανόνες διανομής λογαριασμών του έργου.

Ακολουθούν ορισμένα βήματα που μπορείτε να ακολουθήσετε για να διευκολύνετε τη διαίρεση της χρέωσης μεταξύ πολλών προελεύσεων χρηματοδότησης:

-   Καθορίστε ότι όλες οι συναλλαγές που έχουν καταχωρηθεί για ένα έργο χρησιμοποιούν την ίδια νομισματική μονάδα πωλήσεων με τη σύμβαση έργου.
-   Καθορίστε όρια χρηματοδότησης, έτσι ώστε μια προέλευση χρηματοδότησης να μην τιμολογείται περισσότερο από ένα καθορισμένο ποσό προς ένα έργο.
-   Ρυθμίστε τις παραμέτρους των κανόνων χρηματοδότησης και των ορίων χρηματοδότησης για κάθε εργαζόμενο, στοιχείο, κατηγορία, ομάδα κατηγοριών και τύπο συναλλαγής (ή για όλους τους τύπους συναλλαγών).
-   Επιλέξτε προαιρετικές ημερομηνίες έναρξης και λήξης για να καθορίσετε την περίοδο κατά την οποία θα είναι έγκυρος κάθε κανόνας χρηματοδότησης.
-   Καθορίστε το ποσοστό για το οποίο είναι υπεύθυνη κάθε προέλευση χρηματοδότησης.
-   Καθορίστε ποια προέλευση χρηματοδότησης είναι υπεύθυνη για τη στρογγυλοποίηση διαφορών που προκαλούνται από υπολογισμούς εκχώρησης χρηματοδότησης.
-   Ρυθμίστε κανόνες που καθορίζουν τον τρόπο τιμολόγησης του κόστους έργου σε εξωτερικούς πελάτες και χρεώνεται σε εσωτερικούς οργανισμούς.
-   Καταγράψτε τις συναλλαγές σε ένα λογαριασμό χρηματοδότησης που βρίσκεται σε αναμονή μέχρι να αποκτηθεί πρόσθετη χρηματοδότηση ή μέχρι να αποφασίσετε να επιβαρυνθείτε εσωτερικά με το κόστος.

Για να καθοριστεί ποια ομάδα φόρων θα συσχετιστεί με μια συναλλαγή, γίνεται αναζήτηση του έργου για μια ανάθεση ομάδας φόρων. Σε περίπτωση που δεν έχει γίνει καμία ανάθεση σε ομάδα φόρων σε επίπεδο έργου, γίνεται αναζήτηση της σύμβασης έργου.

### <a name="example-multiple-funding-sources-simple"></a>Παράδειγμα: πολλαπλές πηγές χρηματοδότησης (απλή)

Στον ακόλουθο πίνακα παρουσιάζονται τα σενάρια για τη διαχείριση της ανάθεσης κονδυλίων μεταξύ πολλών προελεύσεων χρηματοδότησης. Τα σενάρια αυτά βασίζονται στις εξής υποθέσεις:

-   Οι ρυθμίσεις προτεραιότητας υπολογίζονται στη διανομή των κονδυλίων προτού εφαρμοστούν άλλα κριτήρια κανόνων χρηματοδότησης.
-   Δεν έχει καθοριστεί εύρος ημερομηνιών για τον καθορισμό της περιόδου d όταν ο κανόνας χρηματοδότησης είναι έγκυρος.

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Σενάριο</strong></td>
<td><strong>Προέλευση χρηματοδότησης</strong></td>
<td><strong>Ποσοστό εκχώρησης</strong></td>
<td><strong>Προτεραιότητα ανάθεσης</strong></td>
</tr>
<tr class="even">
<td>Θέλετε να αναθέσετε το κόστος σε μια πηγή χρηματοδότησης έως ότου εξαντληθούν τα κεφάλαιά της, να κατανείμετε το κόστος σε μια δεύτερη πηγή χρηματοδότησης έως ότου εξαντληθούν τα κεφάλαιά της και, τέλος, να κατανείμετε το υπόλοιπο κόστος σε μια τρίτη πηγή χρηματοδότησης.</td>
<td><ul>
<li>Προέλευση　χρηματοδότησης　1</li>
<li>Προέλευση　χρηματοδότησης　2</li>
<li>Προέλευση　χρηματοδότησης　3</li>
</ul></td>
<td><ul>
<li>100%</li>
<li>100%</li>
<li>100%</li>
</ul></td>
<td><ul>
<li>1</li>
<li>2</li>
<li>3</li>
</ul></td>
</tr>
<tr class="odd">
<td>Θέλετε να δεσμεύσετε το 75 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το 25 τοις εκατό σε μια δεύτερη προέλευση χρηματοδότησης. Όταν κάποια από αυτές τις πηγές χρηματοδότησης έχει εξαντληθεί, θέλετε να πληρώσετε τα υπόλοιπα έξοδα από μια τρίτη πηγή χρηματοδότησης.</td>
<td><ul>
<li>Προέλευση　χρηματοδότησης　1</li>
<li>Προέλευση　χρηματοδότησης　2</li>
<li>Προέλευση　χρηματοδότησης　3</li>
</ul></td>
<td><ul>
<li>75%</li>
<li>25%</li>
<li>100%</li>
</ul></td>
<td><ul>
<li>1</li>
<li>1</li>
<li>2</li>
</ul></td>
</tr>
<tr class="even">
<td>Θέλετε να δεσμεύσετε το 75 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το 25 τοις εκατό σε μια δεύτερη προέλευση χρηματοδότησης. Όταν κάποια από αυτές τις πηγές χρηματοδότησης έχει εξαντληθεί, θέλετε να διαχωρίσετε τα υπόλοιπα έξοδα μεταξύ μιας τρίτης πηγής χρηματοδότησης και μιας τέταρτης πηγής χρηματοδότησης.</td>
<td><ul>
<li>Προέλευση　χρηματοδότησης　1</li>
<li>Προέλευση　χρηματοδότησης　2</li>
<li>Προέλευση　χρηματοδότησης　3</li>
<li>Προέλευση　χρηματοδότησης　4</li>
</ul></td>
<td><ul>
<li>75%</li>
<li>25%</li>
<li>50%</li>
<li>50%</li>
</ul></td>
<td><ul>
<li>1</li>
<li>1</li>
<li>2</li>
<li>2</li>
</ul></td>
</tr>
<tr class="odd">
<td>Θέλετε να δεσμεύσετε το πρώτο 25 τοις εκατό του κόστους σε μία προέλευση χρηματοδότησης και το υπόλοιπο σε μια δεύτερη προέλευση χρηματοδότησης.</td>
<td><ul>
<li>Προέλευση　χρηματοδότησης　1</li>
<li>Προέλευση　χρηματοδότησης　2</li>
</ul></td>
<td><ul>
<li>25%</li>
<li>100%</li>
</ul></td>
<td><ul>
<li>1</li>
<li>2</li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a>Παράδειγμα: πολλαπλές πηγές χρηματοδότησης (σύνθετη)

Έχετε τρεις πηγές χρηματοδότησης που θέλετε να χρησιμοποιήσετε με την ακόλουθη σειρά:

1.  Χρησιμοποιήστε την πηγή χρηματοδότησης 2 και την πηγή χρηματοδότησης 3 εξίσου, έως ότου εξαντληθεί η πηγή χρηματοδότησης 2.
2.  Συνεχίστε να χρησιμοποιείτε την πηγή χρηματοδότησης 3 έως ότου εξαντληθεί.
3.  Χρησιμοποιήστε την πηγή χρηματοδότησης 1 μόλις εξαντληθεί η πηγή χρηματοδότησης 3.

Για να πετύχετε αυτόν τον στόχο, πρώτα πρέπει να κάνετε τα εξής:

-   Καθορισμός ορίων χρηματοδότησης για την πηγή χρηματοδότησης 2 και την πηγή χρηματοδότησης 3, για τα αντίστοιχα ποσά.
-   Δημιουργήσετε τους παρακάτω κανόνες χρηματοδότησης:
    -   Κανόνας 1 (προτεραιότητα 1): Εκχώρηση του 50 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 2 και του 50 τοις εκατό στην πηγή χρηματοδότησης 3.
    -   Κανόνας 2 (προτεραιότητα 2): Εκχώρηση του 100 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 3.
    -   Κανόνας 3 (προτεραιότητα 3): Εκχώρηση του 100 τοις εκατό των συναλλαγών στην πηγή χρηματοδότησης 1.

Αυτή η ρύθμιση λειτουργεί επειδή οι συναλλαγές ελέγχονται με βάση τους κανόνες και τα όρια για να καθοριστεί εάν κάποιο από αυτά ισχύει για τη συναλλαγή. Εάν δεν ισχύουν συγκεκριμένοι κανόνες ή όρια για τη συναλλαγή, ισχύει ο κανόνας "Όλες οι συναλλαγές". Ο κανόνας "Όλες οι συναλλαγές" ταιριάζει με όλες τις συναλλαγές. 

Εάν βρεθεί ένας κανόνας που αντιστοιχεί σε μια συναλλαγή, εφαρμόζεται πρώτα το ποσοστό που έχει εκχωρηθεί σε αυτόν τον κανόνα, αλλά μόνο αφού ελεγχθούν οι αντιστοιχίσεις με βάση τα όρια που έχουν οριστεί. Εάν έχει τηρηθεί ένα όριο και εξαντληθούν τα κεφάλαια μιας πηγής χρηματοδότησης, ο κανόνας χρηματοδότησης που σχετίζεται με το όριο χρηματοδότησης δεν λαμβάνεται υπόψη και το πρόγραμμα ελέγχει για τον επόμενο κανόνα που ισχύει. 

Σε ορισμένες περιπτώσεις, μόνο ένα μέρος μιας συναλλαγής μπορεί να εκχωρηθεί με βάση έναν κανόνα. Αυτό μπορεί να συμβαίνει επειδή ένα όριο επιτυγχάνεται όταν η συναλλαγή έχει εκχωρηθεί. Σε αυτήν την περίπτωση, μόνο ένα συγκεκριμένο ποσό εκχωρείται σύμφωνα με τον εν λόγω κανόνα, όπως το 50 τοις εκατό σε κάθε πηγή χρηματοδότησης. Αυτή είναι η υπόθεση στον κανόνα 1, η οποία περιγράφεται παραπάνω σε αυτήν την ενότητα. Το υπόλοιπο εκχωρείται σύμφωνα με τον επόμενο κανόνα στην ακολουθία. 

Ο παρακάτω πίνακας εξετάζει αυτό το σενάριο με περισσότερες λεπτομέρειες.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Εστίαση</strong></td>
<td><strong>Λεπτομέρειες</strong></td>
</tr>
<tr class="even">
<td>Κανόνες χρηματοδότησης</td>
<td><ul>
<li>Κανόνας 1 (προτεραιότητα 1): όλες οι συναλλαγές. Καταχωρήστε την πηγή χρηματοδότησης 2 στο 50% και την πηγή χρηματοδότηση 3 στο 50%.</li>
<li>Κανόνας 2 (προτεραιότητα 2): όλες οι συναλλαγές. Καταχωρήστε την πηγή χρηματοδότησης 3 στο 100%.</li>
<li>Κανόνας 3 (προτεραιότητα 2): όλες οι συναλλαγές. Καταχωρήστε την πηγή χρηματοδότησης 1 στο 100%.</li>
</ul></td>
</tr>
<tr class="odd">
<td>Όρια χρηματοδότησης</td>
<td><ul>
<li>Όριο πηγής χρηματοδότησης 1 = 10,000.00</li>
<li>Όριο πηγής χρηματοδότησης 2 = 500.00</li>
<li>Όριο πηγής χρηματοδότησης 3 = 750.00</li>
</ul></td>
</tr>
<tr class="even">
<td>Συναλλαγή 1</td>
<td><strong>Ποσό συναλλαγής:</strong> 100.00<strong>Χρηματοδότηση:</strong> Η συναλλαγή καταβάλλεται μόνο σύμφωνα με τον κανόνα 1, επειδή η συναλλαγή πληρώνεται πλήρως μετά την εφαρμογή του κανόνα 1. Η συναλλαγή χρηματοδοτείται ισόποσα μεταξύ της πηγής χρηματοδότησης 2 και της πηγής χρηματοδότησης 3.
<ul>
<li>Πηγή χρηματοδότησης 2: 50.00</li>
<li>Πηγή χρηματοδότησης 3: 50.00</li>
</ul></td>
</tr>
<tr class="odd">
<td>Συναλλαγή 2</td>
<td><strong>Ποσό συναλλαγής:</strong> 5.000.00<strong>Χρηματοδότηση:</strong> Η συναλλαγή καταβάλλεται σύμφωνα με τους τρεις κανόνες. <strong>Κανόνας 1</strong>
<ul>
<li>Πηγή χρηματοδότησης 2: 450.00</li>
<li>Πηγή χρηματοδότησης 3: 450.00</li>
</ul>
<strong>Κανόνας 2</strong>
<ul>
<li>Πηγή χρηματοδότησης 3: 250.00 (= 750.00 – 50.00 – 450.00)</li>
</ul>
<strong>Κανόνας 3</strong>
<ul>
<li>Πηγή χρηματοδότησης 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</li>
</ul></td>
</tr>
<tr class="even">
<td>Σύνολο κονδυλίων που διανέμονται για κάθε πηγή χρηματοδότησης</td>
<td><ul>
<li>Πηγή χρηματοδότησης 1: 3,850.00</li>
<li>Πηγή χρηματοδότησης 2: 500.00</li>
<li>Πηγή χρηματοδότησης 3: 750.00</li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a>Κανόνες χρέωσης
Όταν διαπραγματεύεστε μια σύμβαση έργου με έναν πελάτη, καθορίζετε τον τρόπο και το χρόνο με τον οποίο μπορείτε να τιμολογήσετε τον πελάτη για την εργασία σε ένα έργο. Μετά τη ρύθμιση της σύμβασης έργου και του έργου, μπορείτε να ορίσετε κανόνες χρέωσης για το έργο. Οι κανόνες χρέωσης βασίζονται στους όρους έργου που καθορίζονται στη σύμβαση έργου. Οι κανόνες χρέωσης που μπορείτε να δημιουργήσετε εξαρτώνται από τους όρους της σύμβασης έργου και τον τύπο έργου, για παράδειγμα, ο χρόνος και το υλικό ή η σταθερή τιμή, τα οποία συσχετίζετε με τον κανόνα χρέωσης. Μπορείτε να δημιουργήσετε περισσότερους από έναν κανόνες χρέωσης για μια σύμβαση έργου. Μπορείτε, επίσης, να αναθέσετε έναν κανόνα χρέωσης σε πολλαπλά έργα που σχετίζονται με την ίδια σύμβαση έργου και με παρόμοιους όρους χρέωσης. 

Μπορείτε να ορίσετε τους ακόλουθους τύπους κανόνων χρέωσης:

-   **Μονάδα παράδοσης** – Τιμολογήστε έναν πελάτη όταν ολοκληρώνετε μια μονάδα παράδοσης. Μπορείτε να ορίσετε τις μονάδες παράδοσης στη σύμβαση.
-   **Πρόοδος** – Τιμολογήστε έναν πελάτη όταν ολοκληρώνετε ένα καθορισμένο ποσοστό του έργου. Μπορείτε να ορίσετε έναν κανόνα χρέωσης για τον αυτόματο υπολογισμό του ποσοστού της εργασίας που έχει ολοκληρωθεί ή μπορείτε να υπολογίσετε με μη αυτόματο τρόπο το ποσοστό της εργασίας που έχει ολοκληρωθεί και το ποσό τιμολόγησης του πελάτη.
-   **Ορόσημο** – Τιμολογήστε έναν πελάτη για το πλήρες ποσό ενός ορόσημου έργου όταν επιτυγχάνεται το ορόσημο.
-   **Χρέωση** – Τιμολογήστε έναν πελάτη για τις υπηρεσίες σας συν ένα τέλος διαχείρισης, το οποίο κατά κανόνα αποτελεί ένα ποσοστό του κόστους των υπηρεσιών.
-   **Χρόνος και υλικό** – Τιμολογήστε έναν πελάτη για την αξία του χρόνου και των υλικών που χρησιμοποιούνται σε ένα έργο.

Για όλους τους τύπους κανόνων χρέωσης, μπορείτε να καθορίσετε ένα ποσοστό διατήρησης που αφαιρείται από τα τιμολόγια πελατών, έως ότου ένα έργο φθάσει σε ένα συμφωνημένο στάδιο. Το ποσοστό διατήρησης της πληρωμής καθορίζεται στη σύμβαση έργου. Το ποσό υπολογίζεται με βάση και αφαιρείται από τη συνολική αξία των γραμμών σε ένα τιμολόγιο πελάτη. 

Για τους κανόνες χρέωσης **Χρόνος και υλικό** και **Πρόοδος** μπορείτε να αναθέσετε κατηγορίες με χρέωση. Οι τιμολογημένες κατηγορίες δηλώνουν τις συναλλαγές που θα πρέπει να συμπεριληφθούν στα τιμολόγια πελατών. 

Όταν είστε έτοιμοι να τιμολογήσετε τον πελάτη, το ποσό τιμολόγησης για το έργο υπολογίζεται με βάση τους κανόνες χρέωσης και δημιουργείται μια πρόταση για το τιμολόγιο του έργου. 

Οι παρακάτω ενότητες παρέχουν παραδείγματα που δείχνουν τον τρόπο ρύθμισης και διαχείρισης των κανόνων χρέωσης για ένα έργο.

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a>Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται στον αριθμό των μονάδων που παραδόθηκαν

Ο οργανισμός σας συνάπτει συμφωνία για την παροχή συνολικά πέντε εκπαιδευτικών σεμιναρίων στους υπαλλήλους ενός πελάτη με κόστος 10.000 ανά εκπαιδευτική συνεδρία. Τιμολογήστε τον πελάτη μετά από εκπαιδευτική συνεδρία. 

Όταν ρυθμίζετε τους κανόνες χρέωσης για τη σύμβαση, χρησιμοποιείτε τις παρακάτω τιμές:

-   Η μονάδα παραλαβής είναι μία εκπαιδευτική συνεδρία.
-   Η τιμή μονάδας είναι 10.000 ανά εκπαιδευτική συνεδρία.
-   Ο συνολικός αριθμός των μονάδων είναι πέντε εκπαιδευτικά σεμινάρια.

Όταν ολοκληρώσετε μια εκπαιδευτική συνεδρία, μπορείτε να δημιουργήσετε ένα τιμολόγιο για 10.000, για την πρώτη μονάδα που παρεδόθη και να στείλετε το τιμολόγιο στον πελάτη.

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a>Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε ένα καθορισμένο ποσοστό ολοκλήρωσης έργου (μη αυτόματος υπολογισμός)

Ο οργανισμός σας, μια εταιρεία συμβούλων λογισμικού, συνάπτει μια συμφωνία με έναν πελάτη για να αναπτύξει ένα μέρος ενός προϊόντος που αναπτύσσει ο πελάτης. Ο οργανισμός σας συμφωνεί να παραδώσει τον κώδικα λογισμικού για μια περίοδο έξι μηνών. Ο πελάτης συμφωνεί να καταβάλει στον οργανισμό σας συνολικά 100.000 για την εργασία. Μπορείτε να δημιουργήσετε έναν κανόνα χρέωσης για την τιμολόγηση του πελάτη με βάση το ποσοστό της εργασίας που ολοκληρώνεται στο έργο, όπως καθορίζεται στη σύμβαση.

-   Στο τέλος του πρώτου μήνα, θα συναντήσετε τον πελάτη για να καθορίσετε το ποσοστό της εργασίας που έχει ολοκληρωθεί. Μετά την αναθεώρηση του έργου από εσάς και τον πελάτη, αποφασίζετε ότι το έργο είναι 15 τοις εκατό ολοκληρωμένο.
-   Μπορείτε να δημιουργήσετε ένα τιμολόγιο για 15.000 (15 τοις εκατό των 100.000) και να το στείλετε στον πελάτη.

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a>Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε ένα καθορισμένο ποσοστό ολοκλήρωσης έργου (αυτόματος υπολογισμός)

Ο οργανισμός σας, μια εταιρεία ανάπτυξης λογισμικού, συμφωνεί να αναπτύξει ένα πακέτο λογιστικής μισθοδοσίας για έναν πελάτη για τα 30.000. Ο πελάτης συμφωνεί να πληρώσει τον οργανισμό σας με βάση το ποσοστό της εργασίας που ολοκληρώθηκε. Εκτιμάτε ότι το κόστος του έργου είναι 20.000. Η σύμβαση έργου προσδιορίζει τις κατηγορίες εργασιών που χρησιμοποιείτε στη διαδικασία χρέωσης. Μπορείτε να ορίσετε κανόνες χρέωσης που υπολογίζουν αυτόματα τα ποσά τιμολόγησης για το ποσοστό της εργασίας που ολοκληρώνεται για κάθε κατηγορία. Μπορείτε να δημιουργήσετε έναν προϋπολογισμό για κάθε κατηγορία:

-   **Ανάπτυξη** – Κόστος 15.000 και έσοδα 20.000
-   **Εγκατάσταση** – Κόστος 5.000 και έσοδα 10.000

Όταν δημιουργείτε ένα τιμολόγιο πελάτη για πρώτη φορά, το ποσό τιμολογίου υπολογίζεται αυτόματα με βάση τις εξής πληροφορίες:

-   Μετά από ένα μήνα, ο εργαζόμενος του έργου υποβάλλει ένα φύλλο κατανομής χρόνου για το έργο. Το κόστος των ωρών εργασίας του εργαζομένου είναι 5.000 για την ανάπτυξη και 1.000 για την εγκατάσταση. Η εργασία ανάπτυξης είναι 33 τοις εκατό ολοκληρωμένη (5.000 πραγματικό κόστος/15.000 κόστος προϋπολογισμού) και η εργασία εγκατάστασης είναι 20 τοις εκατό ολοκληρωμένη (1.000 πραγματικό κόστος/5.000 κόστος προϋπολογισμού).
-   Το ποσό τιμολογίου 8.667 υπολογίζεται αυτόματα (33 τοις εκατό των 20.000 + 20 τοις εκατό των 10.000).
-   Μπορείτε να δημιουργήσετε ένα τιμολόγιο για 8.667 και να το στείλετε στον πελάτη.

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a>Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε συμφωνηθέντα ορόσημα

Ο οργανισμός σας, μια εταιρεία συμβούλων επιχειρήσεων, συμφωνεί να διεξάγει έρευνα αγοράς για ένα καταναλωτικό προϊόν, το οποίο προτίθεται να πωλήσει ο πελάτης. Ο πελάτης συμφωνεί να χρησιμοποιήσει τις υπηρεσίες σας για μια περίοδο τριών μηνών, αρχής γενομένης από το Μάρτιο και συμφωνεί να καταβάλει στον οργανισμό σας 50.000. Το έργο έχει τρία ορόσημα:

-   Ορόσημο 1: Συλλέξτε καταναλωτικά δεδομένα – 31 Μαρτίου
-   Ορόσημο 2: Ανάλυση καταναλωτικών δεδομένων-30 Απριλίου
-   Ορόσημο 3: Παρουσιάστε μια πρόταση βιωσιμότητας προϊόντος – 31 Μαΐου

Ο πελάτης συμφωνεί να καταβάλει στον οργανισμό σας 10.000 για το πρώτο ορόσημο, 20.000 για το δεύτερο ορόσημο και 20.000 για το τρίτο ορόσημο. 

Όταν ρυθμίζετε τη σύμβαση έργου, συμφωνείτε με την τιμολόγηση του πελάτη με βάση το ορόσημο που έχει ολοκληρωθεί. Η ρύθμιση κανόνων χρέωσης περιλαμβάνει τα ακόλουθα βήματα:

-   Καθορίστε τα ορόσημα του έργου.
-   Καθορίστε το ποσό τιμολόγησης του πελάτη όταν ολοκληρωθεί κάθε ορόσημο.

Όταν το πρώτο ορόσημο ολοκληρωθεί στις 31 Μαρτίου, μαρκάρετε το ορόσημο ως ολοκληρωμένο και, στη συνέχεια, δημιουργήστε ένα τιμολόγιο για το 10.000 και στείλτε το στον πελάτη. Δεν μπορείτε να δημιουργήσετε ένα τιμολόγιο για ένα ορόσημο, μέχρι να έχετε επισημάνει το ορόσημο ως ολοκληρωμένο.

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a>Παράδειγμα: δημιουργία ενός κανόνα χρέωσης που βασίζεται σε υπηρεσίες συν ένα τέλος διαχείρισης

Ο οργανισμός σας, μια εταιρεία συμβούλων επιχειρήσεων, συμφωνεί να διεξάγει έρευνα αγοράς για την αξιολόγηση της βιωσιμότητας ενός προϊόντος που αναπτύσσει ο πελάτης, μια εταιρεία λιανικής πώλησης. Οι όροι της σύμβασης ορίζουν ότι θα παράσχετε τις υπηρεσίες των τριών κορυφαίων συμβούλων διαχείρισης, οι οποίοι θα διεξάγουν την έρευνα σε βάση χρόνου και ύλης. Ο πελάτης συμφωνεί να καταβάλει 100 ανά ώρα, συν ένα 10 τοις εκατό τέλος διαχείρισης για τις ώρες παροχής συμβουλών που χρεώνονται στο έργο. 

Όταν ρυθμίζετε τη σύμβαση έργου, δημιουργήστε έναν κανόνα χρέωσης για να προσθέσετε μια αμοιβή διαχείρισης 10 τοις εκατό στις ώρες παροχής συμβουλών που χρεώνονται στο έργο. 

Όταν δημιουργείτε ένα τιμολόγιο για τον πελάτη, ο πελάτης χρεώνεται μια χρέωση διαχείρισης 10% συν το κόστος των ωρών διαβούλευσης. Για παράδειγμα, εάν οι τρεις σύμβουλοι εργάστηκαν συνολικά 200 ώρες στο έργο, δημιουργείται ένα τιμολόγιο για τα 22.000 με βάση τον ακόλουθο υπολογισμό:

-   200 ώρες στις 100 ανά ώρα = 20.000
-   έξοδα διαχείρισης 10% = 2.000
-   Συνολικό ποσό τιμολογίου = 22.000

Εάν οι αμοιβές φορολογούνται από έναν πελάτη και επιλέξετε μια ομάδα φόρου πωλήσεων στη σύμβαση έργου, η ομάδα φόρου πωλήσεων καταχωρείται αυτόματα σε έναν κανόνα χρέωσης για χρεώσεις.

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a>Παράδειγμα: Δημιουργία κανόνα χρέωσης για την τιμή του χρόνου και του υλικού

Ο οργανισμός σας, μια εταιρεία συμβούλων λογισμικού, συμφωνεί να παράσχει πέντε τεχνικούς συμβούλους για να εργαστούν σε ένα πρόγραμμα ανάπτυξης λογισμικού για έναν πελάτη για τους επόμενους έξι μήνες. Ο πελάτης συμφωνεί να καταβάλει 150 για κάθε ώρα συμβουλευτικής, συν το κόστος των προμηθειών γραφείου. Ο οργανισμός σας στέλνει ένα τιμολόγιο στον πελάτη στο τέλος κάθε μήνα. 

Όταν ρυθμίζετε τη σύμβαση έργου, συμφωνείτε με την τιμολόγηση του πελάτη κάθε μήνα για το χρόνο και το υλικό του έργου. Μπορείτε να δημιουργήσετε έναν κανόνα χρέωσης, ο οποίος περιλαμβάνει τις εξής πληροφορίες:

-   Η περίοδος σύμβασης είναι έξι μήνες.
-   Ο χρόνος παροχής συμβουλών υπολογίζεται με συντελεστή 150 ανά ώρα.
-   Τα αναλώσιμα γραφείου τιμολογούνται με χρέωση και το συνολικό κόστος για το έργο δεν πρέπει να υπερβαίνει τα 10.000.
-   Μπορείτε να δημιουργήσετε ένα τιμολόγιο πελάτη στο τέλος κάθε ημερολογιακού μήνα κατά τη διάρκεια του έργου.

Κατά τη διάρκεια του πρώτου μήνα, καταγράφονται συνολικά 800 ώρες από τους συμβούλους του έργου. Το κόστος των προμηθειών γραφείου που χρεώνεται στο έργο είναι 2.000. Επομένως, στο τέλος του μήνα, δημιουργείτε ένα τιμολόγιο για 122.000, το οποίο υπολογίζεται ως 800 ώρες με 150 ανά ώρα, συν 2.000 για τα αναλώσιμα γραφείου.





[!INCLUDE[footer-include](../includes/footer-banner.md)]