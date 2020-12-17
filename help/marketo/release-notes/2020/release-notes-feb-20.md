---
unique-page-id: 37355826
description: Versionsinformation -feb '20 - Marketo Docs - Produktdokumentation
title: Versionsinformation -feb '20
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Versionsinformation: Feb &#39;20 {#release-notes-feb}

Följande funktioner finns i utgåvan från 20 februari. Se om din Marketo-utgåva har funktioner tillgängliga.

>[!NOTE]
>
>**Tillgänglighet**
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/star-yellow.svg)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

***Kvartalsvisa*** utgåvorFöljande funktioner släpptes den 21  **februari 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics &quot;Change Owner in Microsoft&quot; Flow Action**: Behåll kontrollen över dina Microsoft Dynamics CRM-data med möjlighet att ändra en lead-/kontaktägare direkt från Marketo Engage. Detta är en förbättring av vår interna CRM-integreringsfunktion.
* **API:er för användarhantering: **Automatisera användar- och rollhanteringen via externa system för identitets- och organisationshantering. Detta är en förbättring av vår API-anropsfunktion.
* **API:er för anpassat objektschema: **Hantera och distribuera automatiskt anpassade objektscheman i olika instanser i Marketo Engage för att säkerställa att datamodeller är enhetliga i alla sälj- och marknadsföringsverktyg. Med detta API kan du definiera och testa anpassade objekt i en sandlåda eller i ett center av hög kvalitet och tillhandahålla så många instanser som behövs. Detta är en förbättring av vår API:s anropsfunktion. Kontakta din Marketo Engage-representant om du vill veta hur du får tillgång till den här förbättringen.
* **API:er för omdirigeringsregler för landningssidor**: Automatisera hanteringen av omdirigeringsregler för landningssidor. Detta är en förbättring av vår API-anropsfunktion.
* **Cachelagring** av formulärbeskrivare: Vi minskar inläsningstiden för inbäddade formulär och förbättrar den övergripande programstabiliteten genom att cachelagra formulär som resurser. Observera att det kan ta upp till fyra minuter att godkänna inbäddade formulär för att de ska visas på webben. Detta är en förbättring av vår förmåga till landningssidor och Forms.

<br> 

**

***Frigör under hela kvartalet***

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.
**Bizible ![(star)](assets/star-yellow.svg)

**

* **Kontobaserad segmentering**: Analysera attribuering på kontonivå med möjlighet att skapa segment och filter för Discover boards baserat på kontoattribut. Använd dessa segment för att fördjupa er i er kontobaserade marknadsföring.
* **Sparar filter**: Spara specifika kontrollpanelsfilter som är unika för varje användare för att analysera dem snabbt och konsekvent.
* **Exportera till PDF**: Dela värdefulla insikter i hela organisationen genom att exportera Bizible Dashboards som PDF:er.

## Säljanslutning {#sales-connect}

* **Disponera fönsteruppdateringar**: Vi har effektiviserat processen för att välja mallar och skicka e-postmeddelanden via Sales Connect. Använd Compose-fönstret i vår webbklient och Salesforce som en enda butik för säljare, med möjlighet att spara mallkategorier, schemalägga e-postmeddelanden, skicka e-postmeddelanden i grupp och skicka e-post med visning och klickning.
* **Uppdateringar** i kommandocentralen: Vi återskapar kommandocentralen Sales Connect för att ge säljarna insikt i alla deras e-postmeddelanden, samtal och uppgifter som har initierats från Sales Connect. De kan även visa information som e-postinteraktion och leveransbarhet via kommandocentralen.

<br> 

## Meddelanden {#announcements}

* **Marketo Engage Success Center**: Vi lanserar Marketo Success Center i februari 2020. Success Center är ett produkthjälpcenter där du kan söka efter produktdokument och communityn, starta guider, få tillgång till innehåll som Marketo University och videor om bästa praxis från andra Marketo Engage. **Obs**: Den här funktionen lanseras som en betaversion i ANZ och kommer att lanseras i Nordamerika senare under kvartalet.

## Föråldringar {#deprecations}

* **Resurs-API &quot;_method&quot;-parameter**: Efter september 2020 kommer Resurs-API-slutpunkter inte längre att acceptera &quot;_method&quot; för att skicka Query Parameters i en POST för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränsen för tillgångs-API:er från 6KiB till 65KiB, så att långa URI:er för begäran kan skickas.
* **Undertryckt stöd för Internet Explorer**: Från och med version 31 juli 2020 stöds inte längre användargränssnittet i Marketo Engage i Internet Explorer.

***Product Release*** [WebinarGå ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) till den 3 mars 23:00 PT / 2:00 ET för ett live webbinarium som leds av vårt produktteam och läs mer om funktionerna i den här versionen.
