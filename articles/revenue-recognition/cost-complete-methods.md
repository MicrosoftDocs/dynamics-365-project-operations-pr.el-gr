---
title: Μέθοδοι κόστους για ολοκλήρωση
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τις μεθόδους που χρησιμοποιούνται για τον υπολογισμό του κόστους για την ολοκλήρωση ενός έργου.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 39c10673afd04ad7d4a94a01211c2f9d335a02c2
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8920290"
---
# <a name="cost-to-complete-methods"></a>Μέθοδοι κόστους για ολοκλήρωση

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τις μεθόδους που χρησιμοποιούνται για τον υπολογισμό του κόστους για την ολοκλήρωση ενός έργου. Υπάρχουν πολλές μέθοδοι που μπορείτε να χρησιμοποιήσετε για τον υπολογισμό του κόστους για την ολοκλήρωση ενός έργου. 

Όταν δημιουργείτε μια εκτίμηση για ένα έργο, στη σελίδα **Δημιουργία εκτίμησης**, στο πεδίο **Μέθοδος κόστους για ολοκλήρωση**, μπορείτε να επιλέξετε μία από τις παρακάτω μεθόδους για να ολοκληρώσετε το κόστος.

| Μέθοδος κόστους για ολοκλήρωση    | Περιγραφή                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Συνολικό κόστος - πραγματική τιμή            | Εισαγάγετε το κόστος εκτίμησης με μη αυτόματο τρόπο στα πεδία **Συνολικό κόστος** ή **Συνολική ποσότητα** χρησιμοποιώντας το κουμπί **Εκτίμηση κόστους** στη **σελίδα εκτίμησης**. Το σύστημα αφαιρεί το πραγματικό κόστος από τα σύνολα που καταχωρήσατε. Το σύνολο είναι το κόστος ολοκλήρωσης του έργου. Αυτή η μέθοδος δεν χρησιμοποιεί τις εκτιμήσεις δαπανών και τις αναθέσεις πόρων που έχουν καταχωρηθεί στο Project Operations που έχει δημιουργηθεί εντός του Microsoft Dataverse. Το συνολικό κόστος ή η συνολική ποσότητα μπορούν να ενημερωθούν με μη αυτόματο τρόπο, ανάλογα με τις ανάγκες.  |
| Συνολική πρόβλεψη - πραγματική τιμή        | Οι αναθέσεις πόρων και οι εκτιμήσεις εξόδων χρησιμοποιούνται για τον καθορισμό του συνολικού ποσού πρόβλεψης έργου. Το πραγματικό κόστος συγκρίνεται με αυτήν την πρόβλεψη για τον υπολογισμό του κόστους που θα ολοκληρωθεί.                                                                                                                                                                                                                                                                          |
| Ως προηγούμενη εκτίμηση         | Εδώ χρησιμοποιούνται οι ίδιες μέθοδοι εκτίμησης που χρησιμοποιήθηκαν την προηγούμενη περίοδο. Αυτή η μέθοδος απαιτεί ένα μοντέλο πρόβλεψης, εάν η προηγούμενη περίοδος απαιτεί ένα μοντέλο πρόβλεψης.                                                                                                                                                                                                                                                                                                                           |
| Ορισμός κόστους για ολοκλήρωση στο μηδέν | Συνήθως χρησιμοποιείται πριν από την κατάργηση του έργου εκτίμησης, αυτή η μέθοδος ταιριάζει με τις συνολικές εκτιμήσεις με καταχωρημένες πραγματικές συναλλαγές και απαλείφει τη στήλη **Κόστος για ολοκλήρωση**. Όταν ολοκληρωθεί, το αποτέλεσμα θα είναι πάντα 100 τοις εκατό. Για κάθε γραμμή κόστους που δημιουργείτε, το πλαίισο ελέγχου **Πρόβλεψη** δεν είναι επιλεγμένο και η συνολική εκτίμηση αντιγράφεται από την προηγούμενη εκτίμηση κόστους. Η πραγματική κατανάλωση για την περίοδο εκτίμησης αφαιρείται από το κόστος για την ολοκλήρωση του έργου.              |
| Από το πρότυπο κόστους           | Η μέθοδος κόστους για ολοκλήρωση που έχει οριστεί στο πρότυπο κόστους που συσχετίζεται με το επιλεγμένο έργο εκτίμησης.                                                                                                                                                                                                                                                                                                                                                                          |


[!INCLUDE[footer-include](../includes/footer-banner.md)]