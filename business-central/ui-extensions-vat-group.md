---
title: Die Mehrwertsteuergruppenverwaltungserweiterung | Microsoft Docs
description: Sie können mit anderen Unternehmen zusammenarbeiten, um eine Mehrwertsteuergruppe zu bilden, und bei der Meldung der Mehrwertsteuer entweder als Mitglied oder als Vertreter der Gruppe fungieren.
author: bholtorf
manager: annbe
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: VAT, value added tax, report
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: 5dfadee976ce39e7d7ead2c09d907050682b4a7f
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989411"
---
# <a name="the-vat-group-management-extension"></a><span data-ttu-id="37654-103">Die Mehrwertsteuergruppenverwaltungserweiterung</span><span class="sxs-lookup"><span data-stu-id="37654-103">The VAT Group Management Extension</span></span>

<span data-ttu-id="37654-104">Sie können einem oder mehreren Unternehmen in Ihrem Land beitreten, um die Mehrwertsteuerberichterstattung unter einer einzigen Registrierungsnummer zu konsolidieren.</span><span class="sxs-lookup"><span data-stu-id="37654-104">You can join one or more businesses in your country to consolidate VAT reporting under a single registration number.</span></span> <span data-ttu-id="37654-105">Diese Art der Anordnung ist bekannt als *Mehrwertsteuergruppe* .</span><span class="sxs-lookup"><span data-stu-id="37654-105">This type of arrangement is known as a *VAT group* .</span></span> <span data-ttu-id="37654-106">Sie können mit der Gruppe als Mitglied oder als Gruppenvertreter zusammenarbeiten.</span><span class="sxs-lookup"><span data-stu-id="37654-106">You can engage with the group as a member or the group representative.</span></span>

## <a name="forming-a-vat-group"></a><span data-ttu-id="37654-107">Bildung einer Mehrwertsteuergruppe</span><span class="sxs-lookup"><span data-stu-id="37654-107">Forming a VAT Group</span></span>
<span data-ttu-id="37654-108">Mehrwertsteuergruppenmitglieder und der Gruppenvertreter können die Anleitung zur unterstützten Einrichtung für die **Mehrwertsteuergruppen-Verwaltungseinrichtung** verwenden, um ihre Zusammenarbeit mit der Gruppe zu definieren und eine Verbindung zwischen ihren [!INCLUDE[d365fin](includes/d365fin_md.md)]-Mandanten zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="37654-108">VAT group members and the group representative can use the **VAT Group Management Setup** assisted setup guide to define their engagement with the group, and create a connection between their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenants.</span></span> <span data-ttu-id="37654-109">Die Gruppenmitglieder verwenden die Verbindung, um ihre Mehrwertsteuererklärung an den Gruppenvertreter zu senden.</span><span class="sxs-lookup"><span data-stu-id="37654-109">The group members will use the connection to submit their VAT returns to the group representative.</span></span> <span data-ttu-id="37654-110">Der Vertreter übermittelt die Mehrwertsteuer an die Steuerbehörden im Auftrag der Gruppe mithilfe einer einzigen Mehrwertsteuererklärung.</span><span class="sxs-lookup"><span data-stu-id="37654-110">The representative will submit VAT to tax authorities on behalf of the group using a single VAT return.</span></span> 

## <a name="vat-group-constellations"></a><span data-ttu-id="37654-111">Mehrwertsteuergruppenkonstellationen</span><span class="sxs-lookup"><span data-stu-id="37654-111">VAT Group Constellations</span></span>
<span data-ttu-id="37654-112">Die Kommunikation erfolgt von den Gruppenmitgliedern mit dem Vertreter.</span><span class="sxs-lookup"><span data-stu-id="37654-112">Communication happens from group members to the representative.</span></span> <span data-ttu-id="37654-113">Der Gruppenvertreter stellt eine API zur Verfügung, mit der die Mitglieder ihre Mehrwertsteuererklärungen an den Mehrwertsteuergruppen-Vertreter übermitteln können.</span><span class="sxs-lookup"><span data-stu-id="37654-113">The group representative exposes an API that allows the members to submit their VAT returns to the VAT group representative.</span></span> 
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="37654-114">unterstützt die Übermittlung von Mehrwertsteuererklärungen innerhalb der Gruppe bei Unternehmen, die [!INCLUDE[d365fin](includes/d365fin_md.md)] lokal oder online verwenden oder irgendeine Kombination davon.</span><span class="sxs-lookup"><span data-stu-id="37654-114">supports inter-group VAT return submissions for companies using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises or online, and in any combination.</span></span> <span data-ttu-id="37654-115">Die Einrichtung der Kommunikation hängt von der Konstellation ab.</span><span class="sxs-lookup"><span data-stu-id="37654-115">The setup of the communication depends on the constellation.</span></span> <span data-ttu-id="37654-116">In den folgenden Abschnitten wird beschrieben, wie Sie verschiedene Gruppenkonstellationen einrichten.</span><span class="sxs-lookup"><span data-stu-id="37654-116">The following sections describe how to set up various group constellations.</span></span>

<span data-ttu-id="37654-117">Die folgende Liste zeigt die empfohlene Reihenfolge der Schritte zum Einrichten einer Mehrwertsteuergruppe:</span><span class="sxs-lookup"><span data-stu-id="37654-117">The following list shows the recommended order of the steps to set up a VAT group:</span></span>

1. <span data-ttu-id="37654-118">Erstellen Sie die Einrichtung in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="37654-118">Create the setup in Azure Active Directory.</span></span> <span data-ttu-id="37654-119">Weitere Informationen finden Sie unter [Anforderungen für die Authentifizierung](ui-extensions-vat-group.md#requirements-for-authentication).</span><span class="sxs-lookup"><span data-stu-id="37654-119">For more information, see [Requirements for Authentication](ui-extensions-vat-group.md#requirements-for-authentication).</span></span>
2. <span data-ttu-id="37654-120">Teilen Sie die technischen Informationen, die Mehrwertsteuergruppen-Mitglieder und die Vertreter benötigen, um ihre [!INCLUDE[d365fin](includes/d365fin_md.md)]-Mandanten zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="37654-120">Share the technical information that VAT group members and the representative need to connect their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenants.</span></span>

  <span data-ttu-id="37654-121">Normalerweise verfügt der Vertreter der Mehrwertsteuergruppe über diese Informationen, wie z. B. den Namen der Umgebung des Mehrwertsteuergruppenvertreters, an den die Mitglieder der Mehrwertsteuergruppe die Mehrwertsteuer übermitteln.</span><span class="sxs-lookup"><span data-stu-id="37654-121">Usually, the VAT group representative has this information, such as the name of the VAT group representative environment to which the VAT group members will submit VAT.</span></span>
3. <span data-ttu-id="37654-122">Erstellen Sie Benutzer im [!INCLUDE[d365fin](includes/d365fin_md.md)] des Mehrwertsteuergruppen-Vertreters, die Mehrwertsteuergruppen-Mitglieder verwenden können, um sich zu authentifizieren und eine Verbindung herzustellen.</span><span class="sxs-lookup"><span data-stu-id="37654-122">Create users in the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] that VAT group members can use to authenticate and connect.</span></span>
4. <span data-ttu-id="37654-123">Führen Sie die Anleitung zur unterstützten Einrichtung **Mehrwertsteuergruppenverwaltung einrichten** aus, um die Mitglieder der Mehrwertsteuergruppe zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="37654-123">Run the **Set up VAT Group Management** assisted setup guide to connect the VAT group members.</span></span>

  <span data-ttu-id="37654-124">Für die Anleitung sind einige Informationen vom Vertreter der Mehrwertsteuergruppe erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37654-124">The guide requires some information from the VAT group representative.</span></span> <span data-ttu-id="37654-125">Weitere Informationen finden Sie im Abschnitt [Einrichtung eines Mehrwertsteuergruppen-Mitglieds](#vat-group-member-setup).</span><span class="sxs-lookup"><span data-stu-id="37654-125">For more information, see the [VAT Group Member Setup](#vat-group-member-setup) section.</span></span> <span data-ttu-id="37654-126">Notieren Sie sich die **Gruppenmitglieds-ID** für jedes Mitglied der Mehrwertsteuergruppe.</span><span class="sxs-lookup"><span data-stu-id="37654-126">Make a note of the **Group Member ID** for each VAT group member.</span></span> <span data-ttu-id="37654-127">Der Vertreter benötigt diese IDs, um die Unternehmen der Mehrwertsteuergruppe hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="37654-127">The representative needs these IDs to add the companies to the VAT group.</span></span>
5. <span data-ttu-id="37654-128">Richten Sie die Erweiterung „Mehrwertsteuergruppenverwaltung“ im [!INCLUDE[d365fin](includes/d365fin_md.md)] des Mehrwertsteuergruppen-Vertreters ein, indem Sie die Anleitung zur unterstützten Einrichtung **Mehrwertsteuergruppenverwaltung einrichten** verwenden.</span><span class="sxs-lookup"><span data-stu-id="37654-128">Set up the VAT Group Management extension in the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Set up VAT Group Management** assisted setup guide.</span></span> 

> [!NOTE]
> <span data-ttu-id="37654-129">Um eine Verbindung zum Vertreter der Mehrwertsteuergruppe herzustellen, benötigen Gruppenmitglieder einen Benutzer mit Zugriff auf das [!INCLUDE[d365fin](includes/d365fin_md.md)] des Mehrwertsteuergruppenvertreters.</span><span class="sxs-lookup"><span data-stu-id="37654-129">To connect to the VAT group representative, group members need a user with access to the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="37654-130">Der Vertreter der Mehrwertsteuergruppe muss hierfür mindestens einen Benutzer erstellen. Aus Sicherheitsgründen empfehlen wir jedoch, für jedes Mitglied der Mehrwertsteuergruppe einen Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="37654-130">The VAT group representative must create at least one user for this, however, for security reasons we recommended that you create a user for each VAT group member.</span></span> <span data-ttu-id="37654-131">Stellen Sie sicher, dass Sie die Anmeldeinformationen für diese Benutzer auf sichere Weise an Mehrwertsteuergruppenmitglieder verteilen.</span><span class="sxs-lookup"><span data-stu-id="37654-131">Make sure to distribute the credentials for these users to VAT group members in a secure way.</span></span>

## <a name="understanding-the-vat-group-management-setup"></a><span data-ttu-id="37654-132">Grundlegendes zum Einrichten der Mehrwertsteuergruppenverwaltung</span><span class="sxs-lookup"><span data-stu-id="37654-132">Understanding the VAT Group Management Setup</span></span>

<span data-ttu-id="37654-133">Der Vertreter der Mehrwertsteuergruppe stellt eine API bereit, mit der Mitglieder der Mehrwertsteuergruppe eine zu ihrem [!INCLUDE[d365fin](includes/d365fin_md.md)]-Mandanten herstellen können und Mehrwertsteuererklärungen übermitteln können.</span><span class="sxs-lookup"><span data-stu-id="37654-133">The VAT group representative exposes an API that VAT group members can use to connect to their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant and submit VAT returns.</span></span> <span data-ttu-id="37654-134">Mehrwertsteuergruppenmitglieder werden [!INCLUDE[d365fin](includes/d365fin_md.md)] häufig in separaten Azure Active Directory-Mandanten verwenden.</span><span class="sxs-lookup"><span data-stu-id="37654-134">VAT group members will often use [!INCLUDE[d365fin](includes/d365fin_md.md)] in separate Azure Active Directory tenants.</span></span> <span data-ttu-id="37654-135">Daher sind weitere Einrichtungsvorgänge erforderlich, um eine Verbindung zwischen dem Mehrwertsteuergruppenmitglied und dem [!INCLUDE[d365fin](includes/d365fin_md.md)] des Vertreters herzustellen.</span><span class="sxs-lookup"><span data-stu-id="37654-135">Therefore, more setup is needed to make a connection between the VAT group member and representative's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> 
  
<span data-ttu-id="37654-136">Mitglieder der Mehrwertsteuergruppe stellen eine Verbindung zum Vertreter her, indem sie einen Webdienst im Mandanten des Mehrwertsteuergruppen-Vertreters aufrufen.</span><span class="sxs-lookup"><span data-stu-id="37654-136">VAT group members connect to the representative by calling a web service on the VAT group representative tenant.</span></span> <span data-ttu-id="37654-137">Der Aufrufer muss mithilfe von OAuth authentifiziert sein.</span><span class="sxs-lookup"><span data-stu-id="37654-137">The caller must be authenticated using OAuth.</span></span> <span data-ttu-id="37654-138">Wenn die Erweiterung „Mehrwertsteuergruppenverwaltung“ eingerichtet ist, werden Sie aufgefordert, sich beim Vertreter der Mehrwertsteuergruppe zu authentifizieren, um einen Zugriffstoken abzurufen und zu speichern.</span><span class="sxs-lookup"><span data-stu-id="37654-138">When the VAT Group Management extension is set up, you will be asked to authenticate to the VAT group representative to get and save an access token.</span></span> <span data-ttu-id="37654-139">Dieses Zugriffstoken wird verwendet, wenn Mehrwertsteuererklärungen an den Vertreter der Mehrwertsteuergruppe gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="37654-139">This access token is used when submitting VAT returns to the VAT group representative.</span></span> 

<span data-ttu-id="37654-140">Die Authentifizierung wird von Azure Active Directory abgewickelt. Daher muss Ihre Einrichtung im Azure Active Directory des Mehrwertsteuergruppen-Vertreters erfolgen, um Verbindungen zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="37654-140">Authentication is handled by Azure Active Directory, so your setup must be made in the VAT group representative's Azure Active Directory to allow connections.</span></span> <span data-ttu-id="37654-141">Eine Azure Active Directory-App-Registrierung muss mit Zugriff auf das [!INCLUDE[d365fin](includes/d365fin_md.md)] des Mehrwertsteuergruppenvertreters konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="37654-141">An Azure Active Directory app registration must be configured with access to the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="37654-142">Dies gilt auch, wenn der Vertreter der Mehrwertsteuergruppe [!INCLUDE[d365fin](includes/d365fin_md.md)] lokal verwendet.</span><span class="sxs-lookup"><span data-stu-id="37654-142">This is also true if the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises.</span></span> <span data-ttu-id="37654-143">Darüber hinaus müssen Sie „Einmaliges Anmelden“ konfigurieren, wenn der Vertreter der Mehrwertsteuergruppe [!INCLUDE[d365fin](includes/d365fin_md.md)] lokal verwendet.</span><span class="sxs-lookup"><span data-stu-id="37654-143">Additionally, you must configure Single Sign-On if the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises.</span></span>

> [!NOTE]
> <span data-ttu-id="37654-144">Für eine begrenzte Zeit wird auch die Authentifizierung mithilfe eines Webdienst-Zugriffsschlüssels unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37654-144">For a limited time, authentication using a web service access key is also supported.</span></span> <span data-ttu-id="37654-145">Weitere Informationen finden Sie unter [Veraltete Funktionen in 2021 Veröffentlichungzyklus 1](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#deprecated-features-in-2021-release-wave-1).</span><span class="sxs-lookup"><span data-stu-id="37654-145">For more information, see [Deprecated Features in 2021 release wave 1](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#deprecated-features-in-2021-release-wave-1).</span></span>

## <a name="requirements-for-authentication"></a><span data-ttu-id="37654-146">Voraussetzungen für die Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="37654-146">Requirements for Authentication</span></span> 
<span data-ttu-id="37654-147">Wenn der Vertreter der Mehrwertsteuergruppe [!INCLUDE[d365fin](includes/d365fin_md.md)] online oder lokal verwendet, verwenden Mehrwertsteuergruppenmitglieder Azure Active Directory, um sich zu authentifizieren, wenn sie Mehrwertsteuererklärungen an den Vertreter der Mehrwertsteuergruppe übermitteln.</span><span class="sxs-lookup"><span data-stu-id="37654-147">When the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] online or on-premises, VAT group members use Azure Active Directory to authenticate when they submit VAT returns to the VAT group representative.</span></span> <span data-ttu-id="37654-148">Wenn die Mehrwertsteuergruppenmitglieder ebenfalls [!INCLUDE[d365fin](includes/d365fin_md.md)] online verwenden, kann sich das Mehrwertsteuergruppenmitglied mithilfe der angegebenen Benutzeranmeldeinformationen und der Endpunktinformationen authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="37654-148">If the VAT group members are also using [!INCLUDE[d365fin](includes/d365fin_md.md)] online, the VAT group member can authenticate using the designated user credentials and the endpoint information.</span></span> <span data-ttu-id="37654-149">Weitere Informationen finden Sie unter [Mehrwertsteuergruppenmitglied-Einrichtung](ui-extensions-vat-group.md#vat-group-member-setup).</span><span class="sxs-lookup"><span data-stu-id="37654-149">For more information, see [VAT Group Member Setup](ui-extensions-vat-group.md#vat-group-member-setup).</span></span>

<span data-ttu-id="37654-150">Mehrwertsteuergruppenmitglieder, die [!INCLUDE[d365fin](includes/d365fin_md.md)] lokal haben, müssen eine App-Registrierung in Azure Active Directory für den [!INCLUDE[d365fin](includes/d365fin_md.md)]-Mandanten des Vertreters der Mehrwertsteuergruppe einrichten.</span><span class="sxs-lookup"><span data-stu-id="37654-150">VAT group members who have [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises must set up an app registration in Azure Active Directory for the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant.</span></span> <span data-ttu-id="37654-151">Die App-Registrierung ermöglicht es, dass mit [!INCLUDE[d365fin](includes/d365fin_md.md)] online des Mehrwertsteuergruppenvertreters das Gruppenmitglied authentifiziert werden kann.</span><span class="sxs-lookup"><span data-stu-id="37654-151">The app registration will enable the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] online to authenticate the group member.</span></span> <span data-ttu-id="37654-152">Weitere Informationen finden Sie unter [Schnellstart: Registrieren einer Anwendung mit der Microsoft-Identitätsplattform](/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="37654-152">For more information, see [Quickstart: Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app).</span></span>

<span data-ttu-id="37654-153">Wenn Sie die App-Registrierung in Azure Active Directory erstellen, müssen Sie Folgendes angeben.</span><span class="sxs-lookup"><span data-stu-id="37654-153">When you create the app registration in Azure Active Directory, you must specify the following.</span></span>

* <span data-ttu-id="37654-154">Im Abschnitt **Authentifizierung** fügen Sie **Web** als Plattform hinzu und verwenden die folgende **Umleitungs-URL** : https://businesscentral.dynamics.com/OAuthLanding.htm.</span><span class="sxs-lookup"><span data-stu-id="37654-154">In the **Authentication** section, add **Web** as a platform, and use the following **Redirect URL** : https://businesscentral.dynamics.com/OAuthLanding.htm.</span></span>
* <span data-ttu-id="37654-155">Im Abschnitt **Authentifizierung** in der Option zur Auswahl **Unterstützte Kontoarten** wählen Sie **Konten in einem beliebigen Organisationsverzeichnis (Beliebiges Azure AD-Verzeichnis – mandantenfähig)** .</span><span class="sxs-lookup"><span data-stu-id="37654-155">In the **Authentication** section, in the option to select **Supported account types** , select **Accounts in any organizational directory (Any Azure AD directory - Multitenant)** .</span></span>
* <span data-ttu-id="37654-156">Im Abschnitt **Zertifikate und Geheimschlüssel** erstellen Sie einen neuen geheimen Clientschlüssel und notieren den Wert.</span><span class="sxs-lookup"><span data-stu-id="37654-156">In the **Certificates & secrets** section, create a new client secret and note the value.</span></span> <span data-ttu-id="37654-157">Die Mehrwertsteuergruppenmitglieder benötigen den Geheimschlüssel, wenn Sie die Verbindung zum Gruppenvertreter einrichten.</span><span class="sxs-lookup"><span data-stu-id="37654-157">The VAT group members will need the secret when they set up the connection to the group representative.</span></span>
* <span data-ttu-id="37654-158">Im Abschnitt **API-Berechtigungen** fügen Sie Berechtigungen zu [!INCLUDE[d365fin](includes/d365fin_md.md)] hinzu.</span><span class="sxs-lookup"><span data-stu-id="37654-158">In the **API permissions** section, add permissions to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="37654-159">Aktivieren Sie den stellvertretenden Zugriff auf **Financials.ReadWrite.All** und **user_impersonation** .</span><span class="sxs-lookup"><span data-stu-id="37654-159">Enable delegated access to **Financials.ReadWrite.All** and **user_impersonation** .</span></span>
* <span data-ttu-id="37654-160">Im Abschnitt **Übersicht** notieren Sie die **Anwendungs-(Client)-ID** .</span><span class="sxs-lookup"><span data-stu-id="37654-160">In the **Overview** section, note the **Application (client) ID** .</span></span> <span data-ttu-id="37654-161">Die Mehrwertsteuergruppenmitglieder benötigen die ID, wenn Sie die Verbindung zum Gruppenvertreter einrichten.</span><span class="sxs-lookup"><span data-stu-id="37654-161">The VAT group members will need the ID when they set up the connection to the group representative.</span></span> 

## <a name="vat-group-member-setup"></a><span data-ttu-id="37654-162">Einrichtung des Mehrwertsteuergruppenmitglieds</span><span class="sxs-lookup"><span data-stu-id="37654-162">VAT Group Member Setup</span></span>
<span data-ttu-id="37654-163">Richten Sie das Mehrwertsteuergruppenmitglied ein, indem Sie die Anleitung zur unterstützten Einrichtung **Mehrwertsteuergruppenverwaltung einrichten** starten.</span><span class="sxs-lookup"><span data-stu-id="37654-163">Set up the VAT group member by starting the **Set up VAT Group Management** assisted setup guide.</span></span> 

> [!NOTE]
> <span data-ttu-id="37654-164">Bevor Sie beginnen, wenden Sie sich an den Vertreter der Mehrwertsteuergruppe für die folgenden Informationen über seinen [!INCLUDE[d365fin](includes/d365fin_md.md)]-Mandanten:</span><span class="sxs-lookup"><span data-stu-id="37654-164">Before you get started, contact the VAT group representative for the following information about their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant:</span></span>
>
> * <span data-ttu-id="37654-165">Die API-URL</span><span class="sxs-lookup"><span data-stu-id="37654-165">The API URL</span></span>
> * <span data-ttu-id="37654-166">Der Name seines Unternehmens</span><span class="sxs-lookup"><span data-stu-id="37654-166">The name of their company</span></span> 
> * <span data-ttu-id="37654-167">Client-ID</span><span class="sxs-lookup"><span data-stu-id="37654-167">Client ID</span></span>
> * <span data-ttu-id="37654-168">Geheimer Clientschlüssel</span><span class="sxs-lookup"><span data-stu-id="37654-168">Client secret</span></span>
> * <span data-ttu-id="37654-169">Anmeldeinformationen für den dedizierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="37654-169">Sign in credentials for the dedicated user</span></span> 

1. <span data-ttu-id="37654-170">Wählen Sie das Symbol ![Glühbirne, das die Funktion „Sie wünschen...“ öffnet](media/ui-search/search_small.png "Was möchten Sie tun?") aus, geben Sie **Mehrwertsteuergruppe** ein und wählen Sie dann den zugehörigen Link.</span><span class="sxs-lookup"><span data-stu-id="37654-170">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Group** , and then choose the related link.</span></span>
2. <span data-ttu-id="37654-171">Um die Mehrwertsteuer-Gruppenrolle des Unternehmens zu definieren, wählen Sie **Mitglied** und dann **Weiter** aus.</span><span class="sxs-lookup"><span data-stu-id="37654-171">To define the company's VAT group role, choose **Member** , and then choose **Next** .</span></span>
3. <span data-ttu-id="37654-172">Kopieren Sie den Wert des Felds **Gruppenmitglieds-ID** , und telen Sie ihn dann mit dem Vertreter der Mehrwertsteuergruppe, damit dieser Ihr Unternehmen als genehmigtes Mitglied der Gruppe hinzufügen kann.</span><span class="sxs-lookup"><span data-stu-id="37654-172">Copy the value of the **Group Member ID** field, and then share it with the VAT group representative so they can add your company as an approved member of the group.</span></span>
4. <span data-ttu-id="37654-173">Fügen Sie die **API-URL** vom Vertreter der Mehrwertsteuergruppe hinzu.</span><span class="sxs-lookup"><span data-stu-id="37654-173">Add the **API URL** from the VAT group representative.</span></span> <span data-ttu-id="37654-174">Normalerweise ist die URL wie folgt formatiert: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`.</span><span class="sxs-lookup"><span data-stu-id="37654-174">Typically, the URL is formatted as follows: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`.</span></span> <span data-ttu-id="37654-175">Zum Beispiel, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`.</span><span class="sxs-lookup"><span data-stu-id="37654-175">For example, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`.</span></span> 
5. <span data-ttu-id="37654-176">Fügen Sie den [!INCLUDE[d365fin](includes/d365fin_md.md)]-Unternehmensnamen des Vertreters der Mehrwertsteuergruppe hinzu, wie z. B. *CRONUS UK Ltd.* .</span><span class="sxs-lookup"><span data-stu-id="37654-176">Add the [!INCLUDE[d365fin](includes/d365fin_md.md)] company name of the VAT group representative, such as *CRONUS UK Ltd* .</span></span>
6. <span data-ttu-id="37654-177">Wählen Sie **Authentifizierungsart** , wählen Sie **OAuth2** und wählen Sie dann **Weiter** .</span><span class="sxs-lookup"><span data-stu-id="37654-177">Choose **Authentication Type** , choose **OAuth2** , and then choose **Next** .</span></span>
7. <span data-ttu-id="37654-178">Im Feld **Client-ID** geben Sie die vom Vertreter der Mehrwertsteuergruppe angegebene ID ein.</span><span class="sxs-lookup"><span data-stu-id="37654-178">In the **Client ID** field, enter the ID provided by the VAT group representative.</span></span>
8. <span data-ttu-id="37654-179">Im Feld **Vom Vertreter der Mehrwertsteuergruppe bereitgestellter geheimer Clientschlüssel** geben Sie den vom Vertreter der Mehrwertsteuergruppe bereitgestellten Geheimschlüssel an.</span><span class="sxs-lookup"><span data-stu-id="37654-179">In the **Client Secret provided by the VAT Group representative** field, enter the secret provided by the VAT group representative.</span></span>
9. <span data-ttu-id="37654-180">Im Feld **OAuth 2.0-Autoritätsendpunkt** geben Sie *https://login.microsoftonline.com/common/oauth2* ein.</span><span class="sxs-lookup"><span data-stu-id="37654-180">In the **OAuth 2.0 Authority Endpoint** field, enter *https://login.microsoftonline.com/common/oauth2* .</span></span>
10. <span data-ttu-id="37654-181">Im Feld **OAuth 2.0-Ressourcen-URL** geben Sie *https://api.businesscentral.dynamics.com/* ein.</span><span class="sxs-lookup"><span data-stu-id="37654-181">In the **OAuth 2.0 Resource URL** field, enter *https://api.businesscentral.dynamics.com/* .</span></span>
11. <span data-ttu-id="37654-182">Im Feld **OAuth 2.0-Umleitungs-URL** geben Sie *https://businesscentral.dynamics.com/OAuthLanding.htm* ein.</span><span class="sxs-lookup"><span data-stu-id="37654-182">In the **OAuth 2.0 Redirect URL** field, enter *https://businesscentral.dynamics.com/OAuthLanding.htm* .</span></span> 
12. <span data-ttu-id="37654-183">Wenn Sie die verschiedenen Felder angegeben haben, wählen Sie **Weiter** und geben Sie dann die Benutzeranmeldeinformationen ein, die vom Vertreter der Mehrwertsteuergruppe bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="37654-183">When you have specified the various fields, choose **Next** , and then enter the user credentials that were provided by the VAT group representative.</span></span>
13. <span data-ttu-id="37654-184">Wählen Sie die MwSt.-Berichtskonfiguration aus, die Sie verwenden, um die Mehrwertsteuer den Behörden in Ihrem Land zu melden.</span><span class="sxs-lookup"><span data-stu-id="37654-184">Choose the VAT report configuration that you use to report VAT to authorities in your country.</span></span>

  <span data-ttu-id="37654-185">Im Vereinigten Königreich würde beispielsweise die Konfiguration des Mehrwertsteuerberichts so eingerichtet, dass die Mehrwertsteuer an die HMRC gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="37654-185">For example, in the United Kingdom, the VAT report configuration would be set up to report VAT to HMRC.</span></span> <span data-ttu-id="37654-186">Die Erweiterung „Mehrwertsteuergruppenverwaltung“ kopiert diese Einrichtung, aber ersetzt die Übermittlungs-codeunit durch‌ eine solche, die die Übermittlung an den Vertreter der Mehrwertsteuergruppe anstelle an die Steuerbehörden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37654-186">The VAT Group Management extension copies this setup, but replaces the submission codeunit with one that supports submission to the VAT group representative rather than the tax authorities.</span></span> <span data-ttu-id="37654-187">Die codeunit wird von Microsoft bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="37654-187">The codeunit is provided by Microsoft.</span></span> <span data-ttu-id="37654-188">Wenn Sie fertig sind, wählen Sie **Weiter** .</span><span class="sxs-lookup"><span data-stu-id="37654-188">When done, choose **Next** .</span></span>

## <a name="using-the-vat-group-management-features"></a><span data-ttu-id="37654-189">Verwenden der Funktionen der Mehrwertsteuergruppenverwaltung</span><span class="sxs-lookup"><span data-stu-id="37654-189">Using the VAT Group Management Features</span></span>

<span data-ttu-id="37654-190">Mehrwertsteuergruppenmitglieder verwenden die Standardprozesse, um Mehrwertsteuererklärungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="37654-190">VAT group members use the standard processes to prepare VAT returns.</span></span> <span data-ttu-id="37654-191">Der einzige Unterschied ist die Auswahl der Berichtsversion **MEHRWERTSTEUERGRUPPE** , wodurch die Mehrwertsteuererklärung an den Vertreter der Mehrwertsteuergruppe und nicht an die Behörden übermittelt wird.</span><span class="sxs-lookup"><span data-stu-id="37654-191">The only difference is to choose the **VATGROUP** report version, which submits the VAT return to the VAT group representative rather than the authorities.</span></span> <span data-ttu-id="37654-192">Weitere Informationen finden sie unter [Informationen zum Mehrwertsteuererklärungsbericht](/business-central/finance-how-report-vat#about-the-vat-return-report).</span><span class="sxs-lookup"><span data-stu-id="37654-192">For more information, see [About the VAT Return Report](/business-central/finance-how-report-vat#about-the-vat-return-report).</span></span>

<span data-ttu-id="37654-193">In den folgenden Abschnitten werden die Aufgaben beschrieben, die Vertreter von Mehrwertsteuergruppen ausführen müssen.</span><span class="sxs-lookup"><span data-stu-id="37654-193">The following sections describe the tasks that VAT group representatives must perform.</span></span>

### <a name="vat-group-submissions"></a><span data-ttu-id="37654-194">Übermittlungen der MwSt.-Gruppe</span><span class="sxs-lookup"><span data-stu-id="37654-194">VAT Group Submissions</span></span>

<span data-ttu-id="37654-195">Auf der Seite **Übermittlungen der Mehrwertsteuergruppe** werden die von Mitgliedern übermittelten Mehrwertsteuererklärungen aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="37654-195">The **VAT Group Submissions** page lists the VAT returns that members have submitted.</span></span> <span data-ttu-id="37654-196">Die Seite dient als Entwurfsspeicherort für die Übermittlungen, bis der Vertreter der Mehrwertsteuergruppe sie in eine Mehrwertsteuererklärung für die Gruppe einbezieht.</span><span class="sxs-lookup"><span data-stu-id="37654-196">The page serves as a draft location for the submissions until the VAT group representative includes them in a VAT return for the group.</span></span> <span data-ttu-id="37654-197">Sie können die Übermittlungen öffnen, um die Mehrwertsteuer für die einzelnen vom Mehrwertsteuergruppenmitglied gemeldeten Felder zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="37654-197">You can open the submissions to review the VAT for the individual boxes reported by the VAT group member.</span></span>

### <a name="creating-a-group-vat-return"></a><span data-ttu-id="37654-198">Erstellen einer Gruppenmehrwertsteuererklärung</span><span class="sxs-lookup"><span data-stu-id="37654-198">Creating a Group VAT Return</span></span>

<span data-ttu-id="37654-199">Um die Mehrwertsteuer im Auftrag der Gruppe zu melden, erstellen Sie auf der Seite **Mehrwertsteuererklärungen** eine Mehrwertsteuererklärung nur für Ihr Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="37654-199">To report VAT on behalf of the group, on the **VAT Returns** page, create a VAT return for your company only.</span></span> <span data-ttu-id="37654-200">Fügen Sie anschließend die neuesten Mehrwertsteuerübermittlungen von Mehrwertsteuergruppenmitgliedern ein, indem Sie die Aktion **Gruppenmehrwertsteuer einschließen** wählen.</span><span class="sxs-lookup"><span data-stu-id="37654-200">Afterward, include the most recent VAT submissions from VAT group members by choosing the **Include Group VAT** action.</span></span>  

<span data-ttu-id="37654-201">Wenn die Mehrwertsteuererklärung des Vertreters der Mehrwertsteuergruppe den Behörden im Auftrag der gesamten Gruppe übermittelt wurde, führen Sie normalerweise die Aktion **MwSt.-Abrechnung berechnen und buchen** aus.</span><span class="sxs-lookup"><span data-stu-id="37654-201">When the VAT Group representative's VAT Return has been submitted to the authorities on behalf of the entire group, you will normally run the **Calculate and Post VAT Settlement** action.</span></span> <span data-ttu-id="37654-202">Die Aktion schließt offene MwSt.-Posten und überträgt Beträge zum MwSt.-Abrechnungskonto.</span><span class="sxs-lookup"><span data-stu-id="37654-202">This action closes open VAT Entries and transfers amounts to the VAT Settlement account.</span></span> <span data-ttu-id="37654-203">Derzeit werden bei dieser Aktion die Gruppenübermittlungen nicht berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="37654-203">Currently, this action does not take the group submissions into account.</span></span> <span data-ttu-id="37654-204">Dies bedeutet, dass nur die MwSt.-Posten des Unternehmens des Vertreters der Mehrwertsteuergruppe gebucht werden.</span><span class="sxs-lookup"><span data-stu-id="37654-204">This means that only the VAT Entries of the VAT Group representative company will be posted.</span></span> <span data-ttu-id="37654-205">Die Übermittlungsbeträge der Mehrwertsteuergruppenmitglieder müssen manuell zum MwSt.-Abrechnungsetrag hinzugebucht werden, damit das MwSt.-Abrechnungskonto des Vertreters der Mehrwertsteuergruppe die Verbindlichkeit dessen, was an die Behörden gemeldet wurde, widerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="37654-205">The VAT Group member submission amounts must be posted to the VAT settlement amount manually, so that the VAT Group representative's VAT Settlement account will reflect the liability of what was reported to authorities.</span></span> <span data-ttu-id="37654-206">Dieses Verhalten wird sich in einem bevorstehenden Update von [!INCLUDE[d365fin](includes/d365fin_md.md)] ändern, sodass die gesamte Gruppenmehrwertsteuer (der Totalbetrag der Berichtszeilen in der Mehrwertsteuererklärung) ausgeglichen wird.</span><span class="sxs-lookup"><span data-stu-id="37654-206">This behavior will change in an upcoming update of [!INCLUDE[d365fin](includes/d365fin_md.md)], so the entire group VAT (the Total Amount on Report Lines on the VAT Return) will be settled.</span></span> 

> [!NOTE]
> <span data-ttu-id="37654-207">Mitglieder der Mehrwertsteuergruppe können übermittelte Mehrwertsteuererklärungen korrigieren, solange der Gruppenvertreter die Mehrwertsteuererklärung für die Gruppe noch nicht herausgegeben hat.</span><span class="sxs-lookup"><span data-stu-id="37654-207">VAT group members can correct submitted VAT returns as long as the group representative has not released the VAT return for the group.</span></span> <span data-ttu-id="37654-208">Um eine Korrektur vorzunehmen, muss das Mitglied der Mehrwertsteuergruppe eine neue Mehrwertsteuererklärung für den Zeitraum der Mehrwertsteuererklärung erstellen und diese dem Vertreter der Mehrwertsteuergruppe übermitteln.</span><span class="sxs-lookup"><span data-stu-id="37654-208">To make a correction, the VAT group member must create a new VAT return for the VAT return period and submit it to the VAT group representative.</span></span> <span data-ttu-id="37654-209">Auf der Seite des Vertreters der Mehrwertsteuergruppe wird die aktuellste Mehrwertsteuererklärung auf der Seite **Mehrwertsteuererklärungen** eingefügt.</span><span class="sxs-lookup"><span data-stu-id="37654-209">On the VAT group representative's side, the latest VAT return will be included on the **VAT Returns** page.</span></span> 

## <a name="see-also"></a><span data-ttu-id="37654-210">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="37654-210">See Also</span></span>
[<span data-ttu-id="37654-211">Arbeiten mit MwSt im Verkauf und Einkauf</span><span class="sxs-lookup"><span data-stu-id="37654-211">Work with VAT on Sales and Purchases</span></span>](finance-work-with-vat.md)  
[<span data-ttu-id="37654-212">Mehrwertsteuer einrichten</span><span class="sxs-lookup"><span data-stu-id="37654-212">Set Up Value-Added Tax</span></span>](finance-setup-vat.md)