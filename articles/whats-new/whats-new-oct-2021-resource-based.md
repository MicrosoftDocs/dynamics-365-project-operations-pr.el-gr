---
title: Τι νέα υπάρχουν, Οκτώβριος 2021 - Λειτουργίες Έργου για σενάρια βασισμένα σε πόρους / μη εφοδιασμένα σενάρια
description: Αυτή θέμα παρέχει πληροφορίες σχετικά με τις ενημερώσεις ποιότητας που είναι διαθέσιμες στην έκδοση Οκτωβρίου 2021 των Λειτουργιών Έργου για μη εφοδιασμένα σενάρια ή σενάρια βασισμένα σε πόρους.
author: sigitac
ms.date: 10/06/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 078869ad01a23bac1108629c5f532ba57a2967e9
ms.sourcegitcommit: f37502a50cabdaf736aeba149feb5f8288e23df7
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/04/2021
ms.locfileid: "7753292"
---
# <a name="whats-new-october-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>Τι νέα υπάρχουν, Οκτώβριος 2021 - Λειτουργίες Έργου για σενάρια βασισμένα σε πόρους / μη εφοδιασμένα σενάρια

*Ισχύει για: Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα*

Αυτό το θέμα ισχύει για τα ακόλουθα στοιχεία και τις εκδόσεις του Dynamics 365 Project Operations:

   - Λειτουργίες Έργου στο περιβάλλον Microsoft Dataverse έκδοση 4.25.0.91
   - Διαχείριση έργου και λογιστικής στο περιβάλλον Dynamics 365 Finance έκδοση 10.0.21

## <a name="features-included-in-this-release"></a>Δυνατότητες που περιλαμβάνονται σε αυτήν την έκδοση

Τα ακόλουθα χαρακτηριστικά περιλαμβάνονται σε αυτήν την έκδοση:

- [Οι παραγγελίες αγοράς έργων](../procurement/non-stocked-materials-project-purchase-orders.md) μπορούν πλέον να χρησιμοποιηθούν για διαχειριζόμενες ανά τμήμα/κεντρικά διαχειριζόμενες προμήθειες έργων.
- [Η κράτηση προμηθευτή](../procurement/vendor-retention-overview.md) σάς επιτρέπει να κρατείτε ένα τμήμα των πληρωμών προς προμηθευτές.

## <a name="project-operations-dual-write-maps-updates"></a>Ενημερώσεις χαρτών διπλής εγγραφής Project Operations

Δεν υπάρχουν ενημερώσεις για αντιστοιχίσεις διπλής εγγραφής Project Operations σε αυτήν την έκδοση. Για μια τρέχουσα λίστα και εκδόσεις των αντιστοιχίσεων διπλής εγγραφής Project Operations, ανατρέξτε στο [Εκδόσεις αντιστοίχισης διπλήης εγγραφής Project Operations](../environment/resource-dual-write-maps.md).

Να εκτελείτε πάντα την πιο πρόσφατη έκδοση της αντιστοίχησης στο περιβάλλον σας και να ενεργοποιείτε όλες τις σχετικές αντιστοιχίσεις πινάκων καθώς ενημερώνετε την έκδοση της λύσης Project Operations Dataverse και της λύσης Οικονομικών. Ορισμένες δυνατότητες και ικανότητες ενδεχομένως να μην λειτουργούν σωστά εάν η πιο πρόσφατη έκδοση του χάρτη δεν ενεργοποιηθεί. Μπορείτε να δείτε την ενεργή έκδοση του χάρτη στη σελίδα διπλής εγγραφής στη στήλη Έκδοση. Για να ενεργοποιήσετε μια νέα έκδοση του χάρτη, επιλέξτε Εκδόσεις χάρτη πίνακα, επιλέξτε την πιο πρόσφατη έκδοση και, στη συνέχεια, αποθηκεύστε την επιλεγμένη έκδοση. Εάν έχετε προσαρμόσει έναν έτοιμο χάρτη πίνακα, αντιστοιχιστείτε ξανά τις αλλαγές. Για περισσότερες πληροφορίες, βλ. [Διαχείριση του κύκλου ζωής εφαρμογής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Εάν αντιμετωπίσετε κάποιο πρόβλημα κατά την εκκίνηση του χάρτη, ακολουθήστε τις οδηγίες στο τμήμα [Ζήτημα των στηλών πίνακα που λείπουν σε χάρτες](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) του οδηγού αντιμετώπισης προβλημάτων διπλής εγγραφής.

## <a name="quality-updates"></a>Ενημερώσεις ποιότητας

### <a name="project-operations-on-dataverse"></a>Project Operations στο Dataverse

| **Περιοχή δυνατοτήτων** | **Αριθμός αναφοράς** | **Ενημέρωση ποιότητας** |
| --- | --- | --- |
| Χρέωση και τιμολόγηση | 2209402 | Διορθώστε τις επικυρώσεις που εμπόδιζαν τα ποσά διατήρησης να τιμολογηθούν όταν μια σύμβαση έργου έχει επιβεβαιωθεί. |
|   Διαχείριση ευκαιριών | 2227414 | Τα πεδία **Προϊόν**, **Εγγραφή Σε** και **IsProductOverriden** αντιγράφονται στις λεπτομέρειες γραμμής προσφοράς και γραμμής σύμβασης. |
| Χρέωση και τιμολόγηση | 2338357 | Η νομισματική μονάδα στο αρχείο καταγραφής χρήσης υλικού πρέπει να είναι η προεπιλεγμένη από τη νομισματική μονάδα του έργου, όταν επιλέγεται το έργο. |
| Χρόνος και έξοδα | 2414777 | Πρέπει να είναι δυνατή η ακύρωση μιας έγκρισης όταν η καταχώρηση δαπανών ή χρόνου έχει περισσότερες από μία συσχετισμένες εγκρίσεις έργου. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Διαχείριση έργου και λογιστική στο Dynamics 365 Finance

| Περιοχή δυνατοτήτων | Αριθμός αναφοράς | Ενημέρωση ποιότητας |
| --- | --- | --- |
| Διαχείριση έργου και λογιστική | [412077](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D412077&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020681298%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=JT2OvagELTPqep4rOiFTwGYF80KkgSHgBJmd%2BHBBgA8%3D&amp;reserved=0) | Με την άδεια πρόσβασης του διευθυντή αγοράς σε μία οικονομική οντότητα φιλτράρεται επίσης η πρόσβαση σε όλα τα έργα σε όλες τις νομικές οντότητες. |
| Διαχείριση έργου και λογιστική | [555604](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D555604&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020701214%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=NGAT/5r0sezqdisYP%2BDzyFDDi5f9gyrr5ZhJZaDLV0k%3D&amp;reserved=0) | Ο αποκλεισμός εκτίμησης αποτυγχάνει όταν ενεργοποιείται η δυνατότητα **ενεργοποίηση της νομισματικής μονάδας σύμβασης έργου για υπολογισμό εκτίμησης**. |
| Διαχείριση έργου και λογιστική | [564701](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D564701&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020731079%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=IyhrFb59YBXjNpJdtPhlEDxoYiFCTrqzQtKZsBZk2DM%3D&amp;reserved=0) | [FRA] Ο φόρος υπό όρους δεν υπολογίζεται σωστά για την τελευταία πληρωμή όταν εφαρμόστηκε κράτηση προμηθευτή και προπληρωμή σε ένα τιμολόγιο παραγγελίας αγοράς. |
| Διαχείριση έργου και λογιστική | [569250](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D569250&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020741035%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=YcB6z9MvvtiyT9d8g2GkHXDUcNfnPdxlYsHblbk%2BCXs%3D&amp;reserved=0) | Οι καταχωρήσεις WIP στο γενικό καθολικό δημοσιεύονται με εσφαλμένο ποσό. |
| Διαχείριση έργου και λογιστική | [581167](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D581167&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020989941%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=9UjX3lX/DOJOPiz%2BlYVge5F3Tpbb%2BUBaN7PVXkpwYJE%3D&amp;reserved=0) | Η αναφορά τιμολογίου έργου παρακάμπτει γραμμές. |
| Διαχείριση έργου και λογιστική | [598810](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D598810&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021408104%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=f2oJYnmjpfUiIKvF6qfLsBcfTjoSOq955%2B87%2BSIh0Io%3D&amp;reserved=0) | Υπάρχει ένα ζήτημα με την δέσμη καταχώρησης τιμολογίου έργου που επεξεργάζεται και καταχωρεί την πρόταση τιμολογίου ακόμα και αν δεν έχουν δημιουργηθεί οι γραμμές τιμολογίου. |
| Διαχείριση έργου και λογιστική | [578970](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D578970&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021876048%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=JMg%2BIRbLiSKeIXN/JArWC3hSGFhNhabERbuKzGBKCC8%3D&amp;reserved=0) | Ενημέρωση για τη δημιουργία μιας εργασίας δέσμης εκτίμησης έργου για την υποστήριξη της εκτέλεσης πολλαπλών δευτερευουσών εργασιών. |
| Διαχείριση έργου και λογιστική | [586034](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D586034&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021895962%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=MRGsdBRM5spFKDJZ/IjrAoWy%2BGTyFVyUU7SCfFJSj6g%3D&amp;reserved=0) | Οι συναλλαγές κουπονιών δεν εξισορροπούν ως "XX/XX/XXXX" (λογιστικό νόμισμα: 0,00 - νόμισμα αναφοράς: 0,01). |
| Διαχείριση έργου και λογιστική | [596669](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D596669&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021955698%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=IpJrV7LW0CegdNrRXfDqBhLEsy8tlSvlaipvZBQFZVg%3D&amp;reserved=0) | Ο αριθμός απαλλαγής από το φόρο για μια νομική οντότητα δεν εμφανίζεται σε ένα εκτυπωμένο τιμολόγιο έργου. |
| Διαχείριση έργου και λογιστική | [598109](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D598109&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021975611%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=erjkqXSdKwjU62xNiVEJomzc5JoiiC9U7f6ofrv4KGE%3D&amp;reserved=0) | Η ρύθμιση της συνεχόμενης ακολουθίας αριθμού κατά την καταχώρηση μιας εκτίμησης δεν υποστηρίζεται μετά την εφαρμογή της Γνωσιακής βάσης 4619395. |
| Διαχείριση έργου και λογιστική | [602677](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D602677&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642022015436%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=4TBJC6dKbgZxWQTlyDkTm%2BzHpL%2BJx5ZcueNWkMJfUK4%3D&amp;reserved=0) | Η τιμή που αντιστρέφεται από το WIP από την καταχώρηση τιμολογίου είναι διαφορετική από την αρχική καταχωρημένη τιμή WIP από την καταχώρηση χρόνου. |
| Διαχείριση έργου και λογιστική | [602728](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D602728&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642022015436%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=Ux5tLxoBzA%2BJtbf5MhLB63/GNJqYcBg8PH4tncXLTsM%3D&amp;reserved=0) | Οι συναλλαγές κουπονιών δεν εξισορροπούνται σωστά λόγω ενός ζητήματος δημοσίευσης με τα τιμολογούμενα έσοδα έργου σε υποθέσεις κράτησης που εφαρμόζονται. |
| Διαχείριση έργου και λογιστική | [607324](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D607324&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642022065219%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=I/SwbTsPpFvMkxLIK7JpligW%2B4nlObh3nCCSppVGvhE%3D&amp;reserved=0) | Οι εκτιμήσεις έργων δημιουργούνται μόνο για μία περίοδο. |
| Ταξίδι και έξοδα | [551911](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D551911&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020701214%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=fDFL3GM5jXJAzIzxwRlOIaq3/ytSHXnpIzGsC4Jjphg%3D&amp;reserved=0) | Οι πολιτικές αναπλήρωσης ταξιδιών αγνοούνται για την έγκριση της ροής εργασιών χωρίς σφάλματα. |
| Ταξίδι και έξοδα | [563752](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D563752&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020731079%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=SVrkNdniaVfhOjc3Brf1gtrFv3SJpPNQ4JYOGnCOxlQ%3D&amp;reserved=0) | Το αναγνωριστικό έργου της γραμμής δαπανών, ο χρεώσιμος αριθμός και ο αριθμός δραστηριότητας, δεν αποθηκεύονται στην εφαρμογή εξόδων για κινητές συσκευές. |
| Ταξίδι και έξοδα | [569458](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D569458&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020750990%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=cC33gCOlM8aa3jR5Hy1Hubf5bszsu2YWwraLLrIYCYk%3D&amp;reserved=0) | Το πεδίο **Συνημμένη απόδειξη** ορίζεται σε **Ναι** ακόμη και εάν στη γραμμή δαπανών δεν έχει επισυναφθεί απόδειξη. |
| Ταξίδι και έξοδα | [571334](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D571334&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020760950%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=Y6dd19CzWyWPa%2BItpWXBEgUuSx8evJxth6VslSRMYsg%3D&amp;reserved=0) | Παρουσιάζεται ένα μήνυμα σφάλματος όταν προσπαθείτε να αλλάξετε την κατηγορία δαπανών σε **Προσωπικά**. |
| Ταξίδι και έξοδα | [572783](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D572783&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020770904%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=nugD/4Rj3d8CNanZf%2BY3vNm9aRqHoh5vF/bHFZD9UxE%3D&amp;reserved=0) | Αφού μια συναλλαγή με πιστωτική κάρτα διαιρεθεί σε μια αναφορά εξόδων, δεν μπορείτε να επεξεργαστείτε τα γονικά έξοδα ή να επισυνάψετε μια απόδειξη. |
| Ταξίδι και έξοδα | [574252](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D574252&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020790818%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=uKYIlgBpKju4jBH%2BK8GXVKCgi6kxSG1AxXVvF75WsbA%3D&amp;reserved=0) | Η πολιτική εξόδων για ενδοεταιρικές συναλλαγές με αναγνωριστικό έργου δεν λειτουργεί σωστά. |
| Ταξίδι και έξοδα | [574489](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D574489&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020800774%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=ErBwfDvDtWWzEJP3STHd5kzPjTe7%2B4nCeG02kH64dWU%3D&amp;reserved=0) | Η καταχωρημένη ημερομηνία λείπει για τις καταχωρημένες αναφορές εξόδων. |
| Ταξίδι και έξοδα | [574504](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D574504&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642020800774%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=SeW6L68CNpJ86TJ2aNqLZoTMq5PHRfu3542mNkKqf%2Bg%3D&amp;reserved=0) | Υπάρχουν θέματα μεθόδου πληρωμής στην εφαρμογή εξόδων για κινητές συσκευές. |
| Ταξίδι και έξοδα | [584799](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D584799&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021129331%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=4Q%2B/R9wPra2P/%2BEk63qgSenyNoJMa5OJsBv2Nn9s%2B%2Bo%3D&amp;reserved=0) | Μια ανάθεση μετακίνησης που έχει δημιουργηθεί για έναν εργαζόμενο μπορεί να χρησιμοποιηθεί για την αναφορά δαπανών ενός άλλου εργαζόμενου και μπορεί να χρησιμοποιήσει την αναπλήρωση μετακίνησης πριν από την ημερομηνία πληρεξούσιου. |
| Ταξίδι και έξοδα | [586023](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D586023&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021169156%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=d9Kmf1ng415Uw0U4aQ5N%2B0RboRmjDW1S2lt91rG9ofc%3D&amp;reserved=0) | Όταν δημιουργείται μια δαπάνη, η αλλαγή των τιμών των οικονομικών διαστάσεων δεν ενημερώνεται σωστά στο επίπεδο λογιστικής κατανομής στο χώρο εργασίας **Διαχείρισης εξόδων**. |
| Ταξίδι και έξοδα | [586081](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D586081&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021179116%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=LlWjcIANIl1gudmiD4WIsluKkF21w9EgVC5uDvBOzg4%3D&amp;reserved=0) | Η κατάσταση έγκρισης κύριας γραμμής εξόδων δεν συγχρονίζεται με την κατάσταση έγκρισης ροής εργασιών γραμμής στοιχείου. |
| Ταξίδι και έξοδα | [590544](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D590544&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021318495%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=MolkGywocB%2BG404npaOv7fcfunnlDUGgAYFOcw8OlKg%3D&amp;reserved=0) | Παρουσιάζεται σφάλμα κατά την καταχώρηση μιας αναφοράς εξόδων όταν είναι ενεργοποιημένη η **ανάκτηση φόρου** στις παραμέτρους διαχείρισης εξόδων. |
| Ταξίδι και έξοδα | [564851](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D564851&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021856138%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=YBsBJdzH%2BqbGzq07u7WILEs%2Bi5Ap6WYzqWnpGWcI4Ac%3D&amp;reserved=0) | Ένας πληρεξούσιος δεν μπορεί να διαγράψει έγγραφα εξόδων για έναν υπάλληλο που έχει αποχωρήσει. |
| Ταξίδι και έξοδα | [587306](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D587306&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021905919%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=TbWDuK1sHY//jTw%2BmehJG3M3N3feEl2oRkTMTkqWOVE%3D&amp;reserved=0) | Η διαγραφή μιας γραμμής εξόδων απαιτεί πολύ χρόνο και επηρεάζει την απόδοση. |
| Ταξίδι και έξοδα | [600455](https://nam06.safelinks.protection.outlook.com/?url=https://fix.lcs.dynamics.com/Issue/Details/?bugId%3D600455&amp;data=04%7C01%7Cjespers%40microsoft.com%7C1ece6f38724a460c13bc08d96784b455%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637654642021995524%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&amp;sdata=MH0sIRbAKhNNyAgYZzO9NovWHM7ZWKsoZYqXCIVHJ5A%3D&amp;reserved=0) | Το **TrvExpTrans** προκαλεί μια ορφανή καρτέλα **TaxUncommitted** διαγράφοντας μόνο την **SourceDocumentLine**. |