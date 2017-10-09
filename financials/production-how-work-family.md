---
title: 'Vorgehensweise: Artikel-Familien in der Produktion verwenden | Microsoft Docs'
description: "Die Hauptaufgabe beim Anpassen eines Basiskalenders für Ihre Firma oder einen Ihrer Geschäftspartner ist, alle Änderungen am Status der Daten als freie Tage oder Arbeitstage einzugeben."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/05/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 060c58991ae48ba768f5c1c0bd7442228e6bc976
ms.contentlocale: de-de
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-production-families"></a><span data-ttu-id="d77a5-103">Vorgehensweise: Arbeiten mit Fertigungsfamilien</span><span class="sxs-lookup"><span data-stu-id="d77a5-103">How to: Work with Production Families</span></span>
<span data-ttu-id="d77a5-104">Eine Fertigungsfamilie ist eine Gruppe einzelner Artikel, deren Zusammenhang in der Ähnlichkeit ihres Fertigungsprozesses liegt.</span><span class="sxs-lookup"><span data-stu-id="d77a5-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span></span> <span data-ttu-id="d77a5-105">Wenn Sie Fertigungsfamilien zusammenstellen, können einzelne Artikel mehrfach, in einem Arbeitsschritt, gefertigt werden, womit Sie den Materialverbrauch optimieren können.</span><span class="sxs-lookup"><span data-stu-id="d77a5-105">By forming production families, some items can be manufactured twice or more in one production, which will optimize material consumption.</span></span>

<span data-ttu-id="d77a5-106">Geben Sie im **Menge**-Feld im **Familien**-Fenster die Menge ein, die gefertigt werden soll, wenn die gesamte Fertigungsfamilie einmal gefertigt wird.</span><span class="sxs-lookup"><span data-stu-id="d77a5-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span></span>

## <a name="example"></a><span data-ttu-id="d77a5-107">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d77a5-107">Example</span></span>
<span data-ttu-id="d77a5-108">Beim Stanzen können vier Teile eines Artikels und 10 Teile eines anderen Artikels aus einem Blech zur gleichen Zeit gestanzt werden.</span><span class="sxs-lookup"><span data-stu-id="d77a5-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span></span> <span data-ttu-id="d77a5-109">Die Stanzmaschine stanzt die kompletten 14 Teile in einem Arbeitsschritt.</span><span class="sxs-lookup"><span data-stu-id="d77a5-109">The punching machine will punch all 14 pieces in one step.</span></span>

<span data-ttu-id="d77a5-110">Fertigungsfamilien verringern die Ausschussmenge, da der normalerweise bei der Fertigung großer Teile entstehende Ausschuss zur Fertigung kleiner Teile verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d77a5-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span></span>

## <a name="to-set-up-a-production-family"></a><span data-ttu-id="d77a5-111">Fertigungsfamilien einrichten</span><span class="sxs-lookup"><span data-stu-id="d77a5-111">To set up a production family</span></span>
1. <span data-ttu-id="d77a5-112">Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **Familien** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d77a5-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span></span>
2. <span data-ttu-id="d77a5-113">Füllen Sie die Felder je nach Bedarf aus.</span><span class="sxs-lookup"><span data-stu-id="d77a5-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a><span data-ttu-id="d77a5-114">Um auf Grundlage eine Produktion familily erzeugen</span><span class="sxs-lookup"><span data-stu-id="d77a5-114">To produce based on a production familily</span></span>
1. <span data-ttu-id="d77a5-115">Wählen Sie ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol nach Seite oder Bericht suchen ") aus und geben Sie **Feste Auftragsplanung** ein. Wählen Sie dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="d77a5-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="d77a5-116">Dient zum Erstellen eines neuen Produktionsauftrags.</span><span class="sxs-lookup"><span data-stu-id="d77a5-116">Create a new production order.</span></span> <span data-ttu-id="d77a5-117">Weitere Informationen finden Sie unter [Gewusst wie: Erstellen von Montageaufträgen](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="d77a5-117">For more information, see [How to: Create Production orders](production-how-to-create-production-orders.md).</span></span>
3. <span data-ttu-id="d77a5-118">Wählen Sie im Feld **Quelltyp** **Familie** aus.</span><span class="sxs-lookup"><span data-stu-id="d77a5-118">In the **Source Type** field, select **Family**.</span></span>  
4. <span data-ttu-id="d77a5-119">Wählen Sie im Feld **Quelle** die entsprechende Produktionsfamilien aus.</span><span class="sxs-lookup"><span data-stu-id="d77a5-119">In the **Source No.** field, select the relevant production family.</span></span>

## <a name="see-also"></a><span data-ttu-id="d77a5-120">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d77a5-120">See Also</span></span>
[<span data-ttu-id="d77a5-121">So wird's gemacht: Neue Fertigungsstücklisten erzeugen</span><span class="sxs-lookup"><span data-stu-id="d77a5-121">How to: Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="d77a5-122">Produktion einrichten</span><span class="sxs-lookup"><span data-stu-id="d77a5-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="d77a5-123">[Produktion](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="d77a5-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="d77a5-124">[Planung](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="d77a5-124">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="d77a5-125">Lagerbest</span><span class="sxs-lookup"><span data-stu-id="d77a5-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="d77a5-126">Einkauf</span><span class="sxs-lookup"><span data-stu-id="d77a5-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="d77a5-127">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d77a5-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
