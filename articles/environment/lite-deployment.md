---
title: Ανάπτυξη Project Operations Lite
description: Αυτό το άρθρο παρέχει πληροφορίες σχετικά με τον τρόπο εγκατάστασης ελαφριάς ανάπτυξης του Project Operations ‑ συμφωνία για προτιμολόγηση.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810978"
---
# <a name="deploy-project-operations-lite"></a>Ανάπτυξη Project Operations Lite

_**Ισχύει για:** Ελαφριά ανάπτυξη - συμφωνία για προτιμολόγηση_



Το Project Operations υποστηρίζει πολλαπλά μοντέλα ανάπτυξης. Για να προσδιορίσετε το μοντέλο καλύτερης ανάπτυξης, ανατρέξτε στο θέμα [Τύποι ανάπτυξης](determine-deployment-type.md).


> [!IMPORTANT]
> Αυτή η ανάπτυξη, η ελαφριά ανάπτυξη – συμφωνία για προτιμολόγηση, έχει ως αποτέλεσμα μια **Dataverse-μόνο ανάπτυξη του Project Operations**.

- [Εγκατάσταση του Project Operations σε νέο περιβάλλον Dataverse](#new)
- [Εγκατάσταση σε υπάρχον περιβάλλον Dataverse](#existing)
- [Εγκατάσταση σε ένα υπάρχον περιβάλλον Dataverse το οποίο διαθέτει στοιχεία διπλής εγγραφής](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a>Εγκατάσταση του Project Operations Lite σε νέο περιβάλλον Dataverse

1. Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, δημιουργήστε ένα νέο περιβάλλον Dataverse στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com). Βεβαιωθείτε ότι είναι ενεργοποιημένη **η δημιουργία βάσης δεδομένων για αυτό το περιβάλλον** και **εφαρμογές Dynamics 365**. Για περισσότερες πληροφορίες σχετικά με τα περιβάλλοντα παροχής, ανατρέξτε στο θέμα [Δημιουργία και διαχείριση περιβαλλόντων στο κέντρο διαχείρισης του Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. Επιλέξτε **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a>Εγκατάσταση του Project Operations Lite σε υφιστάμενο περιβάλλον Dataverse 
1. Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, εντοπίστε το περιβάλλον στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com) στο οποίο θέλετε να εγκαταστήσετε το Project Operations.
1. Εγκαταστήστε το **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365. Για περισσότερες πληροφορίες, ανατρέξτε στη [Διαχείριση εφαρμογών Dynamics 365](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a>Εγκατάσταση του Project Operations Lite σε ένα υπάρχον περιβάλλον Dataverse, όπου υπάρχουν ήδη λύσεις διπλής εγγραφής

Εάν θέλετε να συνεχίσετε να εκτελείτε το Project Operations σε λειτουργία ανάπτυξης lite, θα πρέπει να ακολουθήσετε τα παρακάτω βήματα:

1. Ως [Καθολικός διαχειριστής ή Διαχειριστής του Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) με άδεια Project Operations, εντοπίστε το περιβάλλον στο [Κέντρο διαχείρισης PowerPlatform](https://admin.powerplatform.com) στο οποίο θέλετε να εγκαταστήσετε το Project Operations.
1. Εγκαταστήστε το **Microsoft Dynamics 365 Project Operations** από τη λίστα ανάπτυξης των εφαρμογών Dynamics 365. Για περισσότερες πληροφορίες, ανατρέξτε στη [Διαχείριση εφαρμογών Dynamics 365](/power-platform/admin/manage-apps).
1. Επειδή το περιβάλλον σας διαθέτει στοιχεία διπλής εγγραφής που βοηθούν με την ενοποίηση σε εγκατεστημένες εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων, η εγκατάσταση του Project Operations θα εγκαταστήσει επίσης τις δυνατότητες και τις επεκτάσεις που απαιτούνται για την ενσωμάτωση δεδομένων που σχετίζονται με ένα έργο σε εφαρμογές οικονομικών και επιχειρηματικών δραστηριοτήτων. Επειδή θέλετε να εκτελέσετε το Project Operations σε ελαφριά ανάπτυξη, αυτά τα στοιχεία ενοποίησης θα πρέπει να καταργηθούν, καθώς θα δημιουργήσουν περιορισμούς και υπέρβαση ορίων για σενάρια ελαφριάς ανάπτυξης. Καταργήστε με μη αυτόματο τρόπο την εγκατάσταση των λύσεων **Dynamics 365 Project Operations διπλής εγγραφής** και **Χάρτες οντοτήτων διπλής εγγραφής Dynamics 365 Project Operations** για την κατάργηση αυτών των στοιχείων.
1. Μεταβείτε στο **Project Operations -> Ρυθμίσεις -> Παράμετροι**. Ανοίξτε τη σελίδα λεπτομερειών **Παράμετροι έργου** και ορίστε το πεδίο **Συμπεριφορά αναβάθμισης λύσης** σε **Μόνο ελαφριά**. Με αυτόν τον τρόπο εξασφαλίζεται ότι τυχόν επόμενες αναβαθμίσεις του Project Operations δεν θα επαναφέρουν τα στοιχεία ενοποίησης στο Project Operations.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
