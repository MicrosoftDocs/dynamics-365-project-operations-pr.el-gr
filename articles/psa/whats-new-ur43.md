---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 43, V3
description: Αυτό θέμα παραθέτει τις δυνατότητες και τις επιδιορθώσεις που είναι διαθέσιμες στο Microsoft Dynamics 365 Project Service Automation έκδοση ενημέρωσης 43, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/04/2022
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
ms.openlocfilehash: fcf18a24b3bc354a16a415368063133743e79696
ms.sourcegitcommit: 7e419a5f73f80fa887084e3b212c90586fc397dd
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/05/2022
ms.locfileid: "8710006"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 43, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Έχουμε τη χαρά να ανακοινώσουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Microsoft Dynamics 365 Project Service Automation. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Είναι συμβατό με το Dynamics 365 9.x. Για να κάνετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε τη σελίδα του Κέντρου διαχείρισης για λύσεις Dynamics 365 Online και εγκαταστήστε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).

Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 43, V3. Αυτή η έκδοση έχει αριθμό δομής V3.10.74.200 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Μαΐου 2022.

## <a name="update-release-43"></a>Έκδοση κυκλοφορίας 43

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

Διορθώθηκαν τα ακόλουθα θέματα.


**Χρόνος και έξοδα**

- Κατά την εισαγωγή καταχωρήσεων χρόνου από κρατήσεις ή αναθέσεις πόρων, η αναφορά στον σχετικό πόρο με δυνατότητα κράτησης δεν διατηρείται.
- Όταν το πλέγμα καταχώρησης χρόνου αναπτύσσεται σε πλήρη οθόνη, η περιήγηση στο πλέγμα με το πλήκτρο Tab δεν λειτουργεί.
- Όταν υποβάλετε μια καταχώρηση χρόνου που δημιουργήθηκε από άλλο χρήστη, το πεδίο **Υποβλήθηκε από** συμπληρώνεται εσφαλμένα με το χρήστη που δημιούργησε το φύλλο χρόνου.
