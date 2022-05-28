---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 42, V3
description: Αυτό θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation έκδοση ενημέρωσης 42, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 32cb7a4c5fc29d5c0dcec37dd395ae69037435a2
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2022
ms.locfileid: "8589196"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 42, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατή με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 42, V3. Αυτή η έκδοση έχει αριθμό δομής V3.10.73.61 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Απριλίου 2022.

## <a name="update-release-42"></a>Έκδοση κυκλοφορίας 42

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

Διορθώθηκαν τα ακόλουθα θέματα.

**Χρόνος και έξοδα**

- Όταν απορριφθεί ένα φύλλο χρόνου, ο χρήστης που το έχει απορρίψει έχει αναγνωριστεί λανθασμένα ως **Σύστημα**.
- Όταν γίνεται εισαγωγή των εγγραφών, λείπει η τιμή **Κατηγορία πόρου**.
- Οι υπεύθυνοι έγκρισης έργου μπορούν να εγκρίνουν έργα που έχουν υποβληθεί, όταν τα δικαιώματά τους δεν έχουν οριστεί ειδικά σε **Μπορεί να εγκρίνει**.

**Πωλήσεις**

- Όταν οι πραγματικές τιμές καταγράφονται σε εργασίες μη ριζικού επιπέδου, το πραγματικό κόστος είναι εσφαλμένα συγκεντρωτικό.
