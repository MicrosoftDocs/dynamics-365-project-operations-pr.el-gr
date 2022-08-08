---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 45, V3
description: Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation, Έκδοση ενημέρωσης 45, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
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
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169156"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 45, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατή με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το άρθρο παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι νέες ή έχουν αλλάξει για το Project Service Automation, Έκδοση ενημέρωσης 45, V3. Αυτή η έκδοση έχει αριθμό έκδοσης V3.10.76.168 και είναι γενικά διαθέσιμη μέσω μιας αυτο-ενημέρωσης τον Ιούλιο του 2022.

## <a name="update-release-45"></a>Έκδοση κυκλοφορίας 45

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

Διορθώθηκαν τα ακόλουθα θέματα.

**Πωλήσεις**

- Οι χρήστες δεν μπορούν να δημιουργήσουν με επιτυχία τιμολόγια αφού προσπαθήσουν να δημιουργήσουν ένα τιμολόγιο χωρίς μη χρεωμένες πωλήσεις, εάν βλέπουν επίσης την ίδια παρουσία της σελίδας και δεν την ανανεώσουν.

**Χρόνος και έξοδα**

- Όταν είναι ενεργοποιημένες οι μοντέρνες εγκρίσεις και εγκρίνεται μια ανακληθείσα έγκριση έργου, το στάδιο καρτέλας ενημερώνεται εσφαλμένα σε **Το αίτημα ανάκλησης εγκρίθηκε**.
- Όταν οι μοντέρνες εγκρίσεις ενεργοποιούνται και οι Ροές cloud είναι ανενεργές, η διαδικασία έγκρισης δεν είναι επιτυχής και οι χρήστες που πραγματοποιούν υποβολή ή έγκριση δεν ειδοποιούνται.
