---
title: Χρήση του προσθέτου Project Service για προγραμματισμό των εργασιών σας στο Microsoft Project | MicrosoftDocs
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την προσθήκη, τη ρύθμιση παραμέτρων και τη χρήση του πρόσθετου Microsoft Project για το Microsoft Project Service.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d988419ae5a9d57532902d2553cd7de147e27c1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077046"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="b7265-103">Χρησιμοποιήστε το πρόσθετο Project Service Automation για να προγραμματίσετε την εργασία σας στο Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="b7265-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b7265-104">To [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] σάς διευκολύνει να κάνετε τον προγραμματισμό έργου σας, καθώς και εκτιμήσεις.</span><span class="sxs-lookup"><span data-stu-id="b7265-104">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="b7265-105">Μπορείτε να ορίσετε την εργασία έτσι ώστε οι δαπάνες, η προσπάθεια και η τιμή πωλήσεων να είναι σαφή κατά την υποβολή της τελικής πρότασης.</span><span class="sxs-lookup"><span data-stu-id="b7265-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="b7265-106">Τώρα μπορείτε να εγκαταστήσετε το [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] και να κάνετε τις εργασίες σχεδιασμού σας στο οικείο περιβάλλον του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="b7265-107">Χρησιμοποιήστε τις ισχυρές δυνατότητες προγραμματισμού και διαχείρισης του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και, στη συνέχεια, ενημερώστε το σχέδιο έργου σας στο Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b7265-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="b7265-108">Για να χρησιμοποιήσετε τη διαχείριση εγγράφων του SharePoint για την αποθήκευση των αρχείων [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] για τα έργα [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], ο διαχειριστής του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] θα χρειαστεί να ενεργοποιήσει τη διαχείριση εγγράφων.</span><span class="sxs-lookup"><span data-stu-id="b7265-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="b7265-109">Το [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] είναι συμβατό μόνο με το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span><span class="sxs-lookup"><span data-stu-id="b7265-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="b7265-110">Λήψη και εγκατάσταση του προσθέτου</span><span class="sxs-lookup"><span data-stu-id="b7265-110">Download and install the add-in</span></span>  
 <span data-ttu-id="b7265-111">Να έχετε στη διάθεσή σας τα στοιχεία σύνδεσης στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="b7265-112">Θα χρειαστείτε αυτές τις πληροφορίες, για να συνδεθείτε από το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="b7265-113">Από το κέντρο λήψης, κατεβάστε το πρόσθετο για την υποστηριζόμενη έκδοση του Project Service, είτε [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) είτε [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="b7265-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="b7265-114">Κάντε κλικ στη σύνδεση λήψης.</span><span class="sxs-lookup"><span data-stu-id="b7265-114">Click the download link.</span></span>  

3.  <span data-ttu-id="b7265-115">Όταν ολοκληρωθεί η λήψη, κάντε κλικ στο κουμπί **Ναι** για την εγκατάσταση του προσθέτου.</span><span class="sxs-lookup"><span data-stu-id="b7265-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="b7265-116">Ρύθμιση των παραμέτρων του προσθέτου</span><span class="sxs-lookup"><span data-stu-id="b7265-116">Configure the add-in</span></span>  

1. <span data-ttu-id="b7265-117">Ανοίξτε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και κάντε κλικ στην καρτέλα **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="b7265-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="b7265-118">Κάντε κλικ στο κουμπί **Σύνδεση**.</span><span class="sxs-lookup"><span data-stu-id="b7265-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="b7265-119">Εισαγάγετε τις πληροφορίες εισόδου σας και, στη συνέχεια, κάντε κλικ στο κουμπί **Είσοδος**.</span><span class="sxs-lookup"><span data-stu-id="b7265-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="b7265-120">Τώρα μπορείτε να ξεκινήσετε να χρησιμοποιείτε το πρόσθετο.</span><span class="sxs-lookup"><span data-stu-id="b7265-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="b7265-121">Ανάγνωση από πρότυπο</span><span class="sxs-lookup"><span data-stu-id="b7265-121">Read from a template</span></span>  
 <span data-ttu-id="b7265-122">Κάντε ανάγνωση από ένα πρότυπο που δημιουργήσατε στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] και αντιγράψατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], για να ξεκινήσετε τον σχεδιασμό του έργου.</span><span class="sxs-lookup"><span data-stu-id="b7265-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="b7265-123">[Δημιουργία προτύπου έργου (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="b7265-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="b7265-124">Από την καρτέλα **Project Service** , κάντε κλικ στις επιλογές **Ανάγνωση** > **Πρότυπο έργου Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b7265-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="b7265-125">Επιλέξτε ένα πρότυπο έργου από τη λίστα και, στη συνέχεια, κάντε κλικ στο κουμπί **Άνοιγμα**.</span><span class="sxs-lookup"><span data-stu-id="b7265-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="b7265-126">Από προεπιλογή, οι εργασίες που αντιγράφονται από το πρότυπο στο Project έχουν οριστεί ως μη αυτόματα προγραμματισμένες.</span><span class="sxs-lookup"><span data-stu-id="b7265-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="b7265-127">Αντιστοίχιση [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ρόλων σε πόρους έργου</span><span class="sxs-lookup"><span data-stu-id="b7265-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="b7265-128">Ανοίξτε ένα έργο και κάντε κλικ στην κορδέλα **Εργασία**.</span><span class="sxs-lookup"><span data-stu-id="b7265-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="b7265-129">Κάντε κλικ στο μενού **Γράφημα Gantt** και στη συνέχεια επιλέξτε **Φύλλο πόρων**.</span><span class="sxs-lookup"><span data-stu-id="b7265-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="b7265-130">Στο φύλλο πόρων, κάντε κλικ στο αναπτυσσόμενο μενού **Ρόλος πόρου Project Service** και επιλέξτε έναν ρόλο Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b7265-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="b7265-131">Εκχώρηση πόρων στο έργο σας</span><span class="sxs-lookup"><span data-stu-id="b7265-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="b7265-132">Από την καρτέλα Project Service, επιλέξτε μια γραμμή και κάντε κλικ στο κουμπί **Εύρεση πόρων**.</span><span class="sxs-lookup"><span data-stu-id="b7265-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="b7265-133">Στην οθόνη **Κράτηση πόρου** , επιλέξτε τον πόρο που θέλετε να χρησιμοποιήσετε για το έργο.</span><span class="sxs-lookup"><span data-stu-id="b7265-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="b7265-134">Κάντε κλικ στο κουμπί **Κράτηση** και, στη συνέχεια, κάντε κλικ στο κουμπί **ΟΚ**.</span><span class="sxs-lookup"><span data-stu-id="b7265-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="b7265-135">Δημοσίευση του έργου σας</span><span class="sxs-lookup"><span data-stu-id="b7265-135">Publish your project</span></span>  
<span data-ttu-id="b7265-136">Όταν ο σχεδιασμός του έργου έχει ολοκληρωθεί, το επόμενο βήμα είναι να εισαγάγετε και να δημοσιεύσετε το έργο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="b7265-137">Το έργο θα εισαχθεί στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="b7265-138">Εφαρμόζονται οι διαδικασίες τιμολόγησης και δημιουργίας ομάδας.</span><span class="sxs-lookup"><span data-stu-id="b7265-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="b7265-139">Ανοίξτε το έργο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] για να δείτε ότι η ομάδα, οι εκτιμήσεις έργου και η δομή ανάλυσης εργασίας έχουν δημιουργηθεί.</span><span class="sxs-lookup"><span data-stu-id="b7265-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="b7265-140">Ο παρακάτω πίνακας δείχνει πού μπορείτε να βρείτε τα αποτελέσματα:</span><span class="sxs-lookup"><span data-stu-id="b7265-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  <span data-ttu-id="b7265-141">**Γράφημα Gantt** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-141">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Gantt Chart**</span></span>   | <span data-ttu-id="b7265-142">Εισάγεται στην οθόνη **Δομή ανάλυσης εργασίας** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| <span data-ttu-id="b7265-143">**Φύλλο πόρων** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-143">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Resource Sheet**</span></span> |   <span data-ttu-id="b7265-144">Εισάγεται στην οθόνη **Μέλη ομάδας έργου** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   <span data-ttu-id="b7265-145">**Χρήση** του [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-145">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Use Usage**</span></span>    |    <span data-ttu-id="b7265-146">Εισάγεται στην οθόνη **Εκτιμήσεις έργου** του [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="b7265-147">**Για να εισαγάγετε και να δημοσιεύσετε το έργο σας**</span><span class="sxs-lookup"><span data-stu-id="b7265-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="b7265-148">Από την καρτέλα **Project Service** , κάντε κλικ στις επιλογές **Δημοσίευση** > **Νέο έργο Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b7265-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="b7265-149">Στο παράθυρο διαλόγου **Δημοσίευση σε ένα νέο έργο στο Project Service** , καταχωρίστε το **Όνομα έργου** και επιλέξτε **Πελάτης**.</span><span class="sxs-lookup"><span data-stu-id="b7265-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="b7265-150">Προαιρετικά επιλέξτε **Σύνδεση πλάνου έργου στο Project Service Automation** , για να συνδέσετε το αρχείο σχεδίου του Project με το Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b7265-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="b7265-151">Κάντε κλικ στην επιλογή **Δημοσίευση**.</span><span class="sxs-lookup"><span data-stu-id="b7265-151">Click **Publish**.</span></span>  

   <span data-ttu-id="b7265-152">Η σύνδεση του αρχείου Project με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] καθιστά το αρχείο έργου βασικό και ορίζει τη δομή ανάλυσης εργασίας στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b7265-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="b7265-153">Για να κάνετε αλλαγές στο σχέδιο έργου, πρέπει να το δημιουργήσετε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να το δημοσιεύσετε ως ενημέρωση στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="b7265-154">Επεξεργασία ενός έργου που έχει εισαχθεί</span><span class="sxs-lookup"><span data-stu-id="b7265-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="b7265-155">Για να κάνετε αλλαγές σε ένα σχέδιο έργου που έχει εισαχθεί στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], έχετε δύο επιλογές:</span><span class="sxs-lookup"><span data-stu-id="b7265-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="b7265-156">Ανοίξτε το βασικό αρχείο και επεξεργαστείτε το στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="b7265-157">Αποσυνδέστε το αρχείο και επεξεργαστείτε το στο Project Service.</span><span class="sxs-lookup"><span data-stu-id="b7265-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="b7265-158">Από προεπιλογή, ένα έργο που αποστέλλεται από το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι κλειδωμένο και είναι δυνατή η επεξεργασία μόνο στο Project.</span><span class="sxs-lookup"><span data-stu-id="b7265-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="b7265-159">Για να επεξεργαστείτε το αρχείο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], το αρχείο πρέπει να αποσυνδεθεί.</span><span class="sxs-lookup"><span data-stu-id="b7265-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="b7265-160">Επεξεργασία στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="b7265-161">Από το κύριο μενού, επιλέξτε **Project Service** > **Έργα**.</span><span class="sxs-lookup"><span data-stu-id="b7265-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="b7265-162">Από τη λίστα έργων, ανοίξτε αυτό που δημιουργήσατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="b7265-163">Κάντε κλικ στο κουμπί **Άνοιγμα στο MS Project** από την κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="b7265-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="b7265-164">Θα ανοίξει το συνδεδεμένο βασικό αρχείο στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="b7265-165">Αποσύνδεση ενός αρχείου και επεξεργασία στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b7265-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="b7265-166">Από το κύριο μενού, επιλέξτε **Project Service** > **Έργα**.</span><span class="sxs-lookup"><span data-stu-id="b7265-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="b7265-167">Από τη λίστα έργων, ανοίξτε αυτό που δημιουργήσατε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="b7265-168">Κάντε κλικ στο κουμπί **Αποσύνδεση από το MS Project** από την κορδέλα.</span><span class="sxs-lookup"><span data-stu-id="b7265-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="b7265-169">Αποστολή αρχείου Project στο SharePoint ή σε Ομάδες Office</span><span class="sxs-lookup"><span data-stu-id="b7265-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="b7265-170">Μπορείτε να στείλετε το αρχείο έργου στο SharePoint και να το βρείτε κάτω από τα έγγραφα που σχετίζονται με το έργο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="b7265-171">Ο διαχειριστής σας πρέπει να ρυθμίσει τις παραμέτρους διαχείρισης εγγράφων του SharePoint και να ενεργοποιήσει αυτή τη δυνατότητα για την οντότητα Project.</span><span class="sxs-lookup"><span data-stu-id="b7265-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="b7265-172">Επίσης, μπορείτε να αποστείλετε το αρχείο έργου στο [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)], εάν έχετε ορίσει Ομάδες Office.</span><span class="sxs-lookup"><span data-stu-id="b7265-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="b7265-173">Αποστολή αρχείου για το SharePoint</span><span class="sxs-lookup"><span data-stu-id="b7265-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="b7265-174">Από το κύριο μενού, επιλέξτε **Project Service** > **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="b7265-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="b7265-175">Επιλέξτε **Προς έγγραφα έργου του Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b7265-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="b7265-176">Στο παράθυρο διαλόγου **Ενεργοποίηση ανοίγματος στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** , επιλέξτε **Ναι** ή **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="b7265-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="b7265-177">Αν κάνετε κλικ στο **Ναι** , θα έχετε τη δυνατότητα να επιλέξετε το κουμπί **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** στο Project Service Automation, να εκκινήσετε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να φορτώσετε το αρχείο έργου από τη βιβλιοθήκη εγγράφων του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b7265-177">If you click **Yes** , you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="b7265-178">Αν κάνετε κλικ στο **Όχι** , η σύνδεση για το κουμπί **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** δεν θα λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="b7265-178">If you click **No** , the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="b7265-179">Το αρχείο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι διαθέσιμο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στην περιοχή **Έγγραφα** του εκάστοτε έργου [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="b7265-180">Αποστολή αρχείου για Ομάδες Office</span><span class="sxs-lookup"><span data-stu-id="b7265-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="b7265-181">Από το κύριο μενού, επιλέξτε **Project Service** > **Αποστολή**.</span><span class="sxs-lookup"><span data-stu-id="b7265-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="b7265-182">Επιλέξτε **Προς έγγραφα έργου του Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b7265-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="b7265-183">Στο παράθυρο διαλόγου **Ενεργοποίηση ανοίγματος στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** , επιλέξτε **Ναι** ή **Όχι**.</span><span class="sxs-lookup"><span data-stu-id="b7265-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="b7265-184">Αν κάνετε κλικ στο **Ναι** , θα έχετε τη δυνατότητα να επιλέξετε το κουμπί **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** στο Project Service Automation, να εκκινήσετε το [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να φορτώσετε το αρχείο έργου από τη βιβλιοθήκη εγγράφων του SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b7265-184">If you click **Yes** , you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="b7265-185">Αν κάνετε κλικ στο **Όχι** , η σύνδεση για το κουμπί **Άνοιγμα στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** δεν θα λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="b7265-185">If you click **No** , the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="b7265-186">Το αρχείο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] είναι διαθέσιμο στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] στην περιοχή **Έγγραφα** του εκάστοτε έργου [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="b7265-187">Δημοσίευση του έργου σας ως προτύπου</span><span class="sxs-lookup"><span data-stu-id="b7265-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="b7265-188">Μπορείτε να αποθηκεύσετε το έργο σας και να το χρησιμοποιήσετε ξανά αποθηκεύοντάς το ως πρότυπο έργου στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="b7265-189">Τα πρότυπα έργου είναι σχέδια με δυνατότητα επανάληψης χρήσης στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="b7265-190">[Δημιουργία προτύπου έργου (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="b7265-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="b7265-191">Από την καρτέλα **Project Service** , κάντε κλικ στις επιλογές **Δημοσίευση** > **Νέο πρότυπο έργου Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b7265-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="b7265-192">Στο πρότυπο **Δημοσίευση σε ένα νέο έργο στο Project Service** , καταχωρίστε **Όνομα προτύπου έργου**.</span><span class="sxs-lookup"><span data-stu-id="b7265-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="b7265-193">Προαιρετικά επιλέξτε **Σύνδεση πλάνου έργου στο Project Service Automation** , για να συνδέσετε το αρχείο έργου με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="b7265-194">Κάντε κλικ στην επιλογή **Δημοσίευση**.</span><span class="sxs-lookup"><span data-stu-id="b7265-194">Click **Publish**.</span></span>  

<span data-ttu-id="b7265-195">Η σύνδεση του αρχείου έργου με το [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] καθιστά το αρχείο έργου βασικό και ορίζει τη δομή ανάλυσης εργασίας στο πρότυπο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="b7265-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="b7265-196">Για να κάνετε αλλαγές στο σχέδιο έργου, πρέπει να το δημιουργήσετε στο [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] και να το δημοσιεύσετε ως ενημέρωση στο [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b7265-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="b7265-197">Δείτε επίσης</span><span class="sxs-lookup"><span data-stu-id="b7265-197">See Also</span></span>  
 [<span data-ttu-id="b7265-198">Οδηγός υπευθύνου έργου</span><span class="sxs-lookup"><span data-stu-id="b7265-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)