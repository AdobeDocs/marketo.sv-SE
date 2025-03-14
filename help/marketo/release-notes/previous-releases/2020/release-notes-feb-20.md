---
unique-page-id: 37355826
description: Versionsinformation -feb '20 - Marketo Docs - produktdokumentation
title: Versionsinformation -feb '20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Versionsinformation: 20 feb {#release-notes-feb}

Följande funktioner finns i utgåvan från 20 februari. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa utgåvor_** Följande funktioner släpptes den **21 februari 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics Ändra ägare i Microsoft Flödesåtgärd**: Behåll kontrollen över dina Microsoft Dynamics CRM-data med möjlighet att ändra en lead-/kontaktägare direkt från Marketo Engage. Detta är en förbättring av vår interna CRM-integreringsfunktion.
* **API:er för användarhantering**: Automatisera användar- och rollhantering via externa identitets- och organisationshanteringssystem. Detta är en förbättring av vår API-anropsfunktion.
* **API:er för anpassade objektscheman**: Hantera och tilldela automatiskt anpassade objektscheman över instanser i Marketo Engage för att hålla datamodeller konsekventa över alla sälj- och marknadsföringsverktyg. Med detta API kan du definiera och testa anpassade objekt i en sandlåda eller i ett center av hög kvalitet och tillhandahålla så många instanser som behövs. Detta är en förbättring av vår API:s anropsfunktion. Kontakta din Marketo Engage-representant om du vill veta mer om hur du får tillgång till den här förbättringen.
* **API:er för omdirigeringsregler för landningssidor**: Automatisera hanteringen av omdirigeringsregler för landningssidor. Detta är en förbättring av vår API-anropsfunktion.
* **Cachelagring av formulärbeskrivare**: Vi minskar inläsningstiden för inbäddade formulär och förbättrar den övergripande programstabiliteten genom att cachelagra formulär som resurser. Observera att det kan ta upp till fyra minuter att godkänna inbäddade formulär för att de ska visas på webben. Detta är en förbättring av vår förmåga till landningssidor och Forms.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## Bizible {#bizible}

![(stjärna)](assets/yellow-star.png)

* **Kontobaserad segmentering**: Analysera attribuering på kontonivå med möjlighet att skapa segment och filter för Discover boards baserat på kontoattribut. Använd dessa segment för att fördjupa er i er kontobaserade marknadsföring.
* **Sparar filter**: Spara instrumentpanelsspecifika filter som är unika för varje användare för att analysera dina instrumentpaneler snabbt och konsekvent.
* **Exportera till PDF**: Dela värdefulla insikter i hela organisationen genom att exportera dubbelsidiga instrumentpaneler som PDF.

## Sales Connect {#sales-connect}

* **Disponera fönsteruppdateringar**: Vi har effektiviserat processen för att välja mallar och skicka e-postmeddelanden via Sales Connect. Använd Compose-fönstret i vår webbklient och Salesforce som en enda butik för säljare, med möjlighet att spara mallkategorier, schemalägga e-postmeddelanden, skicka e-postmeddelanden i grupp och skicka e-post med visning och klickning.
* **Uppdateringar för kommandocentralen**: Vi återskapar kommandocentralen Sales Connect för att ge säljarna insikt i alla deras e-postmeddelanden, samtal och uppgifter som har initierats från Sales Connect. De kan även visa information som e-postinteraktion och leveransbarhet via kommandocentralen.

<br> 

## Meddelanden {#announcements}

* **Marketo Engage Success Center**: Vi startar Marketo Success Center i februari 2020. Success Center är ett produkthjälpcenter där du kan söka efter produktdokument och communityn, starta guider, få tillgång till hjälpavsnitt som Marketo University och videor med bästa praxis från andra Marketo Engage. **Obs!** Den här funktionen startas som en betaversion i ANZ och kommer att lanseras i Nordamerika senare under kvartalet.

## Undertryckningar {#deprecations}

* **Resurs-API-parametern &quot;_method&quot;**: Efter september 2020 accepterar inte längre resurs-API-slutpunkter &quot;_method&quot; att skicka frågeparametrar i en POST för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränsen för tillgångs-API:er från 6KiB till 65KiB, så att långa URI:er för begäran kan skickas.
* **Supportborttagning för Internet Explorer**: Från och med juliversionen den 31 juli 2020 stöds inte längre användargränssnittet i Marketo Engage i Internet Explorer.

**_Webbseminarium om produktreleaser_** [Följ oss](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) den 3 mars klockan 11:00 PT/2:00 ET för ett live-webbinarium som är värd för vårt produktteam och läs mer om funktionerna i den här versionen.
