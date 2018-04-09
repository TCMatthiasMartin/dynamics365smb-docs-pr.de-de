---
title: Einrichten von unrealisierter Mehrwertsteuer | Microsoft Docs
description: "Wenn Sie Einnahmen- und Ausgabenrechnung verwenden, können Sie angeben, wie Sie unrealisierte MwSt. für Verkäufe und Einkäufe behandeln möchten."
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 5e21330cd7adc97da9023da7b18944a9f0450b8e
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-unrealized-vat-for-cash-based-accounting"></a><span data-ttu-id="66e8c-103">Einrichten unrealisierter MwSt. für Einnahmen- und Ausgabenrechnung</span><span class="sxs-lookup"><span data-stu-id="66e8c-103">Set Up Unrealized VAT for Cash-Based Accounting</span></span>
<span data-ttu-id="66e8c-104">Wenn Sie Einnahmen- und Ausgabenrechnungs-Methoden ausgleichen, können Sie in [!INCLUDE[d365fin](includes/d365fin_md.md)] festlegen, wie unrealisierte MwSt. zu behandeln ist.</span><span class="sxs-lookup"><span data-stu-id="66e8c-104">If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle unrealized VAT.</span></span>

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a><span data-ttu-id="66e8c-105">Verwenden von Sachkonten für unrealisierte MwSt.</span><span class="sxs-lookup"><span data-stu-id="66e8c-105">To use general ledger accounts for unrealized VAT</span></span>
<span data-ttu-id="66e8c-106">Sie können festlegen, dass MwSt.-Beträge beim Buchen einer Rechnung berechnet und auf ein temporäres Sachkonto gebucht werden und dass die Beträge erst dann auf das korrekte Sachkonto gebucht und in die MwSt.-Abrechnungen einbezogen werden sollen, wenn die eigentliche Zahlung der Rechnung gebucht wird.</span><span class="sxs-lookup"><span data-stu-id="66e8c-106">You can choose to have VAT amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in VAT statements when the actual payment of the invoice is posted.</span></span> <span data-ttu-id="66e8c-107">Bevor Sie dies tun können, müssen Sie die MwSt.-Buchungsmatrix ausfüllen.</span><span class="sxs-lookup"><span data-stu-id="66e8c-107">Before you can do this, you must complete the VAT posting setup.</span></span>

<span data-ttu-id="66e8c-108">Um die Konten für unrealisierte MwSt. zu verwenden, führen Sie diese Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="66e8c-108">To use accounts for unrealized VAT, follow these steps:</span></span>
1. <span data-ttu-id="66e8c-109">Wählen Sie ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und **Finanzbuchhaltung einrichten** eingeben.</span><span class="sxs-lookup"><span data-stu-id="66e8c-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**.</span></span>
2. <span data-ttu-id="66e8c-110">Auf der Seite **Finanzbuchhaltungs-Einrichtung:** im Inforegister **Allgemein**, wählen Sie **Mehr anzeigen** und wählen Sie dann das Kontrollkästchen **Unrealisierte MwSt.** aus.</span><span class="sxs-lookup"><span data-stu-id="66e8c-110">On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.</span></span>
3. <span data-ttu-id="66e8c-111">Schließen Sie die Seite.</span><span class="sxs-lookup"><span data-stu-id="66e8c-111">Close the page.</span></span>
4. <span data-ttu-id="66e8c-112">In der oberen rechter Ecke wählen Sie das Symbol **Nach Seite oder Bericht suchen** aus ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol nach Seite oder Bericht suchen"). Geben Sie **MwSt Buchung einrichten** ein und wählen Sie dann den entsprechenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="66e8c-112">choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**.</span></span>
5. <span data-ttu-id="66e8c-113">Auf der Seite **MwSt.-Buchung einrichten** wählen Sie die MwSt.-Buchungsgruppe aus, und wählen Sie dann **Bearbeiten** aus.</span><span class="sxs-lookup"><span data-stu-id="66e8c-113">On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**.</span></span>
6. <span data-ttu-id="66e8c-114">Im Feld **Unrealisierte MwSt-Art** wählen Sie eine Option aus, um zu bestimmen, wie Zahlungen auf dem Rechnungsbetrag (ohne MwSt.) und den MwSt.-Betrag selbst aufgeteilt wird und wie MwSt.-Beträge vom Konto "Unreal. MwSt." auf das realisierte MwSt.-Konto gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="66e8c-114">In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account.</span></span> <span data-ttu-id="66e8c-115">Die Optionen werden in der folgenden Tabelle beschrieben.</span><span class="sxs-lookup"><span data-stu-id="66e8c-115">The following table describes the options.</span></span>

| <span data-ttu-id="66e8c-116">Option</span><span class="sxs-lookup"><span data-stu-id="66e8c-116">Option</span></span> | <span data-ttu-id="66e8c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66e8c-117">Description</span></span> |
| --- | --- |
| <span data-ttu-id="66e8c-118">Leer</span><span class="sxs-lookup"><span data-stu-id="66e8c-118">Blank</span></span> | <span data-ttu-id="66e8c-119">Wählen Sie diese Option, wenn Sie die Funktion "Unrealisierte MwSt." nicht verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="66e8c-119">Choose this option if you don't want to use the unrealized VAT feature.</span></span> |
| <span data-ttu-id="66e8c-120">Prozent</span><span class="sxs-lookup"><span data-stu-id="66e8c-120">Percentage</span></span> | <span data-ttu-id="66e8c-121">Zahlungen decken sowohl MwSt und den Rechnungsbetrag im Verhältnis zur prozentualen Zahlung des zu begleichenden Gesamtbetrags.</span><span class="sxs-lookup"><span data-stu-id="66e8c-121">Payments covers both VAT and the invoice amount in proportion to the payment's percentage of the remaining invoice amount.</span></span> <span data-ttu-id="66e8c-122">Der gezahlte Steuerbetrag wird vom unrealisierten MwSt-Konto auf das realisierte MwSt-Konto gebucht.</span><span class="sxs-lookup"><span data-stu-id="66e8c-122">The paid VAT amount is transferred from the unrealized VAT account to the realized VAT account.</span></span> |
| <span data-ttu-id="66e8c-123">Erster</span><span class="sxs-lookup"><span data-stu-id="66e8c-123">First</span></span> | <span data-ttu-id="66e8c-124">Zahlungen decken zuerst die MwSt und dann den Rechnungsbetrag.</span><span class="sxs-lookup"><span data-stu-id="66e8c-124">Payments cover VAT first and then invoice amounts.</span></span> <span data-ttu-id="66e8c-125">In diesem Fall entspricht der vom Konto für die unrealisierte Mehrwertsteuer auf das Konto für die realisierte Mehrwertsteuer transferierte Betrag dem Zahlungsbetrag (bis die Mehrwertsteuer vollständig beglichen ist).</span><span class="sxs-lookup"><span data-stu-id="66e8c-125">In this case, the amount transferred from the unrealized VAT account to the VAT account will equal the amount of the payment until the total VAT has been paid.</span></span> |
| <span data-ttu-id="66e8c-126">Letzter</span><span class="sxs-lookup"><span data-stu-id="66e8c-126">Last</span></span> | <span data-ttu-id="66e8c-127">Zahlungen decken zuerst den Rechnungsbetrag und dann die MwSt.</span><span class="sxs-lookup"><span data-stu-id="66e8c-127">Payments cover the invoice amount first and then VAT.</span></span> <span data-ttu-id="66e8c-128">In diesem Fall wird erst dann ein Betrag vom Konto für die unrealisierte Mehrwertsteuer auf das Konto für die realisierte Mehrwertsteuer transferiert, wenn der Zahlungsbetrag (ohne Mehrwertsteuer) vollständig beglichen ist.</span><span class="sxs-lookup"><span data-stu-id="66e8c-128">In this case, no amount will be transferred from the unrealized VAT account to the VAT account until the total amount of the invoice, excluding VAT, has been paid.</span></span> |
| <span data-ttu-id="66e8c-129">Erste (ganz bezahlt)</span><span class="sxs-lookup"><span data-stu-id="66e8c-129">First (Fully Paid)</span></span> | <span data-ttu-id="66e8c-130">Zahlungen decken zuerst die MwSt. (wie die _Erste_ Option), aber es werden erst dann Beträge auf das Steuerkonto transferiert, wenn die MwSt. vollständig gezahlt wurde.</span><span class="sxs-lookup"><span data-stu-id="66e8c-130">Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |
| <span data-ttu-id="66e8c-131">Letzte (ganz bezahlt)</span><span class="sxs-lookup"><span data-stu-id="66e8c-131">Last (Fully Paid)</span></span> | <span data-ttu-id="66e8c-132">Zahlungen decken zuerst den Rechnungsbetrag (wie unter der Option _Letzte_), aber es werden erst dann Beträge auf das Steuerkonto transferiert, wenn die MwSt. vollständig beglichen wurde.</span><span class="sxs-lookup"><span data-stu-id="66e8c-132">Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |

6. <span data-ttu-id="66e8c-133">Geben Sie im Feld **Unreal. Umsatzsteuerkonto** die entsprechende unrealisierte MwSt ein.</span><span class="sxs-lookup"><span data-stu-id="66e8c-133">In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="66e8c-134">Der MwSt-Betrag wird auf dieses Steuerkonto gebucht, wo er verbleibt, bis die Zahlung des Debitors gebucht wird.</span><span class="sxs-lookup"><span data-stu-id="66e8c-134">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="66e8c-135">Der Betrag wird dann auf das Sachkonto für Umsatzsteuer transferiert.</span><span class="sxs-lookup"><span data-stu-id="66e8c-135">The amount is then transferred to the account for sales VAT.</span></span>
7. <span data-ttu-id="66e8c-136">Geben Sie im Feld **Unreal. Vorsteuerkonto** die entsprechende Sachkontonummer ein.</span><span class="sxs-lookup"><span data-stu-id="66e8c-136">In the **Purch. VAT Unreal. Account** field, enter the general ledger account for unrealized purchase VAT.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="66e8c-137">Der MwSt-Betrag wird auf dieses Steuerkonto gebucht, wo er verbleibt, bis die Zahlung des Debitors gebucht wird.</span><span class="sxs-lookup"><span data-stu-id="66e8c-137">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="66e8c-138">Der Betrag wird dann auf das Sachkonto für Mehrwertsteuerkäufe transferiert.</span><span class="sxs-lookup"><span data-stu-id="66e8c-138">The amount is then transferred to the account for purchase VAT.</span></span>

## <a name="see-also"></a><span data-ttu-id="66e8c-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="66e8c-139">See Also</span></span>
[<span data-ttu-id="66e8c-140">Mehrwertsteuer einrichten</span><span class="sxs-lookup"><span data-stu-id="66e8c-140">Setting Up Value Added Tax</span></span>](finance-setup-vat.md)
