---
title: 'Vorgehensweise: Versandagentenmethoden einrichten in | Microsoft Docs'
description: Sie können eine Code für jede einzelne angebotene Versandmethode einrichten, wie auch die Informationen dazu angeben und die Informationen dazu eingeben.e können Sie einen Code für jeden Zusteller anlegen und Informationen dazu eingeben.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 06/17/2019
ms.author: sgroespe
ms.openlocfilehash: 7248f49e92db98cec047d2035ce82d7caf84799f
ms.sourcegitcommit: 6dc83b27ac47f3b39a7b84cfb7446e7f48b8ce63
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2019
ms.locfileid: "1632783"
---
# <a name="set-up-shipment-methods"></a><span data-ttu-id="62d5f-103">Liefermethoden einrichten</span><span class="sxs-lookup"><span data-stu-id="62d5f-103">Set Up Shipment Methods</span></span>
<span data-ttu-id="62d5f-104">Versandmethoden nennt man auch Incoterms; sie hängen oft ab vom Artikel, den Debitoren und den Kreditoren</span><span class="sxs-lookup"><span data-stu-id="62d5f-104">Shipment methods, also called incoterms, often depend on the items, the customers, and the vendors.</span></span> <span data-ttu-id="62d5f-105">Wenn der Debitor beispielsweise auf einer Insel lebt, kann er entscheiden, die Artikel immer auf dem Luftweg oder immer auf dem Seeweg geliefert zu bekommen.</span><span class="sxs-lookup"><span data-stu-id="62d5f-105">For example, if the customer lives on an island, they can choose to have items always shipped by air or always by sea.</span></span> <span data-ttu-id="62d5f-106">Einige Debitoren möglicherweise eine Lieferung am nächsten Tag.</span><span class="sxs-lookup"><span data-stu-id="62d5f-106">Some customers may require next day delivery.</span></span> <span data-ttu-id="62d5f-107">Einige möchten vielleicht den Auftrag abholen.</span><span class="sxs-lookup"><span data-stu-id="62d5f-107">Some may want to pick up the order.</span></span> <span data-ttu-id="62d5f-108">Sie können auf den Debitoren- und Kreditorenkarten angeben, welche Lieferart gewünscht ist.</span><span class="sxs-lookup"><span data-stu-id="62d5f-108">On the customer and vendor cards, you can specify what sort of delivery is desired.</span></span>

<span data-ttu-id="62d5f-109">In der Tabelle **Lieferbedingung** richten Sie die Beschreibung und den Code für jede Lieferbedingung ein.</span><span class="sxs-lookup"><span data-stu-id="62d5f-109">You set up the description and code for each shipment method on the **Shipment Methods** page.</span></span> <span data-ttu-id="62d5f-110">Sie können z. B. den Code "FOB" einrichten und im Feld **Beschreibung** können Sie "Frei an Bord" eingeben.</span><span class="sxs-lookup"><span data-stu-id="62d5f-110">For example, you can set up the code FOB, and enter Free on Board in the **Description** field.</span></span> <span data-ttu-id="62d5f-111">Sie können dann den Code im Feld **Versandmethodencode** an anderer Stelle in der Anwendung eingeben, z. B. auf der Debitorenkarte.</span><span class="sxs-lookup"><span data-stu-id="62d5f-111">You can then enter the code in **Shipment Method Code** fields elsewhere in the system, such as on a customer card.</span></span> <span data-ttu-id="62d5f-112">Wenn Sie dann neue Aufträge, Bestellungen, Rechnungen oder Gutschriften erstellen oder buchen, wird das System die Beschreibung einfügen, die zu dem Code gehört.</span><span class="sxs-lookup"><span data-stu-id="62d5f-112">Then when you create new orders, invoices, credit memos, and so on, the system will enter the description represented by the code.</span></span> <span data-ttu-id="62d5f-113">Sie können die Standardbeträge auf dem Beleg je nach Anforderung ändern.</span><span class="sxs-lookup"><span data-stu-id="62d5f-113">You can change it on the document as needed.</span></span>

## <a name="to-set-up-a-shipment-code"></a><span data-ttu-id="62d5f-114">So richten Sie einen Verandcode ein</span><span class="sxs-lookup"><span data-stu-id="62d5f-114">To set up a shipment code</span></span>
1. <span data-ttu-id="62d5f-115">Wählen Sie das Symbol ![Glühlampe, mit der die Funktion „Wie möchten Sie weiter verfahren“ geöffnet wird](media/ui-search/search_small.png "Wie möchten Sie weiter verfahren?") aus, geben Sie **Versandmethode** ein, und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="62d5f-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="62d5f-116">Wählen Sie auf der Seite **Versandmethode** die Aktion **Neu** aus.</span><span class="sxs-lookup"><span data-stu-id="62d5f-116">On the **Shipment Methods** page, choose the **New** action.</span></span>
3. <span data-ttu-id="62d5f-117">Geben Sie in der neuen Zeile einen Code und eine Beschreibung für die Lieferbedingung an.</span><span class="sxs-lookup"><span data-stu-id="62d5f-117">On the new line, specify a code and description for the shipment method.</span></span>

## <a name="see-also"></a><span data-ttu-id="62d5f-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="62d5f-118">See Also</span></span>
[<span data-ttu-id="62d5f-119">Incoterms</span><span class="sxs-lookup"><span data-stu-id="62d5f-119">Incoterms</span></span>](https://iccwbo.org/resources-for-business/incoterms-rules)  
[<span data-ttu-id="62d5f-120">Zusteller einrichten</span><span class="sxs-lookup"><span data-stu-id="62d5f-120">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)  
<span data-ttu-id="62d5f-121">[Um Pakete zu verfolgen](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="62d5f-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="62d5f-122">Logistik</span><span class="sxs-lookup"><span data-stu-id="62d5f-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="62d5f-123">Lagerbestand</span><span class="sxs-lookup"><span data-stu-id="62d5f-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="62d5f-124">[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="62d5f-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="62d5f-125">[Montageverwaltung](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="62d5f-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="62d5f-126">Designdetails: Logistik</span><span class="sxs-lookup"><span data-stu-id="62d5f-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="62d5f-127">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="62d5f-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  