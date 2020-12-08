---
unique-page-id: 37355534
description: Versionsinformation - jan 2020 - Marketo Docs - produktdokumentation
title: Versionsinformation - jan 2020
translation-type: tm+mt
source-git-commit: 6f49037bf698b1646004720815897f992911f716
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---


# Versionsinformation: Jan 2020 {#release-notes-jan}

Följande funktioner finns i jan 20. Se om din Marketo-utgåva har funktioner tillgängliga.

>[!NOTE]
>
>**Tillgänglighet**
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/star-yellow.svg)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

***Kvartalsvisa versioner*** Följande funktioner kommer att släppas den 17 **januari 2020**.

## Programmet Core Marketo Engage Adobe {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager Resursväljare](https://docs.marketo.com/x/_AA6Ag): Få snabbt tillgång till resurser som är anpassade till ert varumärke med AEM resurser som är tillgängliga direkt i Marketo Engage. Obs! Även om den här funktionen är tillgänglig i både vår Marketo Sky och klassiska upplevelser, finns de administrativa funktionerna i vår klassiska upplevelse. Du måste vara kund hos AEM Assets och ha version 6.5 eller senare.

>[!NOTE]
>
>För närvarande stöds AEM resursväljare bara fullt ut i Firefox. Det stöds inte i Safari och kanske inte fungerar i den senaste versionen av Chrome (version 80), beroende på inställningarna för cookie-filen för samma plats.

* **Microsoft Dynamics - Synkronisera lead till CRM i realtid:** Synkronisering i realtid av leads och kontakter mellan Marketo Engage och Microsoft Dynamics. Skapa leads eller kontakter och se dem i Microsoft Dynamics direkt med flödesåtgärden Synkronisera person till Microsoft.
* **LinkedIn Lead Gen Forms Additional Field Mapping:** Hämta in lead-data från LinkedIn Lead Gen Forms för att skapa mer relevanta upplevelser för både sälj- och marknadsföringskontaktytor. Dra in dolda fält, medgivandefält och testleads-fältet i Marketo Engage.
* **API** för e-postmallsberoenden: Få en lista över resurser som är beroende av en e-postmall för att förstå omfattningen av eventuella ändringar och hantera beroenden till mallar som kan ändras och tas bort snabbare.
* **Förbättringar** för hantering av flera instanser: Navigera till den instans du behöver snabbt med en rullningsbar och alfabetisk listruta med dina prenumerationer.

Kontobaserad marknadsföring ![(stjärna)](assets/star-yellow.svg)

* [Ny kontoidentifiering (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(stjärna)](assets/star-yellow.svg) : Använd kontoprofilering för att identifiera nya målkonton för er ABM-strategi baserat på er AI-drivna idealiska kundprofilmodell. Visa, markera och importera rekommenderade nya konton, tillsammans med deras AI-baserade indikator för anpassning och avsiktsdata, som inte redan finns i Marketo Engage lead- och kontodatabasen för ABM-anpassning. Omedelbart tillgängligt för kvalificerade kunder inom kontoprofilering.

<br> 

## Nytt avsnitt

***Frigör under hela kvartalet***

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

Bizible ![(star)](assets/star-yellow.svg)

* **Integrering** av leads i Marketo Engage: Samla försäljning och marknadsföring med en enhetlig vy av leads över Bizible och Marketo Engage. Med den här uppdateringen kan Marketo Engage nu användas som en extra lead-datakälla, så du behöver inte längre vänta på leads för synkronisering med CRM för att rapportera om lead-generering.
* **Upptäck förbättringar**: Få ut mer av våra Discover Boards i Bizible med förbättringar som har utvecklats utifrån kundens feedback, som möjligheten att gå ned till transaktionsregister från paneler och attribut, lägga till viktiga posträknare och motsvarande kostnads-per-statistik samt lägga till/ta bort kontrollpanelsfilter för flera kontrollpaneler. Du dirigeras också direkt till standardinstrumentpanelen vid inloggning.

## Marketo Sky  {#marketo-sky}

* [Bildredigering](https://help.marketo.com/hc/en-us/articles/360041344614-Marketo-Image-Editor): Få tillgång till Adobe redigeringsmöjligheter utan att behöva lämna Marketo Engage. Med den här nya funktionen kan du enkelt förbättra, beskära och lägga till text i bilder direkt i Design Studio.

## Försäljningsinsikter  {#sales-insight}

* **Salesforce Lightning - gruppåtgärder**: Förbättra effektiviteten i försäljningen och håll köparna engagerade med möjligheten att lägga till upp till 200 kontakter/leads till kampanjer och skicka Marketo Engage-e-postmeddelanden i grupp med Salesforce Lightning.
* **Mobilstöd för Salesforce1**: Nu har du mobil tillgång till alla funktioner i Sales Insight, som Intressant stund och Webbaktiviteter &amp; e-post, var du än är, direkt i Salesforce1-appen.
* **Gränssnittsförbättringar**: Uppdaterat gränssnitt med förbättrad läsbarhet och en design som överensstämmer med vår Marketo Sky.

## Sales Connect  {#sales-connect}

* **Stödrasterkomponenter**: Optimera Sales Connect-instansen med nya rutnätsanpassningsfunktioner. Välj vilka kolumner som ska visas, sök efter kolumner, markera/avmarkera alla kolumner och ange hur många rader med data som ska visas på varje sida.
* [Låsning](https://docs.marketo.com/x/6wA6Ag)av innehåll: Maximera varumärkesjusteringen med en prenumerationsomfattande inställning som styr om icke-administratörer kan skapa och redigera mallar och kampanjer.

>[!NOTE]
>
>* **Borttagning** av TLS 1.0 och 1.1: I en fortsatt strävan att integrera med Adobe releasestruktur håller vi på att ändra borttagningen av TLS 1.0 och TLS 1.1 till 13 januari 2020. Mer detaljerad information finns [här](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
   >
   >
* **ITP 2.1+ Munchkin - uppdatering**: På grund av ändringar i cookie-principen för Safari kommer möjligheten för Munchkin att spåra användare i sessioner på samma domän att begränsas av ITP till antingen 1 eller 7 dagar baserat på webbläsarversionen som används av besökaren. Därför implementerar vi en ny webbtjänst som tillåter att Munchkin-cookies ställs in med en Set-Cookie-rubrik via HTTP-svar. Mer information om hur du implementerar den nya tjänsten finns [här](https://nation.marketo.com/docs/DOC-7351).


***Product Release Webinar*** [Join us](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) on March 3, 11:00 PT / 2:00 ET för ett live webbinarium som leds av vårt produktteam och läs mer om funktionerna i den här versionen.
