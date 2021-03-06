---
title: Επισκόπηση εγκρίσεων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την εργασία με εγκρίσεις στο Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961166"
---
# <a name="approvals-overview"></a>Επισκόπηση εγκρίσεων

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Οι υποβολές χρόνου και εξόδων μετακινούνται μέσω μιας ροής εργασιών έγκρισης. Μετά την έγκριση των καταχωρήσεων, οι συναλλαγές καταγράφονται στις πραγματικές τιμές ή γίνεται κράτηση του χρόνου στο χρονοδιάγραμμα.

## <a name="approvals-workflow"></a>Ροή εργασιών εγκρίσεων
Όταν δημιουργείτε και υποβάλλετε μια καταχώρηση χρόνου ή εξόδων, δημιουργείται μια εγγραφή έγκρισης. Ο υπεύθυνος έγκρισης έργου ή ο διευθυντής σας ελέγχουν και εγκρίνουν την καταχώρισή σας. Εάν η εγγραφή σχετίζεται με ένα έργο, όταν εγκριθεί, θα δημιουργηθούν οι πραγματικές τιμές. Με αυτόν τον τρόπο, το κόστος και η χρέωση πρέπει να παρακολουθούνται. 

## <a name="approve-an-entry"></a>Έγκριση καταχώρησης
Η φόρμα **Εγκρίσεις** σάς δίνει τη δυνατότητα να κάνετε εναλλαγή μεταξύ διαφορετικών προβολών ώστε να μπορείτε να προβάλλετε τους διαφορετικούς τύπους εγκρίσεων.
  
1. Μεταβείτε στη φόρμα **Εγκρίσεις** και επιλέξτε **Έξοδα**, **Ώρα** ή **Ανακλήσεις**.
2. Εξετάστε κάθε έγκριση και επιλέξτε αυτές που θέλετε να εγκρίνετε.
3. Επιλέξτε **Έγκριση** για να εγκρίνετε τις επιλεγμένες καταχωρήσεις.
Το σύστημα θα επεξεργαστεί αυτές τις καταχωρήσεις και θα δημιουργήσει πραγματικές τιμές ή μια κράτηση.

## <a name="reject-an-entry"></a>Απόρριψη καταχώρησης
Ως υπεύθυνος έγκρισης έργου, μπορεί να χρειαστεί να στείλετε ξανά μια καταχώρηση σε ένα χρήστη για διόρθωση.
  
1. Μεταβείτε στη φόρμα **Εγκρίσεις** και επιλέξτε την καταχώρηση που θα απορρίψετε. 
2. Επιλέξτε **Απόρριψη**.
3. Προαιρετικό - Προσθέστε ένα σχόλιο στο παράθυρο διαλόγου **Σχόλια απόρριψης** για να ενημερώσετε το χρήστη γιατί απορρίφθηκε η καταχώρηση.
4. Επιλέξτε **OK**. Η εγγραφή θα επιστραφεί στο χρήστη.
  
## <a name="recall-entries"></a>Ανάκληση καταχωρήσεων
Σε κάποιο σημείο, μπορεί να χρειαστεί να ανακαλέσετε μια καταχώρηση που υποβλήθηκε. Εάν η εγγραφή δεν έχει εγκριθεί, θα επιστραφεί αμέσως. Μια εγκεκριμένη εγγραφή, ωστόσο, μπορεί να έχει σημαντική επίπτωση. Ο υπεύθυνος έγκρισης έργου υποχρεούται να εγκρίνει την ανάκληση προκειμένου να αντιστρέψει τη συναλλαγή στις πραγματικές τιμές.

## <a name="specify-project-approvers"></a>Καθορισμός υπεύθυνων έγκρισης έργου
Κάθε έργο έχει ορισμένα μέλη ομάδας έργου. Μπορείτε να καθορίσετε τα μέλη της ομάδας που θα είναι επίσης υπεύθυνοι έγκρισης έργου.

1. Μεταβείτε στη φόρμα **Έργα** και ανοίξτε το έργο από τη λίστα.
2. Στην καρτέλα **Ομάδα**, επιλέξτε το μέλος της ομάδας που θα είναι υπεύθυνος έγκρισης έργου και, στη συνέχεια, κάντε κλικ στην επιλογή **Επεξεργασία**.
3. Ορίστε το πεδίο **Υπεύθυνος έγκρισης έργου** σε **Ναι**.
4. Επιλέξτε **Αποθήκευση**.
5. Επαναλάβετε τα βήματα 2-4 για να προσθέσετε επιπλέον υπεύθυνους έγκρισης έργου.

## <a name="configure-the-users-manager"></a>Ρύθμιση παραμέτρων του διαχειριστή χρήστη

1. Μεταβείτε στην επιλογή **Ρυθμίσεις** > **Ασφάλεια** > **Χρήστες**.
2. Επιλέξτε το χρήστη στον οποίο αναθέτετε έναν διευθυντή και στην περιοχή **Πληροφορίες οργανισμού**, επιλέξτε το διευθυντή από τη λίστα. 
3. Επιλέξτε **Αποθήκευση**.


