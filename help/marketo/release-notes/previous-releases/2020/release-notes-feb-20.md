---
unique-page-id: 37355826
description: Versionsinformation -feb '20 - Marketo Docs - produktdokumentation
title: Versionsinformation -feb '20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Versionsinformation: 20 feb {#release-notes-feb}

Följande funktioner finns i utgåvan från 20 februari. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa utgåvor_** Följande funktioner släpptes den **21 februari 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **[!DNL Microsoft Dynamics]&quot;Ändra ägare i Microsoft&quot; Flödesåtgärd**: Behåll kontrollen över dina [!DNL Microsoft Dynamics] CRM-data med möjlighet att ändra en lead-/kontaktägare direkt från Marketo Engage. Detta är en förbättring av vår interna CRM-integreringsfunktion.
* **API:er för användarhantering**: Automatisera användar- och rollhantering via externa identitets- och organisationshanteringssystem. Detta är en förbättring av vår API-anropsfunktion.
* **API:er för anpassade objektscheman**: Hantera och tilldela automatiskt anpassade objektscheman över instanser i Marketo Engage för att hålla datamodeller konsekventa över alla sälj- och marknadsföringsverktyg. Med detta API kan du definiera och testa anpassade objekt i en sandlåda eller i ett center av hög kvalitet och tillhandahålla så många instanser som behövs. Detta är en förbättring av vår API:s anropsfunktion. Kontakta Marketo Engage om du vill veta hur du får tillgång till den här förbättringen.
* **API:er för omdirigeringsregler för landningssidor**: Automatisera hanteringen av omdirigeringsregler för landningssidor. Detta är en förbättring av vår API-anropsfunktion.
* **Cachelagring av formulärbeskrivare**: Vi minskar inläsningstiden för inbäddade formulär och förbättrar den övergripande programstabiliteten genom att cachelagra formulär som resurser. Observera att det kan ta upp till fyra minuter att godkänna inbäddade formulär för att de ska visas på webben. Detta är en förbättring av vår förmåga till landningssidor och Forms.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Bizible] {#bizible}

![(stjärna)](assets/yellow-star.png)

* **Kontobaserad segmentering**: Analysera attribuering på kontonivå med möjlighet att skapa segment och filter för Discover boards baserat på kontoattribut. Använd dessa segment för att fördjupa er i er kontobaserade marknadsföring.
* **Sparar filter**: Spara instrumentpanelsspecifika filter som är unika för varje användare för att analysera dina instrumentpaneler snabbt och konsekvent.
* **Exportera till PDF**: Dela värdefulla insikter i hela organisationen genom att exportera dubbelsidiga instrumentpaneler som PDF-filer.

## [!DNL Sales Connect] {#sales-connect}

* **Disponera fönsteruppdateringar**: Vi har effektiviserat processen för att välja mallar och skicka e-postmeddelanden via [!DNL Sales Connect]. Använd Compose-fönstret i webbklienten och Salesforce som en enda butik för säljare, med möjlighet att spara mallkategorier, schemalägga e-postmeddelanden, skicka e-postmeddelanden i grupp samt skicka e-post med visning och klickning.
* **Uppdateringar för kommandocentralen**: Vi återskapar kommandocentralen [!DNL Sales Connect] för att ge säljarna insikt i alla deras e-postmeddelanden, samtal och uppgifter som har initierats från [!DNL Sales Connect]. De kan även visa information som e-postinteraktion och leveransbarhet via kommandocentralen.

<br> 

## Meddelanden {#announcements}

* **Marketo Engage Success Center**: Vi startar Marketo Success Center i februari 2020. Success Center är ett produkthjälpcenter där du kan söka efter produktdokument och communityn, starta guider, få tillgång till hjälpavsnitt som Marketo University och videor med bästa praxis från andra användare, och mycket annat - direkt från din Marketo Engage-instans. **Obs!** Den här funktionen startas som en betaversion i ANZ och kommer att lanseras i Nordamerika senare under kvartalet.

## Utgånget {#deprecations}

* **Resurs-API-parametern &quot;_method&quot;**: Efter september 2020 accepterar inte längre resurs-API-slutpunkter&quot;_method&quot; att skicka frågeparametrar i ett POST-brödtext för att kringgå URI-längdbegränsningar. För att tillgodose begäranden som kräver den här parametern ökas URI-gränsen för tillgångs-API:er från 6KiB till 65KiB, så att långa URI:er för begäran kan skickas.
* **Supportborttagning för Internet Explorer**: Från och med juliversionen den 31 juli 2020 stöds inte längre Marketo Engage användargränssnitt i Internet Explorer.

**_Webbseminarium om produktreleaser_** [Besök oss](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) den 3 mars 11:00AM PT/2:00PM ET för ett live-webbinarium som våra produktteam är värd för och läs mer om funktionerna i den här versionen.
