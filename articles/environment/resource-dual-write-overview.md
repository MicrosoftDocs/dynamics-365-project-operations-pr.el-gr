---
title: Ενοποίηση διπλής εγγραφής Project Operations
description: Αυτό το θέμα παρέχει μια επισκόπηση της ενοποίησης διπλής εγγραφής Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955658"
---
# <a name="project-operations-dual-write-integration-overview"></a>Επισκόπηση ενοποίησης διπλής εγγραφής Project Operations

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Το Project Operations χρησιμοποιεί [δυνατότητες διπλής εγγραφής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) για το συγχρονισμό δεδομένων μεταξύ Microsoft Dataverse και Dynamics 365 Finance.

Η εικόνα που ακολουθεί δείχνει τον τρόπο συγχρονισμού των δεδομένων στο πλαίσιο αυτής της ενοποίησης μεταξύ Dataverse και Οικονομικών.

![Επισκόπηση ροών δεδομένων Project Operations](./media/ProjectOperationsFlows.jpg)

Το Project Operations στο Dataverse παρέχει ένα σύγχρονο περιβάλλον εργασίας χρήστη (UI) και εύκολη επεκτασιμότητα χωρίς κώδικα/χαμηλό κώδικα, χρησιμοποιώντας τις δυνατότητες του Power Platform. Οι διαχειριστές έργου, οι διαχειριστές πόρων, τα μέλη ομάδας έργου και άλλα άτομα προσκηνίου, εκτελούν τις δραστηριότητές τους στο Project Operations στο Dataverse.

Το Project Operations στα οικονομικά παρέχουν υποστήριξη για τη λογιστική έργων και την αναγνώριση των εσόδων. Το Project Operations κάνει προσθήκες στο οικονομικό πλαίσιο των Οικονομικών για τον υπολογισμό του φόρου πωλήσεων, τις νομισματικές ισοτιμίες, τις αναφορές οικονομικών διαστάσεων και πολλά άλλα. Οι εμπειρίες του Λογιστή έργου βασίζονται κυρίως στα Οικονομικά.

Η ενοποίηση του Project Operations αποτελείται από το παρακάτω στοιχείο ενοποίησης:


- [Ρύθμιση Project Operations και ρύθμιση παραμέτρων ενοποίησης δεδομένων](resource-dual-write-setup-integration.md) 
- [Εκτιμήσεις έργου και πραγματικές τιμές](resource-dual-write-estimates-actuals.md)
- [Τιμολόγια έργου](resource-dual-write-project-invoice.md)
- [Διαχείριση εξόδων](resource-dual-write-expense.md)
- [Τιμολόγιο προμηθευτή](resource-dual-write-vendor-invoice.md)
