---
title: Εκτιμήσεις πόρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο υπολογισμού των εκτιμήσεων πόρων στο Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928568"
---
# <a name="resource-estimates"></a>Εκτιμήσεις πόρων

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Οι εκτιμήσεις πόρων προέρχονται από την προσπάθεια με χρονική κλιμάκωση που καθορίζεται στη δομή ανάλυσης εργασίας μαζί με τις εφαρμοστέες διαστάσεις τιμολόγησης. Συνήθως, ο υπολογισμός είναι **τιμή/ώρα για κάθε ρόλο x ώρες.** Η προσπάθεια με χρονική κλιμάκωση για κάθε πόρο αποθηκεύεται στην καρτέλα ανάθεσης πόρου. Η τιμολόγηση αποθηκεύεται σε έναν προκαθορισμένο τιμοκατάλογο. Η μετατροπή μονάδας εφαρμόζεται με βάση τον ισχύοντα τιμοκατάλογο.

![Εκτιμήσεις πόρων](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>Προεπιλογές τιμής κόστους και νομίσματος κόστους

Οι τιμές κόστους είναι προεπιλεγμένες από την οργανωτική μονάδα.

## <a name="default-bill-rate-and-sales-currency"></a>Προεπιλογές συντελεστή χρέωσης και νομίσματος πωλήσεων

Οι τιμές πώλησης εφαρμόζονται μία φορά ανά συμφωνία. Η ιεραρχία για την προεπιλογή τιμοκαταλόγου προς πώληση έχει ως εξής:

1. Εταιρεία
2. Πελάτης
3. Προσφορά/σύμβαση
