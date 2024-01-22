---
description: Använda SMS-alternativ i en smart kampanj - Marketo Docs - produktdokumentation
title: Använda SMS-alternativ i en smart kampanj
feature: Mobile Marketing
source-git-commit: 5e2d1979abcafd8e4a37e55b843be932125c954e
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Använda SMS-alternativ i en smart kampanj {#using-sms-options-in-a-smart-campaign}

Efter dig [skapa ett SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}vill du använda utlösare och filter för smarta listor i en smart kampanj för att få fördelarna.

>[!NOTE]
>
>Om du vill skicka ett SMS har vi en [specifik artikel](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} för det.

>[!PREREQUISITES]
>
>SMS-utlösare/filter visas bara om [Vibes-tjänsten har aktiverats](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## SMS-utlösare {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Här är några exempel:

The **SMS-meddelandestudsar** utlösaren initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

The **Prenumererar på Vibes List** utlösaren initierar ett flöde när en person prenumererar.

The **Klicka på Länk i SMS-meddelande** utlösaren initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

## SMS-filter {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

The **Prenumererar på Vibes List** filter hittar alla som *någonsin* prenumererar på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

I motsats till **Medlem i Vibes List** filtersökningar _alla_ prenumererar för närvarande på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

>[!NOTE]
>
>Alla SMS-filter innehåller **Aktivitetsdatum** -begränsning som standard.

## SMS-flödessteg {#sms-flow-steps}

Det finns tre SMS-flödessteg att välja mellan.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Skicka SMS-meddelande</b></td>
    <td>Den här flödesåtgärden skickar meddelanden till personer från Marketo Smart List som prenumererar på en användare som har valt att prenumerera på Vibes. Det initierar inte prenumerationsprocessen. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">Läs mer</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>Prenumerera på Vibes List</b></td>
    <td>Den här flödesåtgärden initierar SMS-prenumerationsprocessen via en av användaren utvald Vibes-anskaffningskampanj. Vibes skickar sedan ett bekräftelsemeddelande och mottagaren måste svara med "Y" inom 24 timmar för att bekräfta anmälan. När användaren har valt att delta blir han/hon medlem i din tillhörande prenumerationslista för Vibes.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Avbeställ utskick om Vibes List</b></td>
    <td>Den här flödesåtgärden avslutar prenumerationen för varje person i en lista över användare som har valt att prenumerera på Vibes. När en användare skriver"STOP" till din kod uppdateras sin personpost så att den återspeglar att han/hon inte längre är medlem i prenumerationslistan för Adobe.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>The **Prenumerera på Vibes List** och **Avbeställ utskick om Vibes List** flöden har olika krav. För **Prenumerera** måste du välja listan Vibes och värvningskampanjen Vibes. För **Avbeställ**, är det bara listan Vibes som krävs.

>[!MORELIKETHIS]
>
>* [Skicka ett SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definiera smart lista för smart kampanj | Grupp](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
