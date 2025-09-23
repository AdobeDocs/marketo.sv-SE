---
unique-page-id: 10097199
description: Versionsinformation -vinter '16 - Marketo Docs - produktdokumentation
title: Versionsinformation -vinter '16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Versionsinformation: Vinter 16 {#release-notes-winter}

Följande funktioner ingår i vinterversionen 16. Klicka på titellänkarna för att visa detaljerade artiklar för varje funktion.

## [är ett anonymt filter](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Filtret Är anonym har tagits bort för smarta listor. Mer information finns i dokumentet [Next Generation Munchkin Tracking FAQ](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md). Ändringen påverkar inte Web Personalization (RTP), som fortsätter att identifiera anonyma och kända webbesökare och personalisera innehåll i realtid för dessa besökare.

## [Databasinstrumentpanel](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md)  {#database-dashboard}

[!UICONTROL Lead Database] har en uppdaterad sammanfattningsinstrumentpanel som innehåller databasstorlek för totalt antal personer, antal säljbara leads och en uppdelning av leads efter de fem främsta källorna.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Microsoft Edge Browser](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Vi har lagt till [!DNL Microsoft Edge] i listan [över webbläsare](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) som stöds av Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[[!DNL Microsoft Outlook] 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) stöds nu.

## [Start för e-postprogram](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Använd [!UICONTROL Head Start] för att ange att bearbetningen för din sändning ska ske i förväg. I stället för att kvalificera leads och förbereda e-postmeddelanden vid den schemalagda tidpunkten för programmet, ser [!UICONTROL Head Start] till att dessa uppgifter utförs i förväg. På så sätt får er målgrupp e-post vid den schemalagda tidpunkten.

![](assets/image2016-1-11-15-3a38-3a3.png)

Om du vill använda den här funktionen måste e-postprogrammet vara schemalagt minst 12 timmar i förväg och den smarta listan kommer att vara låst 12 timmar före sändningen.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Den här funktionen kommer gradvis att lanseras under en vecka efter vinterversionen 16. Den kan inte användas med smarta kampanjer eller API:t.

## [Förbättringar av mobilmarknadsföring](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**[!DNL PhoneGap]Support:** Vi erbjuder nu [!DNL PhoneGap] support för din mobilapp. [Läs mer](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Stöd för sandlådeappar**:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [Program-API](https://developers.marketo.com/documentation/programs/) {#program-api}

Skapa, uppdatera och klona program via REST API. Detta inkluderar inte skapande eller uppdatering av smarta listor och smarta kampanjer i ett program.

## [Microsoft Dynamics-förbättringar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[[!UICONTROL Sync Status]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)**: Håll reda på synkroniseringsprocessens aktuella genomströmning och eftersläpning. Bryt ned den med antalet infogningar och uppdateringar per objekt.

![](assets/pending-backog-cropped.png)

**[[!UICONTROL Notifications]](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: Få meddelanden om vanliga synkroniseringsfel, tillsammans med en lista över leads som har det felet.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Förbättringar av anpassade objekt](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

Nu kan du skapa många-till-många-relationer mellan leads/konton och ett anpassat objekt genom att använda ett mellanliggande objekt med flera länkfält.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Leadannonser för Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[[!UICONTROL Facebook Lead ads]](https://www.facebook.com/business/a/lead-ads) är ett mer direkt sätt för ett företag att köra lead-genereringskampanjer på [!DNL Facebook]. Användarna fyller i en blankett för att uttrycka sitt intresse för en produkt eller tjänst, så att företaget kan följa upp med dem. Marketo-integrationen med [!UICONTROL Facebook Lead Ads] hämtar automatiskt information som ett lead tillhandahåller i formuläret Lead Ad. Uppföljningsåtgärder och meddelanden kan sedan automatiseras med den nya [!UICONTROL Fills Out Facebook Lead Ads]-utlösaren.

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Webbkampanjschemaläggare (Personalization i realtid)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Schemalägg kampanjen i förväg. Ange ett start- och slutdatum för personaliserat webbinnehåll och upprepa kampanjer på specifika dagar och tidpunkter. Anpassa schemat för att visa kampanjen efter besökarens tid eller en vald tidszon.

![](assets/image2016-1-14-8-3a36-3a36.png)
