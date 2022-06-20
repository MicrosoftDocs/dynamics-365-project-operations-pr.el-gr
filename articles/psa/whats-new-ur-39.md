---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 39, V3
description: Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation, Έκδοση ενημέρωσης 39, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/20/2022
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
ms.openlocfilehash: d5b5938762d98acaead9e26c47bce07e0059faf6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922452"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-39-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 39, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατή με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι νέες ή έχουν αλλάξει για το Project Service Automation, Έκδοση ενημέρωσης 39, V3. Αυτή η έκδοση έχει αριθμό δομής V3.10.60.170 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Ιανουάριο του 2022.

## <a name="update-release-39"></a>Έκδοση κυκλοφορίας 39

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

Διορθώθηκαν τα ακόλουθα θέματα.

**Γενικός**

- Έχουν γίνει πολλές βελτιώσεις στο χάρτη τοποθεσίας για την αραβική μετάφραση.

**Διαχείριση έργων**

- Παρουσιάζεται ένα σφάλμα όταν αλλάζετε το διαχειριστή έργου σε χρήστη που είναι ήδη μέλος της ομάδας στο έργο.

**Πωλήσεις**

- Ο κάτοχος του **τιμοκαταλόγου σύμβασης έργου** είναι εσφαλμένος όταν δημιουργείται αυτόματα ο τιμοκατάλογος. 
- Η έναρξη ισχύος της ημερομηνίας ενός τιμοκαταλόγου δεν τηρείται όταν ο τιμοκατάλογος εφαρμόζεται στην παράμετρο έργου.
- Η μονάδα σύμβασης ενδεχομένως να μην έχει τη σωστή προεπιλεγμένη τιμή κατά την επεξεργασία δύο ξεχωριστών προσφορών.
