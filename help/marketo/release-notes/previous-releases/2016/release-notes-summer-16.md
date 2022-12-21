---
unique-page-id: 11380218
description: Versionsinformation -Sommaren 16 - Marketo Docs - Produktdokumentation
title: Versionsinformation - Sommaren 16
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Versionsinformation: Sommaren 16 {#release-notes-summer}

Följande funktioner ingår i sommarversionen 16. Se om det finns funktioner i din Marketo-utgåva. Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion.

## [Kontobaserad marknadsföring](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo Account Based Marketing innehåller allt i en och samma plattform:

* **Mål** - Kontoidentifiering, kontomatchning och namngivna kontolistor
* **Engagera** - Kontobaserad personalisering, flerkanalsengagemang och kontospecifika arbetsflöden
* **Mät** - Insikter på konto- och listnivå, kundengagemangspoäng samt pipeline- och intäktseffekt

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM finns som tillägg till din Marketo-prenumeration, så kontakta din säljare för att få det implementerat.

## [Granskningsspår](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

Granskningsspårning ger en omfattande historik över de ändringar som gjorts i din Marketo-prenumeration. Det kommer att skapa ansvar bland användare och administratörer, hjälpa till att identifiera orsaken till oväntat beteende och ge säkerhet för att veta vem som gör vad och när. Denna information kommer att finnas tillgänglig när som helst och kan användas för att besvara frågor som:

* Vad hände med den här resursen eller inställningen och vem uppdaterade den senast?
* Vad har X gjort?
* Vem loggar in på vårt konto?

![](assets/audit-trail.png)

## [Marketo-Vibes SMS LaunchPoint-integrering](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Skapa enkelt SMS-meddelanden direkt i Marketo. Anpassa och anpassa ert budskap med hjälp av era omfattande Marketo-data och övervaka enkelt hur det fungerar med SMS-meddelandeinstrumentpanelen.

>[!NOTE]
>
>Den här funktionen kräver att du har ett befintligt Vibes SMS-konto.

![](assets/vibes-sms2.png)

## [Förbättringar i e-post 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variabler på modulnivå**

Tidigare var alla variabler som angavs i e-postmallar&quot;globala&quot; i omfånget. När du använder variabler i moduler är detta inte alltid önskvärt om du tänker använda flera instanser av modulen. I den här versionen kan variabler nu anges som&quot;modulnivå&quot;, vilket gör att du kan ange att användaren ska kunna ange unika värden för varje modul som de används i.

![](assets/module-level-variables.png)

**Syntaxuppdateringar**

* Du kan nu använda mktoAddByDefault för moduler som anges i e-postmallar 2.0 för att ange vilka moduler som ska visas i nya e-postmeddelanden som standard. Detta är mycket bekvämare om du skapar en e-postmall med ett stort antal moduler.
* På bildelement kan du nu ange om den underliggande `<img>` HTML-elementets &quot;height&quot; och &quot;width&quot;-egenskaper ska vara låsta eller redigerbara för slutanvändaren. mktoLockImgSize=&quot;true&quot; gör att höjd/bredd låses (även om bilden ändras). På samma sätt kommer mktoLockImgStyle=&quot;true&quot; att göra så att egenskapen &quot;style&quot; låses.

**Kodsökning**

Använd den nya sökfunktionen för att effektivt söka och ersätta innehåll i e-postkoden. Den här funktionen är också tillgänglig i redigeraren för e-postmallar.

![](assets/2nd-screenshot.png)

**Token Support i Image Elements**

Token kan nu användas i området &quot;Extern URL&quot; i infogningsbildens upplevelse! Om du har angett bilder med `{{my.tokens}}`kan du nu referera till dessa variabler i e-postredigeraren 2.0. Observera att bilden fortfarande visas som skadad på arbetsytan i e-postredigeraren 2.0. Men du kommer att se dem renderade i Förhandsgranska och Skicka exempel innan du skickar ut ditt e-postmeddelande.

## Flera profildomäner {#multiple-branding-domains}

Det är inte alltid då e-postspårningslänkar bara kan profileras med en enda varumärkesdomän. Nu kan ni lägga till flera olika varumärkesdomäner för att få konsumenterna att känna sig trygga, skapa ett effektivare varumärke, förbättra e-postleveransen och, per e-post, välja vilken varumärkesdomän som ska användas för varje e-posts spårningslänkar.

![](assets/multiple-branding-domains.png)

## [Programtoken](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Vi har skapat en ny tokentyp för program. Nu kan du återge programnamn, beskrivning och ID i resurser och smarta kampanjflödessteg.

![](assets/program-tokens.png)

## [Företagsnyckel](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Att kräva att varje person i säljteamet installerar vårt Sales Insight-plugin för Outlook kan vara tråkigt. Vi har introducerat ett nytt sätt att fjärrinstallera plugin-programmet för Outlook med en företagsnyckel. Skicka din IT-avdelning en unik nyckel som finns i Marketo Sales Insight-delen av Admin och låt dem göra resten.

![](assets/enterprise-key.png)

## [Webbpersonaliseringskampanjer](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Ange en tidsfördröjning för webbkampanjer att reagera på webbplatsen.

![](assets/dialog-campaign-delay.png)

## [Content Analytics och Recommendations Export](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Visa innehållsanalyser och rekommendationer offline.

## [API-stöd för e-postredigeraren 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Redan befintliga resurs-API:er, som tidigare bara var kompatibla med e-post och mallar i version 1.0, är nu aktiverade för e-postresurser i version 2.0.

## [Marketo Developer Site](https://developers.marketo.com/) {#marketo-developers-site}

Nytt och förbättrat!

## [Sekretessinställningar](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Marknadsförarna kan använda integritetsinställningar för att bestämma om de ska spåra besökare med hjälp av Munchkin- och webbpersonaliseringsfunktionerna. Spårningsnivån styrs av webbläsarens inställningen Spåra inte, en cookie för avanmälan eller en icke-specifik IP-adress. Dessa metoder kan påverka Marketo värde och funktionalitet inom specifika områden, men om marknadsföraren inte ändrar någonting ändras inte funktionen i Marketo.

Den här funktionen kommer gradvis att lanseras för kunderna under en period av sex veckor. Kontakta Marketo Support om du behöver det direkt.
