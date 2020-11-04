---
title: Εφαρμογή ρύθμισης επίδειξης και δεδομένων ρύθμισης παραμέτρων
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο εφαρμογής της ρύθμισης επίδειξης και των δεδομένων ρύθμισης παραμέτρων για το Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 33b85115963f3561718b8951e5b518fd34de7723
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076781"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="8e272-103">Εφαρμόστε τη ρύθμιση επίδειξης και τα δεδομένα ρύθμισης παραμέτρων για την ελαφριά ανάπτυξη του Project Operations - συμφωνία για προτιμολόγηση</span><span class="sxs-lookup"><span data-stu-id="8e272-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="8e272-104">_\*\*Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="8e272-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="8e272-105">Πραγματοποιήστε λήψη του [πακέτου κύριων δεδομένων](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="8e272-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="8e272-106">Μεταβείτε στον φάκελο *ProjOpsDemoDataSetupAndMaster-ενσωματωμένο CMT* και εκτελέστε το εκτελέσιμο αρχείο *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="8e272-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="8e272-107">Στη σελίδα 1 του Οδηγού ρύθμισης παραμέτρων του Common Data Service, επιλέξτε **Εισαγωγή δεδομένων** και, στη συνέχεια, επιλέξτε **Συνέχεια**.</span><span class="sxs-lookup"><span data-stu-id="8e272-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Μετεγκατάσταση ρύθμισης παραμέτρων](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="8e272-109">Στη σελίδα 2 του οδηγού CMT, επιλέξτε **Microsoft 365** ως **Τύπο ανάπτυξης**.</span><span class="sxs-lookup"><span data-stu-id="8e272-109">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="8e272-110">Επιλέξτε τα πλαίσια ελέγχου **Εμφάνιση μιας λίστας με τους διαθέσιμους οργανισμούς** και **Εμφάνιση πρόσθετων κριτηρίων**.</span><span class="sxs-lookup"><span data-stu-id="8e272-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="8e272-111">Επιλέξτε την περιοχή του μισθωτή σας, καταχωρίστε τα διαπιστευτήριά σας και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="8e272-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Σύνδεση για ρύθμιση παραμέτρων](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="8e272-113">Στη σελίδα 3, από τη λίστα των οργανισμών του μισθωτή, επιλέξτε τον οργανισμό στον οποίο θέλετε να εισαγάγετε τα δεδομένα επίδειξης και, στη συνέχεια, επιλέξτε **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="8e272-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="8e272-114">Στη σελίδα 4, επιλέξτε το συμπιεσμένο αρχείο *MasterAndSetupData* από τον μη συμπιεσμένο φάκελο *ProjOpsDemoDataSetupAndMaster - Ενσωματωμένο CMT*.</span><span class="sxs-lookup"><span data-stu-id="8e272-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Αρχείο zip](./media/3ZipFile.png)

![Επιλογή αρχείου](./media/4SelectAFile.png)

9. <span data-ttu-id="8e272-117">Αφού επιλεγεί το συμπιεσμένο αρχείο, επιλέξτε **Εισαγωγή δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="8e272-117">After the zip file is selected, select **Import Data**.</span></span>

![Εισαγωγή δεδομένων](./media/5ImportData.png)

10. <span data-ttu-id="8e272-119">Η εισαγωγή θα διαρκέσει περίπου δύο-δέκα λεπτά, ανάλογα με την ταχύτητα του δικτύου σας.</span><span class="sxs-lookup"><span data-stu-id="8e272-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="8e272-120">Αφού ολοκληρωθεί, τερματίστε τον οδηγό CMT.</span><span class="sxs-lookup"><span data-stu-id="8e272-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="8e272-121">Ελέγξτε τον οργανισμό σας για δεδομένα στις ακόλουθες 20 οντότητες:</span><span class="sxs-lookup"><span data-stu-id="8e272-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="8e272-122">Νομισματική μονάδα</span><span class="sxs-lookup"><span data-stu-id="8e272-122">Currency</span></span>
- <span data-ttu-id="8e272-123">Οργανική μονάδα</span><span class="sxs-lookup"><span data-stu-id="8e272-123">Organizational Unit</span></span>
- <span data-ttu-id="8e272-124">Επικοινωνία</span><span class="sxs-lookup"><span data-stu-id="8e272-124">Contact</span></span>
- <span data-ttu-id="8e272-125">Ομάδα φόρων</span><span class="sxs-lookup"><span data-stu-id="8e272-125">Tax Group</span></span>
- <span data-ttu-id="8e272-126">Ομάδα πελατών</span><span class="sxs-lookup"><span data-stu-id="8e272-126">Customer Group</span></span>
- <span data-ttu-id="8e272-127">Μονάδα</span><span class="sxs-lookup"><span data-stu-id="8e272-127">Unit</span></span>
- <span data-ttu-id="8e272-128">Ομάδα μονάδων</span><span class="sxs-lookup"><span data-stu-id="8e272-128">Unit Group</span></span>
- <span data-ttu-id="8e272-129">Τιμοκατάλογος</span><span class="sxs-lookup"><span data-stu-id="8e272-129">Price List</span></span>
- <span data-ttu-id="8e272-130">Τιμοκατάλογος παραμέτρων έργου</span><span class="sxs-lookup"><span data-stu-id="8e272-130">Project Parameter Price List</span></span>
- <span data-ttu-id="8e272-131">Συχνότητα τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="8e272-131">Invoice Frequency</span></span>
- <span data-ttu-id="8e272-132">Λεπτομέρεια συχνότητας τιμολογίων</span><span class="sxs-lookup"><span data-stu-id="8e272-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="8e272-133">Κατηγορία πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="8e272-133">Bookable Resource Category</span></span>
- <span data-ttu-id="8e272-134">Κατηγορία συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="8e272-134">Transaction Category</span></span>
- <span data-ttu-id="8e272-135">Κατηγορία εξόδου</span><span class="sxs-lookup"><span data-stu-id="8e272-135">Expense Category</span></span>
- <span data-ttu-id="8e272-136">Τιμή ρόλου</span><span class="sxs-lookup"><span data-stu-id="8e272-136">Role Price</span></span>
- <span data-ttu-id="8e272-137">Τιμή κατηγορίας συναλλαγής</span><span class="sxs-lookup"><span data-stu-id="8e272-137">Transaction Category Price</span></span>
- <span data-ttu-id="8e272-138">Χαρακτηριστικό</span><span class="sxs-lookup"><span data-stu-id="8e272-138">Characteristic</span></span>
- <span data-ttu-id="8e272-139">Πόρος με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="8e272-139">Bookable Resource</span></span>
- <span data-ttu-id="8e272-140">Συσχέτιση κατηγορίας πόρων με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="8e272-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="8e272-141">Χαρακτηριστικό του πόρου με δυνατότητα κράτησης</span><span class="sxs-lookup"><span data-stu-id="8e272-141">Bookable Resource Characteristic</span></span>

![Ολοκλήρωση εισαγωγής](./media/6CompleteImport.png)