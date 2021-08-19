---
title: Εφαρμόστε προσαρμοσμένα πεδία για την εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές σε iOS και Android
description: Αυτό το θέμα παρέχει συνήθη μοτίβα για τη χρήση επεκτάσεων για την εφαρμογή προσαρμοσμένων πεδίων.
author: Yowelle
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 9f19a6d069c4f825be8515a6d26739c50d3b064698fc1872ede07a4e74ee4dcb
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/06/2021
ms.locfileid: "7005751"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>Εφαρμόστε προσαρμοσμένα πεδία για την εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές σε iOS και Android

[!include [banner](../includes/banner.md)]

Αυτό το θέμα παρέχει συνήθη μοτίβα για τη χρήση επεκτάσεων για την εφαρμογή προσαρμοσμένων πεδίων. Εξετάζονται τα εξής θέματα:

- Οι διάφοροι τύποι δεδομένων που υποστηρίζονται από το πλαίσιο του προσαρμοσμένου πεδίου
- Ο τρόπος εμφάνισης πεδίων μόνο για ανάγνωση ή με δυνατότητα επεξεργασίας σε καταχωρήσεις φύλλου κατανομής χρόνου και η αποθήκευση τιμών που παρέχονται από το χρήστη πίσω στη βάση δεδομένων
- Ο τρόπος εμφάνισης πεδίων μόνο για ανάγνωση στην κεφαλίδα του φύλλου κατανομής χρόνου
- Πώς να ενσωματώσετε άλλες προσαρμοσμένες επιχειρηματικές λογικές για την εισαγωγή προεπιλεγμένων τιμών σε πεδία και να κάνετε πρόσθετη επικύρωση

## <a name="audience"></a>Κοινό

Αυτό το θέμα απευθύνεται σε προγραμματιστές που ενσωματώνουν τα προσαρμοσμένα πεδία τους στην εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές η οποία είναι διαθέσιμη για Apple iOS και Google Android. Η υπόθεση είναι ότι οι αναγνώστες εξοικειώνονται με την ανάπτυξη X++ και τη λειτουργικότητα του φύλλου εργασίας του έργου.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>Σύμβαση δεδομένων – TSTimesheetCustomField X++ κλάση

Η κλάση **TSTimesheetCustomField** είναι η κλάση σύμβασης δεδομένων X++ η οποία αναπαριστά πληροφορίες σχετικά με ένα προσαρμοσμένο πεδίο για τη λειτουργικότητα του φύλλου κατανομής χρόνου. Οι λίστες των αντικειμένων προσαρμοσμένων πεδίων μεταβιβάζονται τόσο στη σύμβαση δεδομένων TSTimesheetDetails όσο και στη σύμβαση δεδομένων TSTimesheetEntry για την εμφάνιση προσαρμοσμένων πεδίων στην εφαρμογή για κινητές συσκευές.

- **TSTimesheetDetails** - Σύμβαση κεφαλίδας του φύλλου κατανομής χρόνου.
- **TSTimesheetEntry** - Σύμβαση συναλλαγής φύλλου κατανομής χρόνου. Οι ομάδες αυτών των αντικειμένων που έχουν τις ίδιες πληροφορίες έργου και την τιμή **timesheetLineRecId** αποτελούν μια γραμμή.

### <a name="fieldbasetype-types"></a>fieldBaseType (Τύποι)

Η ιδιότητα **FieldBaseType** στο αντικείμενο **TsTimesheetCustom** προσδιορίζει τον τύπο του πεδίου που εμφανίζεται στην εφαρμογή. Οι ακόλουθοι **Τύποι** τιμών που υποστηρίζονται.

| Τύπος τιμής | Τύπος              | Σημειώσεις |
|-------------|-------------------|-------|
| 0           | Συμβολοσειρά (και απαρίθμηση) | Το πεδίο εμφανίζεται ως πεδίο κειμένου. |
| 1           | Integer           | Η τιμή εμφανίζεται ως αριθμός χωρίς δεκαδικά ψηφία. |
| 2           | Πραγματική              | Η τιμή εμφανίζεται ως αριθμός με δεκαδικά ψηφία.<p>Για να εμφανίσετε την πραγματική τιμή ως νομισματική μονάδα στην εφαρμογή, χρησιμοποιήστε την ιδιότητα **fieldExtenededType**. Μπορείτε να χρησιμοποιήσετε την ιδιότητα **numberOfDecimals** για να ορίσετε τον αριθμό των δεκαδικών ψηφίων που εμφανίζονται.</p> |
| 3           | Ημερομηνία              | Οι μορφές ημερομηνιών καθορίζονται από τη ρύθμιση **Μορφή αριθμού, ώρας και ημερομηνίας** του χρήστη που καθορίζεται στην περιοχή **Προτίμηση γλώσσας και χώρας/περιοχής** στις **Επιλογές χρήστη**. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- Εάν η ιδιότητα **stringOptions** δεν παρέχεται στο αντικείμενο **TSTimesheetCustomField**, παρέχεται στο χρήστη ένα πεδίο ελεύθερου κειμένου.

    Η ιδιότητα **stringLength** μπορεί να χρησιμοποιηθεί για τον ορισμό του μέγιστου μήκους συμβολοσειράς που μπορούν να εισαγάγουν οι χρήστες.

- Εάν η ιδιότητα **stringOptions** παρέχεται στο αντικείμενο **TSTimesheetCustomField**, αυτά τα στοιχεία λίστας είναι οι μόνες τιμές που μπορούν να επιλέξουν οι χρήστες χρησιμοποιώντας τα κουμπιά επιλογής (κουμπιά επιλογής).

    Σε αυτήν την περίπτωση, το πεδίο συμβολοσειράς μπορεί να ενεργήσει ως τιμή απαρίθμησης για το σκοπό της καταχώρησης χρήστη. Για να αποθηκεύσετε την τιμή στη βάση δεδομένων ως απαρίθμηση, αντιστοιχίστε με μη αυτόματο τρόπο την τιμή της συμβολοσειράς στην τιμή "απαρίθμηση" πριν την αποθήκευση στη βάση δεδομένων χρησιμοποιώντας την αλυσίδα εντολών (ανατρέξτε στην ενότητα "χρήση της αλυσίδας εντολών στην κλάση TSTimesheetEntryService για την αποθήκευση μιας καταχώρησης φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων" στη συνέχεια αυτού του θέματος για παράδειγμα).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

Μπορείτε να χρησιμοποιήσετε αυτήν την ιδιότητα για να μορφοποιήσετε πραγματικές τιμές ως νομισματικές μονάδες. Αυτή η προσέγγιση εφαρμόζεται μόνο όταν η τιμή **fieldBaseType** είναι **Πραγματική**.

- **TSCustomFieldExtendedType:None** – Δεν εφαρμόζεται καμία μορφοποίηση.
- **TSCustomFieldExtendedType::Currency** – Μορφοποίηση της τιμής ως νομισματική μονάδα.

    Όταν η μορφοποίηση νομισματικής μονάδας είναι ενεργή, το πεδίο **stringValue** μπορεί να χρησιμοποιηθεί για να περάσει ο κωδικός νομίσματος που θα πρέπει να εμφανίζεται στην εφαρμογή. Η τιμή είναι μια τιμή μόνο για ανάγνωση.

    Το πεδίο **realValue** περιέχει το χρηματικό ποσό που θα πρέπει να αποθηκευτεί στη βάση δεδομένων του.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

Μπορείτε να χρησιμοποιήσετε αυτήν την ιδιότητα για να καθορίστε τη θέση στην οποία θα πρέπει να εμφανίζεται το προσαρμοσμένο πεδίο στην εφαρμογή.

- **TSCustomFieldSection::Header** – Το πεδίο θα εμφανιστεί στην ενότητα **Προβολή περισσότερων λεπτομερειών** στην εφαρμογή. Αυτά τα πεδία είναι πάντα για ανάγνωση.
- **TSCustomFieldSection::Line** – Το πεδίο θα εμφανιστεί μετά από όλα τα έτοιμα πεδία γραμμής στις καταχωρήσεις φύλλου κατανομής χρόνου. Αυτά τα πεδία μπορεί να είναι επεξεργάσιμα ή μόνο για ανάγνωση.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

Αυτή η ιδιότητα προσδιορίζει το πεδίο όταν οι τιμές που παρέχει η εφαρμογή αποθηκεύονται ξανά στη βάση δεδομένων.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

Αυτή η ιδιότητα προσδιορίζει το πεδίο όταν οι τιμές που παρέχει η εφαρμογή αποθηκεύονται ξανά στη βάση δεδομένων.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

Ορίστε αυτήν την ιδιότητα σε **Ναι** για να καθορίσετε ότι το πεδίο στην ενότητα καταχώρησης φύλλου κατανομής χρόνου θα πρέπει να είναι επεξεργάσιμο από τους χρήστες. Ορίστε την ιδιότητα σε **Όχι** ώστε το πεδίο να είναι μόνο για ανάγνωση.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

Ορίστε αυτήν την ιδιότητα σε **Ναι** για να καθορίσετε ότι το πεδίο στην ενότητα καταχώρησης φύλλου κατανομής χρόνου θα πρέπει να είναι υποχρεωτικό.

### <a name="label-str"></a>ετικέτα (str)

Αυτή η ιδιότητα καθορίζει την ετικέτα που εμφανίζεται δίπλα στο πεδίο στην εφαρμογή.

### <a name="stringoptions-list-of-strings"></a>stringOptions (λίστα συμβολοσειρών)

Αυτή η ιδιότητα ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Συμβολοσειρά**. Εάν έχει οριστεί το **stringOptions**, οι τιμές συμβολοσειράς που είναι διαθέσιμες για επιλογή μέσω των κουμπιών επιλογής (κουμπιά επιλογής) καθορίζονται από τις συμβολοσειρές που περιλαμβάνονται στη λίστα. Εάν δεν παρέχονται συμβολοσειρές, επιτρέπεται η καταχώρηση ελεύθερων κειμένων στο πεδίο συμβολοσειράς (ανατρέξτε στην ενότητα "χρήση της αλυσίδας εντολών στην κλάση TSTimesheetEntryService για την αποθήκευση μιας καταχώρησης φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων" στη συνέχεια αυτού του θέματος για παράδειγμα).

### <a name="stringlength-int"></a>stringLength (int)

Αυτή η ιδιότητα καθορίζει το μέγιστο μήκος για ένα πεδίο συμβολοσειράς. Ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Συμβολοσειρά**.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

Αυτή η ιδιότητα καθορίζει τον αριθμό των δεκαδικών ψηφίων που εμφανίζονται για ένα πραγματικό πεδίο. Ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Πραγματικό**.

### <a name="ordersequence-int"></a>orderSequence (int)

Αυτή η ιδιότητα ελέγχει τη σειρά με την οποία εμφανίζονται τα προσαρμοσμένα πεδία στην εφαρμογή, όταν καθορίζονται περισσότερα από ένα προσαρμοσμένα πεδία. Τα πεδία που έχουν χαμηλότερους αριθμούς εμφανίζονται πρώτα.

### <a name="booleanvalue-boolean"></a>booleanValue (δυαδική τιμή)

Για τα πεδία του τύπου **Δυαδική τιμή**, αυτή η ιδιότητα μεταβιβάζει τη δυαδική τιμή του πεδίου μεταξύ του διακομιστή και της εφαρμογής.

### <a name="guidvalue-guid"></a>guidValue (guid)

Για τα πεδία του τύπου **GUID**, αυτή η ιδιότητα μεταβιβάζει την τιμή του καθολικά μοναδικού αναγνωριστικού (GUID) μεταξύ του διακομιστή και της εφαρμογής.

### <a name="int64value-int64"></a>int64Value (int64)

Για τα πεδία του τύπου **Int64**, αυτή η ιδιότητα μεταβιβάζει την τιμή Int64 μεταξύ του διακομιστή και της εφαρμογής.

### <a name="intvalue-int"></a>intValue (int)

Για τα πεδία του τύπου **Int**, αυτή η ιδιότητα μεταβιβάζει την τιμή int μεταξύ του διακομιστή και της εφαρμογής.

### <a name="realvalue-real"></a>realValue (πραγματική)

Για τα πεδία του τύπου **Πραγματική**, αυτή η ιδιότητα μεταβιβάζει την πραγματική τιμή του πεδίου μεταξύ του διακομιστή και της εφαρμογής.

### <a name="stringvalue-str"></a>stringValue (str)

Για τα πεδία του τύπου **Συμβολοσειρά**, αυτή η ιδιότητα μεταβιβάζει την τιμή συμβολοσειράς μεταξύ του διακομιστή και της εφαρμογής. Χρησιμοποιείται επίσης για πεδία τύπου **Πραγματική** που έχουν μορφοποιηθεί ως νομισματική μονάδα. Για αυτά τα πεδία, η ιδιότητα χρησιμοποιείται για τη διαβίβαση του κωδικού νομίσματος στην εφαρμογή.

### <a name="datevalue-date"></a>dateValue (ημερομηνία)

Για τα πεδία του τύπου **Ημερομηνία**, αυτή η ιδιότητα μεταβιβάζει την τιμή ημερομηνίας του πεδίου μεταξύ του διακομιστή και της εφαρμογής.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>Εμφάνιση και αποθήκευση προσαρμοσμένου πεδίου στην ενότητα καταχώρησης φύλλου κατανομής χρόνου

Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές μιας δημιουργίας καταχώρησης φύλλου κατανομής χρόνου. Εμφανίζει τα εκτός πλαισίου πεδία και ένα προσαρμοσμένο πεδίο στην ενότητα "καταχώρηση ώρας" που ονομάζεται "δοκιμή συμβολοσειράς" με μια τιμή απαρίθμησης "δεύτερη επιλογή" που έχει ήδη οριστεί.

![Δοκιμαστικό προσαρμοσμένο πεδίο συμβολοσειράς στην εφαρμογή.](media/timesheet-entry.jpg)



Ακολουθεί ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές του χρήστη που επιλέγει μία από τις επιλογές απαρίθμησης που είναι διαθέσιμες για το προσαρμοσμένο πεδίο "δοκιμή συμβολοσειράς".  Οι δύο επιλογές είναι "πρώτη επιλογή" και "δεύτερη επιλογή" που εμφανίζεται ως κουμπιά επιλογής. Η δεύτερη επιλογή είναι αυτήν τη στιγμή επιλεγμένη.

![Κουμπιά επιλογών (κουμπιά επιλογής) για το προσαρμοσμένο πεδίο συμβολοσειράς δοκιμής.](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>Επέκταση του πίνακα TSTimesheetLine έτσι, ώστε να έχει ένα προσαρμοσμένο πεδίο

Σε τυπικά σενάρια, είναι πιθανό ότι τα δεδομένα για ένα προσαρμοσμένο πεδίο στην ενότητα "καταχώρηση φύλλου κατανομής χρόνου" θα αποθηκευτούν στον πίνακα TSTimesheetLine. Ωστόσο, είναι δυνατή η χρήση άλλων πινάκων, εάν είναι δυνατή η ανάκτηση των δεδομένων με βάση μια καρτέλα TSTimesheetTrans που παρέχεται ή εάν δεν υπάρχει συγκεκριμένο περιβάλλον καρτέλας (για παράδειγμα, εάν το πεδίο έχει οριστεί ως μόνο για ανάγνωση στις παραμέτρους του έργου).

Λάβετε υπόψη σας ότι τα προσαρμοσμένα πεδία δεν χρειάζεται να διαθέτουν καρτέλες της βάσης δεδομένων για τη δημιουργία αντιγράφων ασφαλείας. Μπορούν να δημιουργηθούν δυναμικά με βάση τη λογική του X++. Αυτή η προσέγγιση μπορεί να είναι χρήσιμη σε σενάρια μόνο για ανάγνωση (ανατρέξτε στην ενότητα "χρήση αλυσίδας εντολών στη μέθοδο TSTimesheetDetails Class, buildCustomFieldListForHeader για να συμπληρώσετε τις λεπτομέρειες του φύλλου κατανομής χρόνου" για ένα παράδειγμα τιμών προσαρμοσμένου πεδίου που δημιουργούνται δυναμικά.)

Ακολουθεί ένα στιγμιότυπο οθόνης από Visual Studio του δέντρου αντικειμένου εφαρμογής. Εμφανίζει μια επέκταση του πίνακα TSTimesheetLine με το πεδίο TestLineString να προστίθεται ως προσαρμοσμένο πεδίο.

![Συμβολοσειρά σειράς.](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldList της κλάσης TSTimesheetSettings για να εμφανιστεί ένα πεδίο στην ενότητα "καταχώρηση φύλλου κατανομής χρόνου"

Αυτός ο κωδικός ελέγχει τις ρυθμίσεις εμφάνισης για το πεδίο στην εφαρμογή. Για παράδειγμα, ελέγχει τον τύπο του πεδίου, την ετικέτα, εάν το πεδίο είναι υποχρεωτικό και σε ποια ενότητα εμφανίζεται το πεδίο.

Το παρακάτω παράδειγμα δείχνει ένα πεδίο συμβολοσειράς σε καταχωρήσεις χρόνου. Αυτό το πεδίο έχει δύο επιλογές, **Πρώτη επιλογή** και **Δεύτερη επιλογή**, που είναι διαθέσιμες μέσω κουμπιών επιλογής (κουμπιά επιλογής). Το πεδίο στην εφαρμογή συσχετίζεται με το πεδίο **TestLineString** το οποίο προστίθεται στον πίνακα TSTimesheetLine.

Λάβετε υπόψη σας τη χρήση της μεθόδου **TSTimesheetCustomField::newFromMetatdata()** για να απλοποιήσετε την προετοιμασία των ιδιοτήτων του προσαρμοσμένου πεδίου: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** και **numberOfDecimals**. Μπορείτε επίσης να ορίσετε αυτές τις παραμέτρους με μη αυτόματο τρόπο, όπως προτιμάτε.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldListForEntry της κλάσης TSTimesheetEntry για να καταχωρίσετε τιμές σε ένα φύλλο κατανομής χρόνου

Η μέθοδος **buildCustomFieldListForEntry** χρησιμοποιείται για την εισαγωγή τιμών στις αποθηκευμένες γραμμές φύλλου κατανομής χρόνου στην εφαρμογή για κινητές συσκευές. Χρειάζεται μια καρτέλα TSTimesheetTrans ως παράμετρος. Τα πεδία από αυτήν την καρτέλα μπορούν να χρησιμοποιηθούν για τη συμπλήρωση της τιμής του προσαρμοσμένου πεδίου στην εφαρμογή.

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>Χρησιμοποιήστε την αλυσίδα εντολών στην κλάση TSTimesheetEntryService για να αποθηκεύσετε μια καταχώρηση φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων

Για να αποθηκεύσετε ένα προσαρμοσμένο πεδίο πίσω στη βάση δεδομένων του με τυπική χρήση, πρέπει να επεκτείνετε πολλές μεθόδους:

- Η μέθοδος **timesheetLineNeedsUpdating** χρησιμοποιείται για να καθοριστεί εάν η καρτέλα της σειράς έχει αλλάξει από το χρήστη στην εφαρμογή και πρέπει να αποθηκευτεί στη βάση δεδομένων. Εάν η απόδοση δεν προκαλεί ανησυχία, αυτή η μέθοδος μπορεί να απλοποιηθεί έτσι ώστε να επιστρέφει πάντα **Αληθές**.
- Οι μέθοδοι **populateTimesheetLineFromEntryDuringCreate** και **populateTimesheetLineFromEntryDuringUpdate** μπορούν να επεκταθούν ώστε να εισαγάγουν τιμές στην καρτέλα της βάσης δεδομένων TSTimesheetLine από την καρτέλα της σύμβασης δεδομένων TSTimesheetEntry που παρέχεται. Στο παράδειγμα που ακολουθεί, προσέξτε πώς η αντιστοίχιση μεταξύ του πεδίου βάσης δεδομένων και του πεδίου καταχώρησης γίνεται με μη αυτόματο τρόπο μέσω του κωδικού X++.
- Η μέθοδος **populateTimesheetWeekFromEntry** μπορεί επίσης να επεκταθεί εάν το προσαρμοσμένο πεδίο που έχει αντιστοιχιστεί στο αντικείμενο **TSTimesheetEntry** πρέπει να επιστρέφεται στον πίνακα βάσης δεδομένων TSTimesheetLineweek.

> [!NOTE]
> Το παρακάτω παράδειγμα αποθηκεύει την τιμή **firstOption** ή **secondOption** που επιλέγει ο χρήστης για τη βάση δεδομένων ως μη επεξεργασμένη τιμή συμβολοσειράς. Εάν το πεδίο βάσης δεδομένων είναι ένα πεδίο του τύπου **Απαρίθμηση**, αυτές οι τιμές μπορούν να αντιστοιχιστούν με μη αυτόματο τρόπο σε μια τιμή απαρίθμησης και, στη συνέχεια, να αποθηκευτούν σε ένα πεδίο απαρίθμησης στον πίνακα βάσης δεδομένων.

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>Εμφάνιση προσαρμοσμένου πεδίου στην ενότητα κεφαλίδας φύλλου κατανομής χρόνου

Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές ενός χρήστη που βλέπει ένα φύλλο κατανομής χρόνου. Το κουμπί "Περισσότερες πληροφορίες" έχει επιλεγεί στην επάνω δεξιά γωνία για να εμφανιστεί η επιλογή "Προβολή περισσότερων λεπτομερειών".  

![Εντολή προβολής περισσότερων λεπτομερειών.](media/show-more.png)

Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές που δείχνει την ενότητα "Περισσότερα" ενός φύλλου κατανομής χρόνου. Ένα προσαρμοσμένο πεδίο που ονομάζεται "συντελεστής αξιοποίησης αυτού του φύλλου κατανομής χρόνου (υπολογιζόμενο προσαρμοσμένο πεδίο)" έχει προστεθεί στην ενότητα κεφαλίδας του φύλλου κατανομής χρόνου. Μια τιμή "0,667" που είναι μόνο για ανάγνωση ορίζεται στο προσαρμοσμένο πεδίο.

![Ενότητα Περισσότερα.](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>Επέκταση του πίνακα TSTimesheetTable έτσι, ώστε να έχει ένα προσαρμοσμένο πεδίο

Σε τυπικά σενάρια, είναι πιθανό ότι τα δεδομένα για ένα προσαρμοσμένο πεδίο στην ενότητα κεφαλίδας θα ληφθούν από τον πίνακα TSTimesheetHeader. Ωστόσο, είναι δυνατή η χρήση άλλων πινάκων, εάν είναι δυνατή η ανάκτηση των δεδομένων με βάση μια καρτέλα TSTimesheetTable που παρέχεται ή εάν δεν υπάρχει συγκεκριμένο περιβάλλον καρτέλας (για παράδειγμα, εάν το πεδίο έχει οριστεί ως μόνο για ανάγνωση στις παραμέτρους του έργου).

Λάβετε υπόψη σας ότι τα προσαρμοσμένα πεδία δεν χρειάζεται να διαθέτουν καρτέλες της βάσης δεδομένων για τη δημιουργία αντιγράφων ασφαλείας. Μπορούν να δημιουργηθούν δυναμικά με βάση τη λογική του X++. Το παράδειγμα που ακολουθεί δείχνει αυτήν την προσέγγιση.

Τα πεδία στην ενότητα "κεφαλίδα" είναι πάντα μόνο για ανάγνωση στην εφαρμογή.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldList της κλάσης TSTimesheetSettings για να εμφανιστεί ένα πεδίο στην ενότητα κεφαλίδας

Αυτός ο κωδικός ελέγχει τις ρυθμίσεις εμφάνισης για το πεδίο στην εφαρμογή. Για παράδειγμα, ελέγχει τον τύπο του πεδίου, την ετικέτα, εάν το πεδίο είναι υποχρεωτικό και σε ποια ενότητα εμφανίζεται το πεδίο.

Το παρακάτω παράδειγμα δείχνει μια υπολογιζόμενη τιμή στην ενότητα "κεφαλίδα" στην εφαρμογή.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldListForHeader της κλάσης TSTimesheetDetails για να συμπληρώσετε λεπτομέρειες στο φύλλο κατανομής χρόνου

Η μέθοδος **buildCustomFieldListForHeader** χρησιμοποιείται για την εισαγωγή λεπτομερειών κεφαλίδας φύλλου κατανομής χρόνου στην εφαρμογή για κινητές συσκευές. Χρειάζεται μια καρτέλα TSTimesheetTable ως παράμετρος. Τα πεδία από αυτήν την καρτέλα μπορούν να χρησιμοποιηθούν για τη συμπλήρωση της τιμής του προσαρμοσμένου πεδίου στην εφαρμογή. Το παρακάτω παράδειγμα δεν διαβάζει τις τιμές από τη βάση δεδομένων. Αντ' αυτού, χρησιμοποιεί τη λογική του X++ για τη δημιουργία μιας υπολογιζόμενης τιμής που εμφανίζεται στη συνέχεια στην εφαρμογή.


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a>Άλλες ευκαιρίες δυνατότητα ρύθμισης/επεκτασιμότητας

### <a name="adding-additional-validation-for-the-app"></a>Προσθήκη πρόσθετης επικύρωσης για την εφαρμογή

Η υπάρχουσα λογική για τη λειτουργικότητα του φύλλου κατανομής χρόνου στο επίπεδο βάσης δεδομένων θα συνεχίσει να λειτουργεί όπως αναμενόταν. Για να διακόψετε την ολοκλήρωση των λειτουργιών "Αποθήκευση" ή "υποβολή" και να εμφανιστεί ένα συγκεκριμένο μήνυμα σφάλματος, μπορείτε να προσθέσετε τη **δημιουργία σφάλματος ("μήνυμα προς χρήστη")** στον κώδικα μέσω μιας αλυσίδας επεκτάσεων εντολών. Ακολουθούν τρία παραδείγματα χρήσιμων επεκτάσιμων μεθόδων:

- Εάν το **validateWrite** στον πίνακα TSTimesheetLine επιστρέψει **ψευδές** κατά τη διάρκεια μιας λειτουργίας αποθήκευσης για μια γραμμή φύλλου κατανομής χρόνου, εμφανίζεται ένα μήνυμα σφάλματος στην εφαρμογή για κινητές συσκευές.
- Εάν το **validateSubmit** στον πίνακα TSTimesheetTable επιστρέψει **ψευδές** κατά τη διάρκεια μιας υποβολής φύλλου φύλλου κατανομής χρόνου στην εφαρμογή, εμφανίζεται ένα μήνυμα σφάλματος στον χρήστη.
- Η λογική που συμπληρώνει τα πεδία (για παράδειγμα, η **Ιδιότητα γραμμής**) κατά τη διάρκεια της μεθόδου **εισαγωγή** στον πίνακα TSTimesheetLine θα συνεχίσει να εκτελείται.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>Απόκρυψη και σήμανση έτοιμων πεδίων ως μόνο για ανάγνωση μέσω της ρύθμισης παραμέτρων

Από τις παραμέτρους του έργου, μπορείτε να κάνετε τα έτοιμα πεδία μόνο για ανάγνωση ή να τα έχετε κρυμμένα στην εφαρμογή για κινητές συσκευές. Ορίστε τις επιλογές στην ενότητα **Φύλλα κατανομής χρόνου για κινητές συσκευές** στην καρτέλα **Φύλλο κατανομής χρόνου** της σελίδας **Παράμετροι διαχείρισης έργου και λογιστικής**.

![Παράμετροι έργου.](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>Αλλαγή των δραστηριοτήτων που είναι διαθέσιμες για επιλογή μέσω επεκτάσεων

Οι δραστηριότητες που είναι διαθέσιμες για επιλογή για ένα έργο συμπληρώνονται μέσω των μεθόδων **getActivitiesForProject()** και **getActivityQuery()** στην κλάση **TsTimesheetProjectService**. Μπορείτε να χρησιμοποιήσετε την αλυσίδα εντολών για να αλλάξετε αυτήν τη συμπεριφορά ώστε να ταιριάζει με το σενάριο της επιχείρησής σας για τις δραστηριότητες που είναι διαθέσιμες για επιλογή για ένα συγκεκριμένο έργο.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>Εισαγωγή προεπιλεγμένης κατηγορίας έργου σε καταχωρήσεις φύλλου κατανομής χρόνου

Η καταχώρηση μιας προεπιλεγμένης κατηγορίας έργου σε καταχωρήσεις φύλλου κατανομής χρόνου παρουσιάζεται σε τρία επίπεδα. Μπορείτε να χρησιμοποιήσετε την αλυσίδα εντολών για να επεκτείνετε τη συμπεριφορά σε οποιοδήποτε ή όλα από αυτά τα επίπεδα για να επιτύχετε την επιθυμητή συμπεριφορά. Χρησιμοποιείται η ακόλουθη ιεραρχία:

1. Η εφαρμογή επιχειρεί να τοποθετήσει την προεπιλεγμένη κατηγορία από τον πόρο έργου. Αυτή η προεπιλεγμένη κατηγορία ορίζεται στις μεθόδους **getCurrentUserResource** και **getDelegatedResourcesForCurrentUser** στην κλάση **TSTimesheetSettingsService**.
2. Εάν η προεπιλεγμένη κατηγορία δεν παρέχεται σε επίπεδο πόρου έργου, η εφαρμογή επιχειρεί να την αποσύρει από τη δραστηριότητα του έργου. Αυτή η προεπιλεγμένη κατηγορία ορίζεται στη μέθοδο **getActivitiesForProject** στην κλάση **TSTimesheetProjectService**.
3. Εάν η προεπιλεγμένη κατηγορία δεν παρέχεται σε επίπεδο δραστηριότητας έργου, η προεπιλεγμένη κατηγορία λαμβάνεται από τις παραμέτρους έργου. Αυτή η προεπιλεγμένη κατηγορία ορίζεται στη μέθοδο **getProjectDetailsbyRule** στην κλάση **TSTimesheetProjectService**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]