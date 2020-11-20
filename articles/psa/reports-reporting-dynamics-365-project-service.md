---
title: Αρχική σελίδα αναφοράς
description: Αυτό το θέμα παρέχει συνδέσεις σε πληροφορίες σχετικά με τις αναφορές στο Dynamics 365 Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: e1a645b157c56066e56b22ea8cf0324fbc1ddd2c
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120318"
---
# <a name="reporting-home-page"></a><span data-ttu-id="edec6-103">Αρχική σελίδα αναφοράς</span><span class="sxs-lookup"><span data-stu-id="edec6-103">Reporting home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="edec6-104">Το Microsoft Dynamics 365 Project Service Automation επιτρέπει στους οργανισμούς που βασίζονται σε έργα να διαχειρίζονται αποτελεσματικά τις λειτουργίες της επιχείρησής τους.</span><span class="sxs-lookup"><span data-stu-id="edec6-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="edec6-105">Σε οποιοδήποτε έργο, τα μέλη της ομάδας πρέπει να διαχειρίζονται την ευκαιρία, να κάνουν προσφορά και να σχεδιάζουν την εργασία, να διαχειρίζονται τα έργα, να διαχειρίζονται την εργασία σύμφωνα με το σχέδιο, να τιμολογούν την εργασία και, στη συνέχεια, να κάνουν την εργασία για την ολοκλήρωση του έργου.</span><span class="sxs-lookup"><span data-stu-id="edec6-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="edec6-106">Η δυνατότητα αναφοράς για λειτουργίες είναι το κλειδί για τον καθορισμό της εύρυθμης λειτουργίας του οργανισμού και τη λήψη των απαραίτητων διορθωτικών μέτρων.</span><span class="sxs-lookup"><span data-stu-id="edec6-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="edec6-107">Το PSA χρησιμοποιεί τις μεθόδους αναφοράς και τις τεχνολογίες του Microsoft Dynamics 365 για όλα τα στοιχεία που αναφέρει.</span><span class="sxs-lookup"><span data-stu-id="edec6-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="edec6-108">Για περισσότερες πληροφορίες σχετικά με τις επιλογές αναφοράς, ανατρέξτε στον [οδηγό σύνταξης αναφορών για το Dynamics 365 Customer Engagement (on-premises), έκδοση 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="edec6-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="edec6-109">Οδηγός αναφοράς</span><span class="sxs-lookup"><span data-stu-id="edec6-109">Report Wizard</span></span>

<span data-ttu-id="edec6-110">Ο Οδηγός αναφοράς επιτρέπει στους μη προγραμματιστές να δημιουργούν απλές αναφορές.</span><span class="sxs-lookup"><span data-stu-id="edec6-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="edec6-111">Επειδή η εφαρμογή είναι ενσωματωμένη σε μια υπάρχουσα πλατφόρμα, η εμπειρία είναι η ίδια με την εμπειρία που τεκμηριώνεται στη [Δημιουργία ή την επεξεργασία μιας αναφοράς χρησιμοποιώντας τον "Οδηγό αναφοράς"](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span><span class="sxs-lookup"><span data-stu-id="edec6-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="edec6-112">Ωστόσο, θα χρησιμοποιήσετε τις οντότητες που αφορούν το Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="edec6-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="edec6-113">Προσαρμοσμένες αναφορές υπηρεσιών αναφοράς του SQL Server</span><span class="sxs-lookup"><span data-stu-id="edec6-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="edec6-114">Εάν η επιχείρησή σας απαιτεί μια συγκεκριμένη αναφορά η οποία δεν είναι δυνατό να δημιουργηθεί με χρήση του οδηγού αναφοράς, μπορείτε να δημιουργήσετε μια προσαρμοσμένη αναφορά.</span><span class="sxs-lookup"><span data-stu-id="edec6-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="edec6-115">Πρέπει να έχετε εγκαταστήσει το Microsoft Visual Studio μαζί με τις κατάλληλες επεκτάσεις σύνταξης αναφορών Microsoft SQL Server Data Tools.</span><span class="sxs-lookup"><span data-stu-id="edec6-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="edec6-116">Για περισσότερες πληροφορίες σχετικά με τα εργαλεία και τις εκδόσεις δείτε [Περιβάλλον σύνταξης αναφορών χρησιμοποιώντας το SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="edec6-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="edec6-117">Για πληροφορίες σχετικά με τον τρόπο δημιουργίας μιας προσαρμοσμένης αναφοράς δείτε [Δημιουργία νέας αναφοράς χρησιμοποιώντας SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="edec6-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="edec6-118">Εφαρμογές Power BI insights</span><span class="sxs-lookup"><span data-stu-id="edec6-118">Power BI insights apps</span></span>

<span data-ttu-id="edec6-119">Μαζί, τα Microsoft Power BI και Dynamics 365 σας παρέχουν έναν ισχυρό τρόπο για να εργαστείτε με τα δεδομένα σας, με τη μορφή εφαρμογών Insights.</span><span class="sxs-lookup"><span data-stu-id="edec6-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="edec6-120">Για πληροφορίες σχετικά με τη διαθεσιμότητα των εφαρμογών Insights, ανατρέξτε στην ενότητα [Σελίδα εφαρμογών Power BI insights](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="edec6-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="edec6-121">Πρόσθετοι πόροι</span><span class="sxs-lookup"><span data-stu-id="edec6-121">Additional resources</span></span>
<span data-ttu-id="edec6-122">Για περισσότερες πληροφορίες σχετικά με τις αναφορές στο PSA, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="edec6-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="edec6-123">Εργασία με το μοντέλο δεδομένων Project Service</span><span class="sxs-lookup"><span data-stu-id="edec6-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="edec6-124">Πίνακες εργαλείων</span><span class="sxs-lookup"><span data-stu-id="edec6-124">Dashboards</span></span>](reports-dashboards.md)

