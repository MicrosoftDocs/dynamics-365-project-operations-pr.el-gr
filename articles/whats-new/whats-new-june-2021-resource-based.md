---
title: Τι νέο υπάρχει, Ιούνιος 2021 - Project Operations για σενάρια βάσει πόρων ή μη εφοδιασμένα σενάρια
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τις ενημερώσεις ποιότητας που είναι διαθέσιμες στην έκδοση Ιουνίου 2021 του Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα.
author: sigitac
ms.date: 06/14/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 28890238f9debb96786a31f66dd9a219f88a5338
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293137"
---
# <a name="whats-new-june-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>Τι νέο υπάρχει, Ιούνιος 2021 - Project Operations για σενάρια βάσει πόρων ή μη εφοδιασμένα σενάρια

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Αυτό το θέμα ισχύει για τα ακόλουθα στοιχεία και τις εκδόσεις του Dynamics 365 Project Operations:

- Project Operations στην έκδοση περιβάλλοντος Dynamics 365 Dataverse 4.11.0.156 ή 4.11.0.164.
- Διαχείριση έργων και λογιστική σε περιβάλλοντα εφαρμογών Finance and Operations έκδοση 10.0.19.

## <a name="features-included-in-this-release"></a>Δυνατότητες που περιλαμβάνονται σε αυτήν την έκδοση

Τα ακόλουθα χαρακτηριστικά περιλαμβάνονται σε αυτήν την έκδοση:

- Δυνατότητα διαγραφής [Γραμμών πρότασης τιμολογίου έργου για σενάρια προσαρμογής](../invoicing/correct-project-invoice-proposals.md).
- Οι γραμμές των ανηγμένων δαπανών απεικονίζουν τα ονόματα υποκατηγορίας στην έκθεση δαπανών [Επανενεργοποιημένες εκθέσεις δαπανών-Νέες δυνατότητες](../expense/expense-reports-reimagined.md#new-features).
- Η μέθοδος πληρωμής είναι διαθέσιμη στο νέο παράθυρο δαπανών κατά τη δημιουργία μιας νέας δαπάνης.

## <a name="project-operations-dual-write-maps-updates"></a>Ενημερώσεις χαρτών διπλής εγγραφής Project Operations

Δεν υπάρχουν ενημερώσεις για αντιστοιχίσεις διπλής εγγραφής Project Operations σε αυτήν την έκδοση. 

Για μια τρέχουσα λίστα και εκδόσεις των αντιστοιχίσεων διπλής εγγραφής Project Operations, ανατρέξτε στο [Εκδόσεις αντιστοίχισης διπλήης εγγραφής Project Operations](../environment/resource-dual-write-maps.md).

Να εκτελείτε πάντα η πιο πρόσφατη έκδοση του χάρτη στο περιβάλλον σας και να ενεργοποιείτε όλες τις σχετικές αντιστοιχίσεις πινάκων καθώς ενημερώνετε την έκδοση λύσης Project Operations Dataverse και έκδοση λύσης εφαρμογών Finance and Operations. Ορισμένες δυνατότητες και ικανότητες ενδεχομένως να μην λειτουργούν σωστά εάν η πιο πρόσφατη έκδοση του χάρτη δεν ενεργοποιηθεί. Μπορείτε να δείτε την ενεργή έκδοση του χάρτη στη σελίδα **διπλής εγγραφής** στη στήλη **Έκδοση**. Ενεργοποιήστε μια νέα έκδοση του χάρτη επιλέγοντας **Εκδόσεις αντιστοίχησης πίνακα**, επιλέγοντας την πιο πρόσφατη έκδοση και, στη συνέχεια, αποθηκεύοντας την επιλεγμένη έκδοση. Εάν έχετε προσαρμόσει έναν έτοιμο χάρτη πίνακα, αντιστοιχιστείτε ξανά τις αλλαγές. Για περισσότερες πληροφορίες, βλ. [Διαχείριση του κύκλου ζωής εφαρμογής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Εάν αντιμετωπίσετε κάποιο πρόβλημα κατά την εκκίνηση της αντιστοίχησης, ακολουθήστε τις οδηγίες στην ενότητα [Ζήτημα στηλών πίνακα που λείπουν σε αντιστοιχήσεις](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) του οδηγού αντιμετώπισης προβλημάτων διπλής εγγραφής.

## <a name="quality-updates"></a>Ενημερώσεις ποιότητας

### <a name="project-operations-on-dataverse"></a>Project Operations στο Dataverse

| **Περιοχή δυνατοτήτων** | **Αριθμός αναφοράς** | **Ενημέρωση ποιότητας** |
| --- | --- | --- |
| Χρέωση και τιμολόγηση | 2281417 | Επιδιορθώθηκε το πρόβλημα σχετικά με την αποτυχία της ενέργειας αυτόματης δημιουργίας τιμολογίου μέσω του χρονοδιαγράμματος τιμολογίων. |
| Χρέωση και τιμολόγηση | 2287835 | Βελτιωμένες επιδόσεις επιβεβαίωσης τιμολογίου. |
| Διαχείριση ευκαιριών | 2222555 | Η δυνατότητα χρέωσης των εκτιμήσεων υλικού πρέπει να αντιγραφεί σωστά στις λεπτομέρειες της γραμμής προσφοράς κατά τη χρήση της **Εισαγωγής από την εκτίμηση έργου**. |
| Διαχείριση ευκαιριών | 2223427 | Πλέον, επιτρέπονται προσαρμογές για την ενέργεια, **GenerateReοτεχνersFromReοtionerScheduleOptions**. |
| Διαχείριση ευκαιριών | 2277528 | Υπολογισμός τιμής ορόσημου σταθερής χρέωσης για γραμμές σύμβασης έργου με πολλούς πελάτες. |
| Προγραμματισμός και παρακολούθηση έργων | 2226110 | Επιδιορθώθηκε το περιστασιακό πρόβλημα με τη λειτουργία **Δημιουργία απαίτησης** στο πλέγμα **Ομάδας έργου**. |
| Προγραμματισμός και παρακολούθηση έργων | 2208109 | Οι χρήστες δεν μπορούν να δημιουργήσουν ένα έργο σε μία νομισματική μονάδα με σχετικές εργασίες σε άλλη νομισματική μονάδα. |
| Προγραμματισμός και παρακολούθηση έργων | 2258228 | Η λίστα των πεδίων που επιτρέπεται να τροποποιηθούν με οντότητες **προγραμματισμού** με χρήση του API χρονοδιαγράμματος έχει ενημερωθεί. |
| Προγραμματισμός και παρακολούθηση έργων | 2293989 | Οι σωστές ρυθμίσεις γλώσσας και οι σωστές τοπικές ρυθμίσεις πρέπει να περνούν στο πλέγμα **εργασιών έργου**. |
| Διαχείριση πόρων | 2220493 | Επιδιορθώνει την εμπειρία χρήστη στο πλέγμα **εργασιών**, κατά την ταχεία επισήμανση μιας αίτησης πόρου ως ολοκληρωμένη. |
| Διαχείριση πόρων | 2330496 | Επιδιορθώθηκε το ζήτημα φόρτωσης του **πίνακα χρονοδιαγράμματος**. (Η ενημέρωση ποιότητας είναι διαθέσιμη στην έκδοση 4.11.0.164) |
| Χρόνος και έξοδα | 2194431 | Το πλέγμα **καταχώρησης ώρας** πρέπει να τηρεί την έναρξη της εβδομάδας, όπως ορίζεται στις **ρυθμίσεις συστήματος**. |
| Χρόνος και έξοδα | 2277311 | Αφού διαγράψετε την τιμή σε ένα κελί στο πλέγμα **καταχώρησης ώρας**, ο δρομέας παραμένει στο πλέγμα. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Διαχείριση έργου και λογιστική στο Dynamics 365 Finance

| Περιοχή δυνατοτήτων | Αριθμός αναφοράς | Ενημέρωση ποιότητας |
| --- | --- | --- |
| Διαχείριση έργου και λογιστική | [552976](https://fix.lcs.dynamics.com/Issue/Details/?bugId=552976) | Οι **σημειώσεις φόρμας** και η **ρύθμιση φόρμας** δεν είναι ορατές στη **ρύθμιση διαχείρισης έργου** στις νομικές οντότητες Οικονομικών οι οποίες είναι ενσωματωμένες στο Project Operations. |
| Διαχείριση έργου και λογιστική | [527970](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527970) | Η προεπιλεγμένη περιγραφή για τον ΦΠΑ είναι κενή όταν ο **Τύπος καταχώρησης** = **Φόρος πωλήσεων** για κουπόνια τιμολογίου έργου. |
| Διαχείριση έργου και λογιστική | [565089](https://fix.lcs.dynamics.com/Issue/Details/?bugId=565089) | Οι διπλές συναλλαγές καταχωρούνται όταν η χρέωση βάσει εργασίας χρησιμοποιείται στο Dataverse με ενσωμάτωση στο Project Operations. |
| Διαχείριση έργου και λογιστική | [566869](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566869) | Το ποσοστό ολοκλήρωσης στην αναγνώριση εσόδων είναι λανθασμένο κατά τη χρήση του Project Operations. |
| Διαχείριση έργου και λογιστική | [568107](https://fix.lcs.dynamics.com/Issue/Details/?bugId=568107) | Η αύξηση των εσόδων διπλασιάζεται σε ένα εκκρεμές τιμολόγιο πωλητή σε ένα ενσωματωμένο σενάριο του Project Operations. |
| Διαχείριση έργου και λογιστική | [572370](https://fix.lcs.dynamics.com/Issue/Details/?bugId=572370) | Αδύνατη η καταχώρηση του ημερολογίου ενοποίησης όταν ο κανόνας προφίλ εσόδων έχει οριστεί στην ρύθμιση **ομάδας**. |
| Διαχείριση έργου και λογιστική | [573596](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573596) | Ένα τιμολόγιο αγοράς δεν μπορεί να καταχωρηθεί για εντολές αγοράς έργου που έχουν γραμμές με πολλές μονάδες μέτρησης. |
| Διαχείριση έργου και λογιστική | [573637](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573637) | Η προεπιλεγμένη οικονομική διάσταση σε ένα έργο δεν μπορεί να ενημερωθεί χρησιμοποιώντας την οντότητα δεδομένων έργων **V2**. |
| Διαχείριση έργου και λογιστική | [577211](https://fix.lcs.dynamics.com/Issue/Details/?bugId=577211) | Η διεργασία δέσμης για τη δημιουργία εκτιμήσεων έργου απαιτεί υπερβολικά μεγάλο χρονικό διάστημα για να ολοκληρωθεί. |
| Διαχείριση έργου και λογιστική | [582329](https://fix.lcs.dynamics.com/Issue/Details/?bugId=582329) | Η διαγραφή μιας σύμβασης, διαγράφει και τη διεύθυνση που σχετίζεται με τον πελάτη. |
| Ταξίδι και έξοδα | [514930](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514930) | Η συνθήκη ροής εργασίας για την έγκριση της έκθεσης δαπανών δεν αξιολογείται σωστά. |
| Ταξίδι και έξοδα | [519304](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519304) | Η πολιτική της έκθεσης δαπανών δεν αξιολογεί σωστά το αναγνωριστικό έργου. |
| Ταξίδι και έξοδα | [522463](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522463) | Η ενέργεια **Διαχωρισμός σε προσωπικά για συναλλαγές διεταιρικών δαπανών** δεν λειτουργεί σωστά. |
| Ταξίδι και έξοδα | [534702](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534702) | Οι αιτιολογήσεις μιας γραμμής έκθεσης δαπανών διαγράφονται τυχαία όταν διαγράφονται συγκεκριμένες αιτήσεις μετακίνησης. Αυτό συμβαίνει όταν το αναγνωριστικό εγγραφής της έκθεσης δαπανών και η αίτηση μετακίνησης είναι τα ίδια. |
| Ταξίδι και έξοδα | [544368](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544368) | Υπάρχει ένα πρόβλημα στην εφαρμογή για κινητές συσκευές Δαπάνες όταν το πεδίο **Αναγνωριστικό έργου** απαιτείται στις πολιτικές εκθέσεων δαπανών. |
| Ταξίδι και έξοδα | [545331](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545331) | Δεν είναι δυνατή η επεξεργασία των διεταιρικών δαπανών που σχετίζονται με ένα έργο. Αντ' αυτού, εμφανίζεται το ακόλουθο μήνυμα σφάλματος: "Η αναφορά αντικειμένου δεν έχει οριστεί σε παρουσία αντικειμένου". |
| Ταξίδι και έξοδα | [548659](https://fix.lcs.dynamics.com/Issue/Details/?bugId=548659) | Μετά την καταχώρηση της έκθεσης δαπανών, η εσφαλμένη νομισματική μονάδα και το λανθασμένο ποσό εμφανίζονται στο δευτερεύον καθολικό τράπεζας. |
| Ταξίδι και έξοδα | [558336](https://fix.lcs.dynamics.com/Issue/Details/?bugId=558336) | Έχουν γίνει βελτιώσεις στη δυνατότητα *Διαγραφή συναλλαγών με πιστωτική κάρτα*.  |
| Ταξίδι και έξοδα | [525070](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525070) | Ο φόρος πωλήσεων που περιλαμβάνεται σε μια αναφορά δαπανών δεν υπολογίζεται ομοιόμορφα όταν μια διαφορετική νομισματική μονάδα αναφοράς καθορίζεται σε μια νομική οντότητα. |
| Ταξίδι και έξοδα | [527779](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527779) | Η απόδοση επηρεάζει την προσθήκη μιας νέας δαπάνης μετακίνησης σε μετρητά. |
| Ταξίδι και έξοδα | [537841](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537841) | Οι κανόνες πολιτικής δαπανών δεν ενεργοποιούνται σε έκθεση δαπανών. |
| Ταξίδι και έξοδα | [566386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566386) | Η αποστολή μιας νέας κοινόχρηστης κατηγορίας με χρήση του Πλαισίου διαχείρισης δεδομένων καταργεί όλες τις υποκατηγορίες για όλες τις κοινόχρηστες κατηγορίες. |
| Ταξίδι και έξοδα | [574131](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574131) | Όταν δημιουργείτε μια γραμμή δαπανών και μετά επιλέγετε μια κατηγορία, εμφανίζεται το ακόλουθο μήνυμα σφάλματος: "Ο συνδυασμός DOM της ομάδας φόρων πωλήσεων και STD ομάδας φόρου πωλήσεων στοιχείου δεν είναι έγκυρος." |
| Ταξίδι και έξοδα | [574900](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574900) | Υπάρχουν ζητήματα συγχρονισμού στην εφαρμογή Δαπάνες για κινητές συσκευές. |