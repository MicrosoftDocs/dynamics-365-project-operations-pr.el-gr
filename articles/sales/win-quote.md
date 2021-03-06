---
title: Κλείσιμο προσφοράς
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με το κλείσιμο προσφορών στο Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3c429fa14b4b95420c67a91a6a59af7db2660f68
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898891"
---
# <a name="close-a-quote"></a>Κλείσιμο προσφοράς

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Μια προσφορά έργου μπορεί να κλείσει ως κερδισμένη ή χαμένη. Επειδή οι λειτουργίες ενεργοποίησης και αναθεώρησης δεν υποστηρίζονται σε προσφορές στο Microsoft Dynamics 365 Project Operations, μπορείτε να κλείσετε μια προσχέδια προσφορά.

## <a name="close-a-quote-as-won"></a>Κλείσιμο μιας προσφοράς ως κερδισμένης

Το κλείσιμο μιας προσφοράς έργου ως κερδισμένης θα ορίσει την κατάσταση της προσφοράς σε **Κλειστή** και αιτιολογία κατάστασης θα είναι **Κερδισμένη**. Το κλείσιμο των προσφορών τις καθιστά μόνο για ανάγνωση και δημιουργείται ένα προσχέδιο σύμβασης έργου με όλες τις πληροφορίες προσφοράς. Επειδή δεν είναι δυνατό το άνοιγμα μιας κλειστής προσφοράς, πριν κλείσετε μια προσφορά, το παράθυρο διαλόγου επιβεβαίωσης θα επιβεβαιώσει τις αλλαγές σας.

Η σύμβαση έργου που δημιουργήθηκε από μια προσφορά έργου διατίθεται επίσης στη λειτουργική μονάδα "Διαχείριση έργου και λογιστική" του Project Operations. Εάν μια σύμβαση έργου δεν έχει αντιστοιχιστεί σε ένα έργο σε καμία από τις γραμμές της, αυτή η σύμβαση έργου θα καταστεί διαθέσιμη ως ανενεργή σύμβαση έργου και θα ενεργοποιηθεί μόλις ένα έργο αντιστοιχιστεί τουλάχιστον σε μία από τις γραμμές σύμβασης.

Εάν η προσφορά είναι συνημμένη σε μια ευκαιρία, οποιεσδήποτε άλλες προσφορές έργου στην ευκαιρία κλείνουν αυτόματα ως χαμένες.

### <a name="financial-impact-of-closing-a-quote-as-won"></a>Οικονομικός αντίκτυπος του κλεισίματος μιας προσφοράς ως κερδισμένης

Εάν έχουν σημειωθεί πραγματικές τιμές για το χρόνο που καταγράφηκε σε ένα έργο ενώ εξακολουθεί να είναι προσαρτημένο σε ένα προσχέδιο προσφοράς, καταγράφεται μόνο το κόστος του χρόνου ή της δαπάνης. Αφού κλείσει μια προσφορά ως κερδισμένη, η εφαρμογή θα επαναφέρει το κόστος αντιστρέφοντας τα παλιότερα πραγματικά δεδομένα κόστους και θα δημιουργήσει εκ νέου νέες πραγματικές τιμές κόστους. Η εφαρμογή θα επεξεργαστεί αυτά τα πραγματικά δεδομένα κόστους με βάση τη μέθοδο χρέωσης της συσχετισμένης γραμμή σύμβασης έργου. Εάν ο κωδικός κόστους αναφέρεται σε μια γραμμή σύμβασης χρόνου και υλικού, το σύστημα θα δημιουργήσει αυτόματα τα αντίστοιχα πραγματικά ποσά που δεν έχουν τιμολογηθεί για την ημερομηνία κλεισίματος της προσφοράς και τη δημιουργία της σύμβασης έργου. Εάν ο κωδικός κόστους αναφέρεται σε μια γραμμή σύμβασης προκαθορισμένης τιμής, η εφαρμογή θα σταματήσει την επεξεργασία των πραγματικών τιμών κόστους με βάση τους κανόνες διαίρεσης χρέωσης για τους πελάτες της σύμβασης έργου.

Όλα τα πραγματικά δεδομένα είναι διαθέσιμα στη λειτουργική μονάδα "Διαχείριση έργου και λογιστική" για τον λογιστή έργου για αναθεώρηση, ενημέρωση και καταχώρηση στη γενική λογιστική. 

## <a name="close-a-quote-as-lost"></a>Κλείσιμο μιας προσφοράς ως χαμένης

Το κλείσιμο μιας προσφοράς έργου ως χαμένης θα ορίσει την κατάσταση της προσφοράς σε **Κλειστή** και αιτιολογία κατάστασης θα είναι **Χαμένη**. Το κλείσιμο της προσφοράς την καθιστά μόνο για ανάγνωση. Επειδή δεν είναι δυνατό το άνοιγμα μιας κλειστής προσφοράς, πριν κλείσετε μια προσφορά, το παράθυρο διαλόγου επιβεβαίωσης θα επιβεβαιώσει τις αλλαγές σας.

Εάν η προσφορά έργου που έχει κλείσει ως χαμένη έχει ένα έργο που αναφέρεται σε οποιαδήποτε από τις γραμμές του, αυτό το έργο επισημαίνεται επίσης ως κλειστό και οι κρατήσεις πόρων από εκείνη την ημέρα και μετά ακυρώνονται.

> [!NOTE]
> Στο Project Operations, η κλείσιμο μιας προσφοράς ως κερδισμένης ή χαμένης δεν θα επηρεάσει την εν λόγω κατάσταση της ευκαιρίας, η οποία θα παραμείνει ανοιχτή μέχρι να κλείσει με μη αυτόματο τρόπο.
