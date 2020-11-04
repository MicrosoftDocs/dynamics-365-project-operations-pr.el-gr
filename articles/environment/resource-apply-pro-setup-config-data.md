---
title: Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service for Project Operations
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης και εφαρμογής των δεδομένων διαμόρφωσης στο Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e72b88a4dae1eb89859fdfd55f6d5e6ee5befcd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076789"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="1879d-103">Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service for Project Operations</span><span class="sxs-lookup"><span data-stu-id="1879d-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="1879d-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="1879d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="1879d-105">Εγκατάσταση δεδομένων ρύθμισης παραμέτρων και διαμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="1879d-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="1879d-106">Πραγματοποιήστε λήψη, κατάργηση αποκλεισμού και αποσυμπιέστε το [πακέτο δεδομένων εγκατάστασης και ρύθμισης παραμέτρων](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="1879d-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="1879d-107">Μεταβείτε στον αποσυμπιεσμένο φάκελο και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="1879d-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="1879d-108">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="1879d-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="1879d-110">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="1879d-110">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="1879d-111">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="1879d-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="1879d-112">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="1879d-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="1879d-114">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="1879d-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="1879d-115">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *SampleSetupAndConfigData* από τον μη συμπιεσμένο φάκελο.</span><span class="sxs-lookup"><span data-stu-id="1879d-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Επιλογή συμπιεσμένου αρχείου](./media/3ZipFile.png)

![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="1879d-118">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="1879d-118">After the zip file is selected, select **Import Data**.</span></span>

![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="1879d-120">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="1879d-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="1879d-121">Αφού ολοκληρωθεί η εισαγωγή, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="1879d-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="1879d-122">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 19 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="1879d-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="1879d-123">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="1879d-123">Currency</span></span>
  - <span data-ttu-id="1879d-124">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="1879d-124">Organizational Unit</span></span>
  - <span data-ttu-id="1879d-125">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="1879d-125">Contact</span></span>
  - <span data-ttu-id="1879d-126">Ομάδα φόρων</span><span class="sxs-lookup"><span data-stu-id="1879d-126">Tax Group</span></span>
  - <span data-ttu-id="1879d-127">Ομάδα πελατών</span><span class="sxs-lookup"><span data-stu-id="1879d-127">Customer Group</span></span>
  - <span data-ttu-id="1879d-128">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="1879d-128">Unit</span></span>
  - <span data-ttu-id="1879d-129">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="1879d-129">Unit Group</span></span>
  - <span data-ttu-id="1879d-130">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="1879d-130">Price List</span></span>
  - <span data-ttu-id="1879d-131">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="1879d-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="1879d-132">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="1879d-132">Invoice Frequency</span></span>
  - <span data-ttu-id="1879d-133">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="1879d-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="1879d-134">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="1879d-134">Transaction Category</span></span>
  - <span data-ttu-id="1879d-135">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="1879d-135">Expense Category</span></span>
  - <span data-ttu-id="1879d-136">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="1879d-136">Role Price</span></span>
  - <span data-ttu-id="1879d-137">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="1879d-137">Transaction Category Price</span></span>
  - <span data-ttu-id="1879d-138">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="1879d-138">Characteristic</span></span>
  - <span data-ttu-id="1879d-139">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="1879d-139">Bookable Resource</span></span>
  - <span data-ttu-id="1879d-140">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="1879d-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="1879d-141">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="1879d-141">Bookable Resource Characteristic</span></span>

![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="1879d-143">Ενημέρωση διαμορφώσεων Project Operations</span><span class="sxs-lookup"><span data-stu-id="1879d-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="1879d-144">Περιήγηση στο περιβάλλον CE.</span><span class="sxs-lookup"><span data-stu-id="1879d-144">Navigate to the CE environment.</span></span> <span data-ttu-id="1879d-145">Μπορείτε να το βρείτε ανοίγοντας το [Κέντρο διαχείρισης του Power Platform](https://admin.powerplatform.microsoft.com/environments), επιλέγοντας το περιβάλλον και, στη συνέχεια, επιλέγοντας **Άνοιγμα περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="1879d-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Άνοιγμα περιβάλλοντος](./media/7OpenEnvironment.png)

2. <span data-ttu-id="1879d-147">Μεταβείτε στα στοιχεία **Έργα** > **Πόροι** και, στη συνέχεια, επιλέξτε **Δημιουργία** για να δημιουργήσετε έναν πόρο με κράτηση για τον χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="1879d-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Πόροι με δυνατότητα κράτησης](./media/8BookableResources.png)

3. <span data-ttu-id="1879d-149">Στην καρτέλα **Γενικά** , επιλέξτε τον χρήστη διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="1879d-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="1879d-150">Επαληθεύστε ότι η ζώνη ώρας ταιριάζει με αυτήν στην οποία βρίσκεστε.</span><span class="sxs-lookup"><span data-stu-id="1879d-150">Verify that the time zone matches the one you are in.</span></span> 

![Νέος πόρος με δυνατότητα κράτησης](./media/9NewBookableResource.png)

4. <span data-ttu-id="1879d-152">Στην καρτέλα **Προγραμματισμός** , στο πεδίο **Εταιρεία** , επιλέξτε την εταιρεία **USPM** και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1879d-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Καρτέλα προγραμματισμού](./media/10SchedulingTab.png)

5. <span data-ttu-id="1879d-154">Επιλέξτε την καρτέλα **Ώρες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="1879d-154">Select the **Work hours** tab.</span></span>  

![Ώρες εργασίας](./media/11WorkHours.png)

6. <span data-ttu-id="1879d-156">Κάντε διπλό κλικ σε οποιαδήποτε τιμή στο ημερολόγιο και επιλέξτε **Επεξεργασία** > **Όλα τα συμβάντα στη σειρά**.</span><span class="sxs-lookup"><span data-stu-id="1879d-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Ημερολόγιο εργασίας](./media/12WorkCalendar.png)

7. <span data-ttu-id="1879d-158">Αλλάξτε τις ώρες εργασίας σε μια εργάσιμη ημέρα οκτώ (8) ωρών, επισημάνετε τα σαββατοκύριακα ως μη εργάσιμες ημέρες και βεβαιωθείτε ότι η ζώνη ώρας ταιριάζει με τη δική σας.</span><span class="sxs-lookup"><span data-stu-id="1879d-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="1879d-159">Επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="1879d-159">Select **Save and close**.</span></span>

![Ενημέρωση ημερολογίου](./media/13UpdateCalendar.png)

9. <span data-ttu-id="1879d-161">Μεταβείτε στις **Ρυθμίσεις** > **Πρότυπα ημερολογίου** και επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="1879d-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Πρότυπα ημερολογίου](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="1879d-163">Καταγράψτε ένα όνομα, επιλέξτε τον πρότυπο πόρο που δημιουργήσατε και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1879d-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Αποθήκευση προτύπου ημερολογίου](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="1879d-165">Μεταβείτε στο στοιχείο **Παράμετροι** και κάντε διπλό κλικ στην καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="1879d-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Παράμετροι έργου](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="1879d-167">Ενημερώστε τα παρακάτω πεδία:</span><span class="sxs-lookup"><span data-stu-id="1879d-167">Update the following fields:</span></span>

 - <span data-ttu-id="1879d-168">**Προεπιλεγμένη εταιρεία** : USPM</span><span class="sxs-lookup"><span data-stu-id="1879d-168">**Default company** : USPM</span></span>
 - <span data-ttu-id="1879d-169">**Προεπιλεγμένη οργανωτική μονάδα** : Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="1879d-169">**Default Organizational Unit** : Contoso Robotics Global</span></span>
 - <span data-ttu-id="1879d-170">**Συχνότητα τιμολογίου** : έβδομη και τελευταία ημέρα</span><span class="sxs-lookup"><span data-stu-id="1879d-170">**Invoice Frequency** : Seventh and Last day</span></span>
 - <span data-ttu-id="1879d-171">**Πρότυπο ωρών εργασίας** : Αλλάξτε στο πρότυπο που δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="1879d-171">**Work hour template** : Change to the template you created.</span></span>

13. <span data-ttu-id="1879d-172">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1879d-172">Select **Save**.</span></span> 

![Ενημερωμένες παράμετροι έργου](./media/17UpdatedProjectParameters.png)
