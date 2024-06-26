---
unique-page-id: 37357276
description: Versionsinformation -juni 20 - Marketo Docs - produktdokumentation
title: Versionsinformation -juni 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Versionsinformation: Juni 20 {#release-notes-june}

Följande funktioner finns i versionen från 20 juni. Se om det finns funktioner i din Marketo-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_** Följande funktioner kommer att släppas den **5 juni 2020**.

## Core Marketo Engage {#core-marketo-engage}

* **[Prediktiva målgrupper](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(stjärna)](assets/yellow-star.png): Med nya Smart List- och Smart Campaign-filter från Adobe Sensei kan ni skapa AI-baserade målgruppssegment för e-post, event och webbinära marknadsföringsprogram. Använd AI för att hjälpa er att segmentera målgrupper baserat på leads för att registrera ett event, delta i ett evenemang eller avbeställa ett abonnemang. Bygg lookalike-målgrupper baserat på tidigare program för att effektivt återge tidigare framgångar. Uppnå konverteringsmålen med prediktiv målspårning och få rekommendationer för hur ni kan förfina era målgruppssegment för händelseprogram.
* **Stegvis e-postutökning** ![(stjärna)](assets/yellow-star.png): Förbättring av vår e-postmarknadsföringsfunktion som gör att ni kan skicka upp till 3 miljoner gruppmeddelanden per timme. Vi har omkonstruerat vår batchkampanj och e-postrapportbearbetning för att förbättra prestanda för e-postprogram och batche-postkampanjer. Detta ger kortare ledtider att skicka och kortare slutförandetid. Konfigurera e-postutskick på det sätt du brukar, så blir det ingen extra komplexitet. Den här förbättringen finns som ett produkttillägg som även innehåller ett lanseringspaket för Delivery Services, verktyg för e-postleverans och flera dedikerade IP-adresser.
* **[Målgruppsintegrering med Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Tack vare den nya integrationen med Adobe Experience Cloud (AEC) kan du synkronisera statiska listor med kända leads från Marketo Engage med flera AEC-program för att förbättra befintliga program, låsa upp nya användningsfall och samordna flerkanalskampanjer. Integrationen omfattar Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager och Adobe Advertising Cloud.
* **[Anpassade fält för programmedlem](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Hämta in och använda anpassade fält om en programmedlem. Använd dessa nya fält i era Marketo Engage-formulär, visa dem i programmets medlemslista, utnyttja dem i Smart List-filter och -utlösare och inkludera dem i en ny Smart Campaign Flow Action för förbättrad automatisering och mer detaljerad personalisering. Dessa kan också importeras och exporteras via användargränssnittet och API:erna. Förbättring av våra anpassade dataobjekt och fält.
* **Beskriv programmedlem**: Hämta metadata för programmedlemmar, så att du kan importera och exportera data för anpassade fält för programmedlemmar med hjälp av REST API. Förbättring av vårt API.
* **[Skapa uppgift i Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Skapa aktiviteter för försäljning i Microsoft Dynamics med en ny Flow Action som baseras på kundbeteende som hämtats i Marketo Engage. Förbättring av vår integrering med Microsoft Dynamics CRM.
* **Hämta formulär som används av API-slutpunkt för listresurs**: Hämta en lista med resurser som är beroende av ett formulär. Förbättring av vårt API.
* **Ange e-postförhuvud via API**: Aktivera automatisk översättning och lokalisering av e-postförrubriksfält. Förbättring av vårt API.
* **Cachelagring av bilder och filer**: Vi förbättrar serverstabiliteten i Marketo Engage genom att leverera bild- och filresurser från ett 60-sekunders cacheminne.

## Account-Based Marketing {#account-based-marketing}

![(stjärna)](assets/yellow-star.png)

* **Ny kontoidentifiering, allmänt tillgänglig**

   * Ny kontoidentifiering är en förbättring av vår kontoprofileringsfunktion som gör att du kan identifiera nya målkonton för din ABM-strategi baserat på din AI-baserade idealiska kundprofilmodell. Visa, markera och importera rekommenderade nya konton, tillsammans med deras AI-baserade indikatorer för anpassning och återgivning.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## Bizible {#bizible}

![(stjärna)](assets/yellow-star.png)

* **Integrering av Marketo Engage-program**: Hämta in programdata direkt från Marketo Engage för att skapa kontaktytor längs attribueringsresan i Bizible för att få lämplig kredit för e-post och engagemangsprogram. Bättre integrering med Marketo Engage.
* **Integrering av verksamheten i Marketo Engage (BETA)**: Använd data från Marketo Engage-aktivitet direkt i Bizible för att skapa kontaktytor över hela kundresan och alla attribueringsmodeller. Exempel är förändringar av lead-poäng, intressanta stunder, e-postklick eller andra anpassade aktiviteter. Bättre integrering med Marketo Engage.
* **Bizible B2B Customer Attributes Integration (BETA)**: Det här är en Adobe Experience Cloud-integrering med Adobe Analytics som gör att du kan överföra utvalda Bizible-data direkt till Adobe Analytics för mer ingående analyser. Exemplen omfattar kontobaserad webbplatstrafik och innehållsanalys per företagsnamn, kontoattribut, CRM-möjligheter och värdefulla individer enligt definitionen i den bizible-baserade intäkten och trattfasen.
* **Filter och förbättringar för bizible Discover**: Analysera era data med kanal-, delkanal-, kampanj- och segmentfilter i olika paneler. Förstärk datainsynen med fler fördjupningsattribut. Detta är en förbättring av våra Discover Boards.
* **Synkronisering av aktiviteter för Microsoft Dynamics**: Attribuera säljinteraktioner genom att föra in Microsoft Dynamics CRM-aktiviteter till kontaktpunktsresan och spåra händelser som samtal, avtalade tider eller uppgifter som är kopplade till dina leads eller kontakter. Förbättring av vår integrering med Microsoft Dynamics CRM.

## Försäljningsinsikter {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Instrumentpanel för insikter för Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Vi förnyar vår säljinsiktsförmåga med ny synlighet i kommande marknadsföringsevenemang och kampanjer för att ge säljarna möjlighet att göra rekommendationer mer relevanta för kunder och potentiella kunder baserat på deras behov och intressen. Säljarna kan även se både kontakt- och kontoaktivitet på tidslinjen och enkelt få tillgång till ytterligare aktivitetsinformation. Mer information om hur du uppgraderar ditt paket [här](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Meddelanden {#announcements}

* **ITP 2.1+ RTP-uppdatering**: På grund av ändringar i cookie-principen för Safari kommer möjligheten för RTP-cookies att spåra användare i sessioner på samma domän att begränsas av ITP till antingen 1 eller 7 dagar baserat på webbläsaren och webbläsarversionen som används av besökaren. Därför implementerar vi en ny webbtjänst som tillåter att RTP-cookies ställs in med en Set-Cookie-rubrik via HTTP-svar. Mer information finns [här](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Ändringar av infrastruktur för batchkampanj**: Vi uppgraderar våra batchkampanjtjänster under resten av året. Det här är en sömlös uppdatering som inte påverkar några pågående batchkampanjer och som inte leder till någon beteendeförändring. Ingen åtgärd krävs. Mer information finns här [Nationpost](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Föråldringar {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Från och med version 159 av Munchkin JS loggas en borttagningsvarning i webbläsarkonsolen när Associate Lead-metoden anropas, vilket anger att funktionen kommer att tas bort i en framtida version.  Schemat för fullständig borttagning tillkännages vid ett senare datum.

**_Product Release Webinar_** [Se inspelningen](https://engage.marketo.com/June-Release-2020-On-Demand.html) av vårt webbseminarium om produktreleaser 20 juni.
