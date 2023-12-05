---
description: Lägg till ett flödessteg för SMS - Marketo Docs - Produktdokumentation
title: Lägg till ett flödessteg för SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Lägg till ett flödessteg för SMS {#add-a-flow-step-for-sms}

Marketo Engage har tre flödessteg som du kan använda i SMS Smart Campaigns:

* **Skicka SMS-meddelande** - Den här flödesåtgärden skickar meddelanden till personer från Marketo Smart List som prenumererar på en användare som har valt att prenumerera på Vibes. Det initierar inte prenumerationsprocessen.
* **Prenumerera på Vibes List** - Den här flödesåtgärden initierar SMS-prenumerationsprocessen via en Vibes Acquisition Campaign som valts av användaren. Vibes skickar sedan ett bekräftelsemeddelande. Mottagaren måste svara&quot;Y&quot; för att bekräfta anmälan inom 24 timmar. När användaren har valt att delta blir han/hon medlem i din tillhörande prenumerationslista för Vibes.
* **Avbeställ utskick om Vibes List** - Den här flödesåtgärden avslutar prenumerationen för varje person i en lista över användare som har valt att prenumerera på Vibes. När en användare skriver&quot;stopp&quot; i koden uppdateras sin personpost så att den avspeglar att han/hon inte längre är medlem i prenumerationslistan.

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
