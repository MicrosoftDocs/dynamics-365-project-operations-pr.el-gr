---
title: Ημερήσιες αποζημιώσεις
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τους κανόνες ημερήσιας αποζημίωσης που χρησιμοποιούνται στη διαχείριση δαπανών.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 7d1c4ac7781cb711e2cc0d09606d422b4dd554f3
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908168"
---
# <a name="per-diems"></a>Ημερήσιες αποζημιώσεις

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_


Η ημερήσια αποζημίωση είναι ένα επίδομα που καταβάλλεται σε έναν εργαζόμενο ο οποίος ταξιδεύει για εργασία. Στη διαχείριση εξόδων, μπορείτε να δημιουργήσετε κανόνες ημερήσιας αποζημίωσης για διάφορες καταστάσεις που αφορούν ταξίδια. Οι τιμές ημερήσιας αποζημίωσης βασίζονται στην εποχή του χρόνου, στην τοποθεσία ταξιδίου ή και στα δύο. Όταν δημιουργείτε έναν κανόνα ημερήσιας αποζημίωσης, μπορείτε να προσδιορίσετε ότι ένα ποσοστό της ημερήσιας αποζημίωσης θα παρακρατηθεί εάν ο εργαζόμενος λάβει δωρεάν γεύματα ή υπηρεσίες. Μπορείτε, επίσης, να ορίσετε έναν ελάχιστο και μέγιστο αριθμό ωρών όπου θα ισχύει η τιμή της ημερήσιας αποζημίωσης για τα ταξίδια του εργαζομένου.

## <a name="configuration"></a>Ρύθμιση παραμέτρων 

1. Για να προσθέσετε τοποθεσίες ημερήσιας αποζημίωσης, μεταβείτε στη **Ρύθμιση παραμέτρων** > **Υπολογισμοί και κωδικοί** > **Τοποθεσίες ημερήσιας αποζημίωσης**.
2. Για κάθε μία από τις τοποθεσίες που προστίθενται παραπάνω, επιλέξτε μια τιμή και ένα νόμισμα ημερήσιας αποζημίωσης που θα ισχύουν για μια συγκεκριμένη ημερομηνία άφιξης και αναχώρησης για το ξενοδοχείο, τα γεύματα και άλλες δαπάνες. Οι τιμές και τα νομίσματα ημερήσιας αποζημίωσης διαμορφώνονται στις **Ρυθμίσεις παραμέτρων** > **Υπολογισμοί και κωδικοί** > **Ημερήσιες αποζημιώσεις**.
3. Στη σελίδα **Τοποθεσίες ημερήσιας αποζημίωσης** ρυθμίστε τα επίπεδα ανά ποσοστό ημερήσιας αποζημίωσης. Τα επίπεδα ανά ποσοστό ημερήσιας αποζημίωσης σάς δίνουν τη δυνατότητα να ορίσετε το ποσοστό διαίρεσης μιας ημερήσιας αποζημίωσης για το ξενοδοχείο, τα γεύματα και άλλα έξοδα. 
4. Για να καθορίσετε τη μείωση του ποσοστού γεύματος για πρωινό, μεσημεριανό γεύμα ή δείπνο, ενημερώστε τα πεδία στη σελίδα **Παράμετροι διαχείρισης εξόδων** στην καρτέλα **Ημερήσια αποζημίωση**. 
    
## <a name="submit-expenses-using-per-diem"></a>Υποβολή εξόδων με τη χρήση ημερήσιων αποζημιώσεων
Για να υποβάλετε τα έξοδα χρησιμοποιώντας τις ημερήσιες αποζημιώσεις, χρησιμοποιήστε την κατηγορία εξόδων **Ημερήσια αποζημίωση** όταν δημιουργείτε μια αναφορά εξόδων. Καταχωρείστε την **Ημερήσια αποζημίωση από την ημερομηνία**, την **Ημερήσια αποζημίωση έως** και την **Τοποθεσία ημερήσιας αποζημίωσης**. Το ποσό θα υπολογιστεί με βάση τις τιμές ημερήσιας αποζημίωσης για την επιλεγμένη θέση και η μείωση γεύματος θα υπολογιστεί με βάση τα επίπεδα ανά ποσοστό ημερήσιας αποζημίωσης.
