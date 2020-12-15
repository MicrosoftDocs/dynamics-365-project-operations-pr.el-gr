---
title: Εφαρμογή ρύθμισης επίδειξης και δεδομένων ρύθμισης παραμέτρων - lite
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εφαρμογής της ρύθμισης επίδειξης και των δεδομένων ρύθμισης παραμέτρων για το Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 421c9d28088c92617687641d93b3ad5d6bfea73c
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642093"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="5798d-103">Εφαρμογή δεδομένων ρύθμισης παραμέτρων και ρύθμισης επίδειξης για το Project Operations - lite</span><span class="sxs-lookup"><span data-stu-id="5798d-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="5798d-104">_\*\*Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="5798d-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="5798d-105">Προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="5798d-105">Prerequisites</span></span>

<span data-ttu-id="5798d-106">Πριν ξεκινήσετε τη ρύθμιση παραμέτρων, πρέπει να διαθέτετε ένα περιβάλλον Common Data Service (CDS) το οποίο παρέχεται για το Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="5798d-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="5798d-107">Οδηγίες</span><span class="sxs-lookup"><span data-stu-id="5798d-107">Instructions</span></span>

1. <span data-ttu-id="5798d-108">Πραγματοποιήστε λήψη του [πακέτου κύριων δεδομένων](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="5798d-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="5798d-109">Μεταβείτε στον φάκελο *ProjOpsDemoDataSetupAndMaster-ενσωματωμένο CMT* και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="5798d-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="5798d-110">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="5798d-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="5798d-112">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="5798d-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="5798d-113">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="5798d-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="5798d-114">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="5798d-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="5798d-116">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="5798d-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="5798d-117">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *MasterAndSetupData* από τον μη συμπιεσμένο φάκελο *ProjOpsDemoDataSetupAndMaster - Ενσωματωμένο CMT*.</span><span class="sxs-lookup"><span data-stu-id="5798d-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Αρχείο zip](./media/3ZipFile.png)

![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="5798d-120">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="5798d-120">After the zip file is selected, select **Import Data**.</span></span>

![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="5798d-122">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="5798d-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="5798d-123">Αφού ολοκληρωθεί, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="5798d-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="5798d-124">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 20 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="5798d-124">Check your organization for data in the following 20 entities:</span></span>

-   <span data-ttu-id="5798d-125">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="5798d-125">Currency</span></span>
-   <span data-ttu-id="5798d-126">Λογαριασμ.</span><span class="sxs-lookup"><span data-stu-id="5798d-126">Account</span></span>
-   <span data-ttu-id="5798d-127">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="5798d-127">Organizational Unit</span></span>
-   <span data-ttu-id="5798d-128">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="5798d-128">Contact</span></span>
-   <span data-ttu-id="5798d-129">Ομάδα φόρων</span><span class="sxs-lookup"><span data-stu-id="5798d-129">Tax Group</span></span>
-   <span data-ttu-id="5798d-130">Ομάδα πελατών</span><span class="sxs-lookup"><span data-stu-id="5798d-130">Customer Group</span></span>
-   <span data-ttu-id="5798d-131">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="5798d-131">Unit</span></span>
-   <span data-ttu-id="5798d-132">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="5798d-132">Unit Group</span></span>
-   <span data-ttu-id="5798d-133">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="5798d-133">Price List</span></span>
-   <span data-ttu-id="5798d-134">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="5798d-134">Project Parameter Price List</span></span> 
-   <span data-ttu-id="5798d-135">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="5798d-135">Invoice Frequency</span></span>
-   <span data-ttu-id="5798d-136">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="5798d-136">Bookable Resource Category</span></span>
-   <span data-ttu-id="5798d-137">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="5798d-137">Transaction Category</span></span>
-   <span data-ttu-id="5798d-138">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="5798d-138">Expense Category</span></span>
-   <span data-ttu-id="5798d-139">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="5798d-139">Role Price</span></span>
-   <span data-ttu-id="5798d-140">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="5798d-140">Transaction Category Price</span></span>
-   <span data-ttu-id="5798d-141">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="5798d-141">Characteristic</span></span>
-   <span data-ttu-id="5798d-142">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="5798d-142">Bookable Resource</span></span>
-   <span data-ttu-id="5798d-143">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="5798d-143">Bookable resource category Assn</span></span>
-   <span data-ttu-id="5798d-144">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="5798d-144">Bookable Resource Characteristic</span></span>

![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)
