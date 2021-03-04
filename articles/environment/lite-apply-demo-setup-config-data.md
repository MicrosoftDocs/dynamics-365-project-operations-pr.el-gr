---
title: Εφαρμογή ρύθμισης επίδειξης και δεδομένων ρύθμισης παραμέτρων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εφαρμογής της ρύθμισης επίδειξης και των δεδομένων ρύθμισης παραμέτρων για το Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089119"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="3403c-103">Εφαρμογή δεδομένων ρύθμισης παραμέτρων και ρύθμισης επίδειξης για το Project Operations - lite</span><span class="sxs-lookup"><span data-stu-id="3403c-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="3403c-104">_\*\*Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="3403c-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="3403c-105">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="3403c-105">Prerequisites</span></span>

<span data-ttu-id="3403c-106">Πριν ξεκινήσετε τη ρύθμιση παραμέτρων, πρέπει να διαθέτετε ένα περιβάλλον Common Data Service (CDS) το οποίο παρέχεται για το Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3403c-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="3403c-107">Οδηγίες</span><span class="sxs-lookup"><span data-stu-id="3403c-107">Instructions</span></span>

1. <span data-ttu-id="3403c-108">Πραγματοποιήστε λήψη του [πακέτου κύριων δεδομένων](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="3403c-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="3403c-109">Μεταβείτε στον φάκελο *ProjOpsDemoDataSetupAndMaster-ενσωματωμένο CMT* και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="3403c-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="3403c-110">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="3403c-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="3403c-112">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="3403c-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="3403c-113">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="3403c-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="3403c-114">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="3403c-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="3403c-116">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="3403c-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="3403c-117">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *MasterAndSetupData* από τον μη συμπιεσμένο φάκελο *ProjOpsDemoDataSetupAndMaster - Ενσωματωμένο CMT*.</span><span class="sxs-lookup"><span data-stu-id="3403c-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![Αρχείο zip](./media/3ZipFile.png)

   ![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="3403c-120">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="3403c-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="3403c-122">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="3403c-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="3403c-123">Αφού ολοκληρωθεί, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="3403c-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="3403c-124">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 20 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="3403c-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="3403c-125">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="3403c-125">Currency</span></span>
    -   <span data-ttu-id="3403c-126">Λογαριασμ.</span><span class="sxs-lookup"><span data-stu-id="3403c-126">Account</span></span>
    -   <span data-ttu-id="3403c-127">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="3403c-127">Organizational Unit</span></span>
    -   <span data-ttu-id="3403c-128">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="3403c-128">Contact</span></span>
    -   <span data-ttu-id="3403c-129">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="3403c-129">Unit</span></span>
    -   <span data-ttu-id="3403c-130">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="3403c-130">Unit Group</span></span>
    -   <span data-ttu-id="3403c-131">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="3403c-131">Price List</span></span>
    -   <span data-ttu-id="3403c-132">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="3403c-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="3403c-133">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="3403c-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="3403c-134">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="3403c-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="3403c-135">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="3403c-135">Transaction Category</span></span>
    -   <span data-ttu-id="3403c-136">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="3403c-136">Expense Category</span></span>
    -   <span data-ttu-id="3403c-137">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="3403c-137">Role Price</span></span>
    -   <span data-ttu-id="3403c-138">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="3403c-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="3403c-139">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="3403c-139">Characteristic</span></span>
    -   <span data-ttu-id="3403c-140">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="3403c-140">Bookable Resource</span></span>
    -   <span data-ttu-id="3403c-141">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="3403c-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="3403c-142">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="3403c-142">Bookable Resource Characteristic</span></span>

    ![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)
