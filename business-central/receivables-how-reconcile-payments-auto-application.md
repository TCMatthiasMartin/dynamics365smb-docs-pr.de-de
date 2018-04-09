---
title: Abstimmen von Zahlungen mithilfe der automatischen Anwendung | Microsoft Docs
description: "Beschreibt, wie die automatische Anwendungsfunktion verwendet wird, um Zahlungseingänge Zahlungen oder in ihre entsprechenden offenen Posten anwenden und Zahlungen auszugleichen."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 75b030e6fc1a2cc5cf3c1068337dfd8c1c905543
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---
# <a name="reconcile-payments-using-automatic-application"></a><span data-ttu-id="17667-103">Abstimmen von Zahlungen mithilfe der automatischen Anwendung</span><span class="sxs-lookup"><span data-stu-id="17667-103">Reconcile Payments Using Automatic Application</span></span>
<span data-ttu-id="17667-104">Das Fenster **Zahlungsabstimmungsbuch.-Blatt** gibt Zahlungen an, entweder eingehend von Debitoren oder ausgehend an Kreditoren, die als Transaktionen in Ihrem Bankkonto erfasst wurden und die auf ihre entsprechenden unbezahlten Rechnungen und Gutschriften oder andere offene Posten angewendet werden können.</span><span class="sxs-lookup"><span data-stu-id="17667-104">The **Payment Reconciliation Journal** window specifies payments, either incoming or outgoing, that have been recorded as transactions on your online bank account and that you can apply to their related open customer, vendor, and bank account ledger entries.</span></span> <span data-ttu-id="17667-105">Die Zeilen im Buch.-Blatt werden ausgefüllt, indem ein Bankkontoauszug als Bankfeed oder -Datei importiert wird.</span><span class="sxs-lookup"><span data-stu-id="17667-105">The lines in the journal are filled by importing a bank statement as a bank feed or file.</span></span>

<span data-ttu-id="17667-106">Ein Zahlungsabstimmungsbuch.-Blatt wird mit einem Bankkonto in [!INCLUDE[d365fin](includes/d365fin_md.md)] verknüpft, das das elektronischen Bankkonto widerspiegelt, in der die Zahlungsbuchungen erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="17667-106">A payment reconciliation journal is related to one bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] that reflects the online bank account where the payment transactions are recorded.</span></span> <span data-ttu-id="17667-107">Alle offnen Bankposten, die sich auf ausgeglichene Debitoren- oder Kreditorenposten beziehen, werden geschlossen, wenn Sie die Aktion **Zahlungen buchen und Bankkonto abstimmen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="17667-107">Any open bank account ledger entries related to the applied customer or vendor ledger entries will be closed when you choose the **Post Payments and Reconcile Bank Account** action.</span></span> <span data-ttu-id="17667-108">Dies bedeutet, dass das Bankkonto mit Zahlungen abgestimmt wird, die Sie mit dem Buch.-Blatt buchen.</span><span class="sxs-lookup"><span data-stu-id="17667-108">This means that the bank account is automatically reconciled for payments that you post with the journal.</span></span>

<span data-ttu-id="17667-109">Um den Import von Bankkontoauszügen als Bankfeed zu aktivieren, müssen Sie den Bankfeeddienst Envestnet Yodlee einrichten und aktivieren und dann Ihr Bankkonto mit den entsprechenden Onlinebankkonten verbinden.</span><span class="sxs-lookup"><span data-stu-id="17667-109">If you want to import bank statements as bank feeds, you must first enable the Envestnet Yodlee Bank Feeds service and then link the bank account to its related online bank account.</span></span> <span data-ttu-id="17667-110">Das Zahlungsabstimmungsbuch.-Blatt erkennt dann automatisch Bankfeeds, wenn Sie die Aktion **Import-Bankbuchungen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="17667-110">The payment reconciliation journal will then automatically detect bank feeds when you choose the **Import Bank Transactions** action.</span></span> <span data-ttu-id="17667-111">Darüber hinaus können Sie in einem Bankkonto beliebig viele automatisch festgelegt Importe für neue Bankkontoauszugsfeeds jede Stunde festlegen.</span><span class="sxs-lookup"><span data-stu-id="17667-111">In addition, you can set a bank account up to automatically import new bank statement feeds every hour.</span></span> <span data-ttu-id="17667-112">Transaktionen für Zahlungen, die bereits als ausgeführt und/oder abgestimmt im Fenster Zahlungsabstimmungsbuch.-Blatt gebucht wurden, werden nicht importiert.</span><span class="sxs-lookup"><span data-stu-id="17667-112">Transactions for payments that have already been posted as applied and/or reconciled will not be imported.</span></span> <span data-ttu-id="17667-113">Für weitere Informationen, siehe [Einrichten des Envestnet Yodlee Bank-Feed-Service](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="17667-113">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

<span data-ttu-id="17667-114">Im Fenster **Text zu Konto zuordnen**, können Sie schnell Zuordnungen zwischen Text in Zahlungen und bestimmten Soll-, Haben- und Gegenkonten eingeben, sodass solche Zahlungen auf die angegebenen Konten gebucht werden, wenn Sie Zahlungen im Zahlungsabstimmungsbuch.-Blatt buchen.</span><span class="sxs-lookup"><span data-stu-id="17667-114">With the **Map Text to Account** action, you can set up mappings between text on payments and specific debit, credit, and balancing accounts so that such payments are posted to the specified accounts when you post the payment reconciliation journal.</span></span> <span data-ttu-id="17667-115">Siehe dazu auch Schritt 8.</span><span class="sxs-lookup"><span data-stu-id="17667-115">See step 8.</span></span> <span data-ttu-id="17667-116">Weitere Informationen finden Sie unter [Zuordnen von sich wiederholenden Zahlungen an Konten bei der automatischen Abstimmung](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)</span><span class="sxs-lookup"><span data-stu-id="17667-116">For more information, see [Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).</span></span>

<span data-ttu-id="17667-117">Ähnliche Funktionen sind vorhanden, um Mehrbeträge auf Zahlungsabstimmungsbuch.-Blattzeilen fallweise abzustimmen.</span><span class="sxs-lookup"><span data-stu-id="17667-117">Similar functionality exists to reconcile excess amounts on payment reconciliation journal lines on an ad-hoc basis.</span></span> <span data-ttu-id="17667-118">Weitere Informationen finden Sie unter [Abstimmen von Zahlungen mithilfe der automatischen Anwendung](receivables-how-reconcile-payments-cannot-apply-auto.md).</span><span class="sxs-lookup"><span data-stu-id="17667-118">For more information, see [Reconcile Payments That Cannot be Applied.](receivables-how-reconcile-payments-cannot-apply-auto.md)</span></span>

<span data-ttu-id="17667-119">Sie verwenden die Funktion **Automatisch anwenden** entweder automatisch, wenn Sie die Bankdatei importieren mit Zahlungstransaktionen, oder wenn Sie sie aktivieren, um Zahlungen auf ihre entsprechenden offenen Posten im Rahmen eines Datenabgleichs in einer Buch.-Blattzeile mit Daten für einen oder mehrere offene Posten anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="17667-119">You use the **Apply Automatically** function, either automatically when you import a bank file or feed with payment transactions or when you activate it, to apply payments to their related open entries based on a matching of data on a journal line with data on one or more open entries.</span></span>

<span data-ttu-id="17667-120">In Buch.-Blattzeilen, bei denen eine Zahlung automatisch auf einen oder mehrere offene Posten angewendet wurde, hat das Feld **Passende Werte** einen Wert zwischen Niedrig und Hoch, um die Qualität des Datenabgleichens anzugeben, auf der die vorgeschlagenen Zahlungsanwendung basiert.</span><span class="sxs-lookup"><span data-stu-id="17667-120">On journal lines where a payment has been applied automatically to one or more open entries, the **Match Confidence** field has a value between Low and High to indicate the quality of the data matching that the suggested payment application is based on.</span></span> <span data-ttu-id="17667-121">Darüber hinaus werden -**Kontoart** und **Konto-Nr.**-Felder mit Informationen über den Debitor oder Kreditor ausgefüllt, auf die die Zahlung angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="17667-121">In addition, the **Account Type** and **Account No.** fields are filled with information about the customer or vendor that the payment is applied to.</span></span> <span data-ttu-id="17667-122">Wenn Sie eine Text-zu-Konto-Zuordnung eingerichtet haben, kann die automatische Anwendung einen Abgleichungsvertrauenswert von **Hoch - Text-zu-Konto-Zuordnung** ergeben.</span><span class="sxs-lookup"><span data-stu-id="17667-122">If you have set up a text-to-account mapping, the automatic application can result in a match confidence value of **High - Text-to-Account Mapping**.</span></span>

<span data-ttu-id="17667-123">Für jede Buch.-Blattzeile, die ein Zahlung im Fenster **Zahlungsabstimmungsbuch.-Blatt** darstellt, können Sie das Fenster **Zahlungsanwendung** öffnen, um alle offenen Kandidatenposten für die Zahlung anzuzeigen und detaillierte Informationen für jeden Posten zum Datenabgleich anzuzeigen, auf denen eine Zahlungsanwendung basiert.</span><span class="sxs-lookup"><span data-stu-id="17667-123">For each journal line in the **Payment Reconciliation Journal** window, you can open the **Payment Application** window to see all candidate open entries for the payment and view detailed information for each entry about the data matching that a payment application is based on.</span></span> <span data-ttu-id="17667-124">Hier können Sie manuell Zahlungen ausgleichen, oder Zahlungen erneut ausgleichen, die automatisch auf einen falschen offenen Posten angewendet wurden,.</span><span class="sxs-lookup"><span data-stu-id="17667-124">Here, you can manually apply payments or reapply payments that were applied automatically to a wrong entry.</span></span> <span data-ttu-id="17667-125">Weitere Informationen finden Sie unter [Abstimmen von Zahlungen mithilfe der automatischen Anwendung](receivables-how-review-apply-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="17667-125">For more information, see [Review or Apply Payments After Automatic Application](receivables-how-review-apply-payments-auto-application.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="17667-126">Sie können den Banktransaktionsimport automatisch starten, wenn Sie dafür ein vorhandenes **Zahlungsabstimmungsbuch.-Blatt** im Fenster **Zahlungsabstimmungsbuch.-Blatt** öffnen.</span><span class="sxs-lookup"><span data-stu-id="17667-126">You can start the bank transactions import at the same time as you open the **Payment Reconciliation** Journal window for an existing payment reconciliation journal in the **Payment Reconciliation Journals** window.</span></span> <span data-ttu-id="17667-127">Nachfolgend wird beschrieben, wie Banktransaktionen in das Fenster **Zahlungsabstimmungsbuch-Blatt** importiert werden, nachdem Sie ein neues Buch.-Blatt erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="17667-127">The following procedure describes how to import bank transactions into the **Payment Reconciliation Journal** window after you have created a new journal.</span></span>

## <a name="to-reconcile-payments-using-automatic-application"></a><span data-ttu-id="17667-128">Vorgehensweise zum Abstimmen von Zahlungen mithilfe der automatischen Anwendung</span><span class="sxs-lookup"><span data-stu-id="17667-128">To reconcile payments using automatic application</span></span>
1. <span data-ttu-id="17667-129">Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben **Zahlungsabstimmungsbuch.-Blatt** ein und wählen den zugehörenden Link aus.</span><span class="sxs-lookup"><span data-stu-id="17667-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Reconciliation Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="17667-130">Um in einem neuen Zahlungsabstimmungsbuch.-Blatt zu arbeiten, wählen Sie die Aktion **Neues Buch.-Blatt** aus.</span><span class="sxs-lookup"><span data-stu-id="17667-130">To work in a new payment reconciliation journal, choose the **New Journal** action.</span></span>
3. <span data-ttu-id="17667-131">Wählen Sie im Fenster **Bankkontenübersicht** das Bankkonto aus, mit dem Sie eine Verknüpfung erstellen möchten, und klicken Sie anschließend auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="17667-131">In the **Payment Bank Account List** window, select the bank account that you want to reconcile payments for, and then choose the **OK** button.</span></span>
   <span data-ttu-id="17667-132">Das Fenster **Zahlungsabstimmungsbuch.-Blatt** wird für das ausgewählte Bankkonto vorbereitet geöffnet.</span><span class="sxs-lookup"><span data-stu-id="17667-132">The **Payment Reconciliation Journal** window opens prepared for the selected bank account.</span></span>
4. <span data-ttu-id="17667-133">Wählen Sie die Aktion **Import-Bankbuchungen** aus.</span><span class="sxs-lookup"><span data-stu-id="17667-133">Choose the **Import Bank Transactions** action.</span></span>
   <span data-ttu-id="17667-134">Wenn das Bankkonto für das gewählte Buch.-Blatt nicht zum Importieren von Banktransaktionen eingerichtet ist, dann öffnet sich ein Dialogfeld, um Ihnen dabei zu helfen, die entsprechenden Felder einzutragen.</span><span class="sxs-lookup"><span data-stu-id="17667-134">If the bank account for the selected journal is not set up for import of bank transactions, then a dialog box will open to help you fill in the relevant fields.</span></span>
5. <span data-ttu-id="17667-135">Im Fenster **Datei für den Import auswählen** wählen Sie die Datei aus, die die Banktransaktionen für Zahlungen enthält, die abgestimmt werden sollen, und wählen Sie dann die Schaltfläche **Öffnen**.</span><span class="sxs-lookup"><span data-stu-id="17667-135">In the **Select a file to import** window, select the file that contains the bank transactions for payments that you want to reconcile, and then choose the **Open** button.</span></span>  
6. <span data-ttu-id="17667-136">Wenn der Bankkontoauszugs-Service ausgeführt wird, öffnet sich das Fenster **Bankkontoauszugs-Filter** automatisch. Geben Sie ein Datumsintervall an, sodass die Bankkontoauszüge importiert werden können.</span><span class="sxs-lookup"><span data-stu-id="17667-136">If the Bank Statement service is enabled, in the **Bank Statement Filter** window that opens automatically, specify the date interval for the bank statements to be imported.</span></span>

    <span data-ttu-id="17667-137">Das Fenster **Zahlungsabstimmungsbuch-Blatt** enthält Zeilen für die Zahlungen, die Banktransaktionen in der importierten Datei darstellen.</span><span class="sxs-lookup"><span data-stu-id="17667-137">The **Payment Reconciliation Journal** window is filled with lines for payments representing bank transactions in the imported bank statement.</span></span>

    <span data-ttu-id="17667-138">In Zeilen, bei denen eine Zahlung automatisch auf den zugehörigen offenen Posten angewendet wurde, hat das Feld **Übereinstimmungsgenauigkeit** einen Wert zwischen **Niedrig** und **Hoch**, um die Qualität des Datenabgleichens anzugeben, auf der die vorgeschlagenen Zahlungsanwendung basiert.</span><span class="sxs-lookup"><span data-stu-id="17667-138">On lines for payments that have been automatically applied to their related open entries, the **Match Confidence** field has a value between **Low** and **High** to indicate the quality of the data matching that the suggested payment application is based on.</span></span> <span data-ttu-id="17667-139">Darüber hinaus werden -**Kontoart** und **Konto-Nr.**-Felder mit Informationen über den Debitor oder Kreditor ausgefüllt, auf die die Zahlung angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="17667-139">In addition, the **Account Type** and **Account No.** fields are filled with information about the customer or vendor that the payment is applied to.</span></span>
7. <span data-ttu-id="17667-140">Wählen Sie eine Buch.-Blattzeile, und wählen Sie dann **Manuell anwenden** oder Zahlung manuell anwenden im Fenster **Zahlungsanwendung**.</span><span class="sxs-lookup"><span data-stu-id="17667-140">Select a journal line, and then, choose the **Apply Manually** action to review, reapply, or apply the payment manually in the **Payment Application** window.</span></span> <span data-ttu-id="17667-141">Weitere Informationen finden Sie unter [Abstimmen von Zahlungen mithilfe der automatischen Anwendung](receivables-how-review-apply-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="17667-141">For more information, see [Review or Apply Payments After Automatic Application](receivables-how-review-apply-payments-auto-application.md).</span></span>

    <span data-ttu-id="17667-142">Wenn Sie den manuellen Ausgleich abgeschlossen haben, enthält das Feld **Übereinstimmungsgenauigkeit** in der Buchzeile, die Sie manuell verarbeitet haben **Akzeptiert**.</span><span class="sxs-lookup"><span data-stu-id="17667-142">When you have finished your manual application, the **Match Confidence** field on the journal line that you have processed manually contains **Accepted**.</span></span>
8. <span data-ttu-id="17667-143">Wählen Sie eine nicht ausgeglichene Buch.-Blattzeile für einen wiederkehrende Zahlungseingang oder Ausgabe aus, wie einen Autobenzineinkauf, und wählen Sie dann auf der Registerkarte Start in der Gruppe Anwendungen **Text-zu-Kontenzuordnung** aus.</span><span class="sxs-lookup"><span data-stu-id="17667-143">Select an unapplied journal line for a recurring cash receipt or expense, such as a car gasoline purchase, and then choose the **Map Text to Account** action.</span></span> <span data-ttu-id="17667-144">Weitere Informationen finden Sie unter [Zuordnen von sich wiederholenden Zahlungen an Konten bei der automatischen Abstimmung](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)</span><span class="sxs-lookup"><span data-stu-id="17667-144">For more information, see [Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)</span></span>
9. <span data-ttu-id="17667-145">Wenn Sie Ihre manuelle Zuordnung von Zahlungstext zu Konten abgeschlossen haben, wählen Sie die Aktion **Manuell anwenden** aus.</span><span class="sxs-lookup"><span data-stu-id="17667-145">When you have finished your mapping of payment text to accounts, choose the **Apply Manually** action.</span></span>
10. <span data-ttu-id="17667-146">Wenn Sie sicher sind, dass alle Zahlungen der Buch.-Blattzeilen korrekt angewendet oder zur direkten Buchung festgelegt werden, wählen Sie die Aktion **Buchen** aus.</span><span class="sxs-lookup"><span data-stu-id="17667-146">When you are content that all payments on the journal lines are correctly applied or set to direct posting, choose the **Post** action.</span></span>

<span data-ttu-id="17667-147">Wenn Sie das Zahlungsabstimmungsbuch.-Blatt buchen, werden die saldierten offenen Posten geschlossen und die zugehörigen Debitoren-, Kreditoren- oder Sachkonten werden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="17667-147">When you post the payment reconciliation journal, the applied open entries memos are closed, and the related customer, vendor, or general ledger accounts are updated.</span></span> <span data-ttu-id="17667-148">Für Zahlungen in Buch.-Blattzeilen basierend auf der Text-zu-Kontenzuordnung werden die angegebenen Debitoren-, Kreditoren- und Sachkonten aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="17667-148">For payments on journal lines based on text-to-account mapping, the specified customer, vendor, and general ledger accounts are updated.</span></span> <span data-ttu-id="17667-149">Für alle Buch.-Blattzeilen werden Bankposten erstellt.</span><span class="sxs-lookup"><span data-stu-id="17667-149">For all journal lines, bank account ledger entries are created.</span></span> <span data-ttu-id="17667-150">Alle offenen Bankposten, die sich auf ausgeglichene Debitoren- oder Kreditorenposten beziehen, werden geschlossen, wenn Sie die Aktion **Zahlungen buchen und Bankkonto abstimmen** auswählen.</span><span class="sxs-lookup"><span data-stu-id="17667-150">If you choose the **Post Payments and Reconcile Bank Account** action, any open bank account ledger entries related to the applied customer or vendor ledger entries will be closed.</span></span> <span data-ttu-id="17667-151">Dies bedeutet, dass das Bankkonto mit Zahlungen abgestimmt wird, die Sie mit dem Buch.-Blatt buchen.</span><span class="sxs-lookup"><span data-stu-id="17667-151">This means that the bank account is automatically reconciled for payments that you post with the journal.</span></span>

<span data-ttu-id="17667-152">Sie können den Wert im Feld **Saldo auf Bankkonto nach dem Buchen** zusammen mit dem Wert im Feld **Auszug Schluss-Saldo** verwenden, um zu kontrollieren, wenn das Bankkonto basierend auf den gebuchten Zahlungen abgestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="17667-152">You can compare the value in the **Balance on Bank Account After Posting** field together with the value in the **Statement Ending Balance** field to track when the bank account is reconciled based on payments that you post.</span></span>

> [!NOTE]  
>   <span data-ttu-id="17667-153">Wenn Sie nicht das Bankkonto aus dem Fenster **Zahlungs-Abstimmungs-Buch.Blatt** abstimmen, müssen Sie das Fenster **Bankkonto-Abstimmung** verwenden.</span><span class="sxs-lookup"><span data-stu-id="17667-153">If you do not want to reconcile the bank account from the **Payment Reconciliation Journal** window, then you must use the **Bank Acc. Reconciliation** window.</span></span> <span data-ttu-id="17667-154">Weitere Informationen finden Sie unter [Vorgehensweise: Einrichten von Bankkonten](bank-how-reconcile-bank-accounts-separately.md).</span><span class="sxs-lookup"><span data-stu-id="17667-154">For more information, see [Reconcile Bank Accounts Separately](bank-how-reconcile-bank-accounts-separately.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="17667-155">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="17667-155">See Also</span></span>
[<span data-ttu-id="17667-156">Verwalten von Forderungen</span><span class="sxs-lookup"><span data-stu-id="17667-156">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="17667-157">Verkauf</span><span class="sxs-lookup"><span data-stu-id="17667-157">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="17667-158">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="17667-158">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
