---
title: Στάδια έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τα στάδια του έργου που είναι διαθέσιμα στο Microsoft Dynamics Project Operations (Λειτουργίες έργου).
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: b11c67ebd21fdf423eeae2db8154f26787c2e64f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897946"
---
# <a name="project-stages"></a>Στάδια έργου

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Τα στάδια έργου σχεδιάζονται ώστε να αντικατοπτρίζουν την κατάσταση του έργου καθώς εξελίσσεται. Οι προσαρμογές μπορούν να χρησιμοποιηθούν για την αυτόματη ενημέρωση των σταδίων με τις ροές επιχειρηματικών διαδικασίας, Power Automate ή με επεκτάσεις προσθήκης.

Τα ακόλουθα στάδια καθορίζονται στην προεπιλεγμένη ροή επιχειρηματικής διαδικασίας:

- Δημιουργία
- Προσφορά
- Πρόγραμμα
- Παράδοση
- Ολοκλήρωση
- Κλείσιμο  

## <a name="new"></a>Δημιουργία

Όταν δημιουργείτε ένα έργο, το στάδιο έργου έχει οριστεί στην επιλογή **Νέο**. Εάν το έργο δημιουργήθηκε από ένα πρότυπο, μπορεί να έχει δεδομένα χρονοδιαγράμματος, εκτίμησης και ομάδας. Διαφορετικά, πρόκειται για ένα περίγραμμα του έργου και πρέπει να καταχωρηθούν τα υπόλοιπα στοιχεία.

## <a name="quote"></a>Προσφορά

Όταν συσχετίζετε ένα έργο σε μια προσφορά ή το δημιουργείτε από μια προσφορά, το στάδιο του έργου έχει οριστεί στην επιλογή **Προσφορά** και ενημερώνονται επίσης οι εκτιμώμενες ημερομηνίες έναρξης και λήξης. Ενώ το έργο βρίσκεται στο στάδιο της **Προσφοράς**, η καρτέλα **Πωλήσεις** στη σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της προσφοράς.

## <a name="plan"></a>Πρόγραμμα

Όταν κερδίζετε μια προσφορά που έχει συσχετιστεί με ένα έργο και το έργο μετακινείται στη φάση **Σύμβαση**, το στάδιο έργου ενημερώνεται σε **Πρόγραμμα**. Ενώ το έργο βρίσκεται στο στάδιο **Πρόγραμμα**, η σελίδα **Οντότητα έργου** εμφανίζει λεπτομέρειες της σύμβασης.

## <a name="deliver"></a>Παράδοση

Όταν ολοκληρωθεί το σχέδιο έργου και είστε έτοιμοι να ξεκινήσετε το έργο, ο υπεύθυνος έργου θα πρέπει να ενημερώσει το στάδιο του έργου σε **Παράδοση** για να δείξει ότι το έργο έχει ξεκινήσει.

## <a name="complete"></a>Ολοκληρώθηκε 

Όταν ολοκληρωθεί η εργασία για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Ολοκληρώθηκε**. Με την ενημέρωση του σταδίου του έργου σε **Ολοκληρώθηκε**, ο υπεύθυνος έργου δηλώνει ότι η εργασία έχει ολοκληρωθεί 100 τοις εκατό, αλλά ότι το έργο διατηρείται ανοιχτό έτσι ώστε να είναι δυνατή η καταγραφή τυχόν εκκρεμών καταχωρήσεων χρόνου ή εξόδων.

## <a name="close"></a>Κλείσιμο

Όταν καταγραφούν όλες οι συναλλαγές για το έργο, ο υπεύθυνος έργου μπορεί να ενημερώσει το στάδιο σε **Κλείσιμο**. Σε αυτό το σημείο, καμία συναλλαγή δεν μπορεί να καταγραφεί και το έργο έχει οριστεί ως "μόνο για ανάγνωση".

