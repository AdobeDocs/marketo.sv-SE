---
unique-page-id: 37357276
description: Versionsinformation -juni 20 - Marketo Docs - produktdokumentation
title: Versionsinformation -juni 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Versionsinformation: 20 juni {#release-notes-june}

Följande funktioner finns i versionen från 20 juni. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa utgåvor_** Följande funktioner kommer att släppas den **5 juni 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **[Prediktiva målgrupper](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=sv-SE#predictive-audiences)** ![(stjärna)](assets/yellow-star.png): Med de nya filtren Smart List och Smart Campaign från Adobe Sensei kan du skapa AI-baserade målgruppssegment för e-post, event och webbinära marknadsföringsprogram. Använd AI för att hjälpa er att segmentera målgrupper baserat på leads för att registrera ett event, delta i ett evenemang eller avbeställa ett abonnemang. Bygg lookalike-målgrupper baserat på tidigare program för att effektivt återge tidigare framgångar. Uppnå konverteringsmålen med prediktiv målspårning och få rekommendationer för hur ni kan förfina era målgruppssegment för händelseprogram.
* **Förstärkning av e-post i grupp** ![(stjärna)](assets/yellow-star.png): Förbättring av vår e-postmarknadsföringsfunktion som gör att du kan skicka upp till 3 miljoner gruppmeddelanden per timme. Vi har omkonstruerat vår gruppkampanj och e-postrapportbearbetning för att förbättra prestanda för e-postprogram och gruppe-postkampanjer. Detta ger kortare ledtider att skicka och kortare slutförandetid. Konfigurera e-postutskick på det sätt du brukar, så blir det ingen extra komplexitet. Den här förbättringen finns som ett produkttillägg som även innehåller ett lanseringspaket för Delivery Services, verktyg för e-postleverans och flera dedikerade IP-adresser.
* **[Målgruppsintegrering med Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Ny integrering med Adobe Experience Cloud (AEC) som gör att du kan synkronisera statiska listor med kända leads från Marketo Engage med flera AEC-program för att förbättra befintliga program, låsa upp nya användningsfall och samordna flerkanalskampanjer. Integrationen innefattar Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager och Adobe Advertising Cloud.
* **[Anpassade fält för programmedlemmar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Hämta och använda anpassade fält om en programmedlem. Använd dessa nya fält i dina Marketo Engage-formulär, visa dem i programmets medlemslista, utnyttja dem i Smart List-filter och -utlösare och inkludera dem i en ny Smart Campaign Flow Action för förbättrad automatisering och mer detaljerad personalisering. Dessa kan också importeras och exporteras via användargränssnittet och API:erna. Förbättring av våra anpassade dataobjekt och fältegenskaper.
* **Beskriv programmedlem**: Hämta metadata för programmedlem, så att du kan importera och exportera data för anpassade fält för programmedlemmar med hjälp av REST API. Förbättring av vårt API.
* **[Skapa aktivitet i [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Skapa aktiviteter för försäljning i [!DNL Microsoft Dynamics] med en ny Flow Action som baseras på kundbeteende som hämtats i Marketo Engage. Förbättring av vår interna [!DNL Microsoft Dynamics] CRM-integrering.
* **Hämta formulär som används av API-slutpunkt för listresurs**: Hämta en lista med resurser som är beroende av ett formulär. Förbättring av vårt API.
* **Ange förhuvud för e-post via API**: Aktivera automatisk översättning och lokalisering av e-postförrubriksfält. Förbättring av vårt API.
* **Bild- och filcachning**: Vi förbättrar Marketo Engage-serverns stabilitet genom att hantera bild- och filresurser från ett 60-sekunders cacheminne.

## Account-Based Marketing {#account-based-marketing}

![(stjärna)](assets/yellow-star.png)

* **Ny kontoidentifiering är vanligtvis tillgänglig**

   * Ny kontoidentifiering är en förbättring av vår kontoprofileringsfunktion som gör att du kan identifiera nya målkonton för din ABM-strategi baserat på din AI-baserade idealiska kundprofilmodell. Visa, markera och importera rekommenderade nya konton, tillsammans med deras AI-baserade indikatorer för anpassning och återgivning.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Bizible] {#bizible}

![(stjärna)](assets/yellow-star.png)

* **Integrering av Marketo Engage-program**: Dra in programdata direkt från Marketo Engage för att skapa kontaktytor längs attribueringsresan i [!DNL Bizible] för att få lämplig kredit för e-post och engagemangsprogram. Bättre integrering med Marketo Engage.
* **Integrering av Marketo Engage-aktiviteter (BETA)**: Hämta Marketo Engage-aktivitetsdata direkt till [!DNL Bizible] för att skapa kontaktytor under kundresan och alla attribueringsmodeller. Exempel är förändringar av lead-poäng, intressanta stunder, e-postklick eller andra anpassade aktiviteter. Bättre integrering med Marketo Engage.
* **[!DNL Bizible]B2B Customer Attributes Integration (BETA)**: Det här är en Adobe Experience Cloud-integrering med Adobe Analytics som gör att du kan hämta utvalda Bizible-data direkt till Adobe Analytics för mer ingående analys. Exemplen omfattar kontobaserad webbplatstrafik och innehållsanalys per företagsnamn, kontoattribut, CRM-möjligheter och värdefulla individer som definieras av [!DNL Bizible] tillskrivna intäkter och trattfas.
* **[!DNL Bizible]Identifiera filter och förbättringar**: Analysera dina data med kanal-, delkanal-, kampanj- och segmentfilter på olika instrumentpaneler. Förstärk datainsynen med fler fördjupningsattribut. Detta är en förbättring av våra Discover Boards.
* **Aktiviteter synkroniseras för[!DNL Microsoft Dynamics]**: Attribuera säljinteraktioner genom att föra in [!DNL Microsoft Dynamics] CRM-aktiviteter till kontaktytans resa och spåra händelser som samtal, avtalade tider eller uppgifter som är kopplade till dina leads eller kontakter. Förbättring av vår [!DNL Microsoft Dynamics] CRM-integrering.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Insights Dashboard för Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Vi omformar vår [!DNL Sales Insight]-kapacitet med ny synlighet i kommande marknadsföringsevenemang och kampanjer för att ge säljarna möjlighet att göra rekommendationer mer relevanta för kunder och potentiella kunder baserat på deras behov och intressen. Säljarna kan även se både kontakt- och kontoaktivitet på tidslinjen och enkelt få tillgång till ytterligare aktivitetsinformation. Mer information om hur du uppgraderar ditt paket [här](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md) finns.

<br> 

## Meddelanden {#announcements}

* **ITP 2.1+ RTP-uppdatering**: På grund av ändringar i cookie-principen för [!DNL Safari] kommer möjligheten för RTP-cookies att spåra användare i sessioner på samma domän att begränsas av ITP till antingen 1 eller 7 dagar baserat på webbläsarversionen som används av besökaren. Därför implementerar vi en ny webbtjänst som tillåter att RTP-cookies ställs in med en Set-Cookie-rubrik via HTTP-svar. Mer information finns [här](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Förändringar i infrastrukturen för batchkampanj**: Vi uppgraderar våra batchkampanjtjänster under resten av året. Det här är en sömlös uppdatering som inte påverkar några pågående batchkampanjer och som inte leder till någon beteendeförändring. Ingen åtgärd krävs. Mer information finns i detta [Nation-inlägg](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Utgånget {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Från och med version 159 av [!DNL Munchkin] JS loggas en borttagningsvarning i webbläsarkonsolen när metoden Associate Lead anropas, vilket anger att funktionen kommer att tas bort i en framtida version.  Schemat för fullständig borttagning kommer att tillkännages vid ett senare datum.

**_Webbseminarium om produktreleaser_** [Se inspelningen](https://engage.marketo.com/June-Release-2020-On-Demand.html) av vårt webbseminarium om produktreleaser för juni 2011.
