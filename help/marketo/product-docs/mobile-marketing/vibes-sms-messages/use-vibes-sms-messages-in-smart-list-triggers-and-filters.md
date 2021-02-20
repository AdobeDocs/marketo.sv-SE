---
unique-page-id: 11378871
description: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter - Marketo Docs - Produktdokumentation
title: Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# Använd Vibes SMS-meddelanden i Smart List-utlösare och -filter {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

När du har [skapat ett Vibes SMS-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) vill du använda smarta listutlösare och filter i en smart kampanj för att få fördelarna. Så här gör du.

1. Klicka på **Marknadsföringsaktiviteter** på My Marketo.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Välj en smart kampanj där du vill använda din SMS-resurs. Dra över en utlösare, t.ex. populära **Fyller i formulär**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-utlösare {#sms-triggers}

Det finns andra SMS-utlösare tillgängliga. SMS-utlösarna visas bara om tjänsten Vibes är aktiverad.

![](assets/new-sms-search2.png)

Här är några exempel:

SMS Message Bounces-utlösaren initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

![](assets/sms-message-bounces-real.jpg)

Utlösaren **Prenumererar på Vibes List** initierar ett flöde när en person prenumererar.

![](assets/subscribes-to-vibes-list-real.jpg)

Utlösaren **Click Link in SMS Message** initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-filter {#sms-filters}

Du kan också använda Vibes-filter i smarta listor. Filtret **Prenumererar på Vibes-listan** hittar alla som *någonsin* prenumererar på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Filtret **Member of Vibes List** hittar _alla_ som prenumererar på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

![](assets/image001.png)

>[!NOTE]
>
>Alla SMS-filter innehåller begränsningen **Aktivitetsdatum** som standard.

När du har konfigurerat Vibes-utlösare och -filter i din smarta lista kan du [definiera flödet](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Söka efter och lägga till filter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

