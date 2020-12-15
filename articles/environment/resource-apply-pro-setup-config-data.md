---
title: Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης και εφαρμογής των δεδομένων διαμόρφωσης στο Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7742e81316b217066f9f3b8d5c23aa64f1a7efc4
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642228"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="46fc7-103">Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service</span><span class="sxs-lookup"><span data-stu-id="46fc7-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="46fc7-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="46fc7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="46fc7-105">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="46fc7-105">Prerequisites</span></span>

<span data-ttu-id="46fc7-106">Προτού ξεκινήσετε τη ρύθμιση των δεδομένων στο Common Data Service (CD), πρέπει να πληρούνται οι ακόλουθες προϋποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="46fc7-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="46fc7-107">Παροχή ενός περιβάλλοντος CDS και ενός Dynamics 365 Finance περιβάλλοντος για το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="46fc7-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="46fc7-108">Οι πληροφορίες νομικής οντότητας από το Dynamics 365 Finance είναι κοινόχρηστες στο περιβάλλον CDS.</span><span class="sxs-lookup"><span data-stu-id="46fc7-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="46fc7-109">Αυτό σημαίνει ότι η οντότητα **Εταιρεία** στο CDS έχει τις ακόλουθες εταιρικές καρτέλες:</span><span class="sxs-lookup"><span data-stu-id="46fc7-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="46fc7-110">THPM</span><span class="sxs-lookup"><span data-stu-id="46fc7-110">THPM</span></span>
  - <span data-ttu-id="46fc7-111">USPM</span><span class="sxs-lookup"><span data-stu-id="46fc7-111">USPM</span></span>
  - <span data-ttu-id="46fc7-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="46fc7-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="46fc7-113">Εγκατάσταση δεδομένων ρύθμισης παραμέτρων και διαμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="46fc7-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="46fc7-114">Πραγματοποιήστε λήψη, κατάργηση αποκλεισμού και αποσυμπιέστε το [πακέτο δεδομένων εγκατάστασης και ρύθμισης παραμέτρων](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="46fc7-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="46fc7-115">Μεταβείτε στον αποσυμπιεσμένο φάκελο και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="46fc7-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="46fc7-116">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="46fc7-118">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="46fc7-119">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="46fc7-120">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="46fc7-122">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="46fc7-123">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *SampleSetupAndConfigData* από τον μη συμπιεσμένο φάκελο.</span><span class="sxs-lookup"><span data-stu-id="46fc7-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Επιλογή συμπιεσμένου αρχείου](./media/3ZipFile.png)

![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="46fc7-126">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-126">After the zip file is selected, select **Import Data**.</span></span>

![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="46fc7-128">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="46fc7-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="46fc7-129">Αφού ολοκληρωθεί η εισαγωγή, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="46fc7-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="46fc7-130">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 19 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="46fc7-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="46fc7-131">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="46fc7-131">Currency</span></span>
  - <span data-ttu-id="46fc7-132">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="46fc7-132">Organizational Unit</span></span>
  - <span data-ttu-id="46fc7-133">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="46fc7-133">Contact</span></span>
  - <span data-ttu-id="46fc7-134">Ομάδα φόρων</span><span class="sxs-lookup"><span data-stu-id="46fc7-134">Tax Group</span></span>
  - <span data-ttu-id="46fc7-135">Ομάδα πελατών</span><span class="sxs-lookup"><span data-stu-id="46fc7-135">Customer Group</span></span>
  - <span data-ttu-id="46fc7-136">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="46fc7-136">Unit</span></span>
  - <span data-ttu-id="46fc7-137">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="46fc7-137">Unit Group</span></span>
  - <span data-ttu-id="46fc7-138">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="46fc7-138">Price List</span></span>
  - <span data-ttu-id="46fc7-139">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="46fc7-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="46fc7-140">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="46fc7-140">Invoice Frequency</span></span>
  - <span data-ttu-id="46fc7-141">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="46fc7-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="46fc7-142">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="46fc7-142">Transaction Category</span></span>
  - <span data-ttu-id="46fc7-143">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="46fc7-143">Expense Category</span></span>
  - <span data-ttu-id="46fc7-144">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="46fc7-144">Role Price</span></span>
  - <span data-ttu-id="46fc7-145">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="46fc7-145">Transaction Category Price</span></span>
  - <span data-ttu-id="46fc7-146">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="46fc7-146">Characteristic</span></span>
  - <span data-ttu-id="46fc7-147">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="46fc7-147">Bookable Resource</span></span>
  - <span data-ttu-id="46fc7-148">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="46fc7-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="46fc7-149">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="46fc7-149">Bookable Resource Characteristic</span></span>

![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="46fc7-151">Ενημέρωση διαμορφώσεων Project Operations</span><span class="sxs-lookup"><span data-stu-id="46fc7-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="46fc7-152">Περιήγηση στο περιβάλλον CE.</span><span class="sxs-lookup"><span data-stu-id="46fc7-152">Navigate to the CE environment.</span></span> <span data-ttu-id="46fc7-153">Μπορείτε να το βρείτε ανοίγοντας το [Κέντρο διαχείρισης του Power Platform](https://admin.powerplatform.microsoft.com/environments), επιλέγοντας το περιβάλλον και, στη συνέχεια, επιλέγοντας **Άνοιγμα περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Άνοιγμα περιβάλλοντος](./media/7OpenEnvironment.png)

2. <span data-ttu-id="46fc7-155">Μεταβείτε στα στοιχεία **Έργα** > **Πόροι** και, στη συνέχεια, επιλέξτε **Δημιουργία** για να δημιουργήσετε έναν πόρο με κράτηση για τον χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="46fc7-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Πόροι με δυνατότητα κράτησης](./media/8BookableResources.png)

3. <span data-ttu-id="46fc7-157">Στην καρτέλα **Γενικά**, επιλέξτε τον χρήστη διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="46fc7-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="46fc7-158">Επαληθεύστε ότι η ζώνη ώρας ταιριάζει με αυτήν στην οποία βρίσκεστε.</span><span class="sxs-lookup"><span data-stu-id="46fc7-158">Verify that the time zone matches the one you are in.</span></span> 

![Νέος πόρος με δυνατότητα κράτησης](./media/9NewBookableResource.png)

4. <span data-ttu-id="46fc7-160">Στην καρτέλα **Προγραμματισμός**, στο πεδίο **Εταιρεία**, επιλέξτε την εταιρεία **USPM** και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Καρτέλα προγραμματισμού](./media/10SchedulingTab.png)

5. <span data-ttu-id="46fc7-162">Επιλέξτε την καρτέλα **Ώρες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-162">Select the **Work hours** tab.</span></span>  

![Ώρες εργασίας](./media/11WorkHours.png)

6. <span data-ttu-id="46fc7-164">Κάντε διπλό κλικ σε οποιαδήποτε τιμή στο ημερολόγιο και επιλέξτε **Επεξεργασία** > **Όλα τα συμβάντα στη σειρά**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Ημερολόγιο εργασίας](./media/12WorkCalendar.png)

7. <span data-ttu-id="46fc7-166">Αλλάξτε τις ώρες εργασίας σε μια εργάσιμη ημέρα οκτώ (8) ωρών, επισημάνετε τα σαββατοκύριακα ως μη εργάσιμες ημέρες και βεβαιωθείτε ότι η ζώνη ώρας ταιριάζει με τη δική σας.</span><span class="sxs-lookup"><span data-stu-id="46fc7-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="46fc7-167">Επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-167">Select **Save and close**.</span></span>

![Ενημέρωση ημερολογίου](./media/13UpdateCalendar.png)

9. <span data-ttu-id="46fc7-169">Μεταβείτε στις **Ρυθμίσεις** > **Πρότυπα ημερολογίου** και επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Πρότυπα ημερολογίου](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="46fc7-171">Καταγράψτε ένα όνομα, επιλέξτε τον πρότυπο πόρο που δημιουργήσατε και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Αποθήκευση προτύπου ημερολογίου](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="46fc7-173">Μεταβείτε στο στοιχείο **Παράμετροι** και κάντε διπλό κλικ στην καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="46fc7-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Παράμετροι έργου](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="46fc7-175">Ενημερώστε τα παρακάτω πεδία:</span><span class="sxs-lookup"><span data-stu-id="46fc7-175">Update the following fields:</span></span>

 - <span data-ttu-id="46fc7-176">**Προεπιλεγμένη εταιρεία**: USPM</span><span class="sxs-lookup"><span data-stu-id="46fc7-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="46fc7-177">**Προεπιλεγμένη οργανωτική μονάδα**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="46fc7-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="46fc7-178">**Συχνότητα τιμολογίου**: έβδομη και τελευταία ημέρα</span><span class="sxs-lookup"><span data-stu-id="46fc7-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="46fc7-179">**Πρότυπο ωρών εργασίας**: Αλλάξτε στο πρότυπο που δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="46fc7-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="46fc7-180">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="46fc7-180">Select **Save**.</span></span> 

![Ενημερωμένες παράμετροι έργου](./media/17UpdatedProjectParameters.png)
