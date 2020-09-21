---
title: Επισκόπηση του Project Service Automation
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη λύση ενοποίησης του Dynamics 365 Project Service Automation στο Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 897e1a1c-d31c-42b8-bb59-6b67202d8d61
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 080a545d8713e52d9778367aec1969b815d683e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751618"
---
# <a name="project-service-automation-overview"></a>Επισκόπηση του Project Service Automation

[!include[banner](../includes/banner.md)]

Η λύση ενοποίησης του Project Service Automation στο Finance χρησιμοποιεί τη δυνατότητα ενοποίησης δεδομένων για το συγχρονισμό δεδομένων σε παρουσίες των Dynamics 365 Finance και Dynamics 365 Project Service Automation μέσω Common Data Service. Τα πρότυπα ενοποίησης που είναι διαθέσιμα με τη δυνατότητα ενοποίησης δεδομένων ενεργοποιούν τη ροή των έργων, τις συμβάσεις έργου, τις γραμμές σύμβασης έργου, τα ορόσημα γραμμής σύμβασης έργου, τις εργασίες έργου, τις κατηγορίες των συναλλαγών εξόδων, τις εκτιμήσεις ωρών και τις εκτιμήσεις εξόδων από το Project Service Automation στο Finance.

> [!NOTE]
> - Εάν χρησιμοποιείτε την έκδοση 7.3.0, θα πρέπει να εγκαταστήσετε το KB 4074835. Στη συνέχεια, θα έχετε τη δυνατότητα να ενσωματώσετε έργα σταθερών τιμών.
> - Εάν χρησιμοποιείτε την έκδοση 7.3.0 και πραγματοποιείτε συναλλαγές αμοιβών πάνω από το Project Service Automation, πρέπει να εγκαταστήσετε το KB 4345320, προκειμένου να συμπεριλάβετε αυτές τις χρεώσεις στο τιμολόγιο έργου.
> - Αν χρησιμοποιείτε την έκδοση 8.0, θα μπορείτε να χρησιμοποιείτε την ενοποίηση εργασιών έργου, τις κατηγορίες εξόδων, τις εκτιμήσεις ωρών, τις εκτιμήσεις εξόδων και το κλείδωμα λειτουργιών.
> - Εάν χρησιμοποιείτε την έκδοση 8.0.1 ή νεότερη, θα μπορείτε να συγχρονίσετε πραγματικές τιμές.

Για να μπορέσετε να ενσωματώσετε το Project Service Automation στο Finance, πρέπει να ρυθμίσετε τις παραμέτρους ενοποίησης του Project Service Automation. Για περισσότερες πληροφορίες δείτε [Παράμετροι ενοποίησης του Project Service Automation](PSA-parameters.md).

Αυτή η λύση ενοποίησης δίνει τη δυνατότητα άμεσου συγχρονισμού στα ακόλουθα σενάρια:

- Διατηρήστε τις συμβάσεις έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.
- Δημιουργήστε έργα στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.
- Διατηρήστε τις γραμμές σύμβασης έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.
- Διατηρήστε τα ορόσημα γραμμής σύμβασης έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.
- Διατηρήστε τις εργασίες έργου στο Project Service Automation και συγχρονίστε τις απευθείας από το Project Service Automation στο Finance.
- Διατηρήστε τις κατηγορίες συναλλαγών εξόδων στο Finance και συγχρονίστε τις απευθείας από το Finance στο Project Service Automation.
- Δημιουργήστε ωριαίες εκτιμήσεις έργου στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.
- Δημιουργήστε εκτιμήσεις εξόδων έργου στο Project Service Automation και συγχρονίστε τα απευθείας από το Project Service Automation στο Finance.
- Δημιουργήστε χρόνο έργου, έξοδα και πραγματικές τιμές χρεώσεων στο Project Service Automation και δημιουργήστε συναλλαγές έργου στο ημερολόγιο συναλλαγών στο Project Service Automation, ώστε να είναι δυνατή η καταχώρησή τους στο Finance.

## <a name="data-synchronization"></a>Συγχρονισμός δεδομένων

Η εικόνα που ακολουθεί δείχνει τον τρόπο με τον οποίο συγχρονίζονται τα δεδομένα στα πλαίσια της ενοποίησης μεταξύ Project Service Automation και Finance.

> [!NOTE]
> Αυτήν τη στιγμή δεν είναι διαθέσιμα όλα τα πρότυπα. Τα πρότυπα θα διατεθούν μετά την ολοκλήρωσή τους.

[![Ενοποίηση του Project Service Automation με το Finance](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>Απαιτήσεις συστήματος για το Finance

Για να χρησιμοποιήσετε τη λύση ενοποίησης του Project Service Automation με το Finance, πρέπει να εγκαταστήσετε το Enterprise Edition 7.3 με την ενημέρωση πλατφόρμας 12 ή μεταγενέστερη έκδοση.

## <a name="system-requirements-for-project-service-automation"></a>Απαιτήσεις συστήματος για το Project Service Automation

Για να χρησιμοποιήσετε τη λύση ενοποίησης του Project Service Automation με το Finance, πρέπει να εγκαταστήσετε τα ακόλουθα στοιχεία:

- Έκδοση Dynamics 365 Project Service Automation 9.0.0.0 ή νεότερη
- Λύση Prospect to cash για το Dynamics 365 Sales, έκδοση 1.14.0.0 (v14) ή νεότερη έκδοση
- Λύση Project Service Automation σε Finance για την έκδοση Dynamics 365 Project Service Automation 1.0.0.0 ή μεταγενέστερη

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Εγκατάσταση λύσης ενοποίησης του Project Service Automation με το Finance στην παρουσία Project Service Automation

Πραγματοποιήστε λήψη της λύσης ενοποίησης του Project Service Automation με το Finance από το [Κέντρο λήψης της Microsoft](https://www.microsoft.com/download/details.aspx?id=57016) και ακολουθήστε τις οδηγίες που περιλαμβάνονται με τη λύση.
