---
title: "Vorgehensweise: Übertragen von Sachposten in Kostenposten | Microsoft Docs"
description: "Sie können Sachposten in Kostenposten übertragen."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: cd52387ec1396164f6da1b87a2a97227901df592
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="0d20f-103">So übertragen Sie Sachposten in Kostenposten</span><span class="sxs-lookup"><span data-stu-id="0d20f-103">Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="0d20f-104">Sie können Sachposten in Kostenposten übertragen.</span><span class="sxs-lookup"><span data-stu-id="0d20f-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="0d20f-105">Bevor Sie den Vorgang für das Übertragen von Sachposten in Kostenposten durchführen, müssen Sie die Übertragung vorbereiten, um manuelle Korrekturbuchungen zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="0d20f-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="0d20f-106">So bereiten Sie die Übertragung vor</span><span class="sxs-lookup"><span data-stu-id="0d20f-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="0d20f-107">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Kostenrechnungseinrichtung** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="0d20f-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0d20f-108">Stellen Sie im Fenster **Kostenrechnungseinrichtung** sicher, dass im Feld **Startdatum für Sachkontenübertragung** der richtige Wert eingetragen ist.</span><span class="sxs-lookup"><span data-stu-id="0d20f-108">In the **Cost Accounting Setup** window, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="0d20f-109">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Kostenartenplan** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="0d20f-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="0d20f-110">Im Fenster **Kostenartkarte** prüfen Sie, dass das **Sachkontobereich** Feld für jede Kostenart korrekt verknüpft ist, um Posten aus dem Sachkonto zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="0d20f-110">In the **Cost Type Card** window, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="0d20f-111">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben **Kontenplan** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="0d20f-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="0d20f-112">Überprüfen Sie für jedes Sachkonto im Fenster **Sachkontokarte**, ob das **Kostenartnr.**</span><span class="sxs-lookup"><span data-stu-id="0d20f-112">For each relevant general ledger account, in the **G/L Account Card** window, verify that the **Cost Type No.**</span></span> <span data-ttu-id="0d20f-113">Feld wird korrekt zu einer Kostenart verknüpft.</span><span class="sxs-lookup"><span data-stu-id="0d20f-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="0d20f-114">Weitere Informationen finden Sie unter [Definieren der Beziehung zwischen Kostenarten und Sachkonten](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="0d20f-114">For more information, see [Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span></span>  
7.  <span data-ttu-id="0d20f-115">Vergewissern Sie sich, dass alle entsprechenden Sachposten Dimensionswerte haben, die einer Kostenstelle und zu einem Kostenträger entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0d20f-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="0d20f-116">So übertragen Sie Sachposten in Kostenposten</span><span class="sxs-lookup"><span data-stu-id="0d20f-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="0d20f-117">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben **Sachposten in Kostenrechnung übertragen** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="0d20f-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0d20f-118">Wählen Sie auf Schaltfläche **OK**, um die Umlagerung zu starten.</span><span class="sxs-lookup"><span data-stu-id="0d20f-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="0d20f-119">Der Prozess überträgt alle Sachposten, die nicht bereits übertragen wurden.</span><span class="sxs-lookup"><span data-stu-id="0d20f-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="0d20f-120">Während der Übertragung erstellt der Vorgang Verknüpfungen in den Posten **Posteneintrag** und **Kostentabelle**.</span><span class="sxs-lookup"><span data-stu-id="0d20f-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="0d20f-121">Dies ermöglicht es Ihnen, die Herkunft von Kostenposten nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="0d20f-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0d20f-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0d20f-122">See Also</span></span>  
 <span data-ttu-id="0d20f-123">[Kriterien für die Übertragung von Sachposten in Kostenposten](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0d20f-123">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="0d20f-124">[Automatische Übertragung und kombinierte Posten](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0d20f-124">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
 <span data-ttu-id="0d20f-125">[Ergebnisse der Übertragung](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="0d20f-125">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 <span data-ttu-id="0d20f-126">[Übertragung und Buchung von Kostenzuteilungen](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0d20f-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="0d20f-127">Definieren der Beziehung zwischen Kostenarten und Sachkonten</span><span class="sxs-lookup"><span data-stu-id="0d20f-127">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   
