---
title: Σημειώσεις προγραμματιστή για εγκρίσεις
description: Αυτό το θέμα παρέχει πρόσθετες πληροφορίες προγραμματιστή σχετικά με την εργασία με εγκρίσεις.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483948"
---
# <a name="developer-notes-for-approvals"></a>Σημειώσεις προγραμματιστή για εγκρίσεις

_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_

Το Dynamics 365 Project Operations περιλαμβάνει λογική επικύρωσης που διασφαλίζει τη σωστή μετάβαση καρτέλας μέσω των σταδίων έγκρισης. Οι σωστές μεταβάσεις καρτελών εξασφαλίζουν τα εξής: 

  - Όλες οι γραμμές υποστήριξης δημιουργούνται σε σχετιζόμενους πίνακες, όπως τα ημερολόγια και οι πραγματικές τιμές.
  - Ο υπεύθυνος έγκρισης επισημαίνεται ως **Υπεύθυνος έγκρισης έργου** στο έργο πριν προχωρήσετε.
