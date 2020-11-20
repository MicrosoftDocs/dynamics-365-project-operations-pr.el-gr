---
title: Επισκόπηση lite ανάπτυξης
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη lite ανάπτυξη του Dynamics 365 Project Operations.
author: rumant
manager: Annbe
ms.date: 11/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b66b3656d1ef5266ede1f62657dbe9b8a63c863a
ms.sourcegitcommit: d33ef0ae39f90fe3b0f6b4524f483e8052057361
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/03/2020
ms.locfileid: "4365488"
---
# <a name="lite-deployment-overview"></a><span data-ttu-id="0a638-103">Επισκόπηση lite ανάπτυξης</span><span class="sxs-lookup"><span data-stu-id="0a638-103">Lite deployment overview</span></span>

<span data-ttu-id="0a638-104">_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="0a638-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0a638-105">Ο τύπος lite ανάπτυξης του Dynamics 365 Project Operations έχει τις ακόλουθες δυνατότητες για εταιρείες που βασίζονται σε έργα:</span><span class="sxs-lookup"><span data-stu-id="0a638-105">The Lite deployment type of Dynamics 365 Project Operations has the following capabilities for project-based companies:</span></span>

- <span data-ttu-id="0a638-106">Προγραμματισμός έργου με χρήση του Microsoft Project for the Web</span><span class="sxs-lookup"><span data-stu-id="0a638-106">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="0a638-107">Πολυδιάστατη τιμολόγηση και κοστολόγηση εργατικού δυναμικού</span><span class="sxs-lookup"><span data-stu-id="0a638-107">Multi-dimensional pricing and costing for labor resources</span></span>
- <span data-ttu-id="0a638-108">Τιμολόγηση με βάση την κατηγορία για κατηγορίες δαπανών</span><span class="sxs-lookup"><span data-stu-id="0a638-108">Category-based pricing for expense categories</span></span>
- <span data-ttu-id="0a638-109">Διαχείριση πωλήσεων βάσει έργου με χρήση των δυνατοτήτων του Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="0a638-109">Project-based sales management using Dynamics 365 Sales capabilities</span></span>
- <span data-ttu-id="0a638-110">Universal resource scheduling που ενσωματώνεται με άλλες εφαρμογές, όπως το Dynamics 365 Field Service και το Dynamics 365 Customer Service</span><span class="sxs-lookup"><span data-stu-id="0a638-110">Universal resource scheduling that integrates with other applications such as Dynamics 365 Field Service and Dynamics 365 Customer Service</span></span>
- <span data-ttu-id="0a638-111">Πρόοδος έργου και παρακολούθηση χρόνου</span><span class="sxs-lookup"><span data-stu-id="0a638-111">Project progress and time tracking</span></span>
- <span data-ttu-id="0a638-112">Βασική παρακολούθηση εξόδων για έξοδα βάσει έργου</span><span class="sxs-lookup"><span data-stu-id="0a638-112">Basic expense tracking for project-based expenses</span></span>
- <span data-ttu-id="0a638-113">Μια προτιμολόγηση που μπορεί να αναθεωρηθεί και να αποσταλεί σε ένα χρηματοπιστωτικό σύστημα για επεξεργασία</span><span class="sxs-lookup"><span data-stu-id="0a638-113">Proforma invoicing that can be reviewed and sent to a financial system for processing</span></span>
- <span data-ttu-id="0a638-114">Επεκτασιμότητα μέσω του Power Platform</span><span class="sxs-lookup"><span data-stu-id="0a638-114">Extensibility through the Power Platform</span></span>

<span data-ttu-id="0a638-115">Αυτή η ανάπτυξη θα πρέπει να επιλεγεί και η προσδοκία του Project Operations είναι η χρήση ολόκληρου του κύκλου ζωής του έργου που περιλαμβάνει τις παρακάτω απαιτήσεις:</span><span class="sxs-lookup"><span data-stu-id="0a638-115">Use this deployment type if your expectation from Project Operations is to use the full project lifecycle, including the following requirements:</span></span>

- <span data-ttu-id="0a638-116">Δυνατότητα διαχείρισης πωλήσεων βάσει έργου με άλλους τύπους πωλήσεων με χρήση των δυνατοτήτων στην εφαρμογή "Sales".</span><span class="sxs-lookup"><span data-stu-id="0a638-116">Ability to manage project-based sales with other types of sales using the capabilities in the Sales application.</span></span>
- <span data-ttu-id="0a638-117">Ένα ολοκληρωμένο σύστημα που διαχειρίζεται εσωτερικά και χρεώσιμα προγράμματα για χρονοδιαγράμματα και οικονομικά στοιχεία από τις πωλήσεις έργου ως την τιμολόγηση.</span><span class="sxs-lookup"><span data-stu-id="0a638-117">An integrated system that manages internal and billable projects for schedules and financials from project sales to invoicing.</span></span>
- <span data-ttu-id="0a638-118">Ένας τρίτος προγραμματισμός εταιρικών πόρων (ERP/χρηματοοικονομικό λογιστικό σύστημα για ενοποίηση με το Project Operations.</span><span class="sxs-lookup"><span data-stu-id="0a638-118">A third-party Enterprise resource planning (ERP/Financial accounting system to integrate with Project Operations.</span></span>
- <span data-ttu-id="0a638-119">Ένα σύστημα τρίτου που θα εργάζεται με τους φόρους πωλήσεων, τις συναλλαγματικές ισοτιμίες, τις αποζημιώσεις δαπανών και τις δαπάνες εκτός έργου.</span><span class="sxs-lookup"><span data-stu-id="0a638-119">A third-party system to work with sales taxes, exchange rates, expense reimbursements, and non-project expenses.</span></span>
