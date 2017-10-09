---
title: "So geht es: Aufträge mit XBRL erstellen | Microsoft Docs"
description: "XBRL (eXtensible Business Reporting Language) ist eine XML-basierte Sprache zum Kennzeichnen von Finanzdaten, dies es Unternehmen ermöglicht, Daten effizient und genau zu verarbeiten und freizugeben."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9034287316f4d2c3f110182edf7676934453015d
ms.contentlocale: de-de
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-reports-with-xbrl"></a><span data-ttu-id="f846a-103">Vorgehensweise. Erstellen neuer Vertriebsanalyseberichte mit XBRL</span><span class="sxs-lookup"><span data-stu-id="f846a-103">How to: Create Reports with XBRL</span></span>
<span data-ttu-id="f846a-104">XBRL (eXtensible Business Reporting Language) ist eine XML-basierte Sprache zum Kennzeichnen von Finanzdaten, dies es Unternehmen ermöglicht, Daten effizient und genau zu verarbeiten und freizugeben.</span><span class="sxs-lookup"><span data-stu-id="f846a-104">XBRL, which stands for eXtensible Business Reporting Language, is an XML-based language for tagging financial data, and enabling businesses to efficiently and accurately process and share their data.</span></span> <span data-ttu-id="f846a-105">Die XBRL-Initiative ermöglicht die Erstellung globaler Finanzberichte durch verschiedene ERP-Softwareunternehmen und internationale Buchhaltungsorganisationen.</span><span class="sxs-lookup"><span data-stu-id="f846a-105">The XBRL initiative enables global financial reporting by numerous ERP software companies and international accounting organizations.</span></span> <span data-ttu-id="f846a-106">Das Ziel der Initiative ist es, einen Standard für die einheitlichen Berichterstellung der Finanzdaten für Banken, Investoren und Regierungsbehörden bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="f846a-106">The goal of the initiative is to provide a standard for the uniform reporting of financial information for banks, investors, and government authorities.</span></span> <span data-ttu-id="f846a-107">Solche Geschäftsberichte können Folgendes umfassen:</span><span class="sxs-lookup"><span data-stu-id="f846a-107">Such business reporting can include:</span></span>  

 <span data-ttu-id="f846a-108">• Finanzauswertungen</span><span class="sxs-lookup"><span data-stu-id="f846a-108">• Financial statements</span></span>  
 <span data-ttu-id="f846a-109">• Finanzinformationen</span><span class="sxs-lookup"><span data-stu-id="f846a-109">• Financial information</span></span>  
 <span data-ttu-id="f846a-110">• Finanzfremde Informationen</span><span class="sxs-lookup"><span data-stu-id="f846a-110">• Non-financial information</span></span>  
 <span data-ttu-id="f846a-111">• Behördliche Erklärungen, beispielsweise jährlich oder quartalsweise abzugebende Finanzauswertungen</span><span class="sxs-lookup"><span data-stu-id="f846a-111">• Regulatory filings, such as annual and quarterly financial statements</span></span>  

 [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f846a-112">Microsoft Dynamics NAV ermöglicht Unternehmen die Implementierung von Daten in XBRL. Die Unternehmen profitieren dadurch von der Flexibilität und Automatisierung, die Ihnen XBRL beim Sammeln und gemeinsamen Nutzen von Daten bietet.</span><span class="sxs-lookup"><span data-stu-id="f846a-112"> enables companies to implement data in XBRL, and take advantage of the flexibility and automation it provides for both collecting and sharing data.</span></span>  

## <a name="extensible-business-reporting-language"></a><span data-ttu-id="f846a-113">eXtensible Business Reporting Language</span><span class="sxs-lookup"><span data-stu-id="f846a-113">eXtensible Business Reporting Language</span></span>
<span data-ttu-id="f846a-114">XBRL (e **X**tensible **B**usiness **R**eporting **L**anguage) ist eine XML-basierte Sprache für das Finanzberichtswesen.</span><span class="sxs-lookup"><span data-stu-id="f846a-114">XBRL (e **X**tensible **B**usiness **R**eporting **L**anguage) is an XML-based language for financial reporting.</span></span> <span data-ttu-id="f846a-115">XBRL (eXtensible Business Reporting Language) ist eine XML-basierte Sprache für Finanzberichtswesen. XBRL ist ein Standard für alle Nutzer der Supply-Chain zur einheitlichen Finanzberichterstattung. Dazu können private Unternehmen, das Buchhaltungswesen, Verwaltungen, Analysten, Investmentfirmen, Kapitalmärkte und Kreditgeber als auch Dritte in Schlüsselpositionen wie Softwareentwickler und Datenverwalter gehören.</span><span class="sxs-lookup"><span data-stu-id="f846a-115">XBRL provides a standard for uniform reporting for all users of the financial information supply chain; such as public and private companies, the accounting profession, regulators, analysts, the investment community, capital markets and lenders, as well as key third parties such as software developers and data aggregators.</span></span>  

<span data-ttu-id="f846a-116">Taxonomien sind unter www.xbrl.org erhältlich. Auf der XBRL-Website können Sie Taxonomien herunterladen oder weitere Informationen erhalten.</span><span class="sxs-lookup"><span data-stu-id="f846a-116">Taxonomies are maintained by www.xbrl.org. You can download taxonomies or read more detailed information on the XBRL website.</span></span>  

<span data-ttu-id="f846a-117">Jemand, der Informationen über Ihre finanzielle Situation haben möchte, stellt Ihnen eine Taxonomie zur Verfügung (ein XML-Dokument), die ein oder mehrere Schema/ta enthält, in denen ein oder mehrere Zeilen ausgefüllt werden können. Die Zeilen entsprechen den individuellen Finanzfakten, die vom Sender verlangt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-117">Someone who wants financial information from you, provides you with a taxonomy (an XML document) containing one or more schemas, each with one or more lines to fill out. The lines correspond to the individual financial facts required by the sender.</span></span> <span data-ttu-id="f846a-118">Sie importieren diese Taxonomie in Ihre Anwendung und füllen dann das/die Schema/ta aus, indem Sie eingeben, welche/s Konto/Konten der jeweiligen Zeile entspricht, welcher Zeitrahmen benutzt wird, z. B. Bewegung oder Saldo bis Datum.</span><span class="sxs-lookup"><span data-stu-id="f846a-118">You import this taxonomy into the program and then fill out the schema(s) by entering which account or accounts correspond to each line, what kind of timeframe to use, for example net change or balance at date.</span></span> <span data-ttu-id="f846a-119">In einigen Fällen können Sie ersatzweise eine Konstante eingeben wie z. B. die Mitarbeiteranzahl.</span><span class="sxs-lookup"><span data-stu-id="f846a-119">In some cases you can enter a constant instead, for example, number of employees.</span></span> <span data-ttu-id="f846a-120">Nun können Sie das Instance Document (ein XML-Dokument) an denjenigen schicken, der die Informationen angefordert hat.</span><span class="sxs-lookup"><span data-stu-id="f846a-120">You are now ready to send the instance document (an XML document) to the someone who requests the information.</span></span> <span data-ttu-id="f846a-121">Der Gedanke dahinter ist, dass sich dieser Vorgang mehrmals wiederholen kann, so dass Sie, trotz eventueller Änderungen an der Taxonomie, nur neue Instance Documents für andere Zeiträume exportieren müssen.</span><span class="sxs-lookup"><span data-stu-id="f846a-121">The idea is that this might be a recurring event, so unless changes have been made to the taxonomy, you just export new instance documents for new periods on request.</span></span>  

## <a name="xbrl-is-comprised-of-the-following-components"></a><span data-ttu-id="f846a-122">XBRL besteht aus den folgenden Komponenten</span><span class="sxs-lookup"><span data-stu-id="f846a-122">XBRL is comprised of the following components</span></span>  
<span data-ttu-id="f846a-123">Die XBRL **Spezifikation** erklärt, was XBRL ist, wie XBRL Instance Documents und XBRL-Taxonomien erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-123">The XBRL **Specification** explains what XBRL is, how to build XBRL instance documents and XBRL taxonomies.</span></span> <span data-ttu-id="f846a-124">Die XBRL-Spezifikation erklärt XBRL mit technischen Ausdrücken und ist für Techniker gedacht.</span><span class="sxs-lookup"><span data-stu-id="f846a-124">The XBRL Specification explains XBRL in technical terms and is intended for a technical audience.</span></span>  

<span data-ttu-id="f846a-125">Die XBRL **Schemata** sind die niederen Kernelemente von XBRL.</span><span class="sxs-lookup"><span data-stu-id="f846a-125">The XBRL **Schema** are the core low-level components of XBRL.</span></span> <span data-ttu-id="f846a-126">Das Schema ist die physikalische XSD-Datei, die wiedergibt, wie Instance Documents und Taxonomien erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-126">The schema is the physical XSD file which express how instance documents and taxonomies are to be built.</span></span>  

<span data-ttu-id="f846a-127">Bei den XBRL- **Linkbases** handelt es sich um physische XML-Dateien, die Informationen über die Elemente enthalten, die im XBRL-Schema definiert sind, wie z. B. Labels in einer oder mehreren Sprachen, wie Elemente summiert werden etc.</span><span class="sxs-lookup"><span data-stu-id="f846a-127">The XBRL **Linkbases** are the physical XML files which contain various information about the elements defined in the XBRL Schema, such as labels in one or more languages, how they relate to each other, how to sum up elements, etc.</span></span>  

<span data-ttu-id="f846a-128">Eine XBRL- **Taxonomie** ist ein "Vokabular" oder ein "Wörterbuch", das von einer Gruppe in Einklang mit den XBRL-Spezifikationen erstellt wurde, um Geschäftsinformationen auszutauschen.</span><span class="sxs-lookup"><span data-stu-id="f846a-128">An XBRL **Taxonomy** is a "vocabulary" or "dictionary" created by a group, compliant with the XBRL Specification, in order to exchange business information.</span></span>  

<span data-ttu-id="f846a-129">Ein XBRL **Instance Document** ist ein Geschäftsbericht, wie ein Finanzbericht, für die XBRL-Spezifikation.</span><span class="sxs-lookup"><span data-stu-id="f846a-129">An XBRL **Instance document** is a business report, such as a financial statement prepared to the XBRL specification.</span></span> <span data-ttu-id="f846a-130">Die Bedeutung der Werte in dem Dokument werden durch die Taxonomie erklärt.</span><span class="sxs-lookup"><span data-stu-id="f846a-130">The meaning of the values in the instance document is explained by the taxonomy.</span></span> <span data-ttu-id="f846a-131">Ein Instance Document ist so gut wie nutzlos, wenn Sie nicht wissen, für welche Taxonomie es erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f846a-131">An instance document is somewhat useless unless you know the taxonomy to which it is prepared.</span></span>  

## <a name="layered-taxonomies"></a><span data-ttu-id="f846a-132">Geschichtete Taxonomien</span><span class="sxs-lookup"><span data-stu-id="f846a-132">Layered Taxonomies</span></span>  
<span data-ttu-id="f846a-133">Eine Taxonomie kann aus einer Grundtaxonomie, z .B. US-GAAP oder IAS, und einer oder mehreren Erweiterungen bestehen.</span><span class="sxs-lookup"><span data-stu-id="f846a-133">A taxonomy can consist of a base taxonomy, for example, us-gaap or IAS, and then have one or more extensions.</span></span> <span data-ttu-id="f846a-134">Aus diesem Grund bezieht sich eine Taxonomie auf mehrere Schemata (oder ein einzelnes), die alle separate Taxonomien sind.</span><span class="sxs-lookup"><span data-stu-id="f846a-134">To reflect this, a taxonomy refers to one or more schemas which all are separate taxonomies.</span></span> <span data-ttu-id="f846a-135">Wenn die zusätzlichen Taxonomien in die Datenbank geladen werden, werden die neuen Elemente einfach an die bestehenden Elemente angehängt.</span><span class="sxs-lookup"><span data-stu-id="f846a-135">When the additional taxonomies are loaded into the database, the new elements are simply added to the end of the existing elements.</span></span>  

## <a name="linkbases"></a><span data-ttu-id="f846a-136">Linkbases</span><span class="sxs-lookup"><span data-stu-id="f846a-136">Linkbases</span></span>  
 <span data-ttu-id="f846a-137">In XBRL Spez. 2 wird die Taxonomie in verschiedenen XML-Dateien beschrieben.</span><span class="sxs-lookup"><span data-stu-id="f846a-137">In XBRL Spec. 2, the taxonomy is described in several XML-files.</span></span> <span data-ttu-id="f846a-138">Die erste XML-Datei ist die Taxonomieschemadatei selbst (.xsd-Datei), die lediglich eine ungeordnete Liste von Elementen oder Informationen für den Bericht enthält.</span><span class="sxs-lookup"><span data-stu-id="f846a-138">The primary XML file is the taxonomy schema file itself (.xsd file) which only contains an unordered list of elements or facts to be reported.</span></span> <span data-ttu-id="f846a-139">Zusätzlich sind normalerweise einige Linkbasedateien (.xml) damit verknüpft.</span><span class="sxs-lookup"><span data-stu-id="f846a-139">In addition to this, there are usually associated some linkbase files (.xml).</span></span> <span data-ttu-id="f846a-140">Die Linkbasedateien enthalten Daten, die die einfache Taxonomie (.xsd-Datei) vervollständigen.</span><span class="sxs-lookup"><span data-stu-id="f846a-140">The linkbase files contain data which is complementary to the raw taxonomy (.xsd file).</span></span> <span data-ttu-id="f846a-141">Es gibt sechs Arten von Linkbase-Dateien, von denen vier für  XBRL Produktnamen von Bedeutung sind.</span><span class="sxs-lookup"><span data-stu-id="f846a-141">There are six types of linkbases files of which four have relevance for Product Name XBRL.</span></span> <span data-ttu-id="f846a-142">Und zwar:</span><span class="sxs-lookup"><span data-stu-id="f846a-142">These are:</span></span>  

-   <span data-ttu-id="f846a-143">Beschriftungslinkbase: Diese Linkbase enthält Beschriftungen oder Namen für die Elemente.</span><span class="sxs-lookup"><span data-stu-id="f846a-143">Label linkbase: This linkbase contains labels or names for the elements.</span></span> <span data-ttu-id="f846a-144">Die Datei enthält möglicherweise Beschriftungen in verschiedenen Sprachen, die mit einer XML-Eigenschaft namens "lang" identifiziert werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-144">The file may contain labels in different languages which are identified with an XML property called 'lang'.</span></span> <span data-ttu-id="f846a-145">Die XML-Sprachen-ID enthalten normalerweise eine zweibuchstabige Abkürzung, und obwohl es einfach sein sollte, zu beurteilen, was die Abkürzung bedeutet, gibt es keine Verbindung zum Windows-Sprachcode oder zu den Sprachcodes, die in den Demodaten definiert werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-145">The XML language identifier usually contains a two-letter abbreviation, and although it should be easy to guess what the abbreviation means, there is no connection to the Windows language code or to the language codes defined in the demo data.</span></span> <span data-ttu-id="f846a-146">Wenn der Benutzer daher die Sprachen nach einer bestimmten Taxonomie durchsucht, sieht er alle Beschriftungen für das erste Element in der Taxonomie, was bedeutet, dass er ein Beispiel jeder Sprache anzeigen kann.</span><span class="sxs-lookup"><span data-stu-id="f846a-146">Therefore, when the user looks up the languages for a specific taxonomy, he will see all the labels for the first element in the taxonomy, meaning that he can then see an example of each language.</span></span> <span data-ttu-id="f846a-147">Eine Taxonomie kann mehrere Beschriftungslinkbases haben, die damit verknüpft werden, solange diese Linkbases unterschiedliche Sprachen enthalten.</span><span class="sxs-lookup"><span data-stu-id="f846a-147">A taxonomy can have several label linkbases attached to it as long as these linkbases contain different languages.</span></span>  

-   <span data-ttu-id="f846a-148">Darstellungslinkbase: Diese Linkbase enthält Informationen zur Elementstruktur, genauer gesagt, Informationen darüber, wie der Ersteller der Taxonomie möchte, dass die Anwendung dem Anwender die Taxonomie darstellen soll.</span><span class="sxs-lookup"><span data-stu-id="f846a-148">Presentation linkbase: This linkbase contains information about the structure of the elements, or more precisely; how the issuer of the taxonomy suggests that the program presents the taxonomy to the user.</span></span> <span data-ttu-id="f846a-149">Die Linkbase enthält eine Reihe von Verknüpfungen, die jeweils zwei Elemente als über- und untergeordnet verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="f846a-149">The linkbase contains a series of links that each connect two elements as parent and child.</span></span> <span data-ttu-id="f846a-150">Bei der Anwendung dieser Verknüpfungen können die Elemente hierarchisch dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-150">When applying all these links, the elements can be shown in a hierarchical way.</span></span> <span data-ttu-id="f846a-151">Beachten Sie, dass die Darstellungslinkbase nur das behandelt: Die Darstellung der Elemente für den Anwender.</span><span class="sxs-lookup"><span data-stu-id="f846a-151">Note that the presentation linkbase deals with just that: the presentation of elements to the user.</span></span>  

-   <span data-ttu-id="f846a-152">Berechnungslinkbase: Diese Linkbase enthält Informationen darüber, welche Elemente übernommen werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-152">Calculation linkbase: This linkbase contains information about which elements roll up to which.</span></span> <span data-ttu-id="f846a-153">Die Struktur ähnelt der der Darstellungslinkbase, mit der Ausnahme, dass jeder Link oder "Bogen" über eine "Weight"(Gewicht)-Eigenschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="f846a-153">The structure is quite similar to the presentation linkbase, except that each link or ‘arc’, as they are called, has a weight property.</span></span> <span data-ttu-id="f846a-154">Das Gewicht kann entweder 1 oder -1 betragen und damit anzeigen, ob das Element zu seinem übergeordneten Element addiert oder von ihm subtrahiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f846a-154">The weight can be either 1 or –1 indicating whether the element should be added to or subtracted from its parent.</span></span> <span data-ttu-id="f846a-155">Beachten Sie, dass die Roll-ups für die visuelle Darstellung nicht notwendig sind.</span><span class="sxs-lookup"><span data-stu-id="f846a-155">Note that the rollups are not necessarily in keeping with the visual presentation.</span></span>  

-   <span data-ttu-id="f846a-156">Referenzlinkbase: Bei dieser Linkbase handelt es sich um eine XML-Datei, die zusätzliche Informationen über die Daten enthält, die vom Anwender der Taxonomie benötigt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-156">Reference linkbase: This linkbase is an xml file that contains supplementary information about the data that is required by the taxonomy issuer.</span></span>

## <a name="to-set-up-xbrl-lines"></a><span data-ttu-id="f846a-157">XBRL-Zeilen einrichten:</span><span class="sxs-lookup"><span data-stu-id="f846a-157">To set up XBRL lines</span></span>  
<span data-ttu-id="f846a-158">Nach dem Importieren oder der Aktualisierung der Taxonomie müssen die Zeilen der Schemata mit allen nötigen Informationen gefüllt werden.</span><span class="sxs-lookup"><span data-stu-id="f846a-158">After you import or update the taxonomy, the lines of the schemas must be supplied with all the information that is required.</span></span> <span data-ttu-id="f846a-159">Diese Informationen beinhalten die Unternehmensdaten, die Finanzinformationen, Bemerkungen zu den Finanzinformationen, zusätzliche Schemata und andere Informationen, die zum Erfüllen der bestimmten Anforderungen des Finanzberichtes notwendig sind.</span><span class="sxs-lookup"><span data-stu-id="f846a-159">This information will include basic company information, the actual financial statements, notes to the financial statements, supplemental schedules, and other information that is required to satisfy the particular financial reporting requirements.</span></span>  

<span data-ttu-id="f846a-160">Sie richten die XBRL-Zeilen ein, indem Sie die Daten in der Taxonomie Ihren Daten in der Finanzbuchhaltung zuordnen.</span><span class="sxs-lookup"><span data-stu-id="f846a-160">You set up the XBRL Lines by mapping the data in the taxonomy to the data in your general ledger.</span></span>  

1.  <span data-ttu-id="f846a-161">Wählen Sie ![Nach Seite oder Bericht suchen(media/ui-search/search_small.png "Nach Seiten- oder Berichtsymbol suchen")] und geben **XBRL-Taxonomien** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-161">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **XBRL Taxonomies**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f846a-162">Im Fenster **XBRL-Taxonomies** wählen Sie eine Taxonomie in der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-162">In the **XBRL Taxonomies** window, select a taxonomy from the list.</span></span>  
3.  <span data-ttu-id="f846a-163">Wählen Sie die Aktion **Zeilen** aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-163">Choose the **Lines** action.</span></span>  
4.  <span data-ttu-id="f846a-164">Wählen Sie eine Zeile und füllen Sie die Felder aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-164">Select a line and fill in the fields.</span></span>   
5.  <span data-ttu-id="f846a-165">Durch Klicken auf die Aktion **Information** können Sie die Detailinformationen lesen.</span><span class="sxs-lookup"><span data-stu-id="f846a-165">To read detailed information about what to fill in, choose the **Information** action.</span></span>  
6.  <span data-ttu-id="f846a-166">Um die Sachkonten aus dem Kontenplan den XBRL-Zeilen zuzuordnen, klicken Sie auf **Verknüpfte Finanzbuchhaltungszeile**.</span><span class="sxs-lookup"><span data-stu-id="f846a-166">To set up the mapping of the general ledger accounts in the chart of accounts to the XBRL lines, choose the **G/L Map Lines** action.</span></span>  
7.  <span data-ttu-id="f846a-167">Um dem Finanzbericht eine Notiz hinzuzufügen, wählen Sie die **Notizen** Aktion.</span><span class="sxs-lookup"><span data-stu-id="f846a-167">To add notes to the financial statement, choose the **Notes** action.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f846a-168">Sie können nur Daten exportieren, die der Herkunftsart entsprechen, die Sie in dem Feld **Herkunftsart** ausgewählt haben, einschließlich Beschreibung und Notizen.</span><span class="sxs-lookup"><span data-stu-id="f846a-168">You can only export data that correspond to the source type you have selected in the **Source Type** field that includes description and notes.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f846a-169">Unwichtige Zeilen können als **NICHT ANWENDBAR** gekennzeichnet werden und werden dann nicht exportiert.</span><span class="sxs-lookup"><span data-stu-id="f846a-169">Lines that are not relevant can be marked as line type **NOT APPLICABLE** so the lines are not exported.</span></span>

 ## <a name="to-import-an-xbrl-taxonomy"></a><span data-ttu-id="f846a-170">Importieren von XBRL-Taxonomien</span><span class="sxs-lookup"><span data-stu-id="f846a-170">To import an XBRL taxonomy</span></span>  
<span data-ttu-id="f846a-171">Der erste Schritt, um mit der XBRL-Funktionalität arbeiten zu können, ist, die Taxonomie in Ihre Datenbank zu importieren.</span><span class="sxs-lookup"><span data-stu-id="f846a-171">The first step in working with the XBRL functionality is to import the taxonomy into your company database.</span></span> <span data-ttu-id="f846a-172">Eine Taxonomie besteht aus einem oder mehreren Schema/ta und einigen Linkbases.</span><span class="sxs-lookup"><span data-stu-id="f846a-172">A taxonomy consists of one or more schemas and some linkbases.</span></span> <span data-ttu-id="f846a-173">Wenn Sie den Import des/der Schemas/Schemata und Linkbases durchgeführt haben und die Linkbases dem Schema zugewiesen haben, können Sie die Zeilen einrichten und die Sachkonten des Kontenplans den entsprechenden Taxonomiezeilen zuordnen.</span><span class="sxs-lookup"><span data-stu-id="f846a-173">After you have completed the import of both schemas and linkbases and have applied the linkbases to the schema, you can set up the lines and map the general ledger accounts in the chart of accounts to the appropriate taxonomy lines.</span></span>  

1.  <span data-ttu-id="f846a-174">Wählen Sie ![Nach Seite oder Bericht suchen(media/ui-search/search_small.png "Nach Seiten- oder Berichtsymbol suchen")] und geben **XBRL-Taxonomien** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-174">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **XBRL Taxonomies**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f846a-175">Erstellen Sie im Fenster **XBRL Taxonomie** eine neue Zeile, und geben Sie Name und Beschreibung der Taxonomie ein.</span><span class="sxs-lookup"><span data-stu-id="f846a-175">In the **XBRL Taxonomies** window, create a new line and enter the name and description of the taxonomy.</span></span>  
3.  <span data-ttu-id="f846a-176">Klicken Sie auf **Schemas** und fügen Sie die Beschreibung für das Schema ein.</span><span class="sxs-lookup"><span data-stu-id="f846a-176">Choose the **Schemas** action, and then insert the description of the schema.</span></span>  
4.  <span data-ttu-id="f846a-177">Um das Schema zu importieren, wählen Sie im Fenster **XBRL-Schemata** auf der Registerkarte **Importieren** und wählen Sie dann einen Ordner und eine XSD-Datei aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-177">To import the schema, in the **XBRL Schemas** window, choose the **Import** action, and the select a folder and an XSD file.</span></span> <span data-ttu-id="f846a-178">Wählen Sie die Schaltfläche **Öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-178">Choose the **Open** button.</span></span>  
5.  <span data-ttu-id="f846a-179">Um die Linkbase zu importieren, wählen Sie im Fenster **XBRL-Schemata** auf der Registerkarte **Importieren** und wählen Sie dann einen Ordner und eine XML-Datei aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-179">To import the linkbase, in the **XBRL Schemas** window, choose the **Linkbases** action, and then select a folder and an XML file.</span></span> <span data-ttu-id="f846a-180">Wählen Sie die Schaltfläche **Öffnen** aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-180">Choose the **Open** button..</span></span>  
6.  <span data-ttu-id="f846a-181">Jetzt können Sie die Linkbase auf das Schema anwenden.</span><span class="sxs-lookup"><span data-stu-id="f846a-181">You can now choose to apply the linkbase to the schema.</span></span> <span data-ttu-id="f846a-182">Wiederholen Sie den Vorgang, bis Sie alle Linkbases importiert haben.</span><span class="sxs-lookup"><span data-stu-id="f846a-182">Repeat until you have imported all linkbases.</span></span>  
7. <span data-ttu-id="f846a-183">Wählen Sie die **Auf Taxonomie anwenden** Aktion aus, um die Linkbase auf das Schema anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="f846a-183">Choose the **Apply to Taxonomy** action to apply the linkbase to the schema.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="f846a-184">Anstatt die Linkbases einzeln nach dem Import anzuwenden, können Sie warten, bis Sie alle Linkbases importiert haben, und sie dann alle gleichzeitig anwenden.</span><span class="sxs-lookup"><span data-stu-id="f846a-184">Instead of individually applying the linkbases after the import, you can wait until you have imported all linkbases and then apply them at the same time.</span></span> <span data-ttu-id="f846a-185">Dazu wählen Sie die Schaltfläche **NEIN**, wenn sie aufgefordert werden, die neu importierte Linkbase auf das Schema anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="f846a-185">To do this, choose the **NO** button when you are prompted to apply the newly imported linkbase to the schema.</span></span> <span data-ttu-id="f846a-186">Wählen Sie dann die Zeilen mit den Linkbases aus, die Sie anwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="f846a-186">Then select the lines with the linkbases that you want to apply.</span></span>  

## <a name="to-update-an-xbrl-taxonomy"></a><span data-ttu-id="f846a-187">Um eine XBRL-Taxonomie zu aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f846a-187">To update an XBRL taxonomy</span></span>  
<span data-ttu-id="f846a-188">Wenn sich eine Taxonomie ändert, müssen Sie die aktuelle Taxonomie dementsprechend ändern.</span><span class="sxs-lookup"><span data-stu-id="f846a-188">When a taxonomy changes you need to update the current taxonomy accordingly.</span></span> <span data-ttu-id="f846a-189">Der Grund für die Aktualisierung kann ein verändertes Schema, eine veränderte Linkbase oder eine neue Linkbase sein.</span><span class="sxs-lookup"><span data-stu-id="f846a-189">The reason for the update can be an altered schema, an altered linkbase, or a new linkbase.</span></span> <span data-ttu-id="f846a-190">Nach Aktualisierung der Taxonomie müssen Sie nur die Zeilen an die geänderten oder neuen Zeilen anpassen.</span><span class="sxs-lookup"><span data-stu-id="f846a-190">After updating the taxonomy, you only need to map the lines for the changed or new lines.</span></span>  

1.  <span data-ttu-id="f846a-191">Wählen Sie ![Nach Seite oder Bericht suchen(media/ui-search/search_small.png "Nach Seiten- oder Berichtsymbol suchen")] und geben **XBRL-Taxonomien** ein und wählen dann den zugehörigen Link aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-191">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **XBRL Taxonomies**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f846a-192">Wählen Sie im Fenster **XBRL-Taxonomien** die Aktion **Schemas** aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-192">In the **XBRL Taxonomies** window, choose the **Schemas** action.</span></span>  
3.  <span data-ttu-id="f846a-193">Wählen Sie zum Aktualisieren des Schemas das zu aktualisierende Schema aus, und klicken Sie auf **Importieren**.</span><span class="sxs-lookup"><span data-stu-id="f846a-193">To update a schema, select the schema you want to update, and then choose the **Import** action.</span></span>  
4.  <span data-ttu-id="f846a-194">Um eine neue Linkbase zu aktualisieren oder hinzuzufügen, wählen Sie **Linkbases** aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-194">To update or add a new linkbase, choose the **Linkbases** action.</span></span>  
5.  <span data-ttu-id="f846a-195">Wählen Sie die gewünschte Linkbase aus oder drücken Sie STRG+N, um eine neue Zeile zu erhalten, wählen Sie die Art der Linkbase aus, und fügen Sie dann eine Beschreibung ein.</span><span class="sxs-lookup"><span data-stu-id="f846a-195">Select the relevant linkbase or press Ctrl+N for a new line, select the type of linkbase, and then insert a description.</span></span>  
6.  <span data-ttu-id="f846a-196">Um die Linkbase zu importieren, wählen Sie die **Importieren** Aktion aus.</span><span class="sxs-lookup"><span data-stu-id="f846a-196">To import the linkbase, choose the **Import** action.</span></span>  
7.  <span data-ttu-id="f846a-197">Wählen Sie die Schaltfläche **Ja** aus, um die Linkbase auf das Schema anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="f846a-197">Choose the **Yes** button to apply the linkbase to the schema.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f846a-198">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f846a-198">See Also</span></span>
<span data-ttu-id="f846a-199">[Finanzen](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="f846a-199">[Finance](finance.md)  </span></span>  
[<span data-ttu-id="f846a-200">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="f846a-200">Business Intelligence</span></span>](bi.md)  
<span data-ttu-id="f846a-201">[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f846a-201">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)](ui-work-product.md)</span></span>
