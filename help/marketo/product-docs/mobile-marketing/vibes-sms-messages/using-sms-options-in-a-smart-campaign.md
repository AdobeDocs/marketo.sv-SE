---
description: Använda SMS-alternativ i en smart kampanj - Marketo Docs - produktdokumentation
title: Använda SMS-alternativ i en smart kampanj
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Använda SMS-alternativ i en smart kampanj {#using-sms-options-in-a-smart-campaign}

När du har [skapat ett SMS-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"} vill du använda utlösare och filter för smarta listor i en smart kampanj för att få fördelarna.

>[!NOTE]
>
>Om du vill skicka ett SMS-meddelande har vi en [specifik artikel](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} för det.

>[!PREREQUISITES]
>
>SMS-utlösare/filter visas bara om tjänsten [Vibes har aktiverats](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## SMS-utlösare {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Här är några exempel:

Utlösaren **SMS Message Bounces** initierar ett flöde, som att skicka ett e-postmeddelande, när ett SMS-meddelande studsar.

Utlösaren **Prenumererar på Vibes List** initierar ett flöde när en person prenumererar.

Utlösaren **Click Link in SMS Message** initierar ett flöde när en person klickar på en länk i SMS-meddelandet.

## SMS-filter {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Filtret **Prenumererar på Vibes-listan** hittar alla som har *någonsin* prenumererat på Vibes. Detta inkluderar både personer som inte längre är prenumererade och borttagna, även om borttagna personer utelämnas från flödet. Det här filtret passar bäst för rapportering.

Filtret **Medlem i listan** hittar däremot *alla* som prenumererar på Vibes och är lämpligast att använda i smarta kampanjer eller listor.

>[!NOTE]
>
>Alla SMS-filter innehåller begränsningen **Aktivitetsdatum** som standard.

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
>Flödena **Prenumerera på Vibes List** och **Avsluta prenumerationen på Vibes List** har olika krav. För **prenumerationen** måste du välja listan Vibes och värvningskampanjen Vibes. För **Unsubscribe** krävs bara listan Vibes.

>[!MORELIKETHIS]
>
>* [Skicka ett SMS-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definiera smart lista för smart kampanj | Utlösare &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definiera smart lista för smart kampanj | Grupp &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
