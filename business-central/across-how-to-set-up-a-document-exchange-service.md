---
title: 'Gewusst wie: Einrichten eine Belegaustauschdienstes | Microsoft Docs'
description: Sie verwenden einen externen Anbieter zum Austausch elektronischer Belege mit Ihren Handelspartnern.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 84d985bb329f76c9c4954e56a01f9d6c7f8bc09c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916193"
---
# <a name="set-up-a-document-exchange-service"></a>So richten Sie einen Belegaustauschdienst ein
Sie verwenden einen externen Anbieter zum Austausch elektronischer Belege mit Ihren Handelspartnern. Weitere Informationen finden Sie unter [Daten elektronisch austauschen](across-data-exchange.md).  

## <a name="to-set-up-a-document-exchange-service"></a>So richten Sie einen Belegaustauschdienst ein  
1. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Was möchten Sie tun?"), und geben Sie **Doc. Exch. Service-Einrichtung** , und wählen Sie dann den entsprechenden Link.  
2. Füllen Sie die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Beschreibung|  
    |---------------------------------|---------------------------------------|  
    |**Benutzeragent**|Geben Sie beliebigen Text ein, über den Sie Ihr Unternehmen im Belegaustauschdienst identifizieren können|  
    |**Tenant-ID Belegaustausch**|Geben Sie den Tenant beim Belegaustauschdienst an, der Ihrem Unternehmen entspricht. Dieser wird vom Anbieter des Belegaustauschdienstes bereitgestellt.|  
    |**Aktiviert**|Legen Sie fest, ob der Belegaustauschdienst aktiviert ist. **Hinweis:**  Sobald Sie den Service aktivieren, werden mindestens zwei Aufgabenwarteschlangenposten erstellt, um den Verkehr von elektronischen Belegen zu und von [!INCLUDE[d365fin](includes/d365fin_md.md)] zu verarbeiten. Wenn Sie den Service deaktivieren, werden die Projektwarteschlangenposten gelöscht.|  
    |**Anmeldungs-URL**|Geben Sie die Webseite an, auf der Sie sich für den Belegaustauschdienst anmelden.|  
    |**Dienste-URL**|Geben Sie die Adresse des Belegaustauschdienst an, die aufgerufen wird, wenn Sie elektronische Belege versenden und erhalten.|  
    |**Anmelde-URL**|Geben Sie die Anmeldeseite für den Belegaustauschdienst an. Hier geben Sie den Benutzernamen und das Kennwort Ihres Unternehmens für die Anmeldung beim Service ein.|  
    |**Verbraucherschlüssel**|Geben Sie den dreiteiligen OAuth-Schlüssel für den Consumer-Schlüssel ein. Dieser wird vom Anbieter des Belegaustauschdienstes bereitgestellt.|  
    |**Verbrauchergeheimschlüssel**|Geben Sie das Geheimnis ein, das den Consumer-Schlüssel schützt. Dieser wird vom Anbieter des Belegaustauschdienstes bereitgestellt.|  
    |**Token**|Geben Sie den dreiteiligen OAuth-Schlüssel für das Token ein. Dieser wird vom Anbieter des Belegaustauschdienstes bereitgestellt.|  
    |**Tokengeheimschlüssel**|Geben Sie das Geheimnis ein, das das Token schützt. Dieser wird vom Anbieter des Belegaustauschdienstes bereitgestellt.|  

    > [!NOTE]  
    > Sie informieren Daten werden verschlüsselt automatisch an.

## <a name="see-also"></a>Siehe auch  
[Datenaustausch einrichten](across-set-up-data-exchange.md)  
[Daten elektronisch austauschen](across-data-exchange.md)
