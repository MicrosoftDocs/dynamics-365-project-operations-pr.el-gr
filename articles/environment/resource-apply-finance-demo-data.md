---
title: Εφαρμογή δεδομένων επίδειξης σε ένα περιβάλλον που φιλοξενείται σε cloud του Finance
description: Αυτό το θέμα επεξηγεί τον τρόπο εφαρμογής των δεδομένων επίδειξης από το Project Operations σε ένα περιβάλλον Dynamics 365 Finance που φιλοξενείται στο Cloud.
author: sigitac
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7d8a198b3bfd71ae08bc338d17896519b5ffd6b8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000150"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="ea4b4-103">Εφαρμογή δεδομένων επίδειξης σε ένα περιβάλλον που φιλοξενείται σε cloud του Finance</span><span class="sxs-lookup"><span data-stu-id="ea4b4-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="ea4b4-104">_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_</span><span class="sxs-lookup"><span data-stu-id="ea4b4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ea4b4-105">Αυτό το θέμα ισχύει μόνο για το Microsoft Dynamics 365 Finance έκδοση 10.0.13 και μπορεί να εκτελεστεί μόνο σε περιβάλλον που φιλοξενείται από Cloud.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="ea4b4-106">Ολοκληρώστε τα βήματα σε αυτό το θέμα **ΠΡΙΝ** εφαρμόσετε τις ενημερώσεις ποιότητας στο περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="ea4b4-107">Στο έργο σας LCS, ανοίξτε τη σελίδα **Λεπτομέρειες περιβάλλοντος**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="ea4b4-108">Σημειώστε ότι περιλαμβάνονται οι λεπτομέρειες που απαιτούνται για τη σύνδεση στο περιβάλλον με τη χρήση του πρωτοκόλλου Remote Desktop Protocol (RDP).</span><span class="sxs-lookup"><span data-stu-id="ea4b4-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![Λεπτομέρειες περιβάλλοντος ](./media/1EnvironmentDetails.png)

<span data-ttu-id="ea4b4-110">Το πρώτο σύνολο πιστοποιήσεων που έχουν επισημανθεί είναι τα διαπιστευτήρια τοπικού λογαριασμού και περιέχει μια υπερ-σύνδεση στη σύνδεση απομακρυσμένης επιφάνειας εργασίας.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="ea4b4-111">Τα διαπιστευτήρια περιλαμβάνουν το όνομα χρήστη και τον κωδικό πρόσβασης της διαχείρισης περιβάλλοντος.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="ea4b4-112">Το δεύτερο σύνολο πιστοποιήσεων χρησιμοποιείται για τη σύνδεση στο διακομιστή SQL σε αυτό το περιβάλλον.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="ea4b4-113">Συνδεθείτε στο περιβάλλον με την υπερ-σύνδεση σε **Τοπικούς λογαριασμούς** και χρησιμοποιήστε τα **Διαπιστευτήρια τοπικού λογαριασμού** για τον έλεγχο της ταυτότητάς σας.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="ea4b4-114">Μεταβείτε στα στοιχεία **Υπηρεσίες πληροφοριών Internet** > **Χώροι συγκέντρωσης εφαρμογών** > **AOSService** και τερματίστε την υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="ea4b4-115">Σταματάτε την υπηρεσία σε αυτό το σημείο, ώστε να μπορείτε να συνεχίσετε να αντικαθιστάτε τη βάση δεδομένων SQL.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![Διακοπή AOS](./media/2StopAOS.png)

4. <span data-ttu-id="ea4b4-117">Μεταβείτε στην επιλογή **Υπηρεσίες** και, στη συνέχεια, σταματήστε τα εξής δύο στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="ea4b4-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="ea4b4-118">Microsoft Dynamics 365 Unified Operations: Ομαδική διαχείριση υπηρεσιών</span><span class="sxs-lookup"><span data-stu-id="ea4b4-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="ea4b4-119">Microsoft Dynamics 365 Unified Operations: Πλαίσιο εισαγωγής-εξαγωγής δεδομένων</span><span class="sxs-lookup"><span data-stu-id="ea4b4-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![Διακοπή υπηρεσιών](./media/3StopServices.png)

5. <span data-ttu-id="ea4b4-121">Ανοίξτε το Microsoft SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="ea4b4-122">Συνδεθείτε με διαπιστευτήρια SQL Server και χρησιμοποιήστε τον χρήστη axdbadmin και τον κωδικό πρόσβασης από τη σελίδα LCS **Λεπτομέρειες περιβαλλόντων**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="ea4b4-124">Στο Object Explorer, **Βάσεις δεδομένων** και βρείτε το **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="ea4b4-125">Θα αντικαταστήσετε τη βάση δεδομένων με μια νέα βάση δεδομένων που βρίσκεται στο [Κέντρο λήψης](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="ea4b4-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="ea4b4-126">Αντιγράψτε το αρχείο zip στο VM και εξαγάγετε τα περιεχόμενα zip.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="ea4b4-127">Στο SQL Server Management Studio, κάντε δεξιό κλικ στο στοιχείο **AxDB** και, στη συνέχεια, επιλέξτε **Εργασίες** > **Επαναφορά** > **Βάση δεδομένων**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![Επαναφέρετε τη βάση δεδομένων](./media/5RestoreDatabase.png)

9. <span data-ttu-id="ea4b4-129">Επιλέξτε **Συσκευή προέλευσης** και μεταβείτε στο αρχείο που έχει εξαχθεί από το zip που αντιγράψατε.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![Συσκευές προέλευσης](./media/6SourceDevice.png)

10. <span data-ttu-id="ea4b4-131">Επιλέξτε **Επιλογές** και, στη συνέχεια, επιλέξτε **Αντικατάσταση της υπάρχουσας βάσης δεδομένων** και **Κλείσιμο υπαρχουσών συνδέσεων στη βάση δεδομένων προορισμού**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="ea4b4-132">Επιλέξτε **OK**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-132">Select **OK**.</span></span>

![Επαναφορά ρυθμίσεων](./media/7RestoreSetting.png)

<span data-ttu-id="ea4b4-134">Θα λάβετε επιβεβαίωση ότι η επαναφορά του AXDB ήταν επιτυχής.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="ea4b4-135">Αφού λάβετε αυτήν την επιβεβαίωση, μπορείτε να κλείσετε το SQL Services Management Studio.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="ea4b4-136">Μεταβείτε στα στοιχεία **Υπηρεσίες πληροφοριών Internet** > **Χώροι συγκέντρωσης εφαρμογών** > **AOSService** και εκκινήστε το AOSService.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="ea4b4-137">Μεταβείτε στην επιλογή **Υπηρεσίες** και ξεκινήστε τις δύο υπηρεσίες που διακόψατε νωρίτερα.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="ea4b4-138">Εντοπίστε το εργαλείο AdminUserProvisioning σε αυτό το VM.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="ea4b4-139">Κοιτάξτε κάτω από το K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="ea4b4-140">Εκτελέστε το αρχείο .ext χρησιμοποιώντας τη διεύθυνση χρήστη στο πεδίο **Διεύθυνση ηλεκτρονικού ταχυδρομείου**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="ea4b4-141">Επιλέξτε **Υποβολή**.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-141">Select **Submit**.</span></span>

![Παροχή διαχειριστή](./media/8AdminUserProvisioning.png)

<span data-ttu-id="ea4b4-143">Αυτό διαρκεί λίγα λεπτά για να ολοκληρωθεί.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="ea4b4-144">Θα πρέπει να λάβετε ένα μήνυμα επιβεβαίωσης ότι ο χρήστης-διαχειριστής ενημερωθεί με επιτυχία.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="ea4b4-145">Τέλος, εκτελέστε την υπαγόρευση εντολής ως Διαχειριστής και εκτελέστε iisreset</span><span class="sxs-lookup"><span data-stu-id="ea4b4-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![Επαναφορά IIS](./media/9IISReset.png)

18. <span data-ttu-id="ea4b4-147">Κλείστε την περίοδο λειτουργίας της απομακρυσμένης επιφάνειας εργασίας και χρησιμοποιήστε τη σελίδα **Λεπτομέρειες περιβάλλοντος** του LCS για να συνδεθείτε στο περιβάλλον για να επιβεβαιώσετε ότι λειτουργεί όπως αναμενόταν.</span><span class="sxs-lookup"><span data-stu-id="ea4b4-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]