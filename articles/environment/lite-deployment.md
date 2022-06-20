---
title: Ανάπτυξη Project Operations - lite
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τον τρόπο εγκατάστασης ελαφριάς ανάπτυξης του Project Operations ‑ συμφωνία για προτιμολόγηση.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 86293b725e86db3d4b8bdaf5810b16b7c670e8a3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930318"
---
# <a name="deploy-project-operations---lite"></a>Ανάπτυξη Project Operations - lite

_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_



Το Project Operations υποστηρίζει πολλαπλά μοντέλα ανάπτυξης. Για να προσδιορίσετε το μοντέλο καλύτερης ανάπτυξης, ανατρέξτε στο θέμα [Τύποι ανάπτυξης](determine-deployment-type.md).


> [!IMPORTANT]
> Αυτή η ανάπτυξη, η ελαφριά ανάπτυξη – συμφωνία για προτιμολόγηση, έχει ως αποτέλεσμα μια **Dataverse-μόνο ανάπτυξη του Project Operations**.

- [Εγκατάσταση του Project Operations σε νέο περιβάλλον Dataverse](#new)
- [Εγκατάσταση σε υπάρχον περιβάλλον Dataverse](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>Εγκατάσταση του Project Operations σε νέο περιβάλλον Dataverse

1. Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, δημιουργήστε ένα νέο περιβάλλον Dataverse στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com). Βεβαιωθείτε ότι είναι ενεργοποιημένη **η δημιουργία βάσης δεδομένων για αυτό το περιβάλλον** και **εφαρμογές Dynamics 365**. Για περισσότερες πληροφορίες σχετικά με τα περιβάλλοντα παροχής, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση περιβαλλόντων στο κέντρο διαχείρισης του Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Επιλέξτε **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>Εγκατάσταση του Project Operations σε υφιστάμενο περιβάλλον Dataverse
1. Βεβαιωθείτε ότι το περιβάλλον δεν έχει ρυθμιστεί με δυνατότητα [διπλής εγγραφής](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) καθώς η εγκατάσταση θα εγκαταστήσει τότε τις δυνατότητες [Project Operations για σενάρια βάσει πόρου/μη εφοδιασμένα](project-operations-integrated-deployment-overview.md).
2. Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, εντοπίστε το περιβάλλον στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com) στο οποίο θέλετε να εγκαταστήσετε το Project Operations.
3. Εγκαταστήστε το **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365. Για περισσότερες πληροφορίες, ανατρέξτε στη [Διαχείριση εφαρμογών Dynamics 365](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
