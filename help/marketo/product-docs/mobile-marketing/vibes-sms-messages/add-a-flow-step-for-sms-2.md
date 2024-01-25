---
description: Lägg till ett flödessteg för SMS - Marketo Docs - Produktdokumentation
title: Lägg till ett flödessteg för SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Lägg till ett flödessteg för SMS {#add-a-flow-step-for-sms}

Marketo Engage har tre flödessteg som du kan använda i SMS-smarta kampanjer:

<table>
<tbody>
  <tr>
    <td style="width:25%">Skicka SMS-meddelande</td>
    <td>Den här flödesåtgärden skickar meddelanden till personer från Marketo Smart List som prenumererar på en användare som har valt att prenumerera på Vibes. Det initierar inte prenumerationsprocessen. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">Läs mer</a>.</td>
  </tr>

<tr>
    <td style="width:25%">Prenumerera på Vibes List</td>
    <td>Den här flödesåtgärden initierar SMS-prenumerationsprocessen via en av användaren utvald Vibes-anskaffningskampanj. Vibes skickar sedan ett bekräftelsemeddelande och mottagaren måste svara med "Y" inom 24 timmar för att bekräfta anmälan. När användaren har valt att delta blir han/hon medlem i din tillhörande prenumerationslista för Vibes.</td>
  </tr>
  <tr>
    <td style="width:25%">Avbeställ utskick om Vibes List</td>
    <td>Den här flödesåtgärden avslutar prenumerationen för varje person i en lista över användare som har valt att prenumerera på Vibes. När en användare skriver"STOP" till din kod uppdateras sin personpost så att den återspeglar att han/hon inte längre är medlem i prenumerationslistan för Adobe.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>När SMS-meddelanden skickas:
>
>* Marketo dedupes per telefonnummer. Om flera personer har samma telefonnummer får bara en person meddelandet om de bara är medlemmar i en prenumerationslista för Adobe. Deduping görs på prenumerationslistenivån för Vibes, inte på programnivån för Marketo.
>* Marketo skickar inte till personer som är blocklist eller har avbrutit sin marknadsföring.

Allmän information om hur du ställer in flödessteg finns i [Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Här är grunderna för hur du använder SMS.

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Hitta och välj den smarta kampanj som du vill lägga till SMS-flödet i.

   SCREENSHOT

1. På fliken Smart lista väljer du önskad utlösare (t.ex. &quot;Fylld i formulär&quot;).

   SCREENSHOT

1. I **Flöde** dra över flödessteget (t.ex. **Skicka SMS-meddelande**). Välj SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Väljaren Vibes-lista fungerar som ett ytterligare filter för den målgrupp som redan identifierats i den smarta listan så att den endast riktar sig till de leads som tillhör den listan.
   >
   >The **Prenumerera på Vibes List** och **Avbeställ utskick om Vibes List** flöden har olika krav. För **Prenumerera** måste du välja listan Vibes och värvningskampanjen Vibes. För **Avbeställ**, är det bara listan Vibes som krävs.
