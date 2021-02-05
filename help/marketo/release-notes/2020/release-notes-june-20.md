---
unique-page-id: 37357276
description: Versionsinformation -juni 20 - Marketo Docs - Produktdokumentation
title: Versionsinformation -juni 20
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# Versionsinformation: 20 juni {#release-notes-june}

Följande funktioner finns i versionen från 20 juni. Se om din Marketo-utgåva har funktioner tillgängliga.

>[!AVAILABILITY]
>
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/star-yellow.svg)) kan vara avgiftsbelagda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

***Kvartalsvisa*** utgåvorFöljande funktioner kommer att släppas  **den 5 juni 2020**.

## Core Marketo Engage {#core-marketo-engage}

* ** [Prediktiva målgrupper](https://help.marketo.com/hc/en-us/articles/360045746253) ![(star)](assets/star-yellow.svg)

   **: Med nya Smart List- och Smart Campaign-filter från Adobe Sensei kan ni skapa AI-baserade målgruppssegment för e-post, event och webbinära marknadsföringsprogram. Använd AI för att hjälpa er att segmentera målgrupper baserat på leads för att registrera ett event, delta i ett evenemang eller avbeställa ett abonnemang. Bygg lookalike-målgrupper baserat på tidigare program för att effektivt återge tidigare framgångar. Uppnå konverteringsmålen med prediktiv målspårning och få rekommendationer för hur ni kan förfina era målgruppssegment för händelseprogram.
* **E-postförstärkning för grupp ![(stjärna)](assets/star-yellow.svg): ** Förbättring av vår e-postmarknadsföringsfunktion som gör att du kan skicka upp till 3 miljoner gruppmeddelanden per timme. Vi har omkonstruerat vår batchkampanj och e-postrapportbearbetning för att förbättra prestanda för e-postprogram och batche-postkampanjer. Detta ger kortare ledtider att skicka och kortare slutförandetid. Konfigurera e-postutskick på det sätt du brukar, så blir det ingen extra komplexitet. Den här förbättringen finns som ett produkttillägg som även innehåller ett lanseringspaket för Delivery Services, verktyg för e-postleverans och flera dedikerade IP-adresser.
* ** [Målgruppsintegrering med Adobe Experience Cloud (AEC)](https://docs.marketo.com/x/ogI6Ag): **Integrering med nya Adobe Experience Cloud (AEC) gör att du kan synkronisera statiska listor med kända leads från Marketo Engage med flera AEC-program för att förbättra befintliga program, låsa upp nya användningsfall och samordna flerkanalskampanjer. Integrationen omfattar Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager och Adobe Advertising Cloud.
* ** [Anpassade fält för programmedlemmar](https://docs.marketo.com/x/MQA6Ag)**: Hämta in och använda anpassade fält om en programmedlem. Använd dessa nya fält i era Marketo Engage-formulär, visa dem i programmets medlemslista, utnyttja dem i Smart List-filter och -utlösare och inkludera dem i en ny Smart Campaign Flow Action för förbättrad automatisering och mer detaljerad personalisering. Dessa kan också importeras och exporteras via användargränssnittet och API:erna. Förbättring av våra anpassade dataobjekt och fält.
* **Beskriv programmedlem**: Hämta metadata för programmedlemmar, så att du kan importera och exportera data för anpassade fält för programmedlemmar med hjälp av REST API. Förbättring av vårt API*. *

* ** [Skapa uppgift i Microsoft Dynamics](https://docs.marketo.com/x/jQM6Ag)**: Skapa aktiviteter för försäljning i Microsoft Dynamics med en ny Flow Action som baseras på kundbeteende som hämtats i Marketo Engage. Förbättring av vår Microsoft Dynamics CRM-integration*. *

* **Hämta formulär som används av API-slutpunkt** för listresurs: Hämta en lista med resurser som är beroende av ett formulär. Förbättring av vårt API*.*

* **Ange e-postförhuvud via API**: Aktivera automatisk översättning och lokalisering av e-postförrubriksfält. Förbättring av vårt API*.*

* **Bild- och filcachning**: Vi förbättrar serverstabiliteten i Marketo Engage genom att leverera bild- och filresurser från ett 60-sekunders cacheminne.

**Kontobaserad marknadsföring ![(stjärna)](assets/star-yellow.svg)

**

* **Ny kontoidentifiering, allmänt tillgänglig**

   * Ny kontoidentifiering är en förbättring av vår kontoprofileringsfunktion som gör att du kan identifiera nya målkonton för din ABM-strategi baserat på din AI-baserade idealiska kundprofilmodell. Visa, markera och importera rekommenderade nya konton, tillsammans med deras AI-baserade indikatorer för anpassning och avsikter.

<br> 

**

***Frigör under hela kvartalet***

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.
**Bizible ![(star)](assets/star-yellow.svg)

**

* **Integrering** av Marketo Engage-program: Hämta in programdata direkt från Marketo Engage för att skapa kontaktytor längs attribueringsresan i Bizible för att få lämplig kredit för e-post och engagemangsprogram. Bättre integrering med Marketo Engage.
* **Integrering`<sup>BETA</sup>`** av Marketo Engage-aktiviteter: Använd data från Marketo Engage-aktivitet direkt i Bizible för att skapa kontaktytor över hela kundresan och alla attribueringsmodeller. Exempel är förändringar av lead-poäng, intressanta stunder, e-postklick eller andra anpassade aktiviteter. Bättre integrering med Marketo Engage.
* **Bizible B2B Customer Attributes Integration`<sup>BETA</sup>`**: Det här är en Adobe Experience Cloud-integrering med Adobe Analytics som gör att du kan överföra utvalda Bizible-data direkt till Adobe Analytics för mer ingående analyser. Exemplen omfattar kontobaserad webbplatstrafik och innehållsanalys per företagsnamn, kontoattribut, CRM-möjligheter och värdefulla individer enligt definitionen i den bizible-baserade intäkten och trattfasen.
* **Bizible Discover-filter och förbättringar:** Analysera data med kanal-, delkanal-, kampanj- och segmentfilter på olika instrumentpaneler. Förstärk datainsynen med fler fördjupningsattribut. Detta är en förbättring av våra Discover Boards.
* **Synkronisering av aktiviteter för Microsoft Dynamics**: Attribuera säljinteraktioner genom att föra in Microsoft Dynamics CRM-aktiviteter till kontaktpunktsresan och spåra händelser som samtal, avtalade tider eller uppgifter som är kopplade till dina leads eller kontakter. Förbättring av vår Microsoft Dynamics CRM-integrering.

**Sales Insight ![(star)](assets/star-yellow.svg)

**

* ** [Insiktsinstrumentpanel för Salesforce CRM](https://docs.marketo.com/x/EoGMAg)**: Vi förnyar vår säljinsiktsförmåga med ny synlighet i kommande marknadsföringsevenemang och kampanjer för att ge säljarna möjlighet att göra rekommendationer mer relevanta för kunder och potentiella kunder baserat på deras behov och intressen. Säljarna kan även se både kontakt- och kontoaktivitet på tidslinjen och enkelt få tillgång till ytterligare aktivitetsinformation. Mer information om hur du uppgraderar ditt paket [här](https://docs.marketo.com/x/F4GMAg).

<br> 

## Meddelanden {#announcements}

* **ITP 2.1+ RTP-uppdatering**: På grund av ändringar i cookie-principen för Safari kommer möjligheten för RTP-cookies att spåra användare i sessioner på samma domän att begränsas av ITP till antingen 1 eller 7 dagar baserat på webbläsaren och webbläsarversionen som används av besökaren. Därför implementerar vi en ny webbtjänst som tillåter att RTP-cookies ställs in med en Set-Cookie-rubrik via HTTP-svar. Mer information finns [här](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Förändringar** i infrastrukturen för batchkampanj: Vi uppgraderar våra batchkampanjtjänster under resten av året. Det här är en sömlös uppdatering som inte påverkar några pågående batchkampanjer och som inte leder till någon beteendeförändring. Ingen åtgärd krävs. Mer information finns i det här [Nation-inlägget](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Föråldringar {#deprecations}

* ** [Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/):** Från och med version 159 av Munchkin JS loggas en borttagningsvarning i webbläsarkonsolen när Associate Lead-metoden anropas, vilket anger att funktionen kommer att tas bort i en framtida version.  Schemat för fullständig borttagning tillkännages vid ett senare datum.

***Product Release*** [WebinarSe inspelningen ](https://engage.marketo.com/June-Release-2020-On-Demand.html) av vårt webbseminarium om produktreleaser från 20 juni.
