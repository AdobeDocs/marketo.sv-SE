---
unique-page-id: 11379045
description: Lägg till ett flödessteg för SMS - Marketo Docs - Produktdokumentation
title: Lägg till ett flödessteg för SMS
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Lägg till ett flödessteg för SMS {#add-a-flow-step-for-sms}

Marketo har tre flödessteg som du kan använda i SMS-smarta kampanjer:

* **Skicka SMS-meddelande**  - Den här flödesåtgärden skickar meddelanden till personer från Marketo-smartlistan som prenumererar på en användarvald Vibes-prenumerationslista. Det initierar inte prenumerationsprocessen.
* **Prenumerera på Vibes List**  - Den här flödesåtgärden initierar SMS-prenumerationsprocessen via en av användaren vald Vibes Acquisition Campaign. Vibes skickar sedan ett bekräftelsemeddelande; mottagaren måste svara för att slutföra prenumerationsprocessen.
* **Avbeställ Vibes List** - Denna flödesåtgärd avslutar prenumerationen för varje person i en användarvald Vibes-prenumerationslista.

>[!NOTE]
>
>När SMS-meddelanden skickas:
>
>* Marketo avdupes per telefonnummer. Om flera personer har samma telefonnummer får bara en person meddelandet.
>* Marketo skickar inte till personer som är blocklist eller marknadsföringspausade.

>



Allmän information om hur du ställer in flödessteg finns i [Lägga till ett flödessteg i en smart kampanj](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Här är grunderna för hur du använder SMS.

1. Klicka på **Marknadsföringsaktiviteter** på My Marketo.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Hitta den smarta kampanj som du vill lägga till SMS-flödet i. Klicka på fliken **Flöde**.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Dra över flödet, till exempel **Skicka SMS-meddelande**. Välj SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Väljaren Vibes-lista fungerar som ett ytterligare filter för den målgrupp som redan identifierats i den smarta listan så att den endast riktar sig till de leads som tillhör den listan.
   >
   >
   >**Prenumerera på Vibes List** och **Avbeställ Vibes List** har olika krav. För **prenumerera** måste du välja listan Vibes och kampanjen för förvärv av Vibes. För **Unsubscribe** krävs bara listan Vibes.

