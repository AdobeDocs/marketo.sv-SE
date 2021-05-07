---
description: Versionsinformation - jan 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - jan 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
translation-type: tm+mt
source-git-commit: c1b2a5966da3bda18a2ccaab9b348296ba1d7bfd
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Versionsinformation: Jan 2021 {#release-notes-jan-21}

Följande funktioner finns i jan 21. Se om det finns funktioner i din Marketo-utgåva.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![(stjärna)](assets/yellow-star.png)) är betalda tillägg. Kontakta din Marketo Engage-representant om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den 15 januari 2021 **.**

## Nästa generations användarupplevelse {#next-generation-user-experience}

* Stöd för arbetsytor: Nästa generation av användarupplevelser i Marketo Engage sammanför Adobe Experience Cloud utseende och känsla med produktivitetshöjande innovationer som hjälper marknadsförare att arbeta snabbare och smartare. I den senaste versionen har vi lagt till fullständigt stöd för arbetsytor och partitioner, inklusive möjligheten att dela mappar mellan arbetsytor. Den högra arbetsytan har en växlingsknapp så att du smidigt kan växla mellan gamla och nya upplevelser per funktion utan att tappa kontexten. [Läs ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) mer om nästa generations vanliga frågor om Marketing Nation.

## Flerkanalspersonalisering {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Den befintliga funktionen för Adobe Experience Cloud Audience Sync (AEC) stöder nu kontinuerlig dubbelriktad B2B-målgruppssynkronisering från Marketo Engage till andra AEC-program, inklusive Adobe Experience Platform (AEP)-erbjudanden som Customer Data Platform i realtid och Adobe Experience Platform Activation.  När leads läggs till och tas bort till era målgruppssegment synkroniserar Marketo Engage automatiskt den uppdaterade målgruppen i alla era anslutna AEC-appar. Använd det för att utnyttja Adobe i er flerkanalsmarknadsföring, ommålinriktning, målgruppsundertryckning, personalisering och rapportering.
* **[Continuous Audience Sync to Google, Facebook, and LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Kontinuerligt automatiserad synkronisering med ett annonsnätverk kan aktiveras i en statisk lista och annonsnätverket uppdateras som en listmedlemsändring utan att användaren behöver göra något.
* **[Token för anpassade programmedlemsfält](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Vi har utökat anpassade fältfunktioner för programmedlemmar för att stödja tokenramverket. Marknadsförarna kan infoga anpassade fält-token för programmedlemmar i e-postmeddelanden, landningssidor, SMS-meddelanden, push-meddelanden och webhooks. Använd nya variabler i kampanjflödesåtgärder för att ändra datavärden, skapa en uppgift eller intressanta ögonblick.

## Landningssidor och Forms {#landing-pages-and-forms}

* **Formulär-API**: Hämta in leadinformation eller aktivera närliggande kampanjer och hämta data från andra formulär än Marketo. Formulär från andra företag än Marketo kan integreras med Marketo Engage via REST API. Det nya API:t gör det möjligt att efterlikna Marketo Engage-formulärinlämning med alla tillhörande funktioner.
* **API** för landningssidor: Effektivisera redigerings- och översättningsarbetsflödena i integrerade program med det nya programmeringsgränssnittet Landing Page Preview. Tredjepartsleverantörer kan nu återge helt personliga förhandsvisningar av landningssidor utan att logga in på Marketo Engage.  API:t för landningssidförhandsvisning möjliggör kompletta redigerings- och lokaliseringsarbetsflöden i tredjepartsintegrerade program.

## E-postmarknadsföring {#email-marketing}

* **[Ökade](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)** hämtningsgränser för anpassade objekt: Utvecklare av e-postsnabbskriptning kan snabbt öka antalet anpassade objekt till 100 genom självbetjäning. Marknadsförarna kan öka effektiviteten för smarta kampanjer genom att få tillgång till ett större antal anpassade objekt på första och andra nivån.

## Salesforce CRM-integrering {#salesforce-crm-integration}

* [Salesforce CRM-autentisering](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Protokollet OAuth 2.0 är tillgängligt för synkroniseringsåtgärder mellan Marketo Engage och Salesforce CRM. För nya prenumeranter är det här alternativet aktiverat som standard. Prenumeranter kan begära den här funktionen genom att kontakta Marketo Support.
* [Salesforce CRM Syncing Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratörer kan snabbt granska Salesforce CRM-synkroniseringsstatus från kontrollpanelen. Tidsrymden för synkroniseringsrapporten har ökat från 2 timmar till 5 dagar.
* **Export** av metadata: Förbättrat för att stödja attribut för affärsmöjlighetsobjekt, namngivna konton, programmedlemmens standardfält och anpassade fält.

## Administration {#administration}

* **Sidan** Mitt konto har uppdaterats: Granska viktig prenumerationsinformation på sidan Mitt konto. Användare med alla åtkomstnivåer kan visa prenumerationsnamnet, datacenteridentifieraren och Munchkin-ID:t.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## Sales Insight {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Förbättrade arbetsflöden för testning av e-post (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Öka säljteamets effektivitet med förbättrade e-postflöden för Sales Insight-tester. Säljarna kan skicka testmeddelanden till utvalda e-postadresser innan de skickar massutskick till upp till 200 mottagare.
* **[Insikter i e-poststatus (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Användarna ser ett varningsmeddelande när de försöker skicka ett e-postmeddelande till ett ogiltigt e-post-ID eller en e-postadress som inte längre är prenumererad innan de skickar ett e-postmeddelande.  Leveransstatus för e-postmeddelanden kan granskas på e-postfliken i Sales Insight.
* **Skicka massutskick från  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) konto- och  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) säljprojektspaneler (Salesforce CRM)**: Förbättra effektiviteten i säljarens arbetsflöde och engagera med ett helt konto eller en kontaktlista för affärstillfällen genom att använda nya gruppåtgärdsfunktioner. Skicka e-postmeddelanden eller lägg till kontakter till Marketo Engage-kampanjer med det nya listrutan på kontoflikarna eller på affärsmöjlighetspanelen i stället för att arbeta med enskilda kontakter. Lägg till kontokontakter i en bevakningslista för att få meddelanden när leads blir aktiva.
* **[Sales Insight for Non-Native Salesforce CRM Integrations](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-prenumerationer med anpassade Salesforce CRM-integreringar kan installera Sales Insight-paketet och hjälpa säljarna att prioritera och interagera med de mest lovande leads och möjligheter.
* **[Förbättringar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** av bästa val: Kontakta snabbt aktiva leads från fliken Bästa val genom att mejla eller lägga till dem i en Marketo Engage-kampanj. Visa en lead i Marketo Engage eller lägg till den i bevakningslistan. Gruppåtgärder och sorteringsalternativ på fliken Bästa val sparar tid och förbättrar säljteamets effektivitet.

## Säljanslutning {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **BETA (Email Connection Throttling)**: Förbättra e-postleveransen och skala din personliga säljkommunikation med e-postanslutningsbegränsning för Sales Connect. Vår nya begränsningsteknik hanterar automatiskt e-posttajmning för att skapa sömlösa upplevelser för Exchange- och Gmail-användare. Minska eller eliminera användningen av e-postprogram från tredje part som massutskick.
* **Spårning** av e-postanslutning: Få insikt i hur leads och e-postmallar fungerar med den nya e-poststudsrapporten. Exchange- och Gmail-användare kan välja att ta emot studsmeddelanden som ska samlas i Live-feed, e-postmappar, mallanalys och Campaign Analytics.
* **Konfiguration** av profilsida: Hantera enkelt användarinställningar på den nya profilsidan. Ändra lösenord, redigera geopositionerings- och språkinställningar och granska integreringsstatus på ett och samma ställe.
* **Mallhantering**: Ordna e-postmallar för försäljning i kategorier med en ny dra-och-släpp-funktion som ger snabb åtkomst till relevanta mallar och minskar söktiden.
* **Användarupplevelseuppdateringar** för Sales Connect: Anpassa rutnätslayouten Sales Connect genom att ändra storlek och sortera om kolumner. Dina visningsinställningar sparas automatiskt.

**_Meddelanden och borttagningar_**

* Alla användare måste uppgradera till den senaste versionen av Sales Insight **före 15 januari 2021**. Om du inte har slutfört uppgraderingen uppmanas du att göra det när du loggar in i programmet. Följ instruktionerna [i den här guiden](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Den uppdaterade versionen innehåller en patch för en identifierad säkerhetslucka. Patchen släpptes ursprungligen den 6 april 2016. Obs! **Versionerna 1.4363 eller senare** behöver inte utföra en uppgradering.
* Borttagningen av tjänsten Form 1.0 kommer att träda i kraft i **maj 2021**-versionen. Forms 1.0 är helt inaktuellt, vilket leder till funktionsförlust för alla återstående Forms 1.0-resurser som fortfarande används. Formulärinskickat material som skickats via metoder som inte stöds, t.ex. POST för programmatiska formulär till leadCapture/save och leadCapture/save2-slutpunkterna, kommer att refuseras. Mer information och åtgärder finns i [vårt inlägg i Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021 kommer Marketo Engage att ändra URL-strukturen för landningssidor, formulär samt bilder och filresurser. För befintliga prenumerationer på Marketo Engage börjar vi den gradvisa lanseringen den 1 april 2021. Mer information om tidslinjen kommer att släppas i mars 2021. Mer information om hur varje påverkad resurstyp kommer att ändras finns i [vårt inlägg i Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Product Release Webinar_**

Vill du veta mer om de här funktionerna och förbättringarna? [Registrera dig nu](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) den 21 januari klockan 13:00 PT/04:00 ET för ett live webbinarium med vårt produktteam för att fördjupa dig i dessa innovationer.
