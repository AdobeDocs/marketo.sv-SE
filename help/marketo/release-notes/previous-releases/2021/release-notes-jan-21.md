---
description: Versionsinformation - jan 2021 - Marketo Docs - produktdokumentation
title: Versionsinformation - jan 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1235'
ht-degree: 0%

---

# Versionsinformation: jan 2021 {#release-notes-jan-21}

Följande funktioner finns i jan 21. Se om det finns funktioner i Marketo Edition.

>[!AVAILABILITY]
>
>Funktioner som anges av en stjärna (![(stjärna)](assets/yellow-star.png)) är betalda tillägg. Kontakta Marketo Engage om du vill veta mer.

**_Kvartalsvisa releaser_**

Följande funktioner kommer att släppas den **15 januari 2021**.

## Nästa generations användarupplevelse {#next-generation-user-experience}

* Stöd för Workspaces: Marketo Engage nästa generation av användare förenar Adobe Experience Cloud känsla med produktivitetshöjande innovationer som hjälper marknadsförare att arbeta snabbare och smartare. I den senaste versionen har vi lagt till fullständigt stöd för arbetsytor och partitioner, inklusive möjligheten att dela mappar mellan arbetsytor. Den högra arbetsytan har en växlingsknapp så att du smidigt kan växla mellan gamla och nya upplevelser per funktion utan att tappa kontexten. [Läs mer](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) i nästa generations Frågor och svar om Marketing Nation.

## Flerkanaliga Personalization {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Den befintliga funktionen för Adobe Experience Cloud Audience Sync har nu stöd för dubbelriktad B2B-målgruppssynkronisering från Marketo Engage till andra AEC-program, inklusive Adobe Experience Platform (AEP)-erbjudanden som Real-time Customer Data Platform och Adobe Experience Platform Activation.  När leads läggs till och tas bort till era målgruppssegment synkroniserar Marketo Engage automatiskt den uppdaterade målgruppen i alla era anslutna AEC-appar. Använd det för att utnyttja Adobe flerkanalsmarknadsföring, ommålinriktning, målgruppsdämpning, personalisering och rapportering i hela er AEC-teknologi.
* **[Kontinuerlig målgruppssynkronisering till Google, [!DNL Facebook] och [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Kontinuerlig automatiserad synkronisering med ett annonsnätverk kan aktiveras i en statisk lista och annonsnätverket uppdateras som en lista över medlemsändringar utan att användaren behöver göra något.
* **[Token för anpassade fält för programmedlemmar](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Vi har utökat anpassade fältfunktioner för programmedlemmar för att stödja tokenramverket. Marknadsförarna kan infoga anpassade fält-token för programmedlemmar i e-postmeddelanden, landningssidor, SMS-meddelanden, push-meddelanden och webhooks. Använd nya variabler i kampanjflödesåtgärder för att ändra datavärden, skapa en uppgift eller intressanta ögonblick.

## Landningssidor och Forms {#landing-pages-and-forms}

* **Formulär-API**: Dra in lead-information eller aktivera närliggande kampanjer samtidigt som data hämtas från icke-Marketo-formulär. Formulär från andra företag än Marketo kan integreras med Marketo Engage via REST API. Det nya API:t gör det möjligt att efterlikna inskickandet av Marketo Engage-formulär med alla tillhörande funktioner.
* **API för landningssidor**: Effektivisera arbetsflödena för redigering och översättning i integrerade program med det nya API:t för landningssidförhandsvisning. Tredjepartsleverantörer kan nu återge helt personliga förhandsvisningar av landningssidor utan att logga in på Marketo Engage.  API:t för landningssidförhandsvisning möjliggör kompletta redigerings- och lokaliseringsarbetsflöden i tredjepartsintegrerade program.

## E-postmarknadsföring {#email-marketing}

* **[Hämtningsgränser för anpassade objekt har ökats](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Utvecklare av skriptning för e-posthastighet kan snabbt öka antalet anpassade objekt till 100 genom självbetjäning. Marknadsförarna kan öka effektiviteten för smarta kampanjer genom att få tillgång till ett större antal anpassade objekt på första och andra nivån.

## CRM-integrering för [!DNL Salesforce] {#salesforce-crm-integration}

* [[!DNL Salesforce] CRM-autentisering](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Protokollet OAuth 2.0 är tillgängligt för synkroniseringsåtgärder mellan Marketo Engage och [!DNL Salesforce] CRM. För nya prenumeranter är det här alternativet aktiverat som standard. Prenumeranter kan begära den här funktionen genom att kontakta Marketo Support.
* [[!DNL Salesforce] CRM Syncing Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratörer kan snabbt granska [!DNL Salesforce] CRM-synkroniseringsstatus från kontrollpanelen. Tidsrymden för synkroniseringsrapporten har ökat från 2 timmar till 5 dagar.
* **Export av metadata**: Förbättrad för att stödja attribut för affärsmöjlighetsobjekt, namngivna konton, programmedlemmens standardfält och anpassade fält.

## Administrering {#administration}

* **Uppdaterad min kontosida**: Granska viktig prenumerationsinformation på sidan Mitt konto. Användare med alla åtkomstnivåer kan visa prenumerationsnamnet, datacenteridentifieraren och [!DNL Munchkin]-ID:t.

**_Frigör under hela kvartalet_**

Följande funktioner finns på en icke-kvartalsvis cykel och kommer att släppas under de kommande månaderna.

## [!DNL Sales Insight] {#sales-insight}

![(stjärna)](assets/yellow-star.png)

* **[Förbättrade arbetsflöden för testning av e-post ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Öka säljteamets effektivitet med förbättrade [!DNL Sales Insight] testarbetsflöden för e-post. Säljarna kan skicka testmeddelanden till utvalda e-postadresser innan de skickar massutskick till upp till 200 mottagare.
* **[Insikter i e-poststatus ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Användarna ser ett varningsmeddelande när de försöker skicka ett e-postmeddelande till ett ogiltigt e-post-ID eller en e-postadress som de avbeställt innan de skickar ett e-postmeddelande.  E-postleveransstatus kan granskas på e-postfliken i [!DNL Sales Insight].
* **Skicka massutskick från [konto](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) och [säljprojektspaneler](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) ([!DNL Salesforce] CRM)**: Förbättra effektiviteten i säljarens arbetsflöde och engagera med ett helt konto eller en kontaktlista för affärstillfällen genom att använda nya gruppåtgärdsfunktioner. Skicka e-post eller lägg till kontakter till Marketo Engage-kampanjer med det nya listrutan på kontoflikarna eller på affärsmöjlighetspanelen i stället för att arbeta med enskilda kontakter. Lägg till kontokontakter i en bevakningslista för att få meddelanden när leads blir aktiva.
* **[[!DNL Sales Insight] för icke-ursprungliga [!DNL Salesforce] CRM-integreringar](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-prenumerationer med anpassade Salesforce CRM-integreringar kan installera [!DNL Sales Insight]-paketet och hjälpa säljarna att prioritera och interagera med de mest lovande leads och affärsmöjligheter.
* **[Förbättringar av bästa val](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Kontakta snabbt aktiva leads från fliken Bästa val genom att skicka dem med e-post eller lägga till dem i en Marketo Engage Campaign. Visa en lead i Marketo Engage eller lägg till den i bevakningslistan. Gruppåtgärder och sorteringsalternativ på fliken [!UICONTROL Best Bets] sparar tid och förbättrar säljteamets effektivitet.

## [!DNL Sales Connect] {#sales-connect}

![(stjärna)](assets/yellow-star.png)

* **Begränsning av e-postanslutning (BETA)**: Förbättra e-postleveransen och skala din :1-säljkommunikation med begränsning av e-postanslutning för [!DNL Sales Connect]. Vår nya begränsningsteknik hanterar automatiskt e-posttajmning för att skapa sömlösa upplevelser för [!DNL Exchange]- och Gmail-användare. Minska eller eliminera användningen av massutskick från tredje part.
* **Spårning av studsande e-postanslutning**: Få insikt i lead-kvalitet och prestanda för e-postmallar med den nya studsrapporten för e-post. [!DNL Exchange]- och Gmail-användare kan välja att ta emot studsmeddelanden som samlas in till Live-feed, e-postmappar, mallanalys och kampanjanalys.
* **Profilsidkonfiguration**: Hantera användarinställningar enkelt på den nya profilsidan. Ändra lösenord, redigera geopositionerings- och språkinställningar och granska integreringsstatus på ett och samma ställe.
* **Mallhantering**: Ordna e-postmallar för försäljning i kategorier med en ny dra och släpp-funktion som ger snabb åtkomst till relevanta mallar och minskar söktiden.
* **[!DNL Sales Connect]Uppdateringar av användarupplevelsen**: Anpassa [!DNL Sales Connect]-stödrasterlayouten genom att ändra storlek på och sortera om kolumner. Dina visningsinställningar sparas automatiskt.

**_Meddelanden och borttagningar_**

* Alla användare måste uppgradera till den senaste versionen av Sales Insight **före den 15 januari 2021**. Om du inte har slutfört uppgraderingen uppmanas du att göra det när du loggar in i programmet. Följ instruktionerna [i den här handboken](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Den uppdaterade versionen innehåller en patch för en identifierad säkerhetslucka. Patchen släpptes ursprungligen den 6 april 2016. Obs! **Versionerna 1.4363 eller senare** behöver inte utföra en uppgradering.
* Borttagning av tjänsten Form 1.0 träder i kraft i **maj 2021** . Forms 1.0 är helt inaktuellt, vilket leder till funktionsförlust för alla återstående Forms 1.0-resurser som fortfarande används. Formulärinskickat material som skickats via metoder som inte stöds, t.ex. POST för programmatiska formulär till leadCapture/save och leadCapture/save2-slutpunkterna, kommer att refuseras. Mer information och åtgärder finns i [vårt inlägg i Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021 kommer Marketo Engage att ändra URL-strukturen för landningssidor, formulär samt bilder och filresurser. För befintliga Marketo Engage-prenumerationer börjar vi den gradvisa lanseringen den 1 april 2021. Mer information om tidslinjen kommer att släppas i mars 2021. Mer information om hur varje påverkad resurstyp ändras finns i [vårt inlägg i Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webbseminarium om produktreleaser_**

Vill du veta mer om de här funktionerna och förbättringarna? Var noga med att [registrera dig nu](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) och gå med oss den 21 januari klockan 12:00 PT/4:00 PM för ett live webbinarium med vårt produktteam för att fördjupa dig i dessa innovationer.:00
