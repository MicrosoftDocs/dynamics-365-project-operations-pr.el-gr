---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 40, V3
description: Αυτό θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation έκδοση ενημέρωσης 40, V3.
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
ms.openlocfilehash: 25f375ce648eb7d233f6433739832caee351830d
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2022
ms.locfileid: "8588644"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 40, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατή με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 40, V3. Αυτή η έκδοση έχει αριθμό δομής V3.10.61.61 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Φεβρουάριο 2022.

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
