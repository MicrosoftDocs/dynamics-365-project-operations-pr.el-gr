---
title: Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο ρύθμισης και εφαρμογής των δεδομένων διαμόρφωσης στο Project Operations.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001291"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="e8271-103">Ρύθμιση και εφαρμογή δεδομένων ρύθμισης παραμέτρων στο Common Data Service</span><span class="sxs-lookup"><span data-stu-id="e8271-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="e8271-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="e8271-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="e8271-105">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="e8271-105">Prerequisites</span></span>

<span data-ttu-id="e8271-106">Πριν αρχίσετε να ρυθμίζετε τις παραμέτρους των δεδομένων στο Common Data Service (CDS), πρέπει να πληρούνται οι παρακάτω προϋποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="e8271-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="e8271-107">Παροχή ενός περιβάλλοντος CDS και ενός Dynamics 365 Finance περιβάλλοντος για το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e8271-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="e8271-108">Οι πληροφορίες νομικής οντότητας από το Dynamics 365 Finance είναι κοινόχρηστες στο περιβάλλον CDS.</span><span class="sxs-lookup"><span data-stu-id="e8271-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="e8271-109">Αυτό σημαίνει ότι η οντότητα **Εταιρεία** στο CDS έχει τις ακόλουθες εταιρικές καρτέλες:</span><span class="sxs-lookup"><span data-stu-id="e8271-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="e8271-110">THPM</span><span class="sxs-lookup"><span data-stu-id="e8271-110">THPM</span></span>
  - <span data-ttu-id="e8271-111">USPM</span><span class="sxs-lookup"><span data-stu-id="e8271-111">USPM</span></span>
  - <span data-ttu-id="e8271-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="e8271-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="e8271-113">Εγκατάσταση δεδομένων ρύθμισης παραμέτρων και διαμόρφωσης</span><span class="sxs-lookup"><span data-stu-id="e8271-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="e8271-114">Πραγματοποιήστε λήψη, κατάργηση αποκλεισμού και αποσυμπιέστε το [πακέτο δεδομένων εγκατάστασης και ρύθμισης παραμέτρων](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span><span class="sxs-lookup"><span data-stu-id="e8271-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="e8271-115">Μεταβείτε στον αποσυμπιεσμένο φάκελο και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="e8271-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="e8271-116">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="e8271-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="e8271-118">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="e8271-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="e8271-119">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="e8271-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="e8271-120">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="e8271-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="e8271-122">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="e8271-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="e8271-123">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *SampleSetupAndConfigData* από τον μη συμπιεσμένο φάκελο.</span><span class="sxs-lookup"><span data-stu-id="e8271-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Επιλογή συμπιεσμένου αρχείου](./media/3ZipFile.png)

![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="e8271-126">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="e8271-126">After the zip file is selected, select **Import Data**.</span></span>

![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="e8271-128">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="e8271-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="e8271-129">Αφού ολοκληρωθεί η εισαγωγή, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="e8271-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="e8271-130">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 26 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="e8271-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="e8271-131">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="e8271-131">Currency</span></span>
  - <span data-ttu-id="e8271-132">Γράφημα λογαριασμών</span><span class="sxs-lookup"><span data-stu-id="e8271-132">Chart of Accounts</span></span>
  - <span data-ttu-id="e8271-133">Οικονομικό ημερολόγιο</span><span class="sxs-lookup"><span data-stu-id="e8271-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="e8271-134">Τύποι συναλλαγματικής ισοτιμίας νομίσματος</span><span class="sxs-lookup"><span data-stu-id="e8271-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="e8271-135">Ημερομηνία πληρωμής</span><span class="sxs-lookup"><span data-stu-id="e8271-135">Payment Day</span></span>
  - <span data-ttu-id="e8271-136">Χρονοδιάγραμμα πληρωμής</span><span class="sxs-lookup"><span data-stu-id="e8271-136">Payment Schedule</span></span>
  - <span data-ttu-id="e8271-137">Προθεσμία πληρωμής</span><span class="sxs-lookup"><span data-stu-id="e8271-137">Payment Term</span></span>
  - <span data-ttu-id="e8271-138">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="e8271-138">Organizational Unit</span></span>
  - <span data-ttu-id="e8271-139">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="e8271-139">Contact</span></span>
  - <span data-ttu-id="e8271-140">Ομάδα φόρων</span><span class="sxs-lookup"><span data-stu-id="e8271-140">Tax Group</span></span>
  - <span data-ttu-id="e8271-141">Ομάδα πελατών</span><span class="sxs-lookup"><span data-stu-id="e8271-141">Customer Group</span></span>
  - <span data-ttu-id="e8271-142">Ομάδα προμηθευτών</span><span class="sxs-lookup"><span data-stu-id="e8271-142">Vendor Group</span></span>
  - <span data-ttu-id="e8271-143">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="e8271-143">Unit</span></span>
  - <span data-ttu-id="e8271-144">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="e8271-144">Unit Group</span></span>
  - <span data-ttu-id="e8271-145">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="e8271-145">Price List</span></span>
  - <span data-ttu-id="e8271-146">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="e8271-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="e8271-147">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="e8271-147">Invoice Frequency</span></span>
  - <span data-ttu-id="e8271-148">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="e8271-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="e8271-149">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="e8271-149">Transaction Category</span></span>
  - <span data-ttu-id="e8271-150">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="e8271-150">Expense Category</span></span>
  - <span data-ttu-id="e8271-151">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="e8271-151">Role Price</span></span>
  - <span data-ttu-id="e8271-152">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="e8271-152">Transaction Category Price</span></span>
  - <span data-ttu-id="e8271-153">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="e8271-153">Characteristic</span></span>
  - <span data-ttu-id="e8271-154">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="e8271-154">Bookable Resource</span></span>
  - <span data-ttu-id="e8271-155">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="e8271-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="e8271-156">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="e8271-156">Bookable Resource Characteristic</span></span>

![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="e8271-158">Ενημέρωση διαμορφώσεων Project Operations</span><span class="sxs-lookup"><span data-stu-id="e8271-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="e8271-159">Περιήγηση στο περιβάλλον CE.</span><span class="sxs-lookup"><span data-stu-id="e8271-159">Navigate to the CE environment.</span></span> <span data-ttu-id="e8271-160">Μπορείτε να το βρείτε ανοίγοντας το [Κέντρο διαχείρισης του Power Platform](https://admin.powerplatform.microsoft.com/environments), επιλέγοντας το περιβάλλον και, στη συνέχεια, επιλέγοντας **Άνοιγμα περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="e8271-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Άνοιγμα περιβάλλοντος](./media/7OpenEnvironment.png)

2. <span data-ttu-id="e8271-162">Μεταβείτε στα στοιχεία **Έργα** > **Πόροι** και, στη συνέχεια, επιλέξτε **Δημιουργία** για να δημιουργήσετε έναν πόρο με κράτηση για τον χρήστη σας.</span><span class="sxs-lookup"><span data-stu-id="e8271-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Πόροι με δυνατότητα κράτησης](./media/8BookableResources.png)

3. <span data-ttu-id="e8271-164">Στην καρτέλα **Γενικά**, επιλέξτε τον χρήστη διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="e8271-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="e8271-165">Επαληθεύστε ότι η ζώνη ώρας ταιριάζει με αυτήν στην οποία βρίσκεστε.</span><span class="sxs-lookup"><span data-stu-id="e8271-165">Verify that the time zone matches the one you are in.</span></span> 

![Νέος πόρος με δυνατότητα κράτησης](./media/9NewBookableResource.png)

4. <span data-ttu-id="e8271-167">Στην καρτέλα **Προγραμματισμός**, στο πεδίο **Εταιρεία**, επιλέξτε την εταιρεία **USPM** και μετά επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="e8271-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Καρτέλα προγραμματισμού](./media/10SchedulingTab.png)

5. <span data-ttu-id="e8271-169">Επιλέξτε την καρτέλα **Ώρες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="e8271-169">Select the **Work hours** tab.</span></span>  

![Ώρες εργασίας](./media/11WorkHours.png)

6. <span data-ttu-id="e8271-171">Κάντε διπλό κλικ σε οποιαδήποτε τιμή στο ημερολόγιο και επιλέξτε **Επεξεργασία** > **Όλα τα συμβάντα στη σειρά**.</span><span class="sxs-lookup"><span data-stu-id="e8271-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Ημερολόγιο εργασίας](./media/12WorkCalendar.png)

7. <span data-ttu-id="e8271-173">Αλλάξτε τις ώρες εργασίας σε μια εργάσιμη ημέρα οκτώ (8) ωρών, επισημάνετε τα σαββατοκύριακα ως μη εργάσιμες ημέρες και βεβαιωθείτε ότι η ζώνη ώρας ταιριάζει με τη δική σας.</span><span class="sxs-lookup"><span data-stu-id="e8271-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="e8271-174">Επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="e8271-174">Select **Save and close**.</span></span>

![Ενημέρωση ημερολογίου](./media/13UpdateCalendar.png)

9. <span data-ttu-id="e8271-176">Μεταβείτε στις **Ρυθμίσεις** > **Πρότυπα ημερολογίου** και επιλέξτε **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="e8271-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Πρότυπα ημερολογίου](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="e8271-178">Καταγράψτε ένα όνομα, επιλέξτε τον πρότυπο πόρο που δημιουργήσατε και, στη συνέχεια, επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="e8271-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Αποθήκευση προτύπου ημερολογίου](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="e8271-180">Μεταβείτε στο στοιχείο **Παράμετροι** και κάντε διπλό κλικ στην καρτέλα.</span><span class="sxs-lookup"><span data-stu-id="e8271-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Παράμετροι έργου](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="e8271-182">Ενημερώστε τα παρακάτω πεδία:</span><span class="sxs-lookup"><span data-stu-id="e8271-182">Update the following fields:</span></span>

 - <span data-ttu-id="e8271-183">**Προεπιλεγμένη εταιρεία**: USPM</span><span class="sxs-lookup"><span data-stu-id="e8271-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="e8271-184">**Προεπιλεγμένη οργανωτική μονάδα**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="e8271-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="e8271-185">**Συχνότητα τιμολογίου**: έβδομη και τελευταία ημέρα</span><span class="sxs-lookup"><span data-stu-id="e8271-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="e8271-186">**Πρότυπο ωρών εργασίας**: Αλλάξτε στο πρότυπο που δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="e8271-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="e8271-187">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="e8271-187">Select **Save**.</span></span> 

![Ενημερωμένες παράμετροι έργου](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
