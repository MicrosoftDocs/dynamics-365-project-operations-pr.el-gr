---
title: Ενοποίηση τιμολογίων έργου
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με την ενοποίηση διπλής εγγραφής του Project Operations για τιμολόγηση πελατών.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 61f16ebdbabd6545c09d8d7bd82d99b85dc09975
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029024"
---
# <a name="project-invoice-integration"></a>Ενοποίηση τιμολογίων έργου

Αυτό το άρθρο παρέχει πληροφορίες σχετικά με την ενοποίηση διπλής εγγραφής του Project Operations για τιμολόγηση πελατών.

Στο Project Operations, ο διαχειριστής έργου διαχειρίζεται την καθυστέρηση στη χρέωση του έργου και δημιουργεί ένα προτιμολόγιο για τον πελάτη στο Microsoft Dataverse. Με βάση αυτό το προτιμολόγιο, ο υπάλληλος εισπρακτέων λογαριασμών ή ο λογιστής του έργου δημιουργεί ένα τιμολόγιο πελάτη. Με την ενοποίηση διπλής εγγραφής εξασφαλίζεται ότι οι λεπτομέρειες του προ‑τιμολογίου συγχρονίζονται με τις εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων. Μετά την καταχώρηση του τιμολογίου πελάτη, το σύστημα ενημερώνει τις σχετικές πραγματικές τιμές του έργου στο Dataverse με τη λεπτομέρεια λογιστικής. Το παρακάτω γραφικό παρέχει μια εννοιολογική επισκόπηση υψηλού επιπέδου για αυτήν την ενοποίηση.

   ![Ενοποίηση τιμολογίων έργου.](./media/DW5Invoicing.png)

Αφού ο διαχειριστής έργου επιβεβαιώσει το προ-τιμολόγιο στο Dataverse, οι πληροφορίες κεφαλίδας προ-τιμολογίου συγχρονίζονται με τις εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων χρησιμοποιώντας την αντιστοίχιση πίνακα διπλής εγγραφής, **Πρόταση τιμολογίου έργου V2 (τιμολόγια)**. Πρόκειται για μια μονόδρομη ενοποίηση από το Dataverse στις εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων. Δεν υποστηρίζεται η δημιουργία ή διαγραφή προτάσεων τιμολογίου έργου απευθείας στις εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων.

Η επιβεβαίωση τιμολογίου στο Dataverse ενεργοποιεί επίσης την επιχειρηματική λογική για τη δημιουργία καρτελών που σχετίζονται με τη χρέωση στην οντότητα **Πραγματικές τιμές**. Αυτές οι καρτέλες συγχρονίζονται με τις οικονομικές και επιχειρηματικές δραστηριότητες χρησιμοποιώντας την αντιστοίχιση πίνακα διπλής εγγραφής **Πραγματικές τιμές ενοποίησης Project Operations (msdyn\_actuals).** Για περισσότερες πληροφορίες, δείτε [Εκτιμήσεις και Πραγματικές τιμές](resource-dual-write-estimates-actuals.md). 

Οι γραμμές πρότασης τιμολογίου έργου δημιουργούνται από την περιοδική διεργασία, **Προεργασία φόρμας εισαγωγής**. Αυτή η διαδικασία βασίζεται στις λεπτομέρειες των πραγματικών δεδομένων των πωλήσεων που έχουν χρεωθεί στον πίνακα **Προεργασία πραγματικών τιμών**. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση προτάσεων τιμολογίου έργου](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 