---
title: Μετεγκατάσταση πλήρως τιμολογημένων ορόσημων χρέωσης κατά τη περικοπή
description: Αυτό το άρθρο εξηγεί τον τρόπο μετεγκατάστασης ορόσημων χρέωσης προκαθορισμένης τιμής που έχουν τιμολογηθεί στον πελάτη για ανοικτές συμβάσεις έργου πριν από την ημερομηνία έναρξης κυκλοφορίας.
author: sigitac
ms.date: 01/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 05cd71f9860b5698e3a26bc72660b0b2044206c8
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028702"
---
# <a name="migrate-fully-invoiced-billing-milestones-at-cutover"></a>Μετεγκατάσταση πλήρως τιμολογημένων ορόσημων χρέωσης κατά τη περικοπή

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

## <a name="scenario"></a>Σενάριο

Η Contoso μεταβαίνει σε παραγωγική λειτουργία με το Microsoft Dynamics 365 Project Operations για σενάρια πόρων/μη αποθέματος. Ως μέρος των δραστηριοτήτων περικοπής, η ομάδα υλοποίησης πρέπει να μετεγκαταστήσει τις ανοιχτές συμβάσεις έργου από το παλιό σύστημα. Ορισμένες από τις συμβάσεις έργου περιλαμβάνουν γραμμές σύμβασης που χρησιμοποιούν τη μέθοδο χρέωσης προκαθορισμένης τιμής και έχουν ήδη τιμολογηθεί μερικώς στον τελικό πελάτη. Η ομάδα υλοποίησης πρέπει να μετεγκαταστήσει αυτά τα ορόσημα χρέωσης ως **τιμολόγιο πελάτη που έχει καταχωρηθεί**, επειδή πρέπει να συμπεριληφθούν στη συνολική τιμή της σύμβασης για λόγους αναγνώρισης των εσόδων. Ωστόσο, τα υπόλοιπα πελατών σε εισπρακτέους λογαριασμούς και γενικό καθολικό δεν πρέπει να επηρεαστούν.

## <a name="solution"></a>Λύση

### <a name="prerequisites"></a>Προϋποθέσεις

- Πρέπει να εγκατασταθεί το Dynamics 365 Finance 10.0.24 ή μεταγενέστερη έκδοση.
- Το περιβάλλον όπου θα ολοκληρωθούν τα βήματα μετεγκατάστασης πρέπει να βρίσκεται σε λειτουργία συντήρησης. Δεν πρέπει να εκτελούνται άλλες δραστηριότητες κατά τη μετεγκατάσταση των ορόσημων.
- Τα βήματα μετεγκατάστασης πρέπει να ακολουθούνται ακριβώς όπως περιγράφεται εδώ και μπορούν να χρησιμοποιηθούν μόνο για τη δραστηριότητα περικοπής. Η Microsoft δεν υποστηρίζει άλλη χρήση αυτής της δυνατότητας.

### <a name="create-a-cutover-version-of-the-project-operations-integration-contract-line-milestones-dual-write-map"></a>Δημιουργήστε μια έκδοση περικοπής για την αντιστοίχιση διπλής εγγραφής των ορόσημων της γραμμής σύμβασης ολοκλήρωσης Project Operations 

1. Βεβαιωθείτε ότι η αντιστοίχιση προορισμού για την οντότητα **Ορόσημα γραμμής σύμβασης ολοκλήρωσης Project Operations** είναι ενημερωμένη. 

    1. Στο Finance, μεταβείτε στο **Διαχείριση δεδομένων** \> **Οντότητες δεδομένων** και επιλέξτε την οντότητα **ορόσημα της γραμμής σύμβασης ενσωμάτωσης Project Operations**. 
    2. Επιλέξτε **Τροποποίηση αντιστοιχίσεων προορισμού**. 
    3. Στη σελίδα **Αντιστοίχιση σταδιοποίησης σε προορισμό**, επιλέξτε **Δημιουργία αντιστοίχισης** και, στη συνέχεια, επιβεβαιώστε ότι θέλετε να δημιουργήσετε την αντιστοίχιση.

2. Σταματήστε και ανανεώστε την αντιστοίχιση διπλής εγγραφής **Ορόσημα της γραμμής σύμβασης ολοκλήρωσης Project Operations** (**msdyn\_contractlinescheduleofvalues**). 

    1. Μεταβείτε στη **Διαχείριση δεδομένων** \> **Διπλή εγγραφή**, επιλέξτε την αντιστοίχιση και ανοίξτε τις λεπτομέρειες της. 
    2. Επιλέξτε **Διακοπή** και περιμένετε έως ότου το σύστημα σταματήσει την αντιστοίχιση. 
    3. Επιλέξτε **Ανανέωση πινάκων**.

3. Προσθέστε μια αντιστοίχιση για την κατάσταση συναλλαγής.

    1. Επιλέξτε **Προσθήκη αντιστοίχισης**.
    2. Στη νέα γραμμή, στη στήλη **Εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων**, επιλέξτε το πεδίο **TRANSSTATUS \[TRANSSTATUS\]**.
    3. Στη στήλη **Microsoft Dataverse**, επιλέξτε **msdyn\_invoicestatus \[Invoice status\]**.
    4. Στη στήλη **Τύπος αντιστοίχισης**, επιλέξτε το δεξιό βέλος (**\>**).
    5. Στο παράθυρο διαλόγου που εμφανίζεται, στο πεδίο **Κατεύθυνση συγχρονισμού**, επιλέξτε **Dataverse σε εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων**.
    6. Επιλέξτε **Προσθήκη μετασχηματισμού**.
    7. Στο πεδίο **Τύπος μετασχηματισμού**, επιλέξτε **ValueMap**.
    8. Επιλέξτε **Προσθήκη αντιστοίχισης τιμής**.
    9. Στο αριστερό πεδίο καταχωρίστε **4**. Στο δεξιό πεδίο καταχωρίστε **192350001**. 
    10. Επιλέξτε **Αποθήκευση** και, στη συνέχεια, κλείστε το παράθυρο διαλόγου.

4. Επιλέξτε **Αποθήκευση ως** για να αποθηκεύσετε την έκδοση την αντιστοίχιση διπλής εγγραφής. 
5. Στο τμήμα παραθύρου **Προσθήκη πίνακα**, στο πεδίο **Εκδότης**, επιλέξτε **Προεπιλεγμένος εκδότης**.
6. Στο πεδίο **Έκδοση**, εισαγάγετε την έκδοση.
7. Στο πεδίο **Περιγραφή**, εισαγάγετε μια σημείωση σχετικά με αυτήν την έκδοση περικοπής της αντιστοίχισης. 
8. Επιλέξτε **Αποθήκευση**.
9. Ξεκινήστε την αντιστοίχιση.

### <a name="migrate-invoiced-milestones-to-the-dataverse-environment"></a>Μετεγκατάσταση τιμολογημένων ορόσημων στο περιβάλλον Dataverse

1. Στο περιβάλλον Project Operations Dataverse, δημιουργήστε ορόσημα με κατάσταση τιμολογίου **Έτοιμο για τιμολόγηση**. Σε αυτό το σημείο, μην μετεγκαταστήσετε ορόσημα που δεν έχουν τιμολογηθεί.

    > [!NOTE]
    > Προτού μετεγκαταστήσετε τα ορόσημα χρέωσης, βεβαιωθείτε ότι οι οικονομικές διαστάσεις που σχετίζονται με τη γραμμή σύμβασης έργου έχουν οριστεί σύμφωνα με τα αναμενόμενα. Δεν είναι δυνατή η επεξεργασία των οικονομικών διαστάσεων μετά την ολοκλήρωση της μετεγκατάστασης.

2. Μετά τη μετεγκατάσταση όλων των ορόσημων, σταματήστε τις παρακάτω αντιστοιχίσεις διπλής εγγραφής:

    - Ορόσημα γραμμής σύμβασης ενοποίησης Project Operations (msdyn\_contractlinescheduleofvalues)
    - Πραγματικές τιμές ενοποίησης Project Operations (msdyn\_actuals)
    - Πρόταση τιμολογίου έργου V2 (τιμολόγια)

    Για να σταματήσετε τις αντιστοιχίσεις, ακολουθήστε τα παρακάτω βήματα:

    1. Στο Finance, μεταβείτε στη **Διαχείριση δεδομένων** \> **Διπλή εγγραφή**, επιλέξτε μια αντιστοίχιση και ανοίξτε τις λεπτομέρειες της.
    2. Επιλέξτε **Διακοπή** και περιμένετε έως ότου το σύστημα σταματήσει την αντιστοίχιση.

3. Στο περιβάλλον Project Operations Dataverse, δημιουργήστε και επιβεβαιώστε προ-τιμολόγια για τα ορόσημα χρέωσης. 

    1. Στο χάρτη τοποθεσίας, μεταβείτε στις συμβάσεις έργου, επιλέξτε τις συμβάσεις και, στη συνέχεια, επιλέξτε **Δημιουργία τιμολογίων**.
    2. Αφού δημιουργηθούν τα τιμολόγια, ανοίξτε τα από το μενού **Τιμολόγια** στον χάρτη τοποθεσίας και, στη συνέχεια, επιλέξτε **Επιβεβαίωση**.

    Αυτό το βήμα δημιουργεί τις απαιτούμενες καρτέλες στο περιβάλλον Dataverse. Ωστόσο, δεν επηρεάζει τα οικονομικά και τους εισπρακτέους λογαριασμούς, επειδή οι προηγούμενες απαριθμημένες αντιστοιχίσεις διπλής εγγραφής διακόπηκαν.

4. Αφού επιβεβαιωθούν όλα τα προ-τιμολόγια, επιστρέψτε όλες τις αντιστοιχίσιες διπλής εγγραφής στην αρχική τους κατάσταση.

    1. Ενημερώστε την έκδοση την αντιστοίχιση διπλής εγγραφής **Ορόσημων της γραμμής σύμβασης ολοκλήρωσης Project Operations** (**msdyn\_contractlinescheduleofvalues**) πίσω στην αρχική. 
    2. Επιλέξτε την αντιστοίχιση διπλής εγγραφής στη λίστα αντιστοιχίσεων, **Έκδοση αντιστοίχισης πίνακα** και, στη συνέχεια, επιλέξτε την αρχική έκδοση της αντιστοίχισης πίνακα.
    3. Επιλέξτε **Αποθήκευση**.
    4. Επανεκκινήστε τις παρακάτω αντιστοιχίσεις διπλής εγγραφής:

        - Ορόσημα γραμμής σύμβασης ενοποίησης Project Operations (msdyn\_contractlinescheduleofvalues)
        - Πραγματικές τιμές ενοποίησης Project Operations (msdyn\_actuals)
        - Πρόταση τιμολογίου έργου V2 (τιμολόγια)

Τα ορόσημα έχουν μετεγκατασταθεί και το σύστημα είναι έτοιμο για τα επόμενα βήματα στη δραστηριότητα περικοπής.