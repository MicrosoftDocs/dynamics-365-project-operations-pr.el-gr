---
title: Τι νέο υπάρχει ή άλλαξε στο Project Service Automation, έκδοση ενημέρωσης 17, V3
description: Αυτό το θέμα παραθέτει τις δυνατότητες και επιδιορθώσεις που είναι διαθέσιμες στο Project Service Automation, έκδοση ενημέρωσης 17, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: bb93208217972639f91b39b7b6705d9897373ef7
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126798"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="52416-103">Τι νέο υπάρχει στο Project Service Automation, έκδοση ενημέρωσης 17, V3</span><span class="sxs-lookup"><span data-stu-id="52416-103">Project Service Automation Update Release 17, V3</span></span>

<span data-ttu-id="52416-104">Με χαρά σας ανακοινώνουμε την πιο πρόσφατη ενημέρωση για την εφαρμογή Project Service Automation για το Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="52416-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="52416-105">Αυτή η έκδοση περιλαμβάνει ορισμένες σημαντικές βελτιώσεις όσον αφορά την ποιότητα, την απόδοση και τη χρηστικότητα.</span><span class="sxs-lookup"><span data-stu-id="52416-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="52416-106">Αυτή η έκδοση είναι συμβατή με το Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="52416-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="52416-107">Για να πραγματοποιήσετε ενημέρωση σε αυτήν την έκδοση, επισκεφθείτε το κέντρο διαχείρισης για το Dynamics 365 online, στη σελίδα λύσεων για να εγκαταστήσετε την ενημέρωση.</span><span class="sxs-lookup"><span data-stu-id="52416-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="52416-108">Για περισσότερες πληροφορίες, δείτε [Εγκατάσταση, ενημέρωση ή κατάργηση μιας προτιμώμενης λύσης](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="52416-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="52416-109">Αυτό το θέμα παραθέτει τις νέες ή τροποποιημένες δυνατότητες και επιδιορθώσεις για το PSA V3, έκδοση ενημέρωσης 17.</span><span class="sxs-lookup"><span data-stu-id="52416-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="52416-110">Αυτή η έκδοση έχει αριθμό δομής V3.10.6.34 και είναι γενικά διαθέσιμη μέσω μιας αυτοενημέρωσης που πραγματοποιήθηκε τον Μάρτιο του 2020.</span><span class="sxs-lookup"><span data-stu-id="52416-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="52416-111">Έκδοση κυκλοφορίας 17</span><span class="sxs-lookup"><span data-stu-id="52416-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="52416-112">Επιδιορθώσεις σφαλμάτων</span><span class="sxs-lookup"><span data-stu-id="52416-112">Bug fixes</span></span>

<span data-ttu-id="52416-113">**Γενικά**</span><span class="sxs-lookup"><span data-stu-id="52416-113">**General**</span></span>

- <span data-ttu-id="52416-114">Διόρθωση: ενημέρωση Project Service Automation για την επιβολή αδειών χρήσης μελών ομάδας (το Κέντρο πόρων έργου θα συμπεριλάβει τα μετα-δεδομένα σχεδίου υπηρεσίας μέλους ομάδας 3. x)</span><span class="sxs-lookup"><span data-stu-id="52416-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="52416-115">**Χρόνος και έξοδα**</span><span class="sxs-lookup"><span data-stu-id="52416-115">**Time and Expense**</span></span>

- <span data-ttu-id="52416-116">Διόρθωση: δεν είναι δυνατή η αλλαγή μιας εκτίμησης εξόδων από μια μη μηδενική τιμή σε μηδέν (0).</span><span class="sxs-lookup"><span data-stu-id="52416-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="52416-117">Η αλλαγή παραβλέπεται.</span><span class="sxs-lookup"><span data-stu-id="52416-117">The change is ignored.</span></span>

<span data-ttu-id="52416-118">**Διαχείριση έργων**</span><span class="sxs-lookup"><span data-stu-id="52416-118">**Project Management**</span></span>

- <span data-ttu-id="52416-119">Διόρθωση: προστέθηκε ένα σημάδι ελέγχου για τις μηδενικές τιμές στο όνομα θέσης ενός μέλους ομάδας.</span><span class="sxs-lookup"><span data-stu-id="52416-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="52416-120">Διόρθωση: το πεδίο **msdyn_userresourceid** στην οντότητα **msdyn_resourceassignment** έχει καταργηθεί.</span><span class="sxs-lookup"><span data-stu-id="52416-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="52416-121">Διόρθωση: η αναβάθμιση από 2. x σε 3. x πλέον χειρίζεται κενά περιγράμματα προσπάθειας σε αναθέσεις εργασιών.</span><span class="sxs-lookup"><span data-stu-id="52416-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="52416-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="52416-122">**Sales**</span></span>

- <span data-ttu-id="52416-123">Διόρθωση: το **Invoice.PreValidateInvoiceUpdate** χειρίζεται πλέον το σενάριο της εκ νέου ανάθεσης κατόχων καρτέλας σωστά.</span><span class="sxs-lookup"><span data-stu-id="52416-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="52416-124">Διόρθωση: όταν η κλάση συναλλαγής είναι **Ώρα**, η **Ομάδα μονάδας** δεν είναι επεξεργάσιμη για όλες τις οντότητες συμπεριλαμβανομένων των **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** και **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="52416-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="52416-125">Ωστόσο, η **Μονάδα** είναι μη επεξεργάσιμη μόνο για **JournalLine** και **InvoiceLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="52416-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


