---
description: Använd SMS-alternativ i Smart List-utlösare och -filter - Marketo Docs - Produktdokumentation
title: Använd SMS-alternativ i Smart List-utlösare och -filter
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Använd SMS-alternativ i Smart List-utlösare och -filter {#use-sms-options-in-smart-list-triggers-and-filters}

NYTT DOC

Efter dig [skapa ett SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}vill du använda utlösare och filter för smarta listor i en smart kampanj för att få fördelarna.

>[!PREREQUISITES]
>
>SMS-utlösare/filter visas bara om [Vibes-tjänsten har aktiverats](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## SMS-utlösare {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

Här är några exempel:

The **SMS-meddelandestudsar** utlösaren initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

The **Prenumererar på Vibes List** utlösaren initierar ett flöde när en person prenumererar.

The **Klicka på Länk i SMS-meddelande** utlösaren initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

## SMS-filter {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

Du kan också använda Vibes-filter i Smarta listor. The **Prenumererar på Vibes List** filter hittar alla som *någonsin* prenumererar på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

I motsats till **Medlem i Vibes List** filtersökningar _alla_ prenumererar för närvarande på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

>[!NOTE]
>
>Alla SMS-filter innehåller **Aktivitetsdatum** -begränsning som standard.

När du har ställt in vibes-utlösare och -filter i din smarta lista kan du [definiera flödet](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Skicka ett SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Söka efter och lägga till filter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
