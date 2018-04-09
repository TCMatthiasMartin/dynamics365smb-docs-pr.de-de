---
title: Antworten auf Anforderungen zu Personendaten
description: "Sie müssen auf Datenenbetreffanforderungen reagieren."
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.date: 03/13/2018
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 89f53f24f74401ce384b54d04fbeb473aedad96d
ms.contentlocale: de-de
ms.lasthandoff: 03/22/2018

---

# <a name="responding-to-requests-about-personal-data"></a><span data-ttu-id="e8dcd-103">Antworten auf Anforderungen zu Personendaten</span><span class="sxs-lookup"><span data-stu-id="e8dcd-103">Responding to Requests About Personal Data</span></span>  
<span data-ttu-id="e8dcd-104">Datenenbetreffe können mehrere Arten von Aktionen für die Personendaten abfragen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-104">Data subjects can request several types of actions regarding their personal data.</span></span> <span data-ttu-id="e8dcd-105">Wenn Sie sensible Daten klassifiziert haben und sicher sind, dass sie korrekt sind, kann ein Administrator auf Anforderungen reagieren, indem er den Datenen-Klassifizierungsvorschlag im Rollencenter **Verwalten Sie Benutzer, Benutzergruppen und Berechtigungen** nutzt, wenn Sie den Windows-Client im **IT-Manager** Rollencenter verwenden.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-105">If you have classified the sensitivity of your data, and are sure they are correct, an administrator can respond to requests by using the Data Classification worksheet on the **Manage Users, User Groups, and Permissions** Role Center or, if you are using the Windows client, in the **IT Manager** Role Center.</span></span> <span data-ttu-id="e8dcd-106">Weitere Informationen zum Klassifizieren von Daten und von Abteilungen und Datenenempfindlichkeit, und [Klassifizieren von Daten](/dynamics-nav/classifying-data) Sie sehen. [Abteilungen und Datenen-Empfindlichkeit](admin-classifying-data-sensitivity.md)</span><span class="sxs-lookup"><span data-stu-id="e8dcd-106">For more information about classifying data and classifying data sensitivity, see [Classifying Data](/dynamics-nav/classifying-data) and [Classifying Data Sensitivity](admin-classifying-data-sensitivity.md).</span></span>

<span data-ttu-id="e8dcd-107">Die folgende Tabelle enthält Beispiele über die Anforderungen, auf die Sie reagieren können.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-107">The following table provides examples of the types of requests you can respond to.</span></span>

> [!Note]
> <span data-ttu-id="e8dcd-108">Während wir Funktionen für die Antworten auf diese Art von Anfragen bereitstellen und so auf Personendaten zugreifen, ist es Ihre Verantwortung, sicherzustellen, dass persönlich und sensible Daten entsprechend zugeordnet und klassifiziert werden.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-108">While we provide capabilities for responding to these types of request, and thereby accessing, personal data, it is your responsibility to ensure that personal and sensitive data are located and classified appropriately.</span></span>

|<span data-ttu-id="e8dcd-109">Anforderungsart</span><span class="sxs-lookup"><span data-stu-id="e8dcd-109">Request Type</span></span>|<span data-ttu-id="e8dcd-110">Beschreibung und vorgeschlagene Antwort</span><span class="sxs-lookup"><span data-stu-id="e8dcd-110">Description and Suggested Response</span></span>|
|-----|-----|
|<span data-ttu-id="e8dcd-111">Portabilitätsanforderungen</span><span class="sxs-lookup"><span data-stu-id="e8dcd-111">Portability requests</span></span>|<span data-ttu-id="e8dcd-112">Ein Datenbetreff kann einen Datenenportabilitätsantrag erstellen, d. h. zum Teil, dass Sie die entsprechenden Daten der Personendaten aus Ihrem Systemen exportieren und in einem strukturierten, häufig genutzten Format bereitstellen müssen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-112">A data subject can make a data portability request, meaning, in part, that you must export the data subject's personal data from your systems and provide it in in a structured, commonly used format.</span></span> <span data-ttu-id="e8dcd-113">Um auf diese Anforderungen zu reagieren, verwenden Sie die Funktion Schutz der Privatsphäre, um personenbezogene Daten in eine Excel-Datei zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-113">To respond to these requests, use the Data Privacy Utility to export personal data to an Excel file.</span></span> <span data-ttu-id="e8dcd-114">Mithilfe von Excel können Sie die Personendaten bearbeiten und in einem häufig verwendeten, maschinell lesbaren Format wie .csv oder .xml speichern.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-114">Using Excel, you can edit the personal data and save it in a commonly used, machine-readable format, such as .csv or .xml.</span></span> <span data-ttu-id="e8dcd-115">Administratoren können Daten mithilfe von Anfangskonfigurationspaketen auch exportieren und dann Stammdatentabellen und die zugehörigen Tabellen, die Personendaten enthalten, konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-115">Administrators can also export data using Rapid Start configuration packages, and then configure master data tables and their related tables that contain personal data.</span></span> |
|<span data-ttu-id="e8dcd-116">Anforderung für Löschen</span><span class="sxs-lookup"><span data-stu-id="e8dcd-116">Requests for deletion</span></span>|<span data-ttu-id="e8dcd-117">Ein Datenenbetreff kann anfordern, dass Sie die Personendaten löschen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-117">A data subject can request that you delete their personal data.</span></span> <span data-ttu-id="e8dcd-118">Es gibt verschiedene Arten, Personendaten mithilfe der Anpassungsfunktionen zu löschen, aber die Entscheidung und die Implementierung ist Ihre Verantwortung.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-118">There are several ways to delete personal data using the customization capabilities, but the decision and implementation is your responsibility.</span></span> <span data-ttu-id="e8dcd-119">In einigen Fällen können Sie die Daten direkt bearbeiten, zum Beispiel einen Kontakt löschen und dann die Stapelverarbeitung für stornierte Aktivitäten ausführen, um den Kontakt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-119">In some cases, you may choose to directly edit your data, for example deleting a contact and then running the Delete Canceled Interaction batch job to delete interactions for the contact.</span></span> <br><br> <span data-ttu-id="e8dcd-120">**Hinweis:**, Wenn Sie ein Datum in dem Feld **Löschen des Belegs zulassen vor** der **Debitoren & Verkauf Einr.** oder der **Kreditoren & Einkauf Einr.** angegeben haben, können Sie das Datum ändern, sodass gebuchte Verkaufs- und Einkaufsbelege, die Sie gedruckt haben und für die ein Buchungsdatum für oder vor dem Datum vorliegt, gelöscht werden können.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-120">**Note:** If you have specified a date in the **Allow Document Deletion Before** field on the **Sales & Receivables Setup** or **Purchases & Payables Setup** pages, you might need to change the date so that you can delete posted sales and purchase documents that you have printed and that have posting dates on or before that date.</span></span>|
|<span data-ttu-id="e8dcd-121">Anforderung für Korrektur</span><span class="sxs-lookup"><span data-stu-id="e8dcd-121">Requests for correction</span></span>|<span data-ttu-id="e8dcd-122">Ein Datenenbetreff kann verlagen, dass Sie die falschen Personendaten löschen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-122">A data subject can request that you correct inaccurate personal data.</span></span> <span data-ttu-id="e8dcd-123">Es gibt mehrere Möglichkeiten dazu:</span><span class="sxs-lookup"><span data-stu-id="e8dcd-123">There are several ways to do so.</span></span> <span data-ttu-id="e8dcd-124">In einigen Fällen können Sie Exporttarife nach Excel exportieren, mehrere Datensätze schnell auf einmal bearbeiten und importieren dann die aktualisierten Daten importieren.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-124">In some cases, you can export lists to Excel to quickly bulk-edit multiple records, and then import the updated data.</span></span> <span data-ttu-id="e8dcd-125">Weitere Informationen finden Sie unter [Geschäftsdaten nach Excel exportieren](https://docs.microsoft.com/en-us/dynamics-nav-app/about-export-data).</span><span class="sxs-lookup"><span data-stu-id="e8dcd-125">For more information, see [Exporting your Business Data to Excel](https://docs.microsoft.com/en-us/dynamics-nav-app/about-export-data).</span></span> <span data-ttu-id="e8dcd-126">Sie können auch manuell Eingabefelder, die Personendaten enthalten, wie Bearbeitungsinformationen über einen Debitor auf der Debitorenkarte bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-126">You can also manually edit fields that contain personal data, such as editing information about a customer in the Customer card.</span></span> <span data-ttu-id="e8dcd-127">Es sind jedoch Änderungssätze wie Allgemein, Debitor und Steuerposten für die Integrität des Unternehmensressourcenplanungssystems wichtig.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-127">However, transaction records such as general, customer, and tax ledger entries are essential to the integrity of the enterprise resource planning system.</span></span> <span data-ttu-id="e8dcd-128">Wenn Sie Personendaten in den Geschäfttransaktionsdatensätzen speichern, erwägen Sie, die Anpassungsfunktionen zu verwenden, um solche Personendaten zu ändern.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-128">If you store personal data in business transaction records, consider using the customization capabilities to modify such personal data.</span></span>|

## <a name="restrict-data-processing-for-a-data-subject"></a><span data-ttu-id="e8dcd-129">Beschränken der Datumsverarbeitung für Datenen-Betreff</span><span class="sxs-lookup"><span data-stu-id="e8dcd-129">Restrict Data Processing for a Data Subject</span></span>
<span data-ttu-id="e8dcd-130">Ein Datenbetreff kann verlangen, dass Sie die vorübergehend keine Personendaten verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-130">A data subject can request that you temporarily stop processing their personal data.</span></span> <span data-ttu-id="e8dcd-131">Um solche Anforderungen zu ehren, können Sie ihren Datensatz  als gesperrt markieren aufgrund des Datenschutzes und die Verarbeitung der Daten stoppen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-131">To honor such requests, you can mark their record as blocked due to privacy to stop processing their data.</span></span> <span data-ttu-id="e8dcd-132">Wenn ein Datensatz als gesperrt markiert wird, können Sie keine neuen Transaktionen erstellen, die den Datensatz verwenden.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-132">When a record is marked as blocked, you cannot create new transactions that use that record.</span></span> <span data-ttu-id="e8dcd-133">Beispielsweise können Sie eine neue Rechnung für keinen Debitor erstellen, wenn entweder der Debitor oder der Verkäufer gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-133">For example, you cannot create a new invoice for a customer when either the customer or the salesperson is blocked.</span></span> <span data-ttu-id="e8dcd-134">Um einen Datenbetreff als gesperrt zu kennzeichnen, öffnen Sie die Karte für den Datenbetreff, beispielsweise die Debitoren-, Kreditoren- oder Kontaktkarte, und wählen Sie **Datenschutz gesperrt**.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-134">To mark a data subject as blocked, open the card for the data subject, for example the Customer, Vendor, or Contact cards, and choose the **Privacy Blocked** check box.</span></span> <span data-ttu-id="e8dcd-135">Sie müssen u **Mehr anzeigen**, um das Feld anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-135">You may need to choose **Show More** to display the field.</span></span>

## <a name="handling-data-about-minors"></a><span data-ttu-id="e8dcd-136">Behandlung von Daten Minderjähriger</span><span class="sxs-lookup"><span data-stu-id="e8dcd-136">Handling Data About Minors</span></span>
<span data-ttu-id="e8dcd-137">Wenn das Alter der Kontaktperson tiefer ist als das Alter der Volljährigkeit entsprechend dem Gesetz Ihres Landes, können Sie das mithilfe des Kontrollkästchens **Minderjährig** auf der Karte **Kontakt** aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-137">If a contact person's age is below the age of legal consent according to the laws in your region, you can indicate that by choosing the **Minor** check box on the **Contact** card.</span></span> <span data-ttu-id="e8dcd-138">Wenn Sie dies tun, wird das Kontrollkästchen **Datenschutz gesperrt** automatisch ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-138">When you do, the **Privacy Blocked** check box is automatically selected.</span></span> <span data-ttu-id="e8dcd-139">Wenn Sie die Zustimmung des Feld von den Eltern oder dem Erziehungsberechtigten der minderjährigen Person erhalten, können Sie das Kontrollkästchen **Elterliche Einwilligung erhalten** aktivieren, um die Blockierung des Kontakts aufzuheben.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-139">When you receive consent from the minor's parent or legal guardian, you can choose the **Parental Consent Received** check box to unblock the contact.</span></span> <span data-ttu-id="e8dcd-140">Auch wenn Sie Personendaten für Minderjährige bearbeiten können, können Sie die Profilerstellungsfunktionalität in Microsoft Dynamics 365 for Sales nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-140">Though you can process personal data for minors, you cannot use the profiling functionality in Microsoft Dynamics 365 for Sales.</span></span>

> [!Note]
> <span data-ttu-id="e8dcd-141">Das Änderungsprotokoll kann Details erfassen, wie wann und durch wen die **Elterliche Einwilligung erhalten** im Kontrollkästchen ausgewählt wurde.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-141">The Change Log can record details such as when, and by whom, the **Parental Consent Received** check box was chosen.</span></span> <span data-ttu-id="e8dcd-142">Ein Administrator kann dies mithilfe dem Leitfaden **Änderungsprotokoll einrichten** einrichten und kann auch das Kontrollkästchen **Protokoll-Änderung für die elterliche Einwilligung erhalten** auf der Karte **Kontakt** aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e8dcd-142">An administrator can set that up by using the **Change Log Setup** guide, and also choosing the **Log Modification for Parental Consent Received** check box on the **Contact** card.</span></span> <span data-ttu-id="e8dcd-143">Weitere Informationen finden Sie unter [Änderungen nachverfolgen](/dynamics-nav-app/across-log-changes).</span><span class="sxs-lookup"><span data-stu-id="e8dcd-143">For more information, see [Logging Changes](/dynamics-nav-app/across-log-changes).</span></span>  

## <a name="see-also"></a><span data-ttu-id="e8dcd-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e8dcd-144">See Also</span></span>
[<span data-ttu-id="e8dcd-145">Klassifizieren von Daten</span><span class="sxs-lookup"><span data-stu-id="e8dcd-145">Classifying Data</span></span>](https://docs.microsoft.com/en-us/dynamics-nav/classifying-data)  
[<span data-ttu-id="e8dcd-146">Datensensitivität klassieren</span><span class="sxs-lookup"><span data-stu-id="e8dcd-146">Classifying Data Sensitivity</span></span>](admin-classifying-data-sensitivity.md)  
[<span data-ttu-id="e8dcd-147">Exportieren Ihrer Geschäftsdaten nach Excel</span><span class="sxs-lookup"><span data-stu-id="e8dcd-147">Exporting your Business Data to Excel</span></span>](https://docs.microsoft.com/en-us/dynamics-nav-app/about-export-data)  
