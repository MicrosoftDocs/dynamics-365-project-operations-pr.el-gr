---
title: Προγραμματίστε την εργασία σας στο Microsoft Project με το πρόσθετο Project Service
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη χρήση του πρόσθετου Microsoft Project για το Microsoft Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
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
ms.openlocfilehash: 0c0ea75d34047f7145466ab427d213c5df27fbed
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014566"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>Προγραμματίστε την εργασία σας στο Microsoft Project με το πρόσθετο Project Service

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

To [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] σάς διευκολύνει να κάνετε τον προγραμματισμό έργου σας, καθώς και εκτιμήσεις. Μπορείτε να ορίσετε την εργασία έτσι ώστε οι δαπάνες, η προσπάθεια και η τιμή πωλήσεων να είναι σαφή κατά την υποβολή της τελικής πρότασης.  

Μπορείτε να εγκαταστήσετε το [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] και να κάνετε τις εργασίες σχεδιασμού σας στο οικείο περιβάλλον του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. Χρησιμοποιήστε τις ισχυρές δυνατότητες προγραμματισμού και διαχείρισης του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και, στη συνέχεια, ενημερώστε το σχέδιο έργου σας στο Project Service Automation.  

> [!IMPORTANT]
> - Για να χρησιμοποιήσετε τη διαχείριση εγγράφων του SharePoint για την αποθήκευση των αρχείων [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] για τα έργα [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], ο διαχειριστής του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] θα χρειαστεί να ενεργοποιήσει τη διαχείριση εγγράφων. 
> - Το [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] είναι συμβατό μόνο με το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>Λήψη και εγκατάσταση του προσθέτου  
 Να έχετε στη διάθεσή σας τα στοιχεία σύνδεσης στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Θα χρειαστείτε αυτές τις πληροφορίες, για να συνδεθείτε από το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  Από το κέντρο λήψης, κατεβάστε το πρόσθετο για την υποστηριζόμενη έκδοση του Project Service, είτε [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) είτε [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Επιλέξτε τη σύνδεση λήψης.  

3.  Όταν ολοκληρωθεί η λήψη, επιλέξτε **Ναι** για την εγκατάσταση του προσθέτου.  

## <a name="configure-the-add-in"></a>Ρύθμιση των παραμέτρων του προσθέτου  

1. Ανοίξτε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και κάντε κλικ στην καρτέλα **Project Service**.  

2. Επιλέξτε **Σύνδεση**.  

3. Εισαγάγετε τις πληροφορίες εισόδου σας και, στη συνέχεια, κάντε κλικ στο κουμπί **Είσοδος**.  

   Τώρα μπορείτε να ξεκινήσετε να χρησιμοποιείτε το πρόσθετο.  

## <a name="read-from-a-template"></a>Ανάγνωση από πρότυπο  
 Κάντε ανάγνωση από ένα πρότυπο που δημιουργήσατε στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] και αντιγράψατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], για να ξεκινήσετε τον σχεδιασμό του έργου. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Δημιουργία προτύπου έργου (Project Service Automation)](../psa/create-project-template.md)  

1.  Από την καρτέλα **Project Service**, κάντε κλικ στις επιλογές **Ανάγνωση** > **Πρότυπο έργου Project Service Automation**.  

2.  Επιλέξτε ένα πρότυπο έργου από τη λίστα και, στη συνέχεια, κάντε κλικ στο κουμπί **Άνοιγμα**.  

    > [!NOTE]
    >  Από προεπιλογή, οι εργασίες που αντιγράφονται από το πρότυπο στο Project έχουν οριστεί ως μη αυτόματα προγραμματισμένες.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Αντιστοίχιση [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ρόλων σε πόρους έργου  

1.  Ανοίξτε ένα έργο και κάντε κλικ στην κορδέλα **Εργασία**.  

2. Κάντε κλικ στο μενού **Γράφημα Gantt** και στη συνέχεια επιλέξτε **Φύλλο πόρων**.  

3. Στο φύλλο πόρων, κάντε κλικ στο αναπτυσσόμενο μενού **Ρόλος πόρου Project Service** και επιλέξτε έναν ρόλο Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>Εκχώρηση πόρων στο έργο σας  

1.  Από την καρτέλα Project Service, επιλέξτε μια γραμμή και κάντε κλικ στο κουμπί **Εύρεση πόρων**.  

2.  Στην οθόνη **Κράτηση πόρου**, επιλέξτε τον πόρο που θέλετε να χρησιμοποιήσετε για το έργο.  

3.  Επιλέξτε το στοιχείο **Κράτηση** και, στη συνέχεια, επιλέξτε **ΟΚ**.  

## <a name="publish-your-project"></a>Δημοσίευση του έργου σας  
Όταν ο σχεδιασμός του έργου έχει ολοκληρωθεί, το επόμενο βήμα είναι να εισαγάγετε και να δημοσιεύσετε το έργο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Το έργο θα εισαχθεί στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Εφαρμόζονται οι διαδικασίες τιμολόγησης και δημιουργίας ομάδας. Ανοίξτε το έργο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] για να δείτε ότι η ομάδα, οι εκτιμήσεις έργου και η δομή ανάλυσης εργασίας έχουν δημιουργηθεί. Ο παρακάτω πίνακας δείχνει πού μπορείτε να βρείτε τα αποτελέσματα.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  **Γράφημα Gantt** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]   | Εισάγεται στην οθόνη **Δομή ανάλυσης εργασίας** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. |
| **Φύλλο πόρων** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] |   Εισάγεται στην οθόνη **Μέλη ομάδας έργου** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]   |
|   **Χρήση** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]    |    Εισάγει στην οθόνη **Εκτιμήσεις έργου** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].     |

**Για να εισαγάγετε και να δημοσιεύσετε το έργο σας**  
1. Από την καρτέλα **Project Service**, κάντε κλικ στις επιλογές **Δημοσίευση** > **Νέο έργο Project Service Automation**.  

2. Στο παράθυρο διαλόγου **Δημοσίευση σε ένα νέο έργο στο Project Service**, καταχωρίστε το **Όνομα έργου** και επιλέξτε **Πελάτης**.  

3. Προαιρετικά επιλέξτε **Σύνδεση πλάνου έργου στο Project Service Automation**, για να συνδέσετε το αρχείο σχεδίου του Project με το Project Service Automation.  

4. Επιλέξτε **Δημοσίευση**.  

   Η σύνδεση του αρχείου Project με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] καθιστά το αρχείο έργου βασικό και ορίζει τη δομή ανάλυσης εργασίας στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] μόνο για ανάγνωση.  Για να κάνετε αλλαγές στο σχέδιο έργου, πρέπει να το δημιουργήσετε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να το δημοσιεύσετε ως ενημέρωση στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>Επεξεργασία ενός έργου που έχει εισαχθεί  
 Για να κάνετε αλλαγές σε ένα σχέδιο έργου που έχει εισαχθεί στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], έχετε δύο επιλογές:  

- Ανοίξτε το βασικό αρχείο και επεξεργαστείτε το στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- Αποσυνδέστε το αρχείο και επεξεργαστείτε το στο Project Service. Από προεπιλογή, ένα έργο που αποστέλλεται από το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι κλειδωμένο και είναι δυνατή η επεξεργασία μόνο στο Project. Για να επεξεργαστείτε το αρχείο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], το αρχείο πρέπει να αποσυνδεθεί.  

### <a name="edit-in-pn_microsoft_project"></a>Επεξεργασία σε [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. Από το κύριο μενού, επιλέξτε **Project Service** > **Έργα**.  

2. Από τη λίστα έργων, ανοίξτε αυτό που δημιουργήσατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Κάντε κλικ στο κουμπί **Άνοιγμα στο MS Project** από την κορδέλα. Θα ανοίξει το συνδεδεμένο βασικό αρχείο στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Αποσύνδεση ενός αρχείου και επεξεργασία στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. Από το κύριο μενού, επιλέξτε **Project Service** > **Έργα**.  

2. Από τη λίστα έργων, ανοίξτε αυτό που δημιουργήσατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Κάντε κλικ στο κουμπί **Αποσύνδεση από το MS Project** από την κορδέλα.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>Αποστολή αρχείου Project στο SharePoint ή σε Ομάδες Office  
 Μπορείτε να στείλετε το αρχείο έργου στο SharePoint και να το βρείτε κάτω από τα έγγραφα που σχετίζονται με το έργο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Ο διαχειριστής σας πρέπει να ρυθμίσει τις παραμέτρους διαχείρισης εγγράφων του SharePoint και να ενεργοποιήσει αυτή τη δυνατότητα για την οντότητα Project. 

 Επίσης, μπορείτε να αποστείλετε το αρχείο έργου στο [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)], εάν έχετε ορίσει Ομάδες Office.

### <a name="upload-a-file-for-sharepoint"></a>Αποστολή αρχείου για το SharePoint  

1. Από το κύριο μενού, επιλέξτε **Project Service** > **Αποστολή**.  

2. Επιλέξτε **Προς έγγραφα έργου του Project Service Automation**.  

3. Στο πλαίσιο διαλόγου **Ενεργοποίηση ανοίγματος στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, επιλέξτε **Ναι** ή **Όχι**.  

   - Αν κάνετε κλικ στο **Ναι**, θα έχετε τη δυνατότητα να κάνετε κλικ στο **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** στο Project Service Automation και να εκκινήσετε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να φορτώσετε το αρχείο έργου από τη βιβλιοθήκη εγγράφων του SharePoint.  

   - Εάν επιλέξετε **Όχι**, η σύνδεση για το **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** δεν θα λειτουργήσει.  

4. Το αρχείο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι διαθέσιμο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στην περιοχή **Έγγραφα** του εκάστοτε έργου [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

### <a name="upload-a-file-for-office-groups"></a>Αποστολή αρχείου για Ομάδες Office  

1. Από το κύριο μενού, επιλέξτε **Project Service** > **Αποστολή**.  

2. Επιλέξτε **Προς έγγραφα έργου του Project Service Automation**.  

3. Στο πλαίσιο διαλόγου **Ενεργοποίηση ανοίγματος στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, επιλέξτε **Ναι** ή **Όχι**.  

   - Αν κάνετε κλικ στο **Ναι**, θα έχετε τη δυνατότητα να κάνετε κλικ στο **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** στο Project Service Automation και να εκκινήσετε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να φορτώσετε το αρχείο έργου από τη βιβλιοθήκη εγγράφων του SharePoint.  

   - Εάν επιλέξετε **Όχι**, η σύνδεση για το **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** δεν θα λειτουργήσει.  

4. Το αρχείο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι διαθέσιμο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στην περιοχή **Έγγραφα** του εκάστοτε έργου [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="publish--your-project-as-a-template"></a>Δημοσίευση του έργου σας ως προτύπου  
 Μπορείτε να αποθηκεύσετε το έργο σας και να το χρησιμοποιήσετε ξανά αποθηκεύοντάς το ως πρότυπο έργου στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Τα πρότυπα έργου είναι σχέδια με δυνατότητα επανάληψης χρήσης στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δημιουργία προτύπου έργου (Project Service Automation)](../psa/create-project-template.md). 

1. Από την καρτέλα **Project Service**, κάντε κλικ στις επιλογές **Δημοσίευση** > **Νέο πρότυπο έργου Project Service Automation**.  

2. Στο πλαίσιο διαλόγου **Δημοσίευση σε ένα νέο έργο στο Project Service**, καταχωρίστε **Όνομα προτύπου έργου**.  

3. Προαιρετικά επιλέξτε **Σύνδεση πλάνου έργου στο Project Service Automation**, για να συνδέσετε το αρχείο έργου με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. Επιλέξτε **Δημοσίευση**.  

Η σύνδεση του αρχείου έργου με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] καθιστά το αρχείο έργου βασικό και ορίζει τη δομή ανάλυσης εργασίας στο πρότυπο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] μόνο για ανάγνωση.  Για να κάνετε αλλαγές στο σχέδιο έργου, πρέπει να το δημιουργήσετε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να το δημοσιεύσετε ως ενημέρωση στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>Ανάγνωση χρονοδιαγράμματος φορτωμένου πόρου

Όταν διαβάζετε ένα έργο από το Project Service Automation, το ημερολόγιο του πόρου δεν συγχρονίζεται με το πρόγραμμα-πελάτη επιφάνειας εργασίας. Εάν υπάρχουν διαφορές στη διάρκεια της εργασίας, στην προσπάθεια ή στο τέλος, αυτό συμβαίνει πιθανώς επειδή οι πόροι και το πρόγραμμα-πελάτης επιφάνειας εργασίας δεν διαθέτουν το ίδιο ημερολόγιο προτύπου ώρας εργασίας που εφαρμόζεται στο έργο.


## <a name="data-synchronization"></a>Συγχρονισμός δεδομένων
Οι πίνακες σε αυτήν την ενότητα παρέχουν πληροφορίες σχετικά με το συγχρονισμό των δεδομένων οντότητας μεταξύ του Project Service Automation και του προσθέτου υπολογιστή Microsoft Project.

### <a name="project-task-entity-table"></a>Πίνακας οντότητας εργασίας έργου
Στον ακόλουθο πίνακα περιγράφονται ο τρόπος με τον οποίο συγχρονίζονται τα δεδομένα οντότητας εργασίας έργου μεταξύ του Project Service Automation και του πρόσθετου επιφάνειας εργασίας του Microsoft Project.

| **Οντότητα** | **Πεδίο** | **Microsoft Project σε Project Service Automation** | **Project Service Automation σε Microsoft Project** |
| --- | --- | --- | --- |
| Εργασία έργου | Προθεσμία | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Εκτιμώμενη προσπάθεια | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Αναγνωριστικό προγράμματος-πελάτη MS Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Γονική εργασία | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Εργασία έργου | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Όνομα εργασίας έργου | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Μονάδα πόρων (Δεν χρησιμοποιείται στην έκδοση 3.0) | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Προγραμματισμένη διάρκεια | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Ημερομηνία έναρξης | Συγχρονισμός | Κανένας συγχρονισμός |
| Εργασία έργου | Αναγνωριστικό WBS | Συγχρονισμός | Κανένας συγχρονισμός |

### <a name="team-member-entity-table"></a>Πίνακας οντότητας μέλους ομάδας
Στον ακόλουθο πίνακα περιγράφονται ο τρόπος με τον οποίο συγχρονίζονται τα δεδομένα οντότητας μέλους ομάδας μεταξύ του Project Service Automation και του Microsoft Project.

| **Οντότητα** | **Πεδίο** | **Microsoft Project σε Project Service Automation** | **Project Service Automation σε Microsoft Project** |
| --- | --- | --- | --- |
| Μέλος ομάδας | Αναγνωριστικό προγράμματος-πελάτη MS Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Μέλος ομάδας | Όνομα θέσης | Συγχρονισμός | Κανένας συγχρονισμός |
| Μέλος ομάδας | έργο | Συγχρονισμός | Συγχρονισμός |
| Μέλος ομάδας | Ομάδα έργου | Συγχρονισμός | Συγχρονισμός |
| Μέλος ομάδας | Μονάδα πόρων | Κανένας συγχρονισμός | Συγχρονισμός |
| Μέλος ομάδας | Ρόλος | Κανένας συγχρονισμός | Συγχρονισμός |
| Μέλος ομάδας | Ώρες εργασίας | Κανένας συγχρονισμός | Κανένας συγχρονισμός |

### <a name="resource-assignment-entity-table"></a>Πίνακας οντότητας ανάθεσης πόρου
Στον ακόλουθο πίνακα περιγράφονται ο τρόπος με τον οποίο συγχρονίζονται τα δεδομένα οντότητας ανάθεσης πόρου μεταξύ του Project Service Automation και του Microsoft Project.

| **Οντότητα** | **Πεδίο** | **Microsoft Project σε Project Service Automation** | **Project Service Automation σε Microsoft Project** |
| --- | --- | --- | --- |
| Ανάθεση πόρου | Ημερομηνία "Από" | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Ώρες | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Αναγνωριστικό προγράμματος-πελάτη MS Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Προγραμματισμένη εργασία | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Ομάδα έργου | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Ανάθεση πόρου | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Κλείσιμο εργασίας | Συγχρονισμός | Κανένας συγχρονισμός |
| Ανάθεση πόρου | Έως σήμερα | Συγχρονισμός | Κανένας συγχρονισμός |

### <a name="project-task-dependencies-entity-table"></a>Πίνακας οντότητας εξαρτήσεων εργασίας έργου
Στον ακόλουθο πίνακα περιγράφονται ο τρόπος με τον οποίο συγχρονίζονται τα δεδομένα οντότητας εξαρτήσεων εργασίας έργου μεταξύ του Project Service Automation και του Microsoft Project.

| **Οντότητα** | **Πεδίο** | **Microsoft Project σε Project Service Automation** | **Project Service Automation σε Microsoft Project** |
| --- | --- | --- | --- |
| Εξαρτήσεις εργασίας έργου | Εξάρτηση εργασίας έργου | Συγχρονισμός | Κανένας συγχρονισμός |
| Εξαρτήσεις εργασίας έργου | Τύπος σύνδεσης | Συγχρονισμός | Κανένας συγχρονισμός |
| Εξαρτήσεις εργασίας έργου | Εργασία προκατόχου | Συγχρονισμός | Κανένας συγχρονισμός |
| Εξαρτήσεις εργασίας έργου | Project | Συγχρονισμός | Κανένας συγχρονισμός |
| Εξαρτήσεις εργασίας έργου | Εργασία διαδόχου | Συγχρονισμός | Κανένας συγχρονισμός |

### <a name="additional-resources"></a>Πρόσθετοι πόροι
 [Οδηγός υπευθύνου έργου](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]