---
unique-page-id: 11379045
description: Lägg till ett flödessteg för SMS - Marketo Docs - Produktdokumentation
title: Lägg till ett flödessteg för SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Lägg till ett flödessteg för SMS {#add-a-flow-step-for-sms}

Marketo har tre flödessteg som du kan använda i SMS-smarta kampanjer:

* **Skicka SMS-meddelande** - Den här flödesåtgärden skickar meddelanden till personer från Marketo smartlist som prenumererar på en användarvald Vibes-prenumerationslista. Det initierar inte prenumerationsprocessen.
* **Prenumerera på Vibes List** - Den här flödesåtgärden initierar SMS-prenumerationsprocessen via en Vibes Acquisition Campaign som valts av användaren. Vibes skickar sedan ett bekräftelsemeddelande; mottagaren måste svara för att slutföra prenumerationsprocessen.
* **Avbeställ utskick om Vibes List** - Den här flödesåtgärden avslutar prenumerationen för varje person från en användarvald Vibes-prenumerationslista.

>[!NOTE]
>
>När SMS-meddelanden skickas:
>
>* Marketo dedupes per telefonnummer. Om flera personer har samma telefonnummer får bara en person meddelandet.
>* Marketo skickar inte till personer som är blocklist eller har avbrutit sin marknadsföring.


Allmän information om hur du ställer in flödessteg finns i [Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Här är grunderna för hur du använder SMS.

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Hitta den smarta kampanj som du vill lägga till SMS-flödet i. Klicka på **Flöde** -fliken.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Dra över flödet, till exempel **Skicka SMS-meddelande**. Välj SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Väljaren Vibes-lista fungerar som ett ytterligare filter för den målgrupp som redan identifierats i den smarta listan så att den endast riktar sig till de leads som tillhör den listan.
   >
   >The **Prenumerera på Vibes List** och **Avbeställ utskick om Vibes List** flöden har olika krav. För **Prenumerera** måste du välja listan Vibes och värvningskampanjen Vibes. För **Avbeställ**, är det bara listan Vibes som krävs.
