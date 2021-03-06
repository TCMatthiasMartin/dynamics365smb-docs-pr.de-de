---
title: E-Mail in Business Central einrichten | Microsoft Docs
description: Beschreibt, wie der SMTP-Server des Unternehmens verwendet wird, um in Business Central E-Mails zu senden und zu empfangen und wie die E-Mail-Servereinstellungen verwendet werden, die im Microsoft 365-Abonnement erstellt wurden.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, mail, Microsoft 365
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8c69de24198d8682b2e106e3bf559803c2fed72c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922548"
---
# <a name="set-up-email"></a>E-Mail einrichten
Um E-Mails aus [!INCLUDE[d365fin](includes/d365fin_md.md)] zu senden und zu erhalten, müssen Sie die Felder auf der Seite **SMTP-Mail-Einrichtung** ausfüllen.

Anstatt die SMTP-Serverdetails manuell einzugeben, können Sie die Funktion **Microsoft 365-Server-Einstellungen übernehmen** verwenden, um sie mit den Informationen aus Ihrem Microsoft 365-Abonnement einzugeben.

Sie können E-Mails entweder manuell einrichten wie unten beschrieben oder Sie können den Leitfaden für das unterstützte Setup für die **E-Mail-Einrichtung** verwenden. Weitere Informationen finden Sie unter [Vorbereitungen für das Ausführen von Geschäften](ui-get-ready-business.md).  

## <a name="to-set-up-email"></a>Zum Einrichten von E-Mails
1. Wählen Sie die Symbol ![Glühbirne , die das Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Was möchten Sie tun?") aus, geben Sie **SMTP-E-Mail-Einrichtung** ein und wählen Sie dann den entsprechenden Link.
2. Füllen Sie die Felder je nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]
    > Wenn Sie ein Konto verwenden, für das eine Zwei-Faktor-Authentifizierung erforderlich ist, muss das Kennwort, das Sie in das Feld **Kennwort** eingeben, das gleiche sein wie das, das Sie für Ihr Microsoft 365-Abonnement verwenden, und es muss vom Typ **App-Kennwort** sein. Weitere Informationen finden Sie unter [Verwalten Sie App-Passwörter für die Bestätigung in zwei Schritten](/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).
3. Wählen Sie alternativ die Aktion **Microsoft 365 Server-Einstellungen übernehmen** aus, um Informationen einzufügen, die bereits für Ihr Microsoft 365-Abonnement definiert sind.
4. Wenn alle korrekt Felder ausgefüllt sind, wählen Sie die Aktion **Test-E-Mail-Einrichtung** aus.
5. Wenn der Test erfolgreich war, schließen Sie die Seite.

## <a name="using-a-substitute-sender-address-on-outbound-email-messages"></a>Verwenden eine Ersatz-Absenderadresse für ausgehende E-Mail-Nachrichten
Alle ausgehenden E-Mail-Nachrichten von [!INCLUDE[d365fin](includes/d365fin_md.md)] verwenden die Standardadresse für das Konto, das Sie wie oben beschrieben auf der Seite SMTP-E-Mail-Setup angegeben haben. Sie können jedoch die **Senden Als** oder **Senden im Auftrag von** Funktionen auf Ihrem Exchange-Server zum Ändern der Absenderadresse für ausgehende Nachrichten verwenden. [!INCLUDE[d365fin](includes/d365fin_md.md)] verwendet das Standardkonto zur Authentifizierung bei Exchange, ersetzt jedoch entweder die Absenderadresse durch die von Ihnen angegebene oder ändert sie durch im Namen von.

Im Folgenden finden Sie Beispiele für die Verwendung von Senden als und Senden im Namen von [!INCLUDE[d365fin](includes/d365fin_md.md)].:

 * Wenn Sie Dokumente wie Kauf- oder Verkaufsaufträge an Lieferanten und Kunden senden, möchten Sie möglicherweise, dass sie von einer Adresse _noreply@yourcompanyname.com_ stammen.
 * Wenn Ihr Workflow eine Genehmigungsanfrage per E-Mail unter Verwendung der E-Mail-Adresse des Antragstellers sendet.

> [!Note]
> Sie können nur ein Konto verwenden, um Absenderadressen zu ersetzen. Das heißt, Sie können nicht eine Ersatzadresse für Einkaufsprozesse und eine andere für Verkaufsprozesse haben.

### <a name="to-set-up-the-substitute-sender-address-for-all-outbound-email-messages"></a>Um eine Ersatz-Senderadresse einzurichgen für alle ausgehenden E-Mail-Nachrichten
1. In dem **Exchange Admin Center** für Ihr Microsoft 365-Konto suchen Sie das Postfach, das als Ersatzadresse verwendet werden soll, und kopieren Sie die Adresse oder notieren Sie sie. Wenn Sie eine neue Adresse benötigen, rufen Sie Ihr Microsoft 365 Admin Center auf, um einen neuen Benutzer zu erstellen und dessen Postfach einzurichten.
2. In [!INCLUDE[d365fin](includes/d365fin_md.md)] wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Was möchten Sie tun?") aus, geben Sie **SMTP-E-Mail-Einrichtung** ein und wählen Sie dann den entsprechenden Link.
3. In dem Feld **Senden als** geben Sie in das Feld die Ersatzadresse ein.
4. Kopieren oder notieren Sie die Adresse im Feld **Benutzeridentifikation** .
5. In dem **Exchange Admin Center** suchen Sie die Mailbox, die als Ersatzadresse verwendet werden soll, und geben Sie die Adresse in das Feld **Benutzeridentifikation** im Feld **Senden Als** ein. Weitere Informationen finden Sie unter [Verwenden Sie die Exchange-Verwaltungskonsole, um einzelnen Postfächern Berechtigungen zuzuweisen ](/Exchange/recipients/mailbox-permissions?view=exchserver-2019#use-the-eac-to-assign-permissions-to-individual-mailboxes).

### <a name="to-use-the-substitute-address-in-approval-workflows"></a>Verwendung der Ersatzadresse in Genehmigungsworkflows
1. In [!INCLUDE[d365fin](includes/d365fin_md.md)] wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Was möchten Sie tun?") aus, geben Sie **SMTP-E-Mail-Einrichtung** ein und wählen Sie dann den entsprechenden Link.
2. Kopieren oder notieren Sie die Adresse im Feld **Benutzeridentifikation** .
3. Wählen Sie die ![Glühbirne, die das Tell Me Feature](media/ui-search/search_small.png "Was möchten Sie tun?") Symbol öffnet, geben Sie **Genehmigungsbenutzereinrichtung** ein und wählen Sie dann den entsprechenden Link.
4. In dem **Exchange Admin Center** , finden Sie die Postfächer für jeden Benutzer auf der Seite **Genehmigungsbenutzer einrichten** und im Feld **Senden Als** geben Sie die Adresse aus dem Bereich **Benutzeridentifikation** der Seite **SMTP-E-Mail einrichten** in [!INCLUDE[d365fin](includes/d365fin_md.md)] ein. Weitere Informationen finden Sie unter [Verwalten von Berechtigungen für Empfänger](/Exchange/recipients/mailbox-permissions?view=exchserver-2019).
5. In [!INCLUDE[d365fin](includes/d365fin_md.md)] wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen“ öffnet](media/ui-search/search_small.png "Was möchten Sie tun?") aus, geben Sie **SMTP-E-Mail-Einrichtung** ein und wählen Sie dann den entsprechenden Link.
6. Um die Ersetzung zu aktivieren, aktivieren Sie das Kontrollkästchen **Erlaube Absenderersetzung** .

> [!Note]
> [!INCLUDE[d365fin](includes/d365fin_md.md)] legt fest, welche Adresse in der folgenden Reihenfolge angezeigt werden soll: <br><br> 1. Die Adrsse, die im Feld **E-Mail** auf der Seite **Genehmigungsbenutzer einrichten** für Nachrichten in einem Workflow angegeben ist. <br> 2. Die Adresse im Feld **Senden Als** auf der Seite **SMTP-E-Mail-Setup** einrichten. <br> 3. Die Adresse im Feld **Benutzeer-ID** auf der Seite **SMTP-E-Mail einrichten** .

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a>Öffentliche Ordner und Regeln für die E-Mail-Anmeldung in Exchange Online einrichten
Machen Sie mehr aus der Kommunikation zwischen Verkäufern und Ihren bestehenden oder potenziellen Kunden, indem Sie den E-Mail-Austausch nachverfolgen und diese dann in umsetzbare Gelegenheiten umwandeln. Weitere Informationen finden Sie unter [Austausch von E-Mail-Nachrichten zwischen Verkäufern und Kontakten nachverfolgen](marketing-set-up-email-logging.md).  

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

Als nächstes verbinden Sie [!INCLUDE[prodshort](includes/prodshort.md)] mit Exchange Online. Weitere Informationen finden Sie unter [Austausch von E-Mail-Nachrichten zwischen Verkäufern und Kontakten nachverfolgen](marketing-set-up-email-logging.md).  

## <a name="see-also"></a>Siehe auch
[Freigegebene Postfächer in Exchange Online](/exchange/collaboration-exo/shared-mailboxes)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Einrichten [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Dokumente per E-Mail versenden](ui-how-send-documents-email.md)  
[Anpassen [!INCLUDE[d365fin](includes/d365fin_md.md)] Erweiterungen nutzen](ui-extensions.md)  
[Nutzen von [!INCLUDE[d365fin](includes/d365fin_md.md)] als Ihr Unternehmenspostfach in Outlook](admin-outlook.md)  
[Abrufen von [!INCLUDE[d365fin](includes/d365fin_md.md)] auf meinem mobilen Gerät](install-mobile-app.md)
