---
unique-page-id: 13795395
description: Versionsinformation -vinter '18 - Marketo Docs - produktdokumentation
title: Versionsinformation -vinter '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Versionsinformation: Vinter 18 {#release-notes-winter}

Följande funktioner finns i vinterversionen 18. Se om det finns funktioner i Marketo Edition.

Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion. **Obs!**: Vissa av funktionerna i den här versionen har inte associerade artiklar. Om ett ämne har flera underrubriker placeras länkarna där.

## Förbättringar av kampanjprestanda och dataflöde {#campaign-performance-and-throughput-enhancements}

Marketo utnyttjar vår big data-arkitektur för att öka kampanjens genomströmning och förbättra webbaktivitetsbearbetningen, så att ni kan reagera snabbare på målgruppens handlingar.

## Förbättringar av Marketo [!DNL Salesforce] CRM-integrering {#enhancements-to-marketo-s-salesforce-crm-integration}

Vi har två förbättringar av vår [!DNL Salesforce] CRM-integrering:

* [Marketo Admin-meddelanden](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) för vissa CRM-synkroniseringsfel (autentiseringsuppgifterna har upphört att gälla, API-gränser har uppnåtts osv.)

* [Möjlighet att inaktivera e-postmeddelanden](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) till lead-ägare vid leadtilldelning

Dessa förbättringar kommer att öka under 2018.

## [Marketo Performance Insights](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>[!UICONTROL Performance Insights] är en tilläggsprodukt. Kontakta din Marketo Customer Success Manager eller kontoansvarige för en offert.

Se hur era kampanjer och kanaler påverkar affärsresultaten med attribueringsanalys, interaktiva visualiseringar och en detaljerad datatabell.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Kontobaserade marknadsföringsförbättringar {#account-based-marketing-enhancements}

**[ABM-hierarkier](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

För ABM-kunder med [!DNL Salesforce] eller [!DNL Microsoft Dynamics] ärver nu ABM automatiskt (och visar) de överordnade och underordnade relationer som skapats i CRM. Du kommer att kunna använda dessa relationer i både sammanslagningsrapportering och kampanjkörning.

## E-postmarknadsföring {#email-marketing}

**[Dynamiskt e-postskript](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Snabb skriptning stöds nu i e-postmeddelanden med dynamiskt innehåll. Kombinera snabbt och segmenteringsbaserat dynamiskt innehåll för att skapa personaliserade e-postmeddelanden.

**Mottagarens tidszon**

* **[Månadsvis sjuksköterska](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Vi har lagt till möjligheten att schemalägga vårdprogram en gång i månaden.

* **[Stoppa leverans](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Nu kan du stoppa alla återstående meddelanden som skickas mitt i körningen.

## Annonsnätverksintegrering {#ad-network-integrations}

**[Google kundmatchningsintegrering](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Med den här integreringen kan du skicka en Marketo-målgrupp till Google för målgruppsanpassning med [!DNL Google AdWords], samt ändra målgruppsanpassning för [!DNL YouTube], Search och [!DNL Gmail].

**[[!DNL LinkedIn] API-förbättring för matchade målgrupper](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Med vårt nya [!DNL LinkedIn]-API kan du nu rikta om personer i din Marketo-databas till flera [!DNL LinkedIn] Campaign Manager-konton.

## Web Personalization {#web-personalization}

**Japanska data, Source för webben, Personalization**

Marketo lägger till ytterligare en japansk datakälla för Web Personalization för att förbättra identifieringen (omvänd IP-sökning) och personaliseringen för besökare som kommer från Japan. Organisationsnamn visas på japanska.

**[Skapa ett webbsegment med statiska listor](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization kan nu personalisera innehåll för en känd webbbesökare som ingår i en statisk lista som definieras i marknadsföringsaktiviteter (MLM). Med den här förbättringen kan ni nu marknadsföra statiska listor över alla kanaler och rikta in er på personer på dessa listor med personaliserat innehåll på er webbplats.

## ContentAI {#contentai}

**Förbättring av prediktiv algoritm**

Innehåll som rekommenderas via Marketo optimerade ContentAI-algoritmer genererar upp till dubbelt så många klick som slumpmässigt innehåll.

## Integrering {#integration}

**[Aktivera/inaktivera kampanj-API &#x200B;](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Detta nya API gör att ni kan aktivera och inaktivera utlösarkampanjer via fjärranslutning, så att ni nu kan skapa helt automatiserade programmallar. Skapa en programmall en gång, automatisera kloningen, uppdatera marknadsföringsmaterialet och nu aktivera/schemalägga smarta kampanjer.

## [!DNL ToutApp] {#toutapp}

**Avbeställ uppdatering**

Från och med 1 mars 2018 kommer alla e-postmeddelanden som skickas från [ToutApp.com](https://ToutApp.com) (och med knappen&quot;E-post med [!DNL Tout]&quot; i [!DNL Salesforce]) att ha en länk för att avbryta prenumerationen längst ned.

**Uppdatering av Live-feed**

Vi har uppdaterat utseende och känsla på flikarna Engagement och Task för att göra det enklare och snabbare för säljarna att svara på kundernas aktiviteter direkt från Live Feed.

**Uppdatering av personinformationsvyn**

Den förbättrade personinformationsvyn (PDV) ger en heltäckande bild av dina kontakter genom att sammanföra din [!DNL Tout]- och [!DNL Salesforce] CRM-kontaktinformation.
