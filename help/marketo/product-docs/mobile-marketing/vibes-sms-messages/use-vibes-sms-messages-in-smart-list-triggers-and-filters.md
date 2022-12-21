---
unique-page-id: 11378871
description: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter - Marketo Docs - Produktdokumentation
title: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Efter [skapa ett Vibes SMS-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)vill ni använda smarta listutlösare och filter i en smart kampanj för att få fördelarna. Så här gör du.

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Välj en smart kampanj där du vill använda din SMS-resurs. Dra över en utlösare, till exempel den populära **Fyller i formulär**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-utlösare {#sms-triggers}

Det finns andra SMS-utlösare tillgängliga. SMS-utlösarna visas bara om tjänsten Vibes är aktiverad.

![](assets/new-sms-search2.png)

Här är några exempel:

SMS Message Bounces-utlösaren initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

![](assets/sms-message-bounces-real.jpg)

The **Prenumererar på Vibes List** utlösaren initierar ett flöde när en person prenumererar.

![](assets/subscribes-to-vibes-list-real.jpg)

The **Klicka på Länk i SMS-meddelande** utlösaren initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-filter {#sms-filters}

Du kan också använda Vibes-filter i smarta listor. The **Prenumererar på Vibes List** filter hittar alla som *någonsin* prenumererar på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

I motsats till **Medlem i Vibes List** filtersökningar _alla_ prenumererar för närvarande på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

![](assets/image001.png)

>[!NOTE]
>
>Alla SMS-filter innehåller **Aktivitetsdatum** -begränsning som standard.

När du har konfigurerat Vibes-utlösare och -filter i din smarta lista kan du [definiera flödet](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Söka efter och lägga till filter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

