---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 20, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 20, V3
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 5562b1de1d655328cfbb22e46c7fed53525507b3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006511"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="2e9f3-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 20, V3</span><span class="sxs-lookup"><span data-stu-id="2e9f3-103">Project Service Automation Update Release 20, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2e9f3-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="2e9f3-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2e9f3-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2e9f3-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="2e9f3-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2e9f3-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2e9f3-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 20.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="2e9f3-110">Αυτή η έκδοση έχει αριθμό δομής V 3.10.31.37 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Ιουνίου 2020.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="2e9f3-111">Έκδοση κυκλοφορίας 20</span><span class="sxs-lookup"><span data-stu-id="2e9f3-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2e9f3-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="2e9f3-112">Bug fixes</span></span>

<span data-ttu-id="2e9f3-113">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="2e9f3-113">**Project Management**</span></span>

<span data-ttu-id="2e9f3-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="2e9f3-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="2e9f3-115">Εισαγωγή μελών ομάδας έργου με μια μέθοδο εκχώρησης που απαιτεί αποτελέσματα ωρών σε ένα ασασφές μήνυμα σφάλματος όταν οι καθορισμένες ώρες είναι μηδέν.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="2e9f3-116">Οι χρήστες λαμβάνουν ένα μη έγκυρο σφάλμα, όταν ο μέγιστος αριθμός χαρακτήρων έχει εισαχθεί στο πεδίο **Περιγραφή** για μια εργασία έργου.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="2e9f3-117">Η σελίδα **Λήψης του πρόσθετου Microsoft Dynamics 365 Project Service Automation** ανακατευθύνει στη σελίδα λήψης στα Αγγλικά, όταν οι ρυθμίσεις γλώσσας του χρήστη έχουν οριστεί στα Ιαπωνικά.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="2e9f3-118">Όταν προκύπτει ένα σφάλμα διακομιστή, η ετικέτα συγχρονισμού στην καρτέλα **Χρονοδιάγραμμα** της φόρμας **Έργα** ορισμένες φορές παραμένει.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="2e9f3-119">Οι περιττές ενημερώσεις εργασιών στέλνονται στο διακομιστή όταν τροποποιείται μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="2e9f3-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="2e9f3-120">**Sales**</span></span>

<span data-ttu-id="2e9f3-121">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="2e9f3-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="2e9f3-122">Στη φόρμα **Επαφή**, αν κάνετε διπλό κλικ στη **Δημιουργία τιμολογίου** θα δημιουργηθούν δύο τιμολόγια για μία καρτέλα πραγματικών τιμών.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="2e9f3-123">Στον Internet Explorer 11, οι χρήστες δεν μπορούν να δημιουργήσουν καταχωρήσεις εξόδων.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="2e9f3-124">Η αντιστροφή του κόστους και η αντιστροφή μη χρεωμένων πραγματικών πωλήσεων δεν είναι συνδεδεμένες.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="2e9f3-125">Το κουμπί **Ανανέωση πραγματικών τιμών** στη φόρμα **Έργου** δεν ανανεώνει τις **πραγματικές ώρες εργασίας**.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="2e9f3-126">Η προσθήκη **PreValidateProjectTeamMemberCreate** μπορεί να δημιουργήσει διπλότυπους γενικούς πόρους με δυνατότητα κράτησης, όταν το χαρακτηριστικό **msdyn_isgenericresourceprojectscoped** είναι ορισμένο σε **False**.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="2e9f3-127">Η **Επανάληψη υπολογισμού** απαλείφει τα χρεώσιμα κόστη των λεπτομερειών της σειράς προσφοράς με βάση τα προϊόντα και τις λεπτομέρειες της σειράς σύμβασης.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="2e9f3-128">Σε συγκεκριμένα παραδείγματα, η προσθήκη **PostEstimateLineUpdate** εμφανίζει ένα σφάλμα εξαίρεσης αναφοράς null.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="2e9f3-129">Η διάρκεια της χρονικής φάσης στο **Γράφημα ανάλυσης κερδοφορίας** δεν ταιριάζει με τη διάρκεια του κόστους στη λεπτομέρεια της γραμμής προσφοράς σταθερής τιμής της προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="2e9f3-130">Οι τιμές μονάδας και ομάδας μονάδων δεν είναι προκαθορισμένες σωστά για κατηγορίες εξόδων στις φόρμες **λεπτομέρειες γραμμής σύμβασης** και **λεπτομέρειες γραμμής προσφοράς**.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="2e9f3-131">Οι λίστες **Τιμή κόστους μονάδας οργανισμού** επιτρέπουν επικαλύψεις στην αποτελεσματικότητα ημερομηνίας.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="2e9f3-132">Οι χρήστες δεν επιτρέπεται να αλλάξουν το **OrgUnit** όταν ο τύπος παραγγελίας δεν βασίζεται σε εργασία, επειδή αυτό θα οδηγήσει σε σφάλμα εξαίρεσης αναφοράς null.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="2e9f3-133">Όταν επιχειρείτε να περιηγηθείτε από τη φόρμα **λεπτομερειών γραμμής προσφοράς** πίσω στην καρτέλα **προσφορά**, η φόρμα ανανεώνεται και εμφανίζεται η καρτέλα **σύνοψης**.</span><span class="sxs-lookup"><span data-stu-id="2e9f3-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]