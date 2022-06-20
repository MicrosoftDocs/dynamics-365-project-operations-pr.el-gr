---
title: Ενοποίηση διπλής εγγραφής Project Operations
description: Αυτό το άρθρο παρέχει μια επισκόπηση της ενοποίησης διπλής εγγραφής του Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d365a036f96ff4f7b14107b43e8c6b70df0b5362
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927972"
---
# <a name="project-operations-dual-write-integration-overview"></a>Επισκόπηση ενοποίησης διπλής εγγραφής Project Operations

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Το Project Operations χρησιμοποιεί [δυνατότητες διπλής εγγραφής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) για τον συγχρονισμό δεδομένων στα Microsoft Dataverse και Dynamics 365 Finance.

Η εικόνα που ακολουθεί δείχνει τον τρόπο συγχρονισμού των δεδομένων στο πλαίσιο αυτής της ενοποίησης μεταξύ Dataverse και Οικονομικών.

![Επισκόπηση ροών δεδομένων του Project Operations.](./media/ProjectOperationsFlows.jpg)

Το Project Operations στο Dataverse παρέχει ένα σύγχρονο περιβάλλον εργασίας χρήστη (UI) και εύκολη επεκτασιμότητα χωρίς κώδικα/χαμηλό κώδικα, χρησιμοποιώντας τις δυνατότητες του Power Platform. Οι διαχειριστές έργου, οι διαχειριστές πόρων, τα μέλη ομάδας έργου και άλλα άτομα προσκηνίου, εκτελούν τις δραστηριότητές τους στο Project Operations στο Dataverse.

Το Project Operations στα οικονομικά παρέχουν υποστήριξη για τη λογιστική έργων και την αναγνώριση των εσόδων. Το Project Operations κάνει προσθήκες στο οικονομικό πλαίσιο των Οικονομικών για τον υπολογισμό του φόρου πωλήσεων, τις νομισματικές ισοτιμίες, τις αναφορές οικονομικών διαστάσεων και πολλά άλλα. Οι εμπειρίες του Λογιστή έργου βασίζονται κυρίως στα Οικονομικά.

Η ενοποίηση του Project Operations αποτελείται από το παρακάτω στοιχείο ενοποίησης:


- [Ρύθμιση Project Operations και ρύθμιση παραμέτρων ενοποίησης δεδομένων](resource-dual-write-setup-integration.md) 
- [Εκτιμήσεις έργου και πραγματικές τιμές](resource-dual-write-estimates-actuals.md)
- [Τιμολόγια έργου](resource-dual-write-project-invoice.md)
- [Διαχείριση εξόδων](resource-dual-write-expense.md)
- [Τιμολόγιο προμηθευτή](resource-dual-write-vendor-invoice.md)
