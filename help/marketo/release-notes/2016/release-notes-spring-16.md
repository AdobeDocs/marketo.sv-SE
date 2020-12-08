---
unique-page-id: 11370952
description: Versionsinformation -Spring '16 - Marketo Docs - Produktdokumentation
title: Versionsinformation - våren 16
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---


# Versionsinformation: Spring &#39;16 {#release-notes-spring}

Följande funktioner finns i vårutgåvan 16. Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion.

## [E-postinsikter](http://docs.marketo.com/display/docs/email+insights) {#email-insights}

E-postinsikter är en helt ny historik över e-postanalyser av sammanställda data - helt omdesignade för blixtsnabba prestanda som en del av Project Orion. Den har ett helt nytt användargränssnitt som är optimerat för att passa e-postmarknadsförarnas behov och arbetsflöde.

>[!NOTE]
>
>Vi lanserar e-postinsikter för kunder i grupp, från den 3 juni. Vårt mål är att slutföra detta under de kommande månaderna. Vi meddelar dig via e-post när du har aktiverat.

![](assets/two.png)

## [Väljare för e-postmall](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Skapa vackra e-postmeddelanden med våra nya startmallar! Du kan också snabbt hitta mallarna från miniatyrbilderna.

>[!NOTE]
>
>E-postredigeraren 2.0 (med mallväljaren) kommer gradvis att lanseras från och med den 3 juni. Vi kommer att vara klara den 30 juni. Till skillnad från e-postinsikter meddelas du inte när du har åtkomst. Om du vill se om du gör det följer du stegen i [den här artikeln](https://docs.marketo.com/pages/viewpage.action?pageId=11373011).

![](assets/5-29-home-starter-templates.png)

## [E-postredigering - omdesignad](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

Det stämmer, en helt ny e-postredigerare! Använd lättanvända dra-och-släpp-funktioner för att lägga till och ordna om innehåll. Nya element som bilder, videor, variabler och moduler kommer att förbättra redigeringsupplevelsen. Se även den uppdaterade kodredigeraren, förhandsgranskaren och stödet för preheader.

![](assets/17a-29-modules-next.png)

## [Meddelanden i appar för mobiler](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Skapa fantastiska meddelanden i appen för er app direkt inifrån Marketo. Definiera exakt vem som ska se det och när med meddelandeprogrammet i appen. Övervaka enkelt programmets prestanda med kontrollpanelen.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Inga utkast](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Nu är det dags att omgodkänna allt varje gång ett textutdrag uppdateras! Med No-Draft får alla e-postmeddelanden och landningssidor som använder ett utdrag kodfragmentsuppdateringar och deras tidigare status bibehålls. Varje gång du godkänner ett fragment kan du välja att köra No-Draft och uppdatera allt eller skapa utkast. Det är upp till dig! No-Draft blir tillgängligt för alla kunder och styrs av ett nytt tillstånd i Admin.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Anpassade aktiviteter](http://docs.marketo.com/display/docs/marketo+custom+activities) {#custom-activities}

Marketo-administratörer kan nu definiera och hantera sina anpassade aktivitetstyper via Marketo Custom Activity Definition-modelleraren. På samma sätt som (och i kombination med) Marketo Custom Object Modeler kan administratörer nu utöka datamodellen för att passa just deras affärsbehov. Information om hur du använder den här funktionen finns på [Marketos dokumentationswebbplats](https://docs.marketo.com/display/public/DOCS/Marketo+Custom+Activities).

## [Landningssida, landningssidmall och formulär-API:er](http://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Marketo REST API:er har nu stöd för kontroll över Marketo-landningssidor, landningssidmallar och formulär. Användarna kan nu skapa, uppdatera, godkänna och ta bort dessa resurser direkt via Marketo REST API.

## [IP-Tillåtelselistning för API-åtkomst](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

På samma sätt som funktionen för IP-tillåtelselistning för Marketo-användarinloggningar kan Marketo-administratörer nu ställa in ett tillåtelselista med IP-adresser som kan komma åt Marketo SOAP- och REST-API:er, vilket blockerar åtkomst från icke-auktoriserade IP-adresser. Detta lägger till ett extra säkerhetsskikt till din Marketo-instans och ser till att API-åtkomst bara kan ske inifrån organisationens nätverk. Information om hur du konfigurerar detta finns på [Marketos dokumentationswebbplats](https://docs.marketo.com/display/public/DOCS/Create+a+Whitelist+for+IP-Based+API+Access).

## [Ny Microsoft Dynamics Sync Connector med hög hastighet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Bygg på Orion-arkitekturen - den nya höghastighetsanslutningen för dynamik ger hastigheter upp till 20 gånger snabbare för inledande synkronisering och upp till 5 gånger snabbare för inkrementell synkronisering. Alla nya kunder kommer att ansluta sig till den här kontakten på releasedatum, och vi kommer gradvis att lansera den för befintliga kunder under sommarreleasetidningen.

**Uppdatera data för nya fält**: Nu kan du aktivera nya synkroniseringsfält när som helst och alla datavärden för det fältet uppdateras från Dynamics CRM till Marketo. Du behöver inte längre oroa dig för att du måste markera alla fält under den första konfigurationen. Om du inaktiverar ett befintligt synkroniseringsfält och sedan aktiverar det igen uppdateras alla datavärden för det fältet från Dynamics CRM till Marketo.

**Synkronisera lead som kontakt**: Åtgärden Synkronisera lead till Microsoft-flöde har ett nytt alternativ för att synkronisera som lead eller kontakt.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Fliken** Synkroniseringsfel:  Sök, sök och exportera leads (och andra objekt) som inte kunde synkroniseras med information som åtgärd, riktning, felkod och felmeddelande.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: Connector är helt certifierad för Dynamics 2016 Online- och On-Local-versioner.

**Plugin-uppdateringarna finns nu dokumenterade:** Se artikeln [om uppdatering av](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)plugin-program.

## [Eget instansnamn](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Idag är det svårt att skilja mellan Marketo-instanser, till exempel sandbox- och produktionsinstanser. Med den här funktionen kan du ta reda på vilka instanser du arbetar med just nu.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Tidsbegränsad åtkomst för prenumerationer](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Idag bjuds användare in till Marketo-prenumeration för en obegränsad tidsperiod. Med den här funktionen kan administratörer bjuda in användare till prenumerationer under en begränsad tidsperiod, till exempel två veckor eller en månad.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Rutnät för anpassade objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Nu kan du visa antalet poster och fält för alla publicerade anpassade objekt.

![](assets/custom-objects-grid.png)
