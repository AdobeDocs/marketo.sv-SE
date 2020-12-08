---
unique-page-id: 12982909
description: Schemalägg engagemangsprogram med mottagartidszon - Marketo Docs - Produktdokumentation
title: Schemalägg engagemangsprogram med mottagartidszon
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Schemalägg engagemangsprogram med mottagartidszon {#schedule-engagement-programs-with-recipient-time-zone}

När du [schemalägger en interaktionsprogramström](https://docs.marketo.com/display/DOCS/Schedule+Engagement+Programs+for+Recipient+Time+Zones) och mottagarens tidszon är aktiva, kommer programsändningen att börja köras vid midnatt i den första tidszonen (UTC +14:00). Vi kräver att du schemalägger den första sändningen **minst 25 timmar** i framtiden eftersom det kan finnas personer som kvalificerar sig för sändningen i varje tidszon över hela världen. Om vi påbörjar bearbetningen vid den här tidpunkten i den första tidszonen garanterar vi att vi kommer att leverera e-postmeddelandet vid det schemalagda datumet och den schemalagda tidpunkten för varje mottagare.

1. Gå till fliken **Streams** i ditt engagemangsprogram och klicka på ett strömmens cadence-schema för att redigera det.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Ange dina inställningar](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) för cadence som vanligt och markera sedan kryssrutan **Mottagarens tidszon **. Kom ihåg att din första sändning måste vara minst 25 timmar i framtiden. Klicka på **Spara**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Observera att när mottagartidszon är aktiv visas ingen specifik tidszon i schemat för stängning, eftersom det kan finnas flera. Den visar bara timmen.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Förstå mottagartidszon](../../../../../product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Ange strömavslut](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)

>



