---
title: Προσδιορισμός του τύπου ανάπτυξής σας
description: Αυτό το θέμα παρέχει πληροφορίες για να σας βοηθήσει να καθορίσετε τον σωστό τύπο ανάπτυξης του Project Operations για την εταιρεία σας.
author: stsporen
ms.date: 03/15/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 280578b2710a0bccd1973b51b062fef7a2997780
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584136"
---
# <a name="determine-your-deployment-type"></a>Προσδιορισμός του τύπου ανάπτυξής σας

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

> [!IMPORTANT]
> Αφού αγοράσετε την άδεια χρήσης, ξεκινήστε εδώ για να προσδιορίσετε το καλύτερο μοντέλο ανάπτυξης του Dynamics 365 Project Operations χρησιμοποιώντας τη [ροή καθοδηγούμενης εγκατάστασης](https://aka.ms/provisionprojectoperations).
> Αφού ολοκληρώσετε την καθοδηγούμενη ροή εγκατάστασης, θα κατευθυνθείτε στη σωστή πύλη διαχείρισης για να ολοκληρώσετε την εγκατάσταση. Ανατρέξτε στις λεπτομέρειες ανάπτυξης για να ολοκληρώσετε την εγκατάσταση.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Υπάρχοντες πελάτες του Dynamics που χρησιμοποιούν το Dynamics 365 Project Service Automation
Το Project Operations περιλαμβάνει τις δυνατότητες που παρέχονται με το Project Service Automation. Θα κυκλοφορήσει μια διαδρομή αναβάθμισης για αυτούς τους πελάτες στο κύμα έκδοσης 1 του 2021.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Υπάρχοντες πελάτες του Dynamics 365 Finance χρησιμοποιώντας διαχείριση έργων και λογιστική 

Οι υφιστάμενοι πελάτες του Finance που χρησιμοποιούν τη λειτουργικότητα "Διαχείριση έργου και Λογιστική" μπορούν να συνεχίσουν να τη χρησιμοποιούν ως έχει. Δείτε [Project Operations για σενάρια εφοδιασμένα/παραγγελίας παραγωγής](#pma).


## <a name="deployment-regions"></a>Περιοχές ανάπτυξης
Για να προσδιορίσετε ποιες περιοχές υποστηρίζουν την ανάπτυξη του Project Operations, ανατρέξτε στο θέμα [Γεωγραφική διαθεσιμότητα για το Dynamics 365 και αναφορά Power Platform](https://dynamics.microsoft.com/en-us/geographic-availability/). Επιλέξτε **Προβολή αναφοράς** και αναπτύξτε την επιλογή **Dynamics 365 > Operations Apps > Dynamics 365 Project Operations** για προβολή των υποστηριζόμενων περιοχών.

## <a name="deployment-types"></a>Τύποι ανάπτυξης
Το Project Operations υποστηρίζει πολλές επιλογές ανάπτυξης για να ταιριάζουν με τις απαιτήσεις σας. Είτε είστε νέος είτε υφιστάμενος πελάτης του Dynamics 365, το Project Operations μπορεί να υποστηρίξει τις ανάγκες σας.

Το [Ερωτηματολόγιο ανάπτυξης](https://aka.ms/provisionprojectoperations) θα σας βοηθήσει να καθορίσετε την κατάλληλη ανάπτυξη. Τα αποτελέσματα θα σας καθοδηγήσουν προς έναν από τους ακόλουθους τύπους ανάπτυξης:

- [Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση](#lite)
- [Project Operations για σενάρια πόρων/μη εφοδιασμένα](#integrated)
- [Project Operations για σενάρια εφοδιασμένα/παραγγελίας παραγωγής](#pma)

Το Project Operations υποστηρίζει σενάρια με απόθεμα/παραγγελίας παραγωγής και σενάρια χωρίς απόθεμα/βάσει πόρου στο ίδιο περιβάλλον μέσω διαμορφώσεων σε επίπεδο νομικής οντότητας. Για παράδειγμα, η Contoso μπορεί να χρησιμοποιήσει τις δυνατότητες αποθήκευσης/παραγγελίας παραγωγής στις αμερικάνικες εγκαταστάσεις παραγωγής (Νομική οντότητα = Contoso Manufacturing United States). Η Contoso μπορεί να χρησιμοποιήσει τις δυνατότητες που βασίζονται σε μη εφοδιασμένο/πόρο στο Contoso Robotics Arms που εξυπηρετεί το Ηνωμένο Βασίλειο (Νομική οντότητα = Contoso Robotics United Kingdom).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση

Η ελαφριά ανάπτυξη περιλαμβάνει τις εξής δυνατότητες:

- Διαδικασία πωλήσεων για έργα που επεκτείνουν τις εμπειρίες εφαρμογής Dynamics 365 Sales
- Προγραμματισμός έργου με χρήση του Microsoft Project for the Web
- Πολυδιάστατη τιμολόγηση
- Ενοποιημένη διαχείριση πόρων
- Παρακολούθηση χρόνου
- Βασικά έξοδα
- Προτιμολόγηση proforma για αναθεώρηση και επεξεργασία από υπεύθυνο έργου 

#### <a name="deployment-steps"></a>Βήματα ανάπτυξης
Καθορίστε το καλύτερο μοντέλο ανάπτυξης του Project Operations χρησιμοποιώντας το [ερωτηματολόγιο ανάπτυξης](https://aka.ms/provisionprojectoperations).

Για αυτήν την ανάπτυξη, ανατρέξτε στο θέμα [Εγγραφή για προεπισκόπηση συνδρομών](lite-preview-subscription-sign-up.md) και [Παροχή νέου περιβάλλοντος](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Project Operations για σενάρια πόρων/μη εφοδιασμένα
Το Project Operations για σενάρια πόρου/μη εφοδιασμένα περιλαμβάνουν τις ακόλουθες δυνατότητες:
 
- Διαδικασία πωλήσεων για έργα που επεκτείνουν την εφαρμογή Dynamics 365 Sales
- Προγραμματισμός έργου με χρήση του Microsoft Project for the Web
- Πολυδιάστατη τιμολόγηση
- Ενοποιημένη διαχείριση πόρων
- Παρακολούθηση χρόνου
- Βασικά έξοδα
- Πλήρες έξοδο
- Απόδειξη OCR
- Προτιμολόγια και τιμολόγηση πελάτη 
- Αναγνώριση εσόδων για έργα

#### <a name="deployment-steps"></a>Βήματα ανάπτυξης
Καθορίστε το καλύτερο μοντέλο ανάπτυξης του Project Operations χρησιμοποιώντας το [ερωτηματολόγιο ανάπτυξης](https://aka.ms/provisionprojectoperations).

Για αυτήν την ανάπτυξη, ανατρέξτε στο θέμα [Εγγραφή για προεπισκόπηση συνδρομών](resource-sign-up-preview-subscription.md) και [Παροχή νέου περιβάλλοντος](resource-provision-new-environment.md). 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Project Operations για σενάρια εφοδιασμένα/παραγγελίας παραγωγής

- Σχεδιασμός έργου χρησιμοποιώντας WBS
- Διαχείριση πόρων
- Παρακολούθηση χρόνου
- Πλήρες έξοδο
- Απόδειξη OCR
- Πλήρης τιμολόγηση
- Αναγνώριση εσόδων
- Παραγγελίες παραγωγής
- Υποστήριξη εφοδιασμένων υλικών με απόθεμα

#### <a name="deployment-steps"></a>Βήματα ανάπτυξης
Καθορίστε το καλύτερο μοντέλο ανάπτυξης του Project Operations χρησιμοποιώντας το [ερωτηματολόγιο ανάπτυξης](https://aka.ms/provisionprojectoperations).

Για αυτήν την ανάπτυξη, ανατρέξτε στο θέμα [Εγγραφή για προεπισκόπηση συνδρομών](/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=%2fdynamics365%2ffinance%2ftoc.json) και [Παροχή νέου περιβάλλοντος](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=%2fdynamics365%2ffinance%2ftoc.json). 



[!INCLUDE[footer-include](../includes/footer-banner.md)]