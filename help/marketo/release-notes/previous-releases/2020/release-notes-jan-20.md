---
unique-page-id: 37355534
description: Versionsinformation - jan 2020 - Marketo Docs - produktdokumentation
title: Versionsinformation - jan 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Versionsinformation: jan 2020 {#release-notes-jan}

Följande funktioner finns i jan 20. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna ( ![(stjärna)](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den **17 januari 2020**.

## Core Marketo Engage Adobe Application {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager Resursväljare](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): Få snabbt tillgång till resurser som är anpassade till ert varumärke med AEM-resurser som är tillgängliga direkt i Marketo Engage. Obs! Den här funktionen är tillgänglig i både Marketo Sky och klassiska upplevelser, men de administrativa funktionerna finns i vår klassiska upplevelse. Du måste vara kund hos AEM Assets och ha version 6.5 eller senare.

>[!NOTE]
>
>För närvarande stöds AEM Resursväljare endast fullt ut i Firefox. Det stöds inte i Safari och kanske inte fungerar i den senaste versionen av Chrome (version 80), beroende på inställningarna för cookie-filen för samma webbplats.

* **[!DNL Microsoft Dynamics]- Synkronisera lead till CRM i realtid**: Synkronisering i realtid av leads och kontakter mellan Marketo Engage och [!DNL Microsoft Dynamics]. Skapa leads eller kontakter och visa dem i [!DNL Microsoft Dynamics] omedelbart med flödesåtgärden Synkronisera person till Microsoft.
* **[!DNL LinkedIn]Lead Gen Forms Additional Field Mapping**: Hämta lead-data från [!DNL LinkedIn] Lead Gen Forms för att skapa mer relevanta upplevelser för både sälj- och marknadsföringskontaktytor. Dra in dolda fält, medgivandefält och testleads till Marketo Engage.
* **API för e-postmallsberoenden**: Hämta en lista över resurser som är beroende av en e-postmall för att förstå omfattningen av eventuella ändringar och adressoberoenden till mallar kan ändras och tas bort snabbare.
* **Förbättringar för hantering av flera instanser**: Navigera till den instans du behöver snabbt med en rullningsbar och alfabetisk listruta med dina prenumerationer.

## Account-Based Marketing {#account-based-marketing}

![(stjärna)](assets/yellow-star.png)

* [Ny kontoidentifiering (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(stjärna)](assets/yellow-star.png): Använd kontoprofilering för att identifiera nya målkonton för din ABM-strategi baserat på din AI-drivna idealiska kundprofilmodell. Visa, markera och importera rekommenderade nya konton, tillsammans med deras AI-baserade indikatorer för anpassning och avsiktsdata, som inte redan finns i Marketo Engage lead- och kontodatabas för ABM-anpassning. Omedelbart tillgängligt för kvalificerade kunder inom kontoprofilering.

<br> 

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Bizible] {#bizible}

![(stjärna)](assets/yellow-star.png)

* **Marketo Engage Leads Integration**: Samla försäljning och marknadsföring med en enhetlig vy av leads över [!DNL Bizible] och Marketo Engage. Med den här uppdateringen kan Marketo Engage nu användas som en extra lead-datakälla, så du behöver inte längre vänta på leads för synkronisering med CRM för att rapportera om lead-generering.
* **Upptäck förbättringar**: Få ut mer av våra Discover Boards i [!DNL Bizible] med förbättringar som har utvecklats från kundfeedback, som möjlighet att gå ned till transaktionsposter från paneler och attribut, lägga till viktiga posträknare och motsvarande kostnads-per-mått samt lägga till/ta bort kontrollpanelsfilter för flera instrumentpaneler. Du dirigeras också direkt till standardinstrumentpanelen vid inloggning.

## [!DNL Marketo Sky] {#marketo-sky}

* [Bildredigering](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio): Få åtkomst till Adobe redigeringsfunktioner utan att behöva lämna Marketo Engage. Med den här nya funktionen kan du enkelt förbättra, beskära och lägga till text i bilder direkt i [!UICONTROL Design Studio].

## [!DNL Sales Insight] {#sales-insight}

* **[!DNL Salesforce Lightning]Massåtgärder**: Förbättra effektiviteten inom försäljningen och håll kvar köparna med möjligheten att lägga till upp till 200 kontakter/leads till kampanjer och skicka e-post från Marketo Engage till dem i grupp med [!DNL Salesforce Lightning].
* **Mobilstöd för[!DNL Salesforce1]**: Nu har du mobil tillgång till alla funktioner i [!DNL Sales Insight], som Intressanta stunder och webbaktiviteter och e-postmeddelanden, direkt i appen [!DNL Salesforce1].
* **UI-förbättringar**: Uppdaterat gränssnitt med förbättrad läsbarhet och en design som är förenlig med vår [!DNL Marketo Sky] -upplevelse.

## [!DNL Sales Connect] {#sales-connect}

* **Rutnätskomponenter**: Optimera [!DNL Sales Connect]-instansen med nya rutnätsanpassningsfunktioner. Välj vilka kolumner som ska visas, sök efter kolumner, markera/avmarkera alla kolumner och ange hur många rader med data som ska visas på varje sida.
* **[Låsning av innehåll](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: Maximera varumärkesjusteringen med en inställning för hela prenumerationen som styr om icke-administratörer kan skapa och redigera mallar och kampanjer.

>[!NOTE]
>
>* **Borttagning av TLS 1.0 och 1.1**: I ett kontinuerligt försök att integrera med Adobe versionsstruktur flyttar vi bort borttagningen av TLS 1.0 och TLS 1.1 till 13 januari 2020. Mer detaljerad information finns [här](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ [!DNL Munchkin] Uppdatering**: På grund av ändringar i cookie-principen för [!DNL Safari], begränsas möjligheten för [!DNL Munchkin] att spåra användare mellan sessioner på samma domän av ITP till antingen 1 eller 7 dagar baserat på webbläsarversionen som används av besökaren. Därför implementerar vi en ny webbtjänst som tillåter att Munchkin cookies ställs in med en Set-Cookie-rubrik via HTTP-svar. Mer information om hur du implementerar den nya tjänsten finns [här](https://nation.marketo.com/docs/DOC-7351).

**_Webbseminarium om produktreleaser_** [Följ oss](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) den 3 mars klockan 11:00 PT/2:00 ET för ett live-webbinarium som är värd för vårt produktteam och läs mer om funktionerna i den här versionen.
