---
description: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter - Marketo Docs - Produktdokumentation
title: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

När du har [skapat ett SMS-meddelande från Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"} vill du använda utlösare och filter för Smart List i en smart kampanj för att få fördelarna. Så här gör du.

1. Klicka på **Marknadsföringsaktiviteter** i Min Marketo.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Välj en smart kampanj där du vill använda dina SMS-resurser. Dra över en utlösare. I det här exemplet använder vi **Fyller i formulär**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-utlösare {#sms-triggers}

Det finns andra SMS-utlösare tillgängliga. SMS-utlösarna visas bara om tjänsten Vibes är aktiverad.

SKICKA ETT SMS:

* Marknadsföringsaktiviteter > välj Ny smart kampanj
   * Smart List > Choose Vibes List filter &amp; correct logic > Vibes list: Choose list from drop-down (lista över mobila databaser som synkroniseras från Vibes-plattformen)
      * Kan förfina segmenteringen och använda SMS och e-postfilter och utlösare i en kampanj
      * Vibes-filter: Prenumererar på Vibes List jämfört med Medlem i Vibes List - logiken överensstämmer med e-post
         * Prenumererar på Vibes List - deltagare som tidigare har prenumererat på den Vibes-listan, även om de nu har avbrutit prenumerationen.  - huvudsakligen används för flerkanalsmarknadsföring
            * Obs! Ett SMS-meddelande kommer inte att skickas till någon som avbeställt prenumerationen om de inte finns med i listan Vibes Mobile Database
         * Medlem i Vibes List - aktiv, bekräftad prenumerant
         * Tillagd i lista - listorna Vibes kommer inte att fyllas i med det här filtret; detta gäller för Marketo-listor

![](assets/new-sms-search2.png)

Här är några exempel:

Utlösaren **SMS Message Bounces** initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

![](assets/sms-message-bounces-real.jpg)

Utlösaren **Prenumererar på Vibes List** initierar ett flöde när en person prenumererar.

![](assets/subscribes-to-vibes-list-real.jpg)

Utlösaren **Click Link in SMS Message** initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-filter {#sms-filters}

Du kan också använda Vibes-filter i smarta listor. Filtret **Prenumererar på Vibes-listan** hittar alla som har *någonsin* prenumererat på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Filtret **Medlem i listan** hittar däremot _alla_ som prenumererar på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

![](assets/image001.png)

>[!NOTE]
>
>Alla SMS-filter innehåller begränsningen **Aktivitetsdatum** som standard.

När du har konfigurerat Vibes-utlösare och -filter i din smarta lista kan du [definiera flödet](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definiera smart lista för smart kampanj | Utlösare ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Söka efter och lägga till filter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
