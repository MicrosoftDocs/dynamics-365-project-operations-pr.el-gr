---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 28, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 28, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 079679302b2d8dac3074732b2392a7b811ac9711
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280218"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 28, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα. Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x. Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Αυτό το θέμα απαριθμεί τις δυνατότητες και τις επιδιορθώσεις που είναι νέες ή έχουν αλλάξει για το Project Service Automation V3, ενημέρωση έκδοσης 28. Αυτή η έκδοση έχει έναν αριθμό δομής V3.10.46.32 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης τον Ιανουάριο του 2021.

## <a name="update-release-28"></a>Έκδοση κυκλοφορίας 28

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

**Χρόνος και έξοδα**

Διορθώθηκαν τα ακόλουθα ζητήματα:

- Οι χρήστες μπορούν να χρησιμοποιήσουν τη **Μαζική επεξεργασία** για να ενημερώσουν τις καταχωρήσεις ώρας που έχουν εγκριθεί και υποβληθεί.

**Διαχείριση έργων**

Διορθώθηκαν τα ακόλουθα ζητήματα:

- Σε περιπτώσεις όπου το GUID εργασίας ερμηνεύεται ως αριθμός, δεν είναι δυνατό το άνοιγμα εργασιών για επεξεργασία χρησιμοποιώντας την **Επεξεργασία εργασίας** στην κορδέλα της σελίδας **Δομή ανάλυσης εργασίας**.

**Sales**

Διορθώθηκαν τα ακόλουθα ζητήματα:

- Μια εξαίρεση αναφοράς null δημιουργείται όταν καλείται η προσθήκη **GetEstimatesForProject**.
- Η **Επισήμανση ως έτοιμου για τιμολόγηση** στο πλέγμα ορόσημων ενημερώνει μόνο εν μέρει τα χαρακτηριστικά, εκτός από το χαρακτηριστικό **InvoiceStatus** το οποίο ενημερώνεται.



[!INCLUDE[footer-include](../includes/footer-banner.md)]