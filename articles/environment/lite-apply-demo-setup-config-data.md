---
title: Εφαρμογή ρύθμισης επίδειξης και δεδομένων ρύθμισης παραμέτρων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εφαρμογής της ρύθμισης επίδειξης και των δεδομένων ρύθμισης παραμέτρων για το Project Operations.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7729b4a9ef5f498b78af298f7233d7dd45434bb3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997151"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="b356e-103">Εφαρμογή δεδομένων ρύθμισης παραμέτρων και ρύθμισης επίδειξης για το Project Operations - lite</span><span class="sxs-lookup"><span data-stu-id="b356e-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="b356e-104">_\*\*Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="b356e-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="b356e-105">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="b356e-105">Prerequisites</span></span>

<span data-ttu-id="b356e-106">Πριν ξεκινήσετε τη ρύθμιση παραμέτρων, πρέπει να διαθέτετε ένα περιβάλλον Common Data Service (CDS) το οποίο παρέχεται για το Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b356e-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="b356e-107">Οδηγίες</span><span class="sxs-lookup"><span data-stu-id="b356e-107">Instructions</span></span>

1. <span data-ttu-id="b356e-108">Πραγματοποιήστε λήψη του [πακέτου κύριων δεδομένων](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip).</span><span class="sxs-lookup"><span data-stu-id="b356e-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip).</span></span> 
2. <span data-ttu-id="b356e-109">Μεταβείτε στον φάκελο *ProjOpsSampleSetupData - CE μόνο CMT* και εκτελέστε το εκτελέσιμο αρχείο, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="b356e-109">Navigate to the folder *ProjOpsSampleSetupData - CE only CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="b356e-110">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="b356e-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="b356e-112">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="b356e-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="b356e-113">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="b356e-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="b356e-114">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="b356e-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="b356e-116">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="b356e-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="b356e-117">Στη σελίδα 4, επιλέξτε το αρχείο zip, *SampleSetupAndConfigData* από τον μη συμπιεσμένο φάκελο, *ProjOpsSampleSetupData - CE μόνο CMT*.</span><span class="sxs-lookup"><span data-stu-id="b356e-117">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder, *ProjOpsSampleSetupData - CE only CMT*.</span></span>

   ![Αρχείο zip](./media/3ZipFile.png)

   ![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="b356e-120">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="b356e-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="b356e-122">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="b356e-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="b356e-123">Αφού ολοκληρωθεί, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="b356e-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="b356e-124">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 18 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="b356e-124">Check your organization for data in the following 18 entities:</span></span>

    -   <span data-ttu-id="b356e-125">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="b356e-125">Currency</span></span>
    -   <span data-ttu-id="b356e-126">Λογαριασμ.</span><span class="sxs-lookup"><span data-stu-id="b356e-126">Account</span></span>
    -   <span data-ttu-id="b356e-127">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="b356e-127">Organizational Unit</span></span>
    -   <span data-ttu-id="b356e-128">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="b356e-128">Contact</span></span>
    -   <span data-ttu-id="b356e-129">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="b356e-129">Unit</span></span>
    -   <span data-ttu-id="b356e-130">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="b356e-130">Unit Group</span></span>
    -   <span data-ttu-id="b356e-131">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="b356e-131">Price List</span></span>
    -   <span data-ttu-id="b356e-132">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="b356e-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="b356e-133">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="b356e-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="b356e-134">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="b356e-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="b356e-135">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="b356e-135">Transaction Category</span></span>
    -   <span data-ttu-id="b356e-136">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="b356e-136">Expense Category</span></span>
    -   <span data-ttu-id="b356e-137">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="b356e-137">Role Price</span></span>
    -   <span data-ttu-id="b356e-138">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="b356e-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="b356e-139">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="b356e-139">Characteristic</span></span>
    -   <span data-ttu-id="b356e-140">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="b356e-140">Bookable Resource</span></span>
    -   <span data-ttu-id="b356e-141">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="b356e-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="b356e-142">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="b356e-142">Bookable Resource Characteristic</span></span>

    ![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
