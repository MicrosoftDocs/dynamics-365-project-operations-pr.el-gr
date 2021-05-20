---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 21, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 21, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: ad44f6747486222cc1f48c7b645f2525d382dca3
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949049"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="c426a-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 21, V3</span><span class="sxs-lookup"><span data-stu-id="c426a-103">Project Service Automation Update Release 21, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="c426a-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c426a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="c426a-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="c426a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c426a-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="c426a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c426a-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="c426a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="c426a-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c426a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c426a-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το Project Service Automation V3, έκδοση ενημέρωσης 21.</span><span class="sxs-lookup"><span data-stu-id="c426a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="c426a-110">Αυτή η έκδοση έχει αριθμό δομής V 3.10.32.50 και είναι γενικά διαθέσιμη μέσω της αυτοενημέρωσης Ιουνίου 2020.</span><span class="sxs-lookup"><span data-stu-id="c426a-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="c426a-111">Έκδοση κυκλοφορίας 21</span><span class="sxs-lookup"><span data-stu-id="c426a-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="c426a-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="c426a-112">Bug fixes</span></span>

<span data-ttu-id="c426a-113">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="c426a-113">**Time and Expense**</span></span>

<span data-ttu-id="c426a-114">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="c426a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="c426a-115">Όταν φιλοξενείτε το **Στοιχείο ελέγχου πλέγματος καταχώρησης ώρας** στους πίνακες εργαλείων, το πλέγμα δεν χρησιμοποιεί το πλήρες πλάτος του κοντέινερ πλέγματος του πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="c426a-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="c426a-116">Για συγκεκριμένες ζώνες ώρας, το στοιχείο ελέγχου πλέγματος **Καταχώρηση ώρας** δεν εμφανίζει καρτέλες.</span><span class="sxs-lookup"><span data-stu-id="c426a-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="c426a-117">Οι καταχωρήσεις ώρας που βρίσκονται μετά τις 9:00 μμ εμφανίζονται τη λάθος ημέρα.</span><span class="sxs-lookup"><span data-stu-id="c426a-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="c426a-118">Οι χρήστες δεν μπορούν να υποβάλλουν έξοδα εάν η κατηγορία εξόδων, **Απαιτείται απόδειξη δαπάνης** δεν έχει καμία τιμή.</span><span class="sxs-lookup"><span data-stu-id="c426a-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="c426a-119">**Διαχείριση πόρων**</span><span class="sxs-lookup"><span data-stu-id="c426a-119">**Resource Management**</span></span>

<span data-ttu-id="c426a-120">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="c426a-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="c426a-121">Οι ανενεργές κρατήσεις εμφανίζονται στην προβολή **Συμφωνία**.</span><span class="sxs-lookup"><span data-stu-id="c426a-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="c426a-122">Έλειπε η επικύρωση γενικού πόρου, για να διασφαλιστεί ότι υπάρχει μια έγκυρη κατάσταση κράτησης.</span><span class="sxs-lookup"><span data-stu-id="c426a-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="c426a-123">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="c426a-123">**Project Management**</span></span>

<span data-ttu-id="c426a-124">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="c426a-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="c426a-125">Τα πλέγματα φόρμας **Έργο** (**Ανάθεση πόρου**, **Εργασία**, προβολή **Συμφωνία**, **Εκτιμήσεις εξόδων**) παραμένουν επεξεργάσιμα ακόμα και όταν ένα έργο δεν είναι ενεργό.</span><span class="sxs-lookup"><span data-stu-id="c426a-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="c426a-126">Δεν είναι δυνατή η συγχώνευση διπλότυπων πελατών με τους πελάτες που συνδέονται με επιβεβαιωμένες συμβάσεις έργου.</span><span class="sxs-lookup"><span data-stu-id="c426a-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="c426a-127">Όταν προστίθεται ένας πόρος που δεν έχει έγκυρο ημερολόγιο, το σύστημα δεν επιστρέφει ένα μήνυμα σφάλματος φιλικό προς τον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="c426a-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="c426a-128">Το κουμπί **Προσθήκη εργασίας** στο πλέγμα εργασιών ενεργοποιείται όταν το έργο συνδέεται με το **Πρόσθετο του Microsoft Project**.</span><span class="sxs-lookup"><span data-stu-id="c426a-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="c426a-129">Η προσπάθεια μεγαλώνει ανεξέλεγκτα όταν μια εργασία με μια κατηγορία έχει ανατεθεί σε έναν πόρο με ένα ρόλο για τον οποίο έχει καθοριστεί μια τιμή κόστους.</span><span class="sxs-lookup"><span data-stu-id="c426a-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="c426a-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="c426a-130">**Sales**</span></span>

<span data-ttu-id="c426a-131">Έχουν γίνει οι ακόλουθες βελτιώσεις:</span><span class="sxs-lookup"><span data-stu-id="c426a-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="c426a-132">Η **Συχνότητα τιμολογίων** και η **Έναρξη χρέωσης** έχουν μετακινηθεί στην καρτέλα **Χρονοδιάγραμμα τιμολογίων**.</span><span class="sxs-lookup"><span data-stu-id="c426a-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="c426a-133">Διορθώθηκαν τα ακόλουθα ζητήματα:</span><span class="sxs-lookup"><span data-stu-id="c426a-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="c426a-134">Η **Συνολική τιμή πώλησης** είναι μηδέν (0) για την **Κατηγορία** αν και ο **Ρόλος** έχει μια συνολική τιμή πώλησης που δεν είναι μηδέν.</span><span class="sxs-lookup"><span data-stu-id="c426a-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="c426a-135">Οι πελάτες δεν μπορούν να αλλάξουν την τιμή του πεδίου **Κατάσταση τιμολογίου** σε **Έτοιμο για τιμολόγηση** όταν μια άλλη προσαρμοσμένη διεργασία ενημερώνει ένα πρόσθετο πεδίο.</span><span class="sxs-lookup"><span data-stu-id="c426a-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="c426a-136">Το κουμπί **Ανανέωση γραμμών τιμολογίου** μπορεί να δημιουργήσει πολλές διπλότυπες γραμμές εάν έχει επιλεγεί επανειλημμένα.</span><span class="sxs-lookup"><span data-stu-id="c426a-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="c426a-137">Το κουμπί **Ενημέρωση τιμών** δεν λειτουργεί στο υποπλέγμα **Τιμές ρόλου** στη φόρμα **Γρήγορη προβολή**.</span><span class="sxs-lookup"><span data-stu-id="c426a-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="c426a-138">Η λογική **Επίλυση τιμοκαταλόγου πωλήσεων** δεν χειρίζεται σωστά τις ζώνες ώρας, με αποτέλεσμα τη λανθασμένη επιλογή των τιμοκαταλόγων.</span><span class="sxs-lookup"><span data-stu-id="c426a-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="c426a-139">Το **Συνολικό πραγματικό κόστος** ενός έργου μπορεί να εκπίπτει από ένα κλασματικό ποσό μετά από την έγκριση μιας άπαξ καταχώρησης.</span><span class="sxs-lookup"><span data-stu-id="c426a-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="c426a-140">Η λογικη **Επίλυση τιμής** δεν παρέχει ένα μήνυμα σφάλματος φιλικό προς τον χρήστη εάν η **Ανακτειμένη τιμή ρόλου** δεν έχει τιμές στα πεδία **Κύρια μονάδα** και **Τιμή στην κύρια μονάδα**.</span><span class="sxs-lookup"><span data-stu-id="c426a-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]