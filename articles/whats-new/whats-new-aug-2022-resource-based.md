---
title: Τι νέο υπάρχει, Αύγουστος 2022 - Project Operations για σενάρια βάσει πόρων ή μη εφοδιασμένα σενάρια
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τις ενημερώσεις ποιότητας που είναι διαθέσιμες στην έκδοση Αυγούστου 2022 του Microsoft Dynamics 365 Project Operations για μη εφοδιασμένα σενάρια ή σενάρια βασισμένα σε πόρους.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 112dbb98de09ef342c03d122a29cb8025058e47f
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348010"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Τι νέο υπάρχει, Αύγουστος 2022 - Project Operations για σενάρια βάσει πόρων ή μη εφοδιασμένα σενάρια

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Αυτό το άρθρο ισχύει για τα ακόλουθα στοιχεία και εκδόσεις του Microsoft Dynamics 365 Project Operations:

- Project Operations στο περιβάλλον Dataverse έκδοση 4.45.0.53
- Διαχείριση έργων και λογιστική σε περιβάλλον Dynamics 365 Finance έκδοση 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>Ενημερώσεις χαρτών διπλής εγγραφής Project Operations

Δεν υπάρχουν ενημερώσεις για αντιστοιχίσεις διπλής εγγραφής Project Operations σε αυτήν την έκδοση. Για μια τρέχουσα λίστα και εκδόσεις των αντιστοιχίσεων διπλής εγγραφής Project Operations, ανατρέξτε στο [Εκδόσεις αντιστοίχισης διπλήης εγγραφής Project Operations](../environment/resource-dual-write-maps.md).

Να εκτελείτε πάντα την πιο πρόσφατη έκδοση της αντιστοίχησης στο περιβάλλον σας, και να ενεργοποιείτε όλες τις σχετικές αντιστοιχίσεις πινάκων καθώς ενημερώνετε την έκδοση της λύσης Project Operations Dataverse και της λύσης Οικονομικών. Ορισμένες δυνατότητες και δυνατότητες ενδέχεται να μην λειτουργούν σωστά, εάν η πιο πρόσφατη έκδοση του χάρτη δεν ενεργοποιηθεί. Μπορείτε να προβάλλετε την ενεργή έκδοση του χάρτη στη στήλη **Έκδοση** στη σελίδα **Διπλή εγγραφή**. Για να ενεργοποιήσετε μια νέα έκδοση του χάρτη, επιλέξτε **Εκδόσεις χάρτη πίνακα**, επιλέξτε την πιο πρόσφατη έκδοση και, στη συνέχεια, αποθηκεύστε την επιλεγμένη έκδοση. Εάν έχετε προσαρμόσει έναν χάρτη από out-of-box πίνακα, αντιστοιχιστείτε ξανά με τις αλλαγές. Για περισσότερες πληροφορίες, βλ. [Διαχείριση του κύκλου ζωής εφαρμογής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Εάν αντιμετωπίσετε κάποιο πρόβλημα κατά την εκκίνηση του χάρτη, ακολουθήστε τις οδηγίες στο τμήμα [Ζήτημα των στηλών πίνακα που λείπουν σε χάρτες](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) του οδηγού αντιμετώπισης προβλημάτων διπλής εγγραφής.

## <a name="quality-updates"></a>Ενημερώσεις ποιότητας

### <a name="project-operations-on-dataverse"></a>Project Operations στο Dataverse

| Περιοχή δυνατοτήτων | Αριθμός αναφοράς | Ενημέρωση ποιότητας |
| --- | --- | --- |
| Διαχείριση ευκαιριών | 2762089 | Σφάλμα χειρισμού κατά το κλείσιμο της σύμβασης ως χαμένης εάν είναι απενεργοποιημένη η αυτόματη αποθήκευση στον οργανισμό.|

### <a name="project-management-and-accounting-in-finance"></a>Διαχείριση έργων και λογιστικής στα Οικονομικά

Για πληροφορίες σχετικά με τις επιδιορθώσεις σφαλμάτων που περιλαμβάνονται σε αυτήν την ενημέρωση, συνδεθείτε στο Lifecycle Services (LCS) Microsoft Dynamics και προβάλετε το [άρθρο της γνωσιακής βάσης](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
