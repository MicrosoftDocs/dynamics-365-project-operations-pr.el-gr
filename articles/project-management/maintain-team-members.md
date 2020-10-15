---
title: Διατήρηση μελών ομάδας
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με την κράτηση καθορισμένων πόρων σε ομάδες εργασίας και ανάθεση εργασιών.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: f5b36628e90896c9fe6570de71c95eab83a44ebd
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961869"
---
# <a name="maintain-team-members"></a><span data-ttu-id="bf671-103">Διατήρηση μελών ομάδας</span><span class="sxs-lookup"><span data-stu-id="bf671-103">Maintain team members</span></span>

<span data-ttu-id="bf671-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="bf671-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bf671-105">Μπορείτε να προσθέσετε έναν καθορισμένο πόρο στην ομάδα έργου σας κάνοντας κράτηση απευθείας στην ομάδα.</span><span class="sxs-lookup"><span data-stu-id="bf671-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="bf671-106">Στο Dynamics 365 Project Operations, μεταβείτε στα **Έργα** και επιλέξτε το άνοιγμα του έργου για το οποίο κάνετε κράτηση.</span><span class="sxs-lookup"><span data-stu-id="bf671-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="bf671-107">Στη σελίδα **Έργο**, στην καρτέλα **Ομάδα**, κάντε κλικ στην επιλογή **Δημιουργία**.</span><span class="sxs-lookup"><span data-stu-id="bf671-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="bf671-108">Στο παράθυρο διαλόγου **Γρήγορη δημιουργία μέλους ομάδας έργου**, επιλέξτε τον πόρο με δυνατότητα κράτησης.</span><span class="sxs-lookup"><span data-stu-id="bf671-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="bf671-109">Το πεδίο **Ρόλος** θα συμπληρωθεί με τον προεπιλεγμένο ρόλο του πόρου, σε περίπτωση που του έχει ανατεθεί μια εργασία.</span><span class="sxs-lookup"><span data-stu-id="bf671-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="bf671-110">Μπορείτε να αλλάξετε τον ρόλο.</span><span class="sxs-lookup"><span data-stu-id="bf671-110">You can change the role.</span></span> 
4. <span data-ttu-id="bf671-111">Επιλέξτε τις ημερομηνίες από και έως κατά τις οποίες θα χρειαστεί ο πόρος και επιλέξτε τη μέθοδο ανάθεσης της παραγωγικής ικανότητας του πόρου.</span><span class="sxs-lookup"><span data-stu-id="bf671-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="bf671-112">Εάν θέλετε το μέλος της ομάδας να είναι υπεύθυνος έγκρισης έργου, επιλέξτε **Ναι** στο πεδίο **Υπεύθυνος έγκρισης έργου**.</span><span class="sxs-lookup"><span data-stu-id="bf671-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="bf671-113">Τα μέλη της ομάδας μπορούν να εγκρίνουν τις καταχωρήσεις χρόνου και εξόδων που υποβάλλονται για αυτό το έργο.</span><span class="sxs-lookup"><span data-stu-id="bf671-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="bf671-114">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="bf671-114">Select **Save**.</span></span>

<span data-ttu-id="bf671-115">Τώρα, μπορείτε να αναθέσετε τον πόρο με δυνατότητα κράτησης σε εργασίες του έργου.</span><span class="sxs-lookup"><span data-stu-id="bf671-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="bf671-116">Στη σελίδα **Έργο**, επιλέξτε την καρτέλα **Χρονοδιάγραμμα** για να αναθέσετε εργασίες στο νέο πόρο.</span><span class="sxs-lookup"><span data-stu-id="bf671-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="bf671-117">Ο επιλογέας πόρων που εκκινείται από το πεδίο **Πόροι** στο πλέγμα εργασιών θα εμφανίζει τα μέλη της ομάδας που μπορείτε να επιλέξετε.</span><span class="sxs-lookup"><span data-stu-id="bf671-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="bf671-118">Στο Project Operations, οι κρατήσεις πόρων και οι αναθέσεις εργασιών δεν συνδέονται στενά.</span><span class="sxs-lookup"><span data-stu-id="bf671-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="bf671-119">Όταν χρησιμοποιείτε τον επιλογέα πόρων στο χρονοδιάγραμμα, μπορείτε να αναθέσετε εργασίες σε μέλη της ομάδας για περισσότερες ώρες από αυτές που καλύπτουν οι κρατήσεις τους στο έργο.</span><span class="sxs-lookup"><span data-stu-id="bf671-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="bf671-120">Οι διαφορές μεταξύ των κρατήσεων και των αναθέσεων για τα μέλη της ομάδας εμφανίζονται στις καρτέλες **Ομάδα** και **Συμφωνία πόρων**.</span><span class="sxs-lookup"><span data-stu-id="bf671-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="bf671-121">Μπορείτε, επίσης, να συνδυάσετε τις διαφορές μεταξύ των κρατήσεων και των αναθέσεων για πόρους σε πιο αναλυτικό επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="bf671-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="bf671-122">Χρησιμοποιήστε τον επιλογέα πόρων στην καρτέλα **Χρονοδιάγραμμα** για να αναζητήσετε και να επιλέξετε πόρους με δυνατότητα κράτησης που δεν ανήκουν ήδη στην ομάδα έργου.</span><span class="sxs-lookup"><span data-stu-id="bf671-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="bf671-123">Οι πόροι εμφανίζονται στον επιλογέα πόρων ως **Άλλοι πόροι**.</span><span class="sxs-lookup"><span data-stu-id="bf671-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="bf671-124">Όταν κάνετε μια επιλογή, ο πόρος προστίθεται στην ομάδα έργου και ανατίθεται στην εργασία, αλλά δεν δημιουργούνται κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="bf671-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="bf671-125">Μπορείτε να χρησιμοποιήσετε τη δυνατότητα παράτασης κράτησης της καρτέλας **Εναρμόνιση** ή τον **Πίνακα χρονοδιαγράμματος** για να κάνετε κράτηση της παραγωγικής ικανότητας του πόρου στο έργο.</span><span class="sxs-lookup"><span data-stu-id="bf671-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="bf671-126">Αφού γίνει κράτηση ενός μέλους ομάδας στο έργο σας, μπορείτε να χρησιμοποιήσετε τη **Διατήρηση κρατήσεων** ή τον **Πίνακα χρονοδιαγράμματος** απευθείας για να διαχειριστείτε τις κρατήσεις του.</span><span class="sxs-lookup"><span data-stu-id="bf671-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>
