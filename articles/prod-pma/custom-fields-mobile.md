---
title: Εφαρμόστε προσαρμοσμένα πεδία για την εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές σε iOS και Android
description: Αυτό το θέμα παρέχει συνήθη μοτίβα για τη χρήση επεκτάσεων για την εφαρμογή προσαρμοσμένων πεδίων.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 5dae571fce746b49281587f5349774a7f2c4111b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270993"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="77a70-103">Εφαρμόστε προσαρμοσμένα πεδία για την εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές σε iOS και Android</span><span class="sxs-lookup"><span data-stu-id="77a70-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="77a70-104">Αυτό το θέμα παρέχει συνήθη μοτίβα για τη χρήση επεκτάσεων για την εφαρμογή προσαρμοσμένων πεδίων.</span><span class="sxs-lookup"><span data-stu-id="77a70-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="77a70-105">Εξετάζονται τα εξής θέματα:</span><span class="sxs-lookup"><span data-stu-id="77a70-105">The following topics are covered:</span></span>

- <span data-ttu-id="77a70-106">Οι διάφοροι τύποι δεδομένων που υποστηρίζονται από το πλαίσιο του προσαρμοσμένου πεδίου</span><span class="sxs-lookup"><span data-stu-id="77a70-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="77a70-107">Ο τρόπος εμφάνισης πεδίων μόνο για ανάγνωση ή με δυνατότητα επεξεργασίας σε καταχωρήσεις φύλλου κατανομής χρόνου και η αποθήκευση τιμών που παρέχονται από το χρήστη πίσω στη βάση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="77a70-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="77a70-108">Ο τρόπος εμφάνισης πεδίων μόνο για ανάγνωση στην κεφαλίδα του φύλλου κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="77a70-109">Πώς να ενσωματώσετε άλλες προσαρμοσμένες επιχειρηματικές λογικές για την εισαγωγή προεπιλεγμένων τιμών σε πεδία και να κάνετε πρόσθετη επικύρωση</span><span class="sxs-lookup"><span data-stu-id="77a70-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="77a70-110">Κοινό</span><span class="sxs-lookup"><span data-stu-id="77a70-110">Audience</span></span>

<span data-ttu-id="77a70-111">Αυτό το θέμα απευθύνεται σε προγραμματιστές που ενσωματώνουν τα προσαρμοσμένα πεδία τους στην εφαρμογή Microsoft Dynamics 365 Project Timesheet για κινητές συσκευές η οποία είναι διαθέσιμη για Apple iOS και Google Android.</span><span class="sxs-lookup"><span data-stu-id="77a70-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="77a70-112">Η υπόθεση είναι ότι οι αναγνώστες εξοικειώνονται με την ανάπτυξη X++ και τη λειτουργικότητα του φύλλου εργασίας του έργου.</span><span class="sxs-lookup"><span data-stu-id="77a70-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="77a70-113">Σύμβαση δεδομένων – TSTimesheetCustomField X++ κλάση</span><span class="sxs-lookup"><span data-stu-id="77a70-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="77a70-114">Η κλάση **TSTimesheetCustomField** είναι η κλάση σύμβασης δεδομένων X++ η οποία αναπαριστά πληροφορίες σχετικά με ένα προσαρμοσμένο πεδίο για τη λειτουργικότητα του φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="77a70-115">Οι λίστες των αντικειμένων προσαρμοσμένων πεδίων μεταβιβάζονται τόσο στη σύμβαση δεδομένων TSTimesheetDetails όσο και στη σύμβαση δεδομένων TSTimesheetEntry για την εμφάνιση προσαρμοσμένων πεδίων στην εφαρμογή για κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="77a70-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="77a70-116">**TSTimesheetDetails** - Σύμβαση κεφαλίδας του φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="77a70-117">**TSTimesheetEntry** - Σύμβαση συναλλαγής φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="77a70-118">Οι ομάδες αυτών των αντικειμένων που έχουν τις ίδιες πληροφορίες έργου και την τιμή **timesheetLineRecId** αποτελούν μια γραμμή.</span><span class="sxs-lookup"><span data-stu-id="77a70-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="77a70-119">fieldBaseType (Τύποι)</span><span class="sxs-lookup"><span data-stu-id="77a70-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="77a70-120">Η ιδιότητα **FieldBaseType** στο αντικείμενο **TsTimesheetCustom** προσδιορίζει τον τύπο του πεδίου που εμφανίζεται στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="77a70-121">Οι ακόλουθοι **Τύποι** τιμών που υποστηρίζονται.</span><span class="sxs-lookup"><span data-stu-id="77a70-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="77a70-122">Τύπος τιμής</span><span class="sxs-lookup"><span data-stu-id="77a70-122">Types value</span></span> | <span data-ttu-id="77a70-123">Τύπος</span><span class="sxs-lookup"><span data-stu-id="77a70-123">Type</span></span>              | <span data-ttu-id="77a70-124">Σημειώσεις</span><span class="sxs-lookup"><span data-stu-id="77a70-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="77a70-125">1</span><span class="sxs-lookup"><span data-stu-id="77a70-125">0</span></span>           | <span data-ttu-id="77a70-126">Συμβολοσειρά (και απαρίθμηση)</span><span class="sxs-lookup"><span data-stu-id="77a70-126">String (and Enum)</span></span> | <span data-ttu-id="77a70-127">Το πεδίο εμφανίζεται ως πεδίο κειμένου.</span><span class="sxs-lookup"><span data-stu-id="77a70-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="77a70-128">1</span><span class="sxs-lookup"><span data-stu-id="77a70-128">1</span></span>           | <span data-ttu-id="77a70-129">Integer</span><span class="sxs-lookup"><span data-stu-id="77a70-129">Integer</span></span>           | <span data-ttu-id="77a70-130">Η τιμή εμφανίζεται ως αριθμός χωρίς δεκαδικά ψηφία.</span><span class="sxs-lookup"><span data-stu-id="77a70-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="77a70-131">2</span><span class="sxs-lookup"><span data-stu-id="77a70-131">2</span></span>           | <span data-ttu-id="77a70-132">Πραγματική</span><span class="sxs-lookup"><span data-stu-id="77a70-132">Real</span></span>              | <span data-ttu-id="77a70-133">Η τιμή εμφανίζεται ως αριθμός με δεκαδικά ψηφία.</span><span class="sxs-lookup"><span data-stu-id="77a70-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="77a70-134">Για να εμφανίσετε την πραγματική τιμή ως νομισματική μονάδα στην εφαρμογή, χρησιμοποιήστε την ιδιότητα **fieldExtenededType**.</span><span class="sxs-lookup"><span data-stu-id="77a70-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="77a70-135">Μπορείτε να χρησιμοποιήσετε την ιδιότητα **numberOfDecimals** για να ορίσετε τον αριθμό των δεκαδικών ψηφίων που εμφανίζονται.</span><span class="sxs-lookup"><span data-stu-id="77a70-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="77a70-136">3</span><span class="sxs-lookup"><span data-stu-id="77a70-136">3</span></span>           | <span data-ttu-id="77a70-137">Ημερομηνία</span><span class="sxs-lookup"><span data-stu-id="77a70-137">Date</span></span>              | <span data-ttu-id="77a70-138">Οι μορφές ημερομηνιών καθορίζονται από τη ρύθμιση **Μορφή αριθμού, ώρας και ημερομηνίας** του χρήστη που καθορίζεται στην περιοχή **Προτίμηση γλώσσας και χώρας/περιοχής** στις **Επιλογές χρήστη**.</span><span class="sxs-lookup"><span data-stu-id="77a70-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="77a70-139">4</span><span class="sxs-lookup"><span data-stu-id="77a70-139">4</span></span>           | <span data-ttu-id="77a70-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="77a70-140">Boolean</span></span>           | |
| <span data-ttu-id="77a70-141">15</span><span class="sxs-lookup"><span data-stu-id="77a70-141">15</span></span>          | <span data-ttu-id="77a70-142">GUID</span><span class="sxs-lookup"><span data-stu-id="77a70-142">GUID</span></span>              | |
| <span data-ttu-id="77a70-143">16</span><span class="sxs-lookup"><span data-stu-id="77a70-143">16</span></span>          | <span data-ttu-id="77a70-144">Int64</span><span class="sxs-lookup"><span data-stu-id="77a70-144">Int64</span></span>             | |

- <span data-ttu-id="77a70-145">Εάν η ιδιότητα **stringOptions** δεν παρέχεται στο αντικείμενο **TSTimesheetCustomField**, παρέχεται στο χρήστη ένα πεδίο ελεύθερου κειμένου.</span><span class="sxs-lookup"><span data-stu-id="77a70-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="77a70-146">Η ιδιότητα **stringLength** μπορεί να χρησιμοποιηθεί για τον ορισμό του μέγιστου μήκους συμβολοσειράς που μπορούν να εισαγάγουν οι χρήστες.</span><span class="sxs-lookup"><span data-stu-id="77a70-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="77a70-147">Εάν η ιδιότητα **stringOptions** παρέχεται στο αντικείμενο **TSTimesheetCustomField**, αυτά τα στοιχεία λίστας είναι οι μόνες τιμές που μπορούν να επιλέξουν οι χρήστες χρησιμοποιώντας τα κουμπιά επιλογής (κουμπιά επιλογής).</span><span class="sxs-lookup"><span data-stu-id="77a70-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="77a70-148">Σε αυτήν την περίπτωση, το πεδίο συμβολοσειράς μπορεί να ενεργήσει ως τιμή απαρίθμησης για το σκοπό της καταχώρησης χρήστη.</span><span class="sxs-lookup"><span data-stu-id="77a70-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="77a70-149">Για να αποθηκεύσετε την τιμή στη βάση δεδομένων ως απαρίθμηση, αντιστοιχίστε με μη αυτόματο τρόπο την τιμή της συμβολοσειράς στην τιμή "απαρίθμηση" πριν την αποθήκευση στη βάση δεδομένων χρησιμοποιώντας την αλυσίδα εντολών (ανατρέξτε στην ενότητα "χρήση της αλυσίδας εντολών στην κλάση TSTimesheetEntryService για την αποθήκευση μιας καταχώρησης φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων" στη συνέχεια αυτού του θέματος για παράδειγμα).</span><span class="sxs-lookup"><span data-stu-id="77a70-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="77a70-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="77a70-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="77a70-151">Μπορείτε να χρησιμοποιήσετε αυτήν την ιδιότητα για να μορφοποιήσετε πραγματικές τιμές ως νομισματικές μονάδες.</span><span class="sxs-lookup"><span data-stu-id="77a70-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="77a70-152">Αυτή η προσέγγιση εφαρμόζεται μόνο όταν η τιμή **fieldBaseType** είναι **Πραγματική**.</span><span class="sxs-lookup"><span data-stu-id="77a70-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="77a70-153">**TSCustomFieldExtendedType:None** – Δεν εφαρμόζεται καμία μορφοποίηση.</span><span class="sxs-lookup"><span data-stu-id="77a70-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="77a70-154">**TSCustomFieldExtendedType::Currency** – Μορφοποίηση της τιμής ως νομισματική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="77a70-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="77a70-155">Όταν η μορφοποίηση νομισματικής μονάδας είναι ενεργή, το πεδίο **stringValue** μπορεί να χρησιμοποιηθεί για να περάσει ο κωδικός νομίσματος που θα πρέπει να εμφανίζεται στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="77a70-156">Η τιμή είναι μια τιμή μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="77a70-156">The value is a read-only value.</span></span>

    <span data-ttu-id="77a70-157">Το πεδίο **realValue** περιέχει το χρηματικό ποσό που θα πρέπει να αποθηκευτεί στη βάση δεδομένων του.</span><span class="sxs-lookup"><span data-stu-id="77a70-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="77a70-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="77a70-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="77a70-159">Μπορείτε να χρησιμοποιήσετε αυτήν την ιδιότητα για να καθορίστε τη θέση στην οποία θα πρέπει να εμφανίζεται το προσαρμοσμένο πεδίο στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="77a70-160">**TSCustomFieldSection::Header** – Το πεδίο θα εμφανιστεί στην ενότητα **Προβολή περισσότερων λεπτομερειών** στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="77a70-161">Αυτά τα πεδία είναι πάντα για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="77a70-161">These fields are always read-only.</span></span>
- <span data-ttu-id="77a70-162">**TSCustomFieldSection::Line** – Το πεδίο θα εμφανιστεί μετά από όλα τα έτοιμα πεδία γραμμής στις καταχωρήσεις φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="77a70-163">Αυτά τα πεδία μπορεί να είναι επεξεργάσιμα ή μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="77a70-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="77a70-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="77a70-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="77a70-165">Αυτή η ιδιότητα προσδιορίζει το πεδίο όταν οι τιμές που παρέχει η εφαρμογή αποθηκεύονται ξανά στη βάση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="77a70-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="77a70-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="77a70-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="77a70-167">Αυτή η ιδιότητα προσδιορίζει το πεδίο όταν οι τιμές που παρέχει η εφαρμογή αποθηκεύονται ξανά στη βάση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="77a70-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="77a70-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="77a70-168">isEditable (NoYes)</span></span>

<span data-ttu-id="77a70-169">Ορίστε αυτήν την ιδιότητα σε **Ναι** για να καθορίσετε ότι το πεδίο στην ενότητα καταχώρησης φύλλου κατανομής χρόνου θα πρέπει να είναι επεξεργάσιμο από τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="77a70-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="77a70-170">Ορίστε την ιδιότητα σε **Όχι** ώστε το πεδίο να είναι μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="77a70-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="77a70-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="77a70-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="77a70-172">Ορίστε αυτήν την ιδιότητα σε **Ναι** για να καθορίσετε ότι το πεδίο στην ενότητα καταχώρησης φύλλου κατανομής χρόνου θα πρέπει να είναι υποχρεωτικό.</span><span class="sxs-lookup"><span data-stu-id="77a70-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="77a70-173">ετικέτα (str)</span><span class="sxs-lookup"><span data-stu-id="77a70-173">label (str)</span></span>

<span data-ttu-id="77a70-174">Αυτή η ιδιότητα καθορίζει την ετικέτα που εμφανίζεται δίπλα στο πεδίο στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="77a70-175">stringOptions (λίστα συμβολοσειρών)</span><span class="sxs-lookup"><span data-stu-id="77a70-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="77a70-176">Αυτή η ιδιότητα ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Συμβολοσειρά**.</span><span class="sxs-lookup"><span data-stu-id="77a70-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="77a70-177">Εάν έχει οριστεί το **stringOptions**, οι τιμές συμβολοσειράς που είναι διαθέσιμες για επιλογή μέσω των κουμπιών επιλογής (κουμπιά επιλογής) καθορίζονται από τις συμβολοσειρές που περιλαμβάνονται στη λίστα.</span><span class="sxs-lookup"><span data-stu-id="77a70-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="77a70-178">Εάν δεν παρέχονται συμβολοσειρές, επιτρέπεται η καταχώρηση ελεύθερων κειμένων στο πεδίο συμβολοσειράς (ανατρέξτε στην ενότητα "χρήση της αλυσίδας εντολών στην κλάση TSTimesheetEntryService για την αποθήκευση μιας καταχώρησης φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων" στη συνέχεια αυτού του θέματος για παράδειγμα).</span><span class="sxs-lookup"><span data-stu-id="77a70-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="77a70-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="77a70-179">stringLength (int)</span></span>

<span data-ttu-id="77a70-180">Αυτή η ιδιότητα καθορίζει το μέγιστο μήκος για ένα πεδίο συμβολοσειράς.</span><span class="sxs-lookup"><span data-stu-id="77a70-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="77a70-181">Ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Συμβολοσειρά**.</span><span class="sxs-lookup"><span data-stu-id="77a70-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="77a70-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="77a70-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="77a70-183">Αυτή η ιδιότητα καθορίζει τον αριθμό των δεκαδικών ψηφίων που εμφανίζονται για ένα πραγματικό πεδίο.</span><span class="sxs-lookup"><span data-stu-id="77a70-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="77a70-184">Ισχύει μόνο όταν το **fieldBaseType** έχει οριστεί σε **Πραγματικό**.</span><span class="sxs-lookup"><span data-stu-id="77a70-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="77a70-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="77a70-185">orderSequence (int)</span></span>

<span data-ttu-id="77a70-186">Αυτή η ιδιότητα ελέγχει τη σειρά με την οποία εμφανίζονται τα προσαρμοσμένα πεδία στην εφαρμογή, όταν καθορίζονται περισσότερα από ένα προσαρμοσμένα πεδία.</span><span class="sxs-lookup"><span data-stu-id="77a70-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="77a70-187">Τα πεδία που έχουν χαμηλότερους αριθμούς εμφανίζονται πρώτα.</span><span class="sxs-lookup"><span data-stu-id="77a70-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="77a70-188">booleanValue (δυαδική τιμή)</span><span class="sxs-lookup"><span data-stu-id="77a70-188">booleanValue (boolean)</span></span>

<span data-ttu-id="77a70-189">Για τα πεδία του τύπου **Δυαδική τιμή**, αυτή η ιδιότητα μεταβιβάζει τη δυαδική τιμή του πεδίου μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="77a70-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="77a70-190">guidValue (guid)</span></span>

<span data-ttu-id="77a70-191">Για τα πεδία του τύπου **GUID**, αυτή η ιδιότητα μεταβιβάζει την τιμή του καθολικά μοναδικού αναγνωριστικού (GUID) μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="77a70-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="77a70-192">int64Value (int64)</span></span>

<span data-ttu-id="77a70-193">Για τα πεδία του τύπου **Int64**, αυτή η ιδιότητα μεταβιβάζει την τιμή Int64 μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="77a70-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="77a70-194">intValue (int)</span></span>

<span data-ttu-id="77a70-195">Για τα πεδία του τύπου **Int**, αυτή η ιδιότητα μεταβιβάζει την τιμή int μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="77a70-196">realValue (πραγματική)</span><span class="sxs-lookup"><span data-stu-id="77a70-196">realValue (real)</span></span>

<span data-ttu-id="77a70-197">Για τα πεδία του τύπου **Πραγματική**, αυτή η ιδιότητα μεταβιβάζει την πραγματική τιμή του πεδίου μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="77a70-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="77a70-198">stringValue (str)</span></span>

<span data-ttu-id="77a70-199">Για τα πεδία του τύπου **Συμβολοσειρά**, αυτή η ιδιότητα μεταβιβάζει την τιμή συμβολοσειράς μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="77a70-200">Χρησιμοποιείται επίσης για πεδία τύπου **Πραγματική** που έχουν μορφοποιηθεί ως νομισματική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="77a70-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="77a70-201">Για αυτά τα πεδία, η ιδιότητα χρησιμοποιείται για τη διαβίβαση του κωδικού νομίσματος στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="77a70-202">dateValue (ημερομηνία)</span><span class="sxs-lookup"><span data-stu-id="77a70-202">dateValue (date)</span></span>

<span data-ttu-id="77a70-203">Για τα πεδία του τύπου **Ημερομηνία**, αυτή η ιδιότητα μεταβιβάζει την τιμή ημερομηνίας του πεδίου μεταξύ του διακομιστή και της εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="77a70-204">Εμφάνιση και αποθήκευση προσαρμοσμένου πεδίου στην ενότητα καταχώρησης φύλλου κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="77a70-205">Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές μιας δημιουργίας καταχώρησης φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="77a70-206">Εμφανίζει τα εκτός πλαισίου πεδία και ένα προσαρμοσμένο πεδίο στην ενότητα "καταχώρηση ώρας" που ονομάζεται "δοκιμή συμβολοσειράς" με μια τιμή απαρίθμησης "δεύτερη επιλογή" που έχει ήδη οριστεί.</span><span class="sxs-lookup"><span data-stu-id="77a70-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![Δοκιμαστικό προσαρμοσμένο πεδίο συμβολοσειράς στην εφαρμογή](media/timesheet-entry.jpg)



<span data-ttu-id="77a70-208">Ακολουθεί ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές του χρήστη που επιλέγει μία από τις επιλογές απαρίθμησης που είναι διαθέσιμες για το προσαρμοσμένο πεδίο "δοκιμή συμβολοσειράς".</span><span class="sxs-lookup"><span data-stu-id="77a70-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="77a70-209">Οι δύο επιλογές είναι "πρώτη επιλογή" και "δεύτερη επιλογή" που εμφανίζεται ως κουμπιά επιλογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="77a70-210">Η δεύτερη επιλογή είναι αυτήν τη στιγμή επιλεγμένη.</span><span class="sxs-lookup"><span data-stu-id="77a70-210">The second option is currently selected.</span></span>

![Κουμπιά επιλογών (κουμπιά επιλογής) για το προσαρμοσμένο πεδίο συμβολοσειράς δοκιμής](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="77a70-212">Επέκταση του πίνακα TSTimesheetLine έτσι, ώστε να έχει ένα προσαρμοσμένο πεδίο</span><span class="sxs-lookup"><span data-stu-id="77a70-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="77a70-213">Σε τυπικά σενάρια, είναι πιθανό ότι τα δεδομένα για ένα προσαρμοσμένο πεδίο στην ενότητα "καταχώρηση φύλλου κατανομής χρόνου" θα αποθηκευτούν στον πίνακα TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="77a70-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="77a70-214">Ωστόσο, είναι δυνατή η χρήση άλλων πινάκων, εάν είναι δυνατή η ανάκτηση των δεδομένων με βάση μια καρτέλα TSTimesheetTrans που παρέχεται ή εάν δεν υπάρχει συγκεκριμένο περιβάλλον καρτέλας (για παράδειγμα, εάν το πεδίο έχει οριστεί ως μόνο για ανάγνωση στις παραμέτρους του έργου).</span><span class="sxs-lookup"><span data-stu-id="77a70-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="77a70-215">Λάβετε υπόψη σας ότι τα προσαρμοσμένα πεδία δεν χρειάζεται να διαθέτουν καρτέλες της βάσης δεδομένων για τη δημιουργία αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="77a70-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="77a70-216">Μπορούν να δημιουργηθούν δυναμικά με βάση τη λογική του X++.</span><span class="sxs-lookup"><span data-stu-id="77a70-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="77a70-217">Αυτή η προσέγγιση μπορεί να είναι χρήσιμη σε σενάρια μόνο για ανάγνωση (ανατρέξτε στην ενότητα "χρήση αλυσίδας εντολών στη μέθοδο TSTimesheetDetails Class, buildCustomFieldListForHeader για να συμπληρώσετε τις λεπτομέρειες του φύλλου κατανομής χρόνου" για ένα παράδειγμα τιμών προσαρμοσμένου πεδίου που δημιουργούνται δυναμικά.)</span><span class="sxs-lookup"><span data-stu-id="77a70-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="77a70-218">Ακολουθεί ένα στιγμιότυπο οθόνης από Visual Studio του δέντρου αντικειμένου εφαρμογής.</span><span class="sxs-lookup"><span data-stu-id="77a70-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="77a70-219">Εμφανίζει μια επέκταση του πίνακα TSTimesheetLine με το πεδίο TestLineString να προστίθεται ως προσαρμοσμένο πεδίο.</span><span class="sxs-lookup"><span data-stu-id="77a70-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![Συμβολοσειρά σειράς](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="77a70-221">Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldList της κλάσης TSTimesheetSettings για να εμφανιστεί ένα πεδίο στην ενότητα "καταχώρηση φύλλου κατανομής χρόνου"</span><span class="sxs-lookup"><span data-stu-id="77a70-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="77a70-222">Αυτός ο κωδικός ελέγχει τις ρυθμίσεις εμφάνισης για το πεδίο στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="77a70-223">Για παράδειγμα, ελέγχει τον τύπο του πεδίου, την ετικέτα, εάν το πεδίο είναι υποχρεωτικό και σε ποια ενότητα εμφανίζεται το πεδίο.</span><span class="sxs-lookup"><span data-stu-id="77a70-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="77a70-224">Το παρακάτω παράδειγμα δείχνει ένα πεδίο συμβολοσειράς σε καταχωρήσεις χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="77a70-225">Αυτό το πεδίο έχει δύο επιλογές, **Πρώτη επιλογή** και **Δεύτερη επιλογή**, που είναι διαθέσιμες μέσω κουμπιών επιλογής (κουμπιά επιλογής).</span><span class="sxs-lookup"><span data-stu-id="77a70-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="77a70-226">Το πεδίο στην εφαρμογή συσχετίζεται με το πεδίο **TestLineString** το οποίο προστίθεται στον πίνακα TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="77a70-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="77a70-227">Λάβετε υπόψη σας τη χρήση της μεθόδου **TSTimesheetCustomField::newFromMetatdata()** για να απλοποιήσετε την προετοιμασία των ιδιοτήτων του προσαρμοσμένου πεδίου: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** και **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="77a70-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="77a70-228">Μπορείτε επίσης να ορίσετε αυτές τις παραμέτρους με μη αυτόματο τρόπο, όπως προτιμάτε.</span><span class="sxs-lookup"><span data-stu-id="77a70-228">You can also set these parameters manually, as you prefer.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="77a70-229">Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldListForEntry της κλάσης TSTimesheetEntry για να καταχωρίσετε τιμές σε ένα φύλλο κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="77a70-230">Η μέθοδος **buildCustomFieldListForEntry** χρησιμοποιείται για την εισαγωγή τιμών στις αποθηκευμένες γραμμές φύλλου κατανομής χρόνου στην εφαρμογή για κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="77a70-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="77a70-231">Χρειάζεται μια καρτέλα TSTimesheetTrans ως παράμετρος.</span><span class="sxs-lookup"><span data-stu-id="77a70-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="77a70-232">Τα πεδία από αυτήν την καρτέλα μπορούν να χρησιμοποιηθούν για τη συμπλήρωση της τιμής του προσαρμοσμένου πεδίου στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="77a70-233">Χρησιμοποιήστε την αλυσίδα εντολών στην κλάση TSTimesheetEntryService για να αποθηκεύσετε μια καταχώρηση φύλλου κατανομής χρόνου από την εφαρμογή ξανά στη βάση δεδομένων</span><span class="sxs-lookup"><span data-stu-id="77a70-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="77a70-234">Για να αποθηκεύσετε ένα προσαρμοσμένο πεδίο πίσω στη βάση δεδομένων του με τυπική χρήση, πρέπει να επεκτείνετε πολλές μεθόδους:</span><span class="sxs-lookup"><span data-stu-id="77a70-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="77a70-235">Η μέθοδος **timesheetLineNeedsUpdating** χρησιμοποιείται για να καθοριστεί εάν η καρτέλα της σειράς έχει αλλάξει από το χρήστη στην εφαρμογή και πρέπει να αποθηκευτεί στη βάση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="77a70-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="77a70-236">Εάν η απόδοση δεν προκαλεί ανησυχία, αυτή η μέθοδος μπορεί να απλοποιηθεί έτσι ώστε να επιστρέφει πάντα **Αληθές**.</span><span class="sxs-lookup"><span data-stu-id="77a70-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="77a70-237">Οι μέθοδοι **populateTimesheetLineFromEntryDuringCreate** και **populateTimesheetLineFromEntryDuringUpdate** μπορούν να επεκταθούν ώστε να εισαγάγουν τιμές στην καρτέλα της βάσης δεδομένων TSTimesheetLine από την καρτέλα της σύμβασης δεδομένων TSTimesheetEntry που παρέχεται.</span><span class="sxs-lookup"><span data-stu-id="77a70-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="77a70-238">Στο παράδειγμα που ακολουθεί, προσέξτε πώς η αντιστοίχιση μεταξύ του πεδίου βάσης δεδομένων και του πεδίου καταχώρησης γίνεται με μη αυτόματο τρόπο μέσω του κωδικού X++.</span><span class="sxs-lookup"><span data-stu-id="77a70-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="77a70-239">Η μέθοδος **populateTimesheetWeekFromEntry** μπορεί επίσης να επεκταθεί εάν το προσαρμοσμένο πεδίο που έχει αντιστοιχιστεί στο αντικείμενο **TSTimesheetEntry** πρέπει να επιστρέφεται στον πίνακα βάσης δεδομένων TSTimesheetLineweek.</span><span class="sxs-lookup"><span data-stu-id="77a70-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="77a70-240">Το παρακάτω παράδειγμα αποθηκεύει την τιμή **firstOption** ή **secondOption** που επιλέγει ο χρήστης για τη βάση δεδομένων ως μη επεξεργασμένη τιμή συμβολοσειράς.</span><span class="sxs-lookup"><span data-stu-id="77a70-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="77a70-241">Εάν το πεδίο βάσης δεδομένων είναι ένα πεδίο του τύπου **Απαρίθμηση**, αυτές οι τιμές μπορούν να αντιστοιχιστούν με μη αυτόματο τρόπο σε μια τιμή απαρίθμησης και, στη συνέχεια, να αποθηκευτούν σε ένα πεδίο απαρίθμησης στον πίνακα βάσης δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="77a70-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="77a70-242">Εμφάνιση προσαρμοσμένου πεδίου στην ενότητα κεφαλίδας φύλλου κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="77a70-243">Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές ενός χρήστη που βλέπει ένα φύλλο κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="77a70-244">Το κουμπί "Περισσότερες πληροφορίες" έχει επιλεγεί στην επάνω δεξιά γωνία για να εμφανιστεί η επιλογή "Προβολή περισσότερων λεπτομερειών".</span><span class="sxs-lookup"><span data-stu-id="77a70-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![Εντολή προβολής περισσότερων λεπτομερειών](media/show-more.png)

<span data-ttu-id="77a70-246">Παρακάτω περιλαμβάνεται ένα στιγμιότυπο οθόνης από την εφαρμογή για κινητές συσκευές που δείχνει την ενότητα "Περισσότερα" ενός φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="77a70-247">Ένα προσαρμοσμένο πεδίο που ονομάζεται "συντελεστής αξιοποίησης αυτού του φύλλου κατανομής χρόνου (υπολογιζόμενο προσαρμοσμένο πεδίο)" έχει προστεθεί στην ενότητα κεφαλίδας του φύλλου κατανομής χρόνου.</span><span class="sxs-lookup"><span data-stu-id="77a70-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="77a70-248">Μια τιμή "0,667" που είναι μόνο για ανάγνωση ορίζεται στο προσαρμοσμένο πεδίο.</span><span class="sxs-lookup"><span data-stu-id="77a70-248">A read-only value of "0.667" is set on the custom field.</span></span>

![Ενότητα Περισσότερα](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="77a70-250">Επέκταση του πίνακα TSTimesheetTable έτσι, ώστε να έχει ένα προσαρμοσμένο πεδίο</span><span class="sxs-lookup"><span data-stu-id="77a70-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="77a70-251">Σε τυπικά σενάρια, είναι πιθανό ότι τα δεδομένα για ένα προσαρμοσμένο πεδίο στην ενότητα κεφαλίδας θα ληφθούν από τον πίνακα TSTimesheetHeader.</span><span class="sxs-lookup"><span data-stu-id="77a70-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="77a70-252">Ωστόσο, είναι δυνατή η χρήση άλλων πινάκων, εάν είναι δυνατή η ανάκτηση των δεδομένων με βάση μια καρτέλα TSTimesheetTable που παρέχεται ή εάν δεν υπάρχει συγκεκριμένο περιβάλλον καρτέλας (για παράδειγμα, εάν το πεδίο έχει οριστεί ως μόνο για ανάγνωση στις παραμέτρους του έργου).</span><span class="sxs-lookup"><span data-stu-id="77a70-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="77a70-253">Λάβετε υπόψη σας ότι τα προσαρμοσμένα πεδία δεν χρειάζεται να διαθέτουν καρτέλες της βάσης δεδομένων για τη δημιουργία αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="77a70-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="77a70-254">Μπορούν να δημιουργηθούν δυναμικά με βάση τη λογική του X++.</span><span class="sxs-lookup"><span data-stu-id="77a70-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="77a70-255">Το παράδειγμα που ακολουθεί δείχνει αυτήν την προσέγγιση.</span><span class="sxs-lookup"><span data-stu-id="77a70-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="77a70-256">Τα πεδία στην ενότητα "κεφαλίδα" είναι πάντα μόνο για ανάγνωση στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="77a70-257">Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldList της κλάσης TSTimesheetSettings για να εμφανιστεί ένα πεδίο στην ενότητα κεφαλίδας</span><span class="sxs-lookup"><span data-stu-id="77a70-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="77a70-258">Αυτός ο κωδικός ελέγχει τις ρυθμίσεις εμφάνισης για το πεδίο στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="77a70-259">Για παράδειγμα, ελέγχει τον τύπο του πεδίου, την ετικέτα, εάν το πεδίο είναι υποχρεωτικό και σε ποια ενότητα εμφανίζεται το πεδίο.</span><span class="sxs-lookup"><span data-stu-id="77a70-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="77a70-260">Το παρακάτω παράδειγμα δείχνει μια υπολογιζόμενη τιμή στην ενότητα "κεφαλίδα" στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-260">The following example shows a computed value in the header section in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="77a70-261">Χρησιμοποιήστε την αλυσίδα εντολών στη μέθοδο buildCustomFieldListForHeader της κλάσης TSTimesheetDetails για να συμπληρώσετε λεπτομέρειες στο φύλλο κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="77a70-262">Η μέθοδος **buildCustomFieldListForHeader** χρησιμοποιείται για την εισαγωγή λεπτομερειών κεφαλίδας φύλλου κατανομής χρόνου στην εφαρμογή για κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="77a70-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="77a70-263">Χρειάζεται μια καρτέλα TSTimesheetTable ως παράμετρος.</span><span class="sxs-lookup"><span data-stu-id="77a70-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="77a70-264">Τα πεδία από αυτήν την καρτέλα μπορούν να χρησιμοποιηθούν για τη συμπλήρωση της τιμής του προσαρμοσμένου πεδίου στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="77a70-265">Το παρακάτω παράδειγμα δεν διαβάζει τις τιμές από τη βάση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="77a70-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="77a70-266">Αντ' αυτού, χρησιμοποιεί τη λογική του X++ για τη δημιουργία μιας υπολογιζόμενης τιμής που εμφανίζεται στη συνέχεια στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="77a70-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


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

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="77a70-267">Άλλες ευκαιρίες δυνατότητα ρύθμισης/επεκτασιμότητας</span><span class="sxs-lookup"><span data-stu-id="77a70-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="77a70-268">Προσθήκη πρόσθετης επικύρωσης για την εφαρμογή</span><span class="sxs-lookup"><span data-stu-id="77a70-268">Adding additional validation for the app</span></span>

<span data-ttu-id="77a70-269">Η υπάρχουσα λογική για τη λειτουργικότητα του φύλλου κατανομής χρόνου στο επίπεδο βάσης δεδομένων θα συνεχίσει να λειτουργεί όπως αναμενόταν.</span><span class="sxs-lookup"><span data-stu-id="77a70-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="77a70-270">Για να διακόψετε την ολοκλήρωση των λειτουργιών "Αποθήκευση" ή "υποβολή" και να εμφανιστεί ένα συγκεκριμένο μήνυμα σφάλματος, μπορείτε να προσθέσετε τη **δημιουργία σφάλματος ("μήνυμα προς χρήστη")** στον κώδικα μέσω μιας αλυσίδας επεκτάσεων εντολών.</span><span class="sxs-lookup"><span data-stu-id="77a70-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="77a70-271">Ακολουθούν τρία παραδείγματα χρήσιμων επεκτάσιμων μεθόδων:</span><span class="sxs-lookup"><span data-stu-id="77a70-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="77a70-272">Εάν το **validateWrite** στον πίνακα TSTimesheetLine επιστρέψει **ψευδές** κατά τη διάρκεια μιας λειτουργίας αποθήκευσης για μια γραμμή φύλλου κατανομής χρόνου, εμφανίζεται ένα μήνυμα σφάλματος στην εφαρμογή για κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="77a70-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="77a70-273">Εάν το **validateSubmit** στον πίνακα TSTimesheetTable επιστρέψει **ψευδές** κατά τη διάρκεια μιας υποβολής φύλλου φύλλου κατανομής χρόνου στην εφαρμογή, εμφανίζεται ένα μήνυμα σφάλματος στον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="77a70-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="77a70-274">Η λογική που συμπληρώνει τα πεδία (για παράδειγμα, η **Ιδιότητα γραμμής**) κατά τη διάρκεια της μεθόδου **εισαγωγή** στον πίνακα TSTimesheetLine θα συνεχίσει να εκτελείται.</span><span class="sxs-lookup"><span data-stu-id="77a70-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="77a70-275">Απόκρυψη και σήμανση έτοιμων πεδίων ως μόνο για ανάγνωση μέσω της ρύθμισης παραμέτρων</span><span class="sxs-lookup"><span data-stu-id="77a70-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="77a70-276">Από τις παραμέτρους του έργου, μπορείτε να κάνετε τα έτοιμα πεδία μόνο για ανάγνωση ή να τα έχετε κρυμμένα στην εφαρμογή για κινητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="77a70-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="77a70-277">Ορίστε τις επιλογές στην ενότητα **Φύλλα κατανομής χρόνου για κινητές συσκευές** στην καρτέλα **Φύλλο κατανομής χρόνου** της σελίδας **Παράμετροι διαχείρισης έργου και λογιστικής**.</span><span class="sxs-lookup"><span data-stu-id="77a70-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![Παράμετροι έργου](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="77a70-279">Αλλαγή των δραστηριοτήτων που είναι διαθέσιμες για επιλογή μέσω επεκτάσεων</span><span class="sxs-lookup"><span data-stu-id="77a70-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="77a70-280">Οι δραστηριότητες που είναι διαθέσιμες για επιλογή για ένα έργο συμπληρώνονται μέσω των μεθόδων **getActivitiesForProject()** και **getActivityQuery()** στην κλάση **TsTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="77a70-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="77a70-281">Μπορείτε να χρησιμοποιήσετε την αλυσίδα εντολών για να αλλάξετε αυτήν τη συμπεριφορά ώστε να ταιριάζει με το σενάριο της επιχείρησής σας για τις δραστηριότητες που είναι διαθέσιμες για επιλογή για ένα συγκεκριμένο έργο.</span><span class="sxs-lookup"><span data-stu-id="77a70-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="77a70-282">Εισαγωγή προεπιλεγμένης κατηγορίας έργου σε καταχωρήσεις φύλλου κατανομής χρόνου</span><span class="sxs-lookup"><span data-stu-id="77a70-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="77a70-283">Η καταχώρηση μιας προεπιλεγμένης κατηγορίας έργου σε καταχωρήσεις φύλλου κατανομής χρόνου παρουσιάζεται σε τρία επίπεδα.</span><span class="sxs-lookup"><span data-stu-id="77a70-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="77a70-284">Μπορείτε να χρησιμοποιήσετε την αλυσίδα εντολών για να επεκτείνετε τη συμπεριφορά σε οποιοδήποτε ή όλα από αυτά τα επίπεδα για να επιτύχετε την επιθυμητή συμπεριφορά.</span><span class="sxs-lookup"><span data-stu-id="77a70-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="77a70-285">Χρησιμοποιείται η ακόλουθη ιεραρχία:</span><span class="sxs-lookup"><span data-stu-id="77a70-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="77a70-286">Η εφαρμογή επιχειρεί να τοποθετήσει την προεπιλεγμένη κατηγορία από τον πόρο έργου.</span><span class="sxs-lookup"><span data-stu-id="77a70-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="77a70-287">Αυτή η προεπιλεγμένη κατηγορία ορίζεται στις μεθόδους **getCurrentUserResource** και **getDelegatedResourcesForCurrentUser** στην κλάση **TSTimesheetSettingsService**.</span><span class="sxs-lookup"><span data-stu-id="77a70-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="77a70-288">Εάν η προεπιλεγμένη κατηγορία δεν παρέχεται σε επίπεδο πόρου έργου, η εφαρμογή επιχειρεί να την αποσύρει από τη δραστηριότητα του έργου.</span><span class="sxs-lookup"><span data-stu-id="77a70-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="77a70-289">Αυτή η προεπιλεγμένη κατηγορία ορίζεται στη μέθοδο **getActivitiesForProject** στην κλάση **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="77a70-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="77a70-290">Εάν η προεπιλεγμένη κατηγορία δεν παρέχεται σε επίπεδο δραστηριότητας έργου, η προεπιλεγμένη κατηγορία λαμβάνεται από τις παραμέτρους έργου.</span><span class="sxs-lookup"><span data-stu-id="77a70-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="77a70-291">Αυτή η προεπιλεγμένη κατηγορία ορίζεται στη μέθοδο **getProjectDetailsbyRule** στην κλάση **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="77a70-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]