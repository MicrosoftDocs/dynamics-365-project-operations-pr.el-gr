---
title: Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο δημιουργίας προσαρμοσμένων συνόλων επιλογών ή οντοτήτων.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2000f7e710267560fe2bd52b0e33024617d108ea
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898261"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a>Δημιουργία προσαρμοσμένων πεδίων και οντοτήτων ως διαστάσεις τιμολόγησης

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Ολοκληρώστε τα παρακάτω βήματα κάθε φορά που θέλετε να δημιουργήσετε ένα προσαρμοσμένο σύνολο επιλογών ή μια οντότητα.

> [!IMPORTANT]
> Συνιστούμε να κάνετε όλες τις προσαρμοσμένες αλλαγές διάστασης τιμολόγησης σε μια ξεχωριστή λύση. Αυτή η σημαντική βέλτιστη πρακτική παρέχει την ευελιξία στο μέλλον για την ενημέρωση ή την κατάργηση αλλαγών όπου είναι απαραίτητο, θα σας βοηθήσει με την περαιτέρω χρήση της εργασίας σας και διευκολύνει τη μεταφορά αυτών των αλλαγών σε μια άλλη παρουσία. Αφού πραγματοποιήσετε όλες τις απαιτούμενες αλλαγές, εξαγάγετε αυτήν τη λύση ως **Διαχειριζόμενη λύση** και εισαγάγετέ την σε άλλες παρουσίες, για να επαναχρησιμοποιήσετε την ρύθμιση τιμολόγησης.


## <a name="create-a-custom-solution-for-pricing-dimensions"></a>Δημιουργία προσαρμοσμένης λύσης για διαστάσεις τιμολόγησης
1. Κάντε κλικ στις **Ρυθμίσεις** > **Λύσεις** και μετά επιλέξτε **Νέα** για να δημιουργήσετε μια νέα λύση. 
2. Ονομάστε τη λύση, **\<your organization name> διαστάσεις τιμολόγησης**, καταχωρίστε τις υπόλοιπες πληροφορίες και μετά επιλέξτε **Αποθήκευση**.
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Δημιουργία προσαρμοσμένων πεδίων και συνόλων επιλογών στη λύση διάστασης τιμολόγησης

Μια διάσταση τιμολόγησης μπορεί να είναι μια σύνολο επιλογών ή μια οντότητα. Και τα δύο πρέπει να δημιουργηθούν στη λύση τιμολόγησης. Τα βήματα σε αυτήν τη διαδικασία εξηγούν πώς μπορείτε να δημιουργήσετε διαστάσεις βασισμένες σε οντότητες και διαστάσεις που βασίζονται σε σύνολα επιλογών.

### <a name="entity-based-dimensions"></a>Διαστάσεις βάσει οντότητας

1. Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και έπειτα κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**.
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Οντότητες**.
3. Επιλέξτε **Νέα** για να δημιουργήσετε μια νέα οντότητα που καλείται **Τυπικός τίτλος**. 
4. Πληκτρολογήστε τις απαιτούμενες υπόλοιπες πληροφορίες και, στη συνέχεια επιλέξτε **Αποθήκευση**.


### <a name="option-set-based-dimensions"></a>Διαστάσεις που βασίζονται σε σύνολο επιλογών 
Μπορείτε να δημιουργήσετε δύο διαστάσεις που βασίζονται σε σύνολο επιλογών. Χρησιμοποιήστε την **Τοποθεσία εργασίας πόρου** για να παρακολουθήσετε την τιμή της **Αρχικής** τοποθεσίας εργασίας και την **Επί τόπου** εργασία και να χρησιμοποιήσετε τις **Ώρες εργασίας πόρου** με τιμές **Κανονικές** και **Υπερωρίες** για να εφαρμόσετε μια αύξηση όταν ολοκληρωθεί η εργασία.


1. Μεταβείτε στο **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**. 
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Σύνολα επιλογών**. 
3. Επιλέξτε **Νέο** για να δημιουργήσετε ένα νέο σύνολο επιλογών, καταγράψτε τις υπόλοιπες απαιτούμενες πληροφορίες και επιλέξτε **Αποθήκευση**.

## <a name="create-data-for-entity-based-dimensions"></a>Δημιουργία δεδομένων για διαστάσεις βασισμένες σε οντότητες

Μπορείτε να δημιουργήσετε δεδομένα για διαστάσεις βασισμένες σε οντότητες με μη αυτόματο τρόπο ή χρησιμοποιώντας κλήσης εισαγωγής Microsoft Excel ή κλήσεις εξυπηρέτησης. Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για τη δημιουργία δύο τυπικών τίτλων, **Μηχανικός συστημάτων** και **Επικεφαλής μηχανικός συστημάτων** από τη διάσταση βάσει οντότητας **Τυπικός τίτλος**. Εάν τα δεδομένα που θέλετε να δημιουργήσετε είναι μικρά, όπως στο παρακάτω παράδειγμα, μπορείτε να χρησιμοποιήσετε μια τυπική φόρμα.

1. Επιλέξτε **Πρόσθετα κριτήρια εύρεσης**, επιλέξτε την οντότητα **Τυπικός τίτλος** και, στη συνέχεια, επιλέξτε **Αποτελέσματα**. Θα εμφανιστούν όλες οι γραμμές στην οντότητα **Τυπικός τίτλος**.
2. Επιλέξτε **Νέο** και στο πεδίο **Όνομα**, καταχωρίστε "Μηχανικός συστήματος" και μετά επιλέξτε **Αποθήκευση**.
3. Κλείσιμο της φόρμας. 
4. Επαναλάβετε τα βήματα 1-3, για να δημιουργήσετε έναν άλλο τυπικό τίτλο για τον "επικεφαλής μηχανικό συστημάτων".

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>Προσθήκη όλων των απαιτούμενων οντοτήτων και σχετικών στοιχείων στη λύση διάστασης τιμολόγησης
Θα πρέπει να προσθέσετε τις παρακάτω οντότητες στη λύση τιμολόγησης. Χρησιμοποιήστε τα βήματα σε αυτήν τη διαδικασία για να κάνετε κάποιες σημαντικές αλλαγές σχήματος στη λύση τιμολόγησης, έτσι ώστε οι οντότητες να συνειδητοποιήσουν τις νέες διαστάσεις τιμολόγησης.

1. Επιλέξτε **Ρυθμίσεις** > **Λύσεις** και κάντε διπλό κλικ στις **διαστάσεις τιμολόγησης \<your organization name>**. 
2. Στην εξερεύνηση λύσεων, στο αριστερό παράθυρο περιήγησης, επιλέξτε **Προσθήκη υπάρχουσας** > **Οντότητες**.
3. Στο παράθυρο διαλόγου **Στοιχεία λύσης**, επιλέξτε τις ακόλουθες οντότητες:

  - Πραγματικό
  - Πόρος με δυνατότητα κράτησης
  - Γραμμή εκτίμησης
  - Λεπτομέρεια γραμμής τιμολογίου
  - Γραμμή ημερολογίου
  - Λεπτομέρεια γραμμής σύμβασης έργου
  - Μέλος ομάδας έργου
  - Λεπτομέρειες γραμμής προσφοράς
  - Αύξηση τιμής ρόλου
  - Τιμή ρόλου 
  - Χρονική καταχώρηση 


> [!NOTE]
> Βεβαιωθείτε ότι θα συμπεριλάβετε όλες τις φόρμες και τις προβολές για κάθε μια από τις οντότητες που επιλέγονται.

4. Όταν σας ζητηθεί να συμπεριλάβετε εξαρτημένες οντότητες για τις οντότητες που επιλέξατε παραπάνω, επιλέξτε **Όχι**.

