---
title: "Ausführen der Produktion aus | Microsoft Docs"
description: "Nach der Ausgabe des Materials kann mit den eigentlichen Fertigungsarbeitsgängen begonnen werden. Diese können dann in der Reihenfolge ausgeführt werden, die im FA-Arbeitsplan definiert ist."
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
ms.openlocfilehash: 61c89c50b549a802df1973538edb83d3baf328e4
ms.contentlocale: de-de
ms.lasthandoff: 09/22/2017

---
# <a name="manufacturing"></a><span data-ttu-id="288a5-103">Produktion</span><span class="sxs-lookup"><span data-stu-id="288a5-103">Manufacturing</span></span>
<span data-ttu-id="288a5-104">Nach der Ausgabe des Materials kann mit den eigentlichen Fertigungsarbeitsgängen begonnen werden. Diese können dann in der Reihenfolge ausgeführt werden, die im FA-Arbeitsplan definiert ist.</span><span class="sxs-lookup"><span data-stu-id="288a5-104">When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.</span></span>  

<span data-ttu-id="288a5-105">Ein aus Systemsicht wichtiger Aspekt beim Ausführen der Produktion ist das Buchen der Istmeldung in die Datenbank, um den Status zu melden, sowie das Aktualisieren des Lagerbestands mit den fertig gestellten Artikeln.</span><span class="sxs-lookup"><span data-stu-id="288a5-105">An important part of executing production, from a system point of view, is to post production output to the database to report progress and to update inventory with the finished items.</span></span> <span data-ttu-id="288a5-106">Istmeldungsbuchungen können manuell, also durch Ausfüllen und Buchen von Buch.-Blattzeilen nach Ausführen von Fertigungsarbeitsgängen, vorgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="288a5-106">Output posting can be done manually, by filling and posting journal lines after production operations.</span></span> <span data-ttu-id="288a5-107">Alternativ können die Buchungen auch mithilfe der Buchungsmethode "Rückwärts" gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="288a5-107">Or, it can be done automatically with the use of backward flushing.</span></span> <span data-ttu-id="288a5-108">In diesem Fall wird der Materialverbrauch automatisch zusammen mit der Istmeldung gebucht, wenn der Status des Fertigungsauftrags zu "Beendet" geändert wird.</span><span class="sxs-lookup"><span data-stu-id="288a5-108">In that case material consumption is automatically posted along with output when the production order changes to finished.</span></span>  

<span data-ttu-id="288a5-109">Als Alternative zum Stapelbuchungsblatt für die Istmeldungsbuchung mehrerer Fertigungsaufträge können Sie das Fenster **Produktions Buch.-Blatt** verwenden, um Verbrauch und/oder Istmeldung für eine Fertigungsauftragszeile zu buchen.</span><span class="sxs-lookup"><span data-stu-id="288a5-109">As an alternative to the batch journal for output posting for multiple production orders, you can use the **Production Journal** window to post consumption and/or output for one production order line.</span></span>  

<span data-ttu-id="288a5-110">Die folgende Tabelle enthält eine Abfolge von Aufgaben sowie Links zu den entsprechenden Themen, in denen diese Aufgaben erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="288a5-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="288a5-111">**Aufgabe**</span><span class="sxs-lookup"><span data-stu-id="288a5-111">**To**</span></span>|<span data-ttu-id="288a5-112">**Siehe**</span><span class="sxs-lookup"><span data-stu-id="288a5-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="288a5-113">Verstehen Sie, wie Fertigungsaufträge arbeiten.</span><span class="sxs-lookup"><span data-stu-id="288a5-113">Understand how production orders work.</span></span>|[<span data-ttu-id="288a5-114">Info zu Fertigungsaufträgen</span><span class="sxs-lookup"><span data-stu-id="288a5-114">About Production Orders</span></span>](production-about-production-orders.md)|
|<span data-ttu-id="288a5-115">Manuelles Erstellen von Produktionsaufträgen.</span><span class="sxs-lookup"><span data-stu-id="288a5-115">Create production orders manually.</span></span>|[<span data-ttu-id="288a5-116">Vorgehensweise: Fertigungsaufträge erstellen:</span><span class="sxs-lookup"><span data-stu-id="288a5-116">How to: Create Production Orders</span></span>](production-how-to-create-production-orders.md)|
|<span data-ttu-id="288a5-117">Lagern Sie alle oder ausgewählte Arbeitsgänge im Fertigungsauftrag an einen Subunternehmer aus.</span><span class="sxs-lookup"><span data-stu-id="288a5-117">Outsource all or selected operations in a production order to a subcontractor.</span></span>|[<span data-ttu-id="288a5-118">Vorgehensweise: Nebenvertrag-Fertigung</span><span class="sxs-lookup"><span data-stu-id="288a5-118">How to: Subcontract Manufacturing</span></span>](production-how-to-subcontract-manufacturing.md)|
|<span data-ttu-id="288a5-119">Erfassen und Buchen der fertig gestellten Menge – zusammen mit Materialverbrauch und Zeitaufwand – für eine einzelne freigegebene Fertigungsauftragszeile.</span><span class="sxs-lookup"><span data-stu-id="288a5-119">Record and post production output along with material and time consumption for a single released production order line.</span></span>|[<span data-ttu-id="288a5-120">Vorgehensweise: Gemeinsames Erfassen und Buchen von Verbrauch und Istmeldungen für eine einzelne freigegebene Fertigungsauftragszeile</span><span class="sxs-lookup"><span data-stu-id="288a5-120">How to: Post Consumption and Output for One Released Production Order Line</span></span>](production-how-to-register-consumption-and-output.md)|  
|<span data-ttu-id="288a5-121">Stapelbuchung der Komponenten pro Arbeitsgang in einem Buch.-Blatt, die verschiedene  Fertigungsaufträge verarbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="288a5-121">Batch post the quantity of components used per operation in a journal that can processes multiple planned production orders.</span></span>|[<span data-ttu-id="288a5-122">So wird's gemacht: Verbrauch mit Stapelverarbeitung buchen</span><span class="sxs-lookup"><span data-stu-id="288a5-122">How to: Batch Post Consumption</span></span>](production-how-to-post-consumption.md)|
|<span data-ttu-id="288a5-123">Stapelbuchung der Komponenten pro Arbeitsgang in einem Buch.-Blatt, die verschiedene  Fertigungsaufträge verarbeiten kann, buchen.</span><span class="sxs-lookup"><span data-stu-id="288a5-123">Post the quantity of finished items and the time spent per operation in a journal that can processes multiple released production orders.</span></span>|[<span data-ttu-id="288a5-124">Vorgehensweise: Ausgabe über Stapelverarbeitung buchen und Bearbeitungszeiten prüfen</span><span class="sxs-lookup"><span data-stu-id="288a5-124">How to: Batch Post Output and Run Times</span></span>](production-how-to-post-output-quantity.md)|  
|<span data-ttu-id="288a5-125">Buchen der Anzahl von Artikeln, die in den einzelnen abgeschlossenen Arbeitsgängen gefertigt wurden und nicht als fertig gestellte Menge, sondern als Ausschussmaterial betrachtet werden</span><span class="sxs-lookup"><span data-stu-id="288a5-125">Post the number of items produced in each finished operation which do not qualify as finished output, but as scrapped material.</span></span>|[<span data-ttu-id="288a5-126">Vorgehensweise:  Ausschuss buchen:</span><span class="sxs-lookup"><span data-stu-id="288a5-126">How to: Post Scrap</span></span>](production-how-to-post-scrap.md)|
|<span data-ttu-id="288a5-127">Anzeigen der Fertigungsbereichsauslastung aufgrund geplanter und freigegebener Fertigungsaufträge.</span><span class="sxs-lookup"><span data-stu-id="288a5-127">View the shop floor load as a result of planned and released production orders.</span></span>|[<span data-ttu-id="288a5-128">Vorgehensweise: Anzeigen der Auslastung der Arbeitsplätze und Arbeitsplatzgruppen</span><span class="sxs-lookup"><span data-stu-id="288a5-128">How to: View the Load in Work and Machine Centers</span></span>](production-how-to-view-the-load-on-work-centers.md)|      
|<span data-ttu-id="288a5-129">Buchen verbrauchter Kapazitäten, die keinem Fertigungsauftrag zugeordnet sind (beispielsweise Wartungsarbeiten), mithilfe des Fensters **Kapazitäts Buch.-Blatt**</span><span class="sxs-lookup"><span data-stu-id="288a5-129">Use the **Capacity Journal** window to post consumed capacities that are not assigned to a production order, such as maintenance work.</span></span>|[<span data-ttu-id="288a5-130">So wird's gemacht: Kapazitäten buchen</span><span class="sxs-lookup"><span data-stu-id="288a5-130">How to: Post Capacities</span></span>](production-how-to-post-capacities.md)|  
|<span data-ttu-id="288a5-131">Berechnen und Regulieren der Kosten für gefertigte Artikel und verbrauchte Komponenten zur finanziellen Abstimmung</span><span class="sxs-lookup"><span data-stu-id="288a5-131">Calculate and adjust the cost of finished production items and consumed components for financial reconciliation.</span></span>|[<span data-ttu-id="288a5-132">Info zu Kosten des beendeten Auftrags</span><span class="sxs-lookup"><span data-stu-id="288a5-132">About Finished Production Order Costs</span></span>](finance-about-finished-production-order-costs.md)|  

## <a name="see-also"></a><span data-ttu-id="288a5-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="288a5-133">See Also</span></span>  
[<span data-ttu-id="288a5-134">Produktion einrichten</span><span class="sxs-lookup"><span data-stu-id="288a5-134">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="288a5-135">[Planung](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="288a5-135">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="288a5-136">Lagerbest</span><span class="sxs-lookup"><span data-stu-id="288a5-136">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="288a5-137">Einkauf</span><span class="sxs-lookup"><span data-stu-id="288a5-137">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="288a5-138">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="288a5-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
