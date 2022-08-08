---
title: Παραγγελία μη εφοδιασμένων υλικών για ένα έργο με χρήση παραγγελιών αγοράς έργου
description: Αυτό το άρθρο εξηγεί τον τρόπο παραγγελίας μη εφοδιασμένων υλικών για ένα έργο με χρήση εντολών αγοράς έργου.
author: sigitac
ms.date: 09/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: fe24faa143869af2396f3b0f28aae31417cadda7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929812"
---
# <a name="order-procurement-categories-or-non-stocked-materials-for-a-project-using-project-purchase-orders"></a>Κατηγορίες προμήθειεας εντολών ή μη εφοδιασμένα υλικά για ένα έργο με χρήση εντολών αγοράς έργου

_**Ισχύει για:** Project Operations για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα_

Το τμήμα Προμηθειών του οργανισμού σας ενδέχεται να χρησιμοποιεί [παραγγελίες αγοράς](/dynamics365/supply-chain/procurement/purchase-order-overview) για την παρακολούθηση παραγγελιών αγαθών και υπηρεσιών. Οι εντολές αγοράς για κατηγορίες προμήθειεας ή μη εφοδιασμένα υλικά μπορούν να αποδοθούν σε ένα έργο. Η τιμολόγηση αυτών των παραγγελιών αγοράς καταγράφει το κόστος για το έργο.

## <a name="prerequisites"></a>Προϋποθέσεις
Ολοκληρώστε τα παρακάτω βήματα για να ενεργοποιήσετε τη λειτουργία παραγγελιών αγοράς έργου.

1. Στο Dynamics 365 Finance, μεταβείτε στον χώρο εργασίας **Διαχείριση δυνατοτήτων**.
2. Στη λίστα δυνατοτήτων, εντοπίστε και επιλέξτε τη δυνατότητα **Ενεργοποιήστε παραγγελίες αγοράς έργου στο Project Operations για σενάρια που βασίζονται σε πόρους/μη αποθέματος**.
3. Επιλέξτε **Ενεργοποίηση**.
4. Ρυθμίστε τις παραμέτρους μη εφοδιασμένων υλικών και εκκρεμών τιμολογίων προμηθευτών, όπως περιγράφεται στην ενότητα [Ρύθμιση παραμέτρων μη αποθέματος και εκκρεμών τιμολογίων προμηθευτή](configure-materials-nonstocked.md).
5. Ρύθμιση παραμέτρων κατηγοριών όπως περιγράφεται στο [Χρησιμοποιήστε κατηγορίες προμήθειεας με εντολές αγοράς έργου και εκκρεμή τιμολόγια προμηθευτών](configure-procurement-categories.md).

## <a name="create-a-project-purchase-order-from-the-project-purchase-order-list"></a>Δημιουργία παραγγελίας αγοράς έργου από τη λίστα παραγγελιών προμήθειας έργου

1. Στα Οικονομικά, μεταβείτε στην επιλογή **Διαχείριση έργων και λογιστική** > **Έργα** > **Όλα τα έργα** και επιλέξτε ένα έργο.
2. Στο παράθυρο ενεργειών, στην καρτέλα **Διαχείριση**, στην ομάδα **Δημιουργία**, επιλέξτε **Εργασία στοιχείου** > **Παραγγελία αγοράς**.
3. Στη σελίδα **Δημιουργία παραγγελίας αγοράς**, επιλέξτε τον προμηθευτή στον οποίο θέλετε να δώσετε την παραγγελία προμήθειας, εισαγάγετε άλλες πληροφορίες, ανάλογα με την περίπτωση και, στη συνέχεια, επιλέξτε **OK**.
4. Στη σελίδα **Παραγγελία αγοράς**, στο πλέγμα **γραμμές παραγγελίας αγοράς**, επιλέξτε **Προσθήκη γραμμής**.
5. Εισαγάγετε έναν αριθμό στοιχείου ή κατηγορία προμήθειας, μια ποσότητα, μια μονάδα, μια τιμή μονάδας και άλλες πληροφορίες, ανάλογα με την περίπτωση.

    > [!NOTE]
    > Μόνο κατηγορίες προμήθειας, μη εφοδιασμένα στοιχεία και υπηρεσίες μπορούν να χρησιμοποιηθούν με παραγγελίες προμήθειας έργου. Τα στοιχεία αποθέματος δεν υποστηρίζονται.

6. Συνεχίστε να προσθέτετε στοιχεία ή κατηγορίες προμήθειας όπως απαιτείται και επιβεβαιώστε την παραγγελία αγοράς.

    Οι αποδείξεις αγαθών και υπηρεσιών μπορούν να καταχωρούνται με τη δημιουργία και την καταχώρηση μιας απόδειξης προϊόντος.

    > [!NOTE]
    > Οι παραλαβές προϊόντων δεν καταγράφονται στις πραγματικές τιμές του έργου στο Microsoft Dataverse και δεν επηρεάζουν το δευτερεύον καθολικό έργου.

    Αφού ένας πωλητής στείλει το τιμολόγιο για στοιχεία και υπηρεσίες στην παραγγελία αγοράς, το τμήμα υποστήριξης πωλήσεων μπορεί να δημιουργήσει ένα τιμολόγιο για την παραγγελία αγοράς, πηγαίνει στην επιλογή **Τιμολόγιο** > **Δημιουργία** > **Τιμολόγιο** στο Παράθυρο ενεργειών. Για περισσότερες πληροφορίες σχετικά με τα εκκρεμή τιμολόγια προμηθευτών, ανατρέξτε στο θέμα [Αγορά μη αποθέματος υλικού χρησιμοποιώντας ένα εκκρεμές τιμολόγιο προμηθευτή](pending-vendor-invoices.md).