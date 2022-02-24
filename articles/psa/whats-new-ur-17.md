---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 17, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 17, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: f9fb941a95b0610dc546b1c12a87aa7faef4d676
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143714"
---
# <a name="project-service-automation-update-release-17-v3"></a>Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 17, V3

[!include [banner](../includes/psa-now-project-operations.md)]

Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365. Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.  Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x. Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση. Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το PSA V3, έκδοση ενημέρωσης 17. Αυτή η έκδοση έχει αριθμό δομής V3.10.6.34 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Μάρτιο του 2020.


## <a name="update-release-17"></a>Έκδοση κυκλοφορίας 17

### <a name="bug-fixes"></a>Επιδιορθώσεις σφαλμάτων

**Γενικά**

- Διόρθωση: ενημέρωση Project Service Automation για την επιβολή αδειών χρήσης μελών ομάδας (το Κέντρο πόρων έργου θα συμπεριλάβει τα μετα-δεδομένα σχεδίου υπηρεσίας μέλους ομάδας 3. x)
 
**Χρόνος και έξοδα**

- Διόρθωση: δεν είναι δυνατή η αλλαγή μιας εκτίμησης εξόδων από μια μη μηδενική τιμή σε μηδέν (0). Η αλλαγή παραβλέπεται.

**Διαχείριση έργων**

- Διόρθωση: προστέθηκε ένα σημάδι ελέγχου για τις μηδενικές τιμές στο όνομα θέσης ενός μέλους ομάδας.
- Διόρθωση: το πεδίο **msdyn_userresourceid** στην οντότητα **msdyn_resourceassignment** έχει καταργηθεί.
- Διόρθωση: η αναβάθμιση από 2. x σε 3. x πλέον χειρίζεται κενά περιγράμματα προσπάθειας σε αναθέσεις εργασιών.

**Sales**

- Διόρθωση: το **Invoice.PreValidateInvoiceUpdate** χειρίζεται πλέον το σενάριο της εκ νέου ανάθεσης κατόχων καρτέλας σωστά.
- Διόρθωση: όταν η κλάση συναλλαγής είναι **Ώρα**, η **Ομάδα μονάδας** δεν είναι επεξεργάσιμη για όλες τις οντότητες συμπεριλαμβανομένων των **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** και **ContractLineDetails**. Ωστόσο, η **Μονάδα** είναι μη επεξεργάσιμη μόνο για **JournalLine** και **InvoiceLineDetails**.


