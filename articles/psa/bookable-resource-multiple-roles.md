---
title: Υπολογισμός πωλήσεων και κόστους του έργου όταν ένας πόρος με δυνατότητα κράτησης καλύπτει πολλαπλούς ρόλους σε ένα έργο
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τον τρόπο με τον οποίο οι διαστάσεις τιμολόγησης μπορούν να χρησιμοποιηθούν για την υποστήριξη τιμολόγησης και κοστολόγησης για έναν πόρο που καλύπτει πολλαπλούς ρόλους σε ένα έργο.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4076968"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="55821-103">Υπολογισμός πωλήσεων και κόστους του έργου όταν ένας πόρος με δυνατότητα κράτησης καλύπτει πολλαπλούς ρόλους σε ένα έργο</span><span class="sxs-lookup"><span data-stu-id="55821-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="55821-104">Οι εταιρείες που βασίζονται σε έργα έχουν συχνά την ανάγκη ένας πόρος να εκτελεί πολλαπλούς ρόλους σε ένα έργο.</span><span class="sxs-lookup"><span data-stu-id="55821-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="55821-105">Όλοι αυτοί οι ρόλοι θα μπορούσαν να τιμολογούνται και να κοστολογούνται διαφορετικά, γεγονός που σημαίνει ότι ο χρόνος του ίδιου πόρου στο έργο μπορεί να λάβει διαφορετική οικονομική εκτίμηση ανάλογα με το κόστος χρέωσης και τις μοναδιαίες τιμές για κάθε ρόλο.</span><span class="sxs-lookup"><span data-stu-id="55821-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="55821-106">Το Project Service Automation επιτρέπει την παραμετροποίηση των τιμών στην καρτέλα μέλους ομάδας για τον κατονομαζόμενο πόρο και επιτρέπει διαφορετικές παρακάμψεις σε κάθε μία από τις εργασίες που έχουν ανατεθεί στο μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="55821-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="55821-107">Το παρακάτω παράδειγμα περιγράφει τον τρόπο με τον οποίο η απλή παράκαμψη αυτής της τιμής, επιτρέπει σε έναν πόρο να έχει πολλούς ρόλους σε ένα έργο με διαφορετικές χρεώσεις κόστους και χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="55821-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="55821-108">Δημιουργία εργασιών</span><span class="sxs-lookup"><span data-stu-id="55821-108">Create tasks</span></span>
<span data-ttu-id="55821-109">Δημιουργήστε δύο εργασίες έργου για 40 ώρες έκαστη, την Εργασία Α και την Εργασία Β. Επιλέξτε την Εργασία Α ως πρόδρομο της Εργασίας Β.</span><span class="sxs-lookup"><span data-stu-id="55821-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="55821-110">Ρυθμίστε ρόλο και οργανωτική μονάδα για ένα γενικό μέλος ομάδας έργου</span><span class="sxs-lookup"><span data-stu-id="55821-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="55821-111">Στη σελίδα **Προγραμματισμός** , επιλέξτε τη γραμμή **Εργασιών** για την Εργασία Α.</span><span class="sxs-lookup"><span data-stu-id="55821-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="55821-112">Στο πεδίο **Πόροι** , επιλέξτε **Δημιουργία** στην αναπτυσσόμενη λίστα.</span><span class="sxs-lookup"><span data-stu-id="55821-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="55821-113">Στη σελίδα **Γρήγορη δημιουργία μέλους ομάδας** , καθορίστε τα χαρακτηριστικά του γενικού μέλους ομάδας που μπορεί να εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="55821-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="55821-114">Επιλέξτε τον κατάλληλο ρόλο και οργανωτική μονάδα και, στη συνέχεια, επιλέξτε **Αποθήκευση και κλείσιμο**.</span><span class="sxs-lookup"><span data-stu-id="55821-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="55821-115">Ένα γενικό μέλος ομάδας δημιουργείται και εκχωρείται σε αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="55821-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="55821-116">Επαναλάβετε αυτά τα βήματα για την Εργασία Β και βεβαιωθείτε ότι ο ρόλος και η οργανωτική μονάδα του μέλους ομάδας γενικής χρήσης που δημιουργήσατε για την Εργασία Β, είναι διαφορετικά από την Εργασία Α.</span><span class="sxs-lookup"><span data-stu-id="55821-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="55821-117">Ρυθμίστε ρόλο και οργανωτική μονάδα για μια εργασία έργου</span><span class="sxs-lookup"><span data-stu-id="55821-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="55821-118">Αφού δημιουργήσετε την Εργασία Α, επιλέξτε την εργασία και, στη συνέχεια, επιλέξτε **Επεξεργασία εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="55821-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="55821-119">Στη σελίδα **Λεπτομερειών εργασίας** , εντοπίστε τα πεδία **Ρόλος** και **Οργανωτική μονάδα** , προσθέστε τις τιμές που απαιτούνται από έναν πόρο που θα εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="55821-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="55821-120">Εάν ολοκληρώνετε αυτό το σενάριο χρησιμοποιώντας τα δεδομένα επίδειξης του Project Service Automation, επιλέξτε **Συμβουλές υποψήφιου πελάτη** για τον ρόλο και **Fabrikam US** ως την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="55821-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="55821-121">Επιλέξτε την Εργασία Β και, στη συνέχεια, επιλέξτε **Επεξεργασία εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="55821-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="55821-122">Στη σελίδα **Λεπτομερειών εργασίας** , εντοπίστε τα πεδία **Ρόλος** και **Οργανωτική μονάδα** , προσθέστε τις τιμές που απαιτούνται από έναν πόρο που θα εκτελέσει αυτήν την εργασία.</span><span class="sxs-lookup"><span data-stu-id="55821-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="55821-123">Βεβαιωθείτε ότι οι τιμές στα πεδία **Ρόλος** και **Οργανωτική μονάδα** είναι διαφορετικές για την Εργασία Β από αυτές για την Εργασία Α.</span><span class="sxs-lookup"><span data-stu-id="55821-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="55821-124">Εάν ολοκληρώνετε αυτό το σενάριο χρησιμοποιώντας τα δεδομένα επίδειξης του Project Service Automation, επιλέξτε **Τεχνικός δικτύου** για τον ρόλο και **Fabrikam US** ως την οργανωτική μονάδα.</span><span class="sxs-lookup"><span data-stu-id="55821-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="55821-125">Αποθηκεύστε και κλείστε τη σελίδα **Λεπτομέρειες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="55821-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="55821-126">Μέλος ομάδας και συμπεριφορά εκτιμήσεων</span><span class="sxs-lookup"><span data-stu-id="55821-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="55821-127">Στη σελίδα **Λεπτομερειών εργασίας** στο **Μέλος ομάδας** , επιλέξτε τα δύο γενικά μέλη της ομάδας και, στη συνέχεια, επιλέξτε **Δημιουργία απαιτήσεων**.</span><span class="sxs-lookup"><span data-stu-id="55821-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="55821-128">Με τον τρόπο αυτό θα δημιουργηθούν απαιτήσεις πόρων.</span><span class="sxs-lookup"><span data-stu-id="55821-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="55821-129">Επιλέξτε τη σειρά μελών ομάδας για τη **Συνεννόηση με υποψήφιο πελάτη** και, στη συνέχεια, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="55821-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="55821-130">Ο πίνακας χρονοδιαγράμματος ανοίγει και κάνει κράτηση ενός πόρου σε αυτήν την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="55821-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="55821-131">Επιλέξτε τη σειρά μελών ομάδας για τον **Τεχνικό δικτύου** και, στη συνέχεια, επιλέξτε **Κράτηση**.</span><span class="sxs-lookup"><span data-stu-id="55821-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="55821-132">Ο πίνακας χρονοδιαγράμματος ανοίγει και κάνει κράτηση του ίδιου πόρου σε αυτήν την απαίτηση.</span><span class="sxs-lookup"><span data-stu-id="55821-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="55821-133">Πλέγμα Μέλους ομάδας</span><span class="sxs-lookup"><span data-stu-id="55821-133">Team Member grid</span></span> 
<span data-ttu-id="55821-134">Στο πλέγμα **Μέλους ομάδας** , παρατηρήστε ότι οι δύο καρτέλες του μέλους γενικής ομάδας διαγράφονται και έχουν αντικατασταθεί από έναν πόρο.</span><span class="sxs-lookup"><span data-stu-id="55821-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="55821-135">Υπάρχει ένα σύνολο τιμών για αυτόν τον πόρο, ο οποίος εμφανίζει ένα προεπιλεγμένο σύνολο τιμών για τον **Ρόλο** και την **Οργανωτική μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="55821-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="55821-136">Όταν αναπτύσσετε τη γραμμή της καρτέλας Μέλους ομάδας, μπορείτε να δείτε διακριτές αναθέσεις στην καρτέλα μέλους ομάδας και για τις δύο αυτές εργασίες.</span><span class="sxs-lookup"><span data-stu-id="55821-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="55821-137">Κάθε γραμμή ανάθεσης έχει συγκεκριμένες τιμές εργασιών για τον **Ρόλο** και την **Οργανωτική μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="55821-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="55821-138">Πλέγμα εκτιμήσεων</span><span class="sxs-lookup"><span data-stu-id="55821-138">Estimates grid</span></span> 
<span data-ttu-id="55821-139">Όταν μεταβαίνετε στο πλέγμα **Εκτιμήσεις** , θα παρατηρήσετε ότι και οι δύο αναθέσεις για τον ίδιο πόρο τιμολογούνται διαφορετικά.</span><span class="sxs-lookup"><span data-stu-id="55821-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="55821-140">Η ανάθεση για τον πόρο στην Εργασία Α διατιμάται με χρήση της τιμής του χαρακτηριστικού **Ρόλος** της **Συνεννόησης με υποψήφιο πελάτη**.</span><span class="sxs-lookup"><span data-stu-id="55821-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="55821-141">Η ανάθεση για τον ίδιο πόρο στην Εργασία Β διατιμάται με χρήση της τιμής του χαρακτηριστικού **Ρόλος** του **Τεχνικού δικτύου**.</span><span class="sxs-lookup"><span data-stu-id="55821-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>




