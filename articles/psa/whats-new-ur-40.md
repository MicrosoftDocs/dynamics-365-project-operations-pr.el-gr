---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 40, V3
description: Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation, Έκδοση ενημέρωσης 40, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912792"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 40, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατή με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι νέες ή έχουν αλλάξει για το Project Service Automation, Έκδοση ενημέρωσης 40, V3. Αυτή η έκδοση έχει αριθμό δομής V3.10.61.61 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Φεβρουάριο 2022.

## <a name="update-release-40"></a>Έκδοση κυκλοφορίας 40

### <a name="features"></a>Δυνατότητες
Φάση 1 της αναβάθμισης από Project Service Automation σε Project Operations - Η ελαφριά έκδοση θα κυκλοφορήσει το Φεβρουάριο του 2022 σε όλους τους πελάτες. Για να ελέγξετε την επιλεξιμότητα, δείτε [Αναβάθμιση από Project Service Automation σε Project Operations](upgrade-project-operations-non-stocked.md). Αν η εφαρμογή δεν εμφανίζεται στην παρουσία σας στο Κέντρο διαχείρισης Power Platform, επικοινωνήστε με την υποστήριξη και ζητήστε να ενεργοποιηθεί η σύνδεση στο περιβάλλον σας. Το αίτημα πρέπει να περιλαμβάνει μια λίστα αναγνωριστικών περιβάλλοντος όπου πρέπει να ενεργοποιηθεί το περιβάλλον εργασίας.

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

Διορθώθηκαν τα ακόλουθα θέματα.

**Χρόνος και έξοδα**
- Μια καταχώρηση σημείωσης λείπει όταν μια καταχώρηση χρόνου απορριφθεί ή ακυρωθεί. 

**Πωλήσεις**

- Όταν ενημερώνετε τις εκτιμήσεις κόστους ή πωλήσεων χρησιμοποιώντας τις έτοιμες προσθήκες, επιτρέπεται λανθασμένα να στέλνετε ωφέλιμα φορτία JSON που δεν είναι έγκυρα έξω από το περιβάλλον εργασίας χρήστη.
- Όταν ενημερώνετε τις γραμμές προσφοράς χρησιμοποιώντας τη γρήγορη προβολή, έχετε το δικαίωμα να ενεργοποιήσετε προσφορές.
