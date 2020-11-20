---
title: Παράκαμψη τιμοκαταλόγων πωλήσεων έργου
description: Αυτό το θέμα παρέχει πληροφορίες σχετικά με τη δημιουργία προσαρμοσμένων τιμοκαταλόγων πωλήσεων.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c97dca8685c2db7d256017cf4442416feb0e005b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130848"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="57010-103">Παράκαμψη τιμοκαταλόγων πωλήσεων έργου</span><span class="sxs-lookup"><span data-stu-id="57010-103">Override project sales price lists</span></span>

<span data-ttu-id="57010-104">_**Ισχύει για:** Εργασίες έργου για σενάρια βασισμένα σε πόρους/μη εφοδιασμένα, ανάπτυξη Lite - συμφωνία για προτιμολόγηση_</span><span class="sxs-lookup"><span data-stu-id="57010-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="57010-105">Τιμοκατάλογοι έργου συγκεκριμένου πελάτη</span><span class="sxs-lookup"><span data-stu-id="57010-105">Customer-specific project price lists</span></span>

<span data-ttu-id="57010-106">Οι συμφωνίες τιμών για συγκεκριμένους πελάτες μπορούν να ρυθμιστούν ως τιμοκατάλογοι έργου σε μια καρτέλα λογαριασμού στο Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="57010-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="57010-107">Για να ορίσετε έναν τιμοκατάλογο έργου για συγκεκριμένο πελάτη, στην περιοχή **Πωλήσεις**, μεταβείτε στην καρτέλα λογαριασμού.</span><span class="sxs-lookup"><span data-stu-id="57010-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="57010-108">Ανοίξτε τη σελίδα λίστας **Λογαριασμοί**.</span><span class="sxs-lookup"><span data-stu-id="57010-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="57010-109">Εντοπίστε και κάντε διπλό κλικ σε μια καρτέλα πελάτη για να ανοίξετε τη σελίδα λεπτομερειών **Λογαριασμός**.</span><span class="sxs-lookup"><span data-stu-id="57010-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="57010-110">Στην καρτέλα **Τιμοκατάλογοι έργου**, επιλέξτε \*\*+ Τιμοκατάλογος νέου έργου^^.</span><span class="sxs-lookup"><span data-stu-id="57010-110">On the **Project Price lists** tab, select \*\*+ New Project Price List^^.</span></span>
4. <span data-ttu-id="57010-111">Στη σελίδα **Τιμοκατάλογοι νέου έργου**, επιλέξτε έναν τιμοκατάλογο από το αναπτυσσόμενο μενού.</span><span class="sxs-lookup"><span data-stu-id="57010-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="57010-112">Περιλαμβάνονται μόνο οι τιμοκατάλογοι που έχουν το περιβάλλον ρυθμισμένο σε **Πωλήσεις** και των οποίων το νόμισμα ταιριάζει με το νόμισμα του λογαριασμού.</span><span class="sxs-lookup"><span data-stu-id="57010-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="57010-113">Δώστε όνομα στη συσχέτιση και επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="57010-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="57010-114">Δημιουργείται ένας τιμοκατάλογος έργου συγκεκριμένου πελάτη.</span><span class="sxs-lookup"><span data-stu-id="57010-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="57010-115">Αυτός ο τιμοκατάλογος θα χρησιμοποιηθεί για την προεπιλογή των τιμών έργου σε προσφορές έργων ή συμβάσεις που δημιουργούνται για αυτόν τον πελάτη, όπου η ημερομηνία δημιουργίας της προσφοράς ή της σύμβασης έργου εμπίπτει στην ημερομηνία ισχύος του τιμοκαταλόγου.</span><span class="sxs-lookup"><span data-stu-id="57010-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="57010-116">Προσαρμοσμένη τιμολόγηση σε προσφορές έργων</span><span class="sxs-lookup"><span data-stu-id="57010-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="57010-117">Στις προσφορές έργου, μπορείτε να έχετε τιμολόγηση έργου που ξεκινά με έναν προεπιλεγμένο τυπικό τιμοκατάλογο που αφορά τις προεπιλογές από τον πελάτη ή από τις παραμέτρους του έργου.</span><span class="sxs-lookup"><span data-stu-id="57010-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="57010-118">Όταν χρειάζεστε προσαρμοσμένη τιμολόγηση για εργασία που σχετίζεται με το έργο σε μια συγκεκριμένη προσφορά, μπορείτε να την λάβετε από τη συσχετισμένη οντότητα των τιμοκαταλόγων έργου.</span><span class="sxs-lookup"><span data-stu-id="57010-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="57010-119">Ολοκληρώστε τα παρακάτω βήματα για να ορίσετε την τιμολόγηση έργου για συγκεκριμένες τιμές προσφοράς.</span><span class="sxs-lookup"><span data-stu-id="57010-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="57010-120">Ανοίξτε την προσφορά έργου και επιλέξτε την καρτέλα **Τιμοκατάλογοι έργου**.</span><span class="sxs-lookup"><span data-stu-id="57010-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="57010-121">Στο υποπλέγμα επιλέξτε **Δημιουργία προσαρμοσμένης τιμολόγησης**.</span><span class="sxs-lookup"><span data-stu-id="57010-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="57010-122">Όλοι οι τιμοκατάλογοι έργου που επισυνάπτονται στην προσφορά αντιγράφονται σε νέους τιμοκαταλόγους.</span><span class="sxs-lookup"><span data-stu-id="57010-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="57010-123">Τα ονόματα των νέων τιμοκαταλόγων αντικατοπτρίζουν το όνομα της προσφοράς με μια σήμανση ημερομηνίας-ώρας για τη δημιουργία αυτών των τιμοκαταλόγων.</span><span class="sxs-lookup"><span data-stu-id="57010-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="57010-124">Μπορείτε να χρησιμοποιήσετε κάθε έναν από αυτούς τους τιμοκαταλόγους και να κάνετε ενημερώσεις για τις τιμές εργασίας (τιμή ρόλου) και εξόδων (τιμή κατηγορίας).</span><span class="sxs-lookup"><span data-stu-id="57010-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="57010-125">Αυτές οι τιμές θα ισχύσουν μόνο για αυτήν την προσφορά έργου.</span><span class="sxs-lookup"><span data-stu-id="57010-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="57010-126">Τιμοκατάλογοι σε σύμβαση έργου</span><span class="sxs-lookup"><span data-stu-id="57010-126">Price lists on a project contract</span></span>

<span data-ttu-id="57010-127">Σε μια σύμβαση έργου, η τιμολόγηση έργου είναι πάντα προεπιλεγμένη ως προσαρμοσμένος τιμοκατάλογος με το όνομα της σύμβασης και τη σήμανση ημερομηνίας που δημιουργήθηκε να είναι προσαρτημένη στο όνομα.</span><span class="sxs-lookup"><span data-stu-id="57010-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="57010-128">Αυτό ισχύει αν η σύμβαση δημιουργήθηκε όταν κερδήθηκε η προσφορά ή αν το συμβόλαιο δημιουργήθηκε από την αρχή.</span><span class="sxs-lookup"><span data-stu-id="57010-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="57010-129">Εάν είναι απαραίτητο, μπορείτε να καταργήσετε αυτήν τη συσχέτιση στον προσαρμοσμένο τιμοκατάλογο και να συσχετίσετε έναν τυπικό τιμοκατάλογο με τη σύμβαση έργου.</span><span class="sxs-lookup"><span data-stu-id="57010-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="57010-130">Όταν συσχετίζετε έναν τυπικό τιμοκατάλογο με τους τιμοκαταλόγους έργου σε προσφορά ή συμβόλαιο, οποιεσδήποτε αλλαγές γίνονται στις τιμές στον τιμοκατάλογο θα επηρεάσουν όλες τις προσφορές και τις συμβάσεις που χρησιμοποιούν τον τιμοκατάλογο.</span><span class="sxs-lookup"><span data-stu-id="57010-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>
