---
unique-page-id: 12982909
description: Schemalägg engagemangsprogram med mottagartidszon - Marketo Docs - produktdokumentation
title: Schemalägg engagemangsprogram med mottagartidszon
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Schemalägg engagemangsprogram med mottagartidszon {#schedule-engagement-programs-with-recipient-time-zone}

När du schemalägger en interaktionsprogramström och mottagarens tidszon är aktiva, kommer programsändningen att börja köras vid midnatt i den första tidszonen (UTC +14:00). Vi kräver att du schemalägger den första sändningen **minst 25 timmar** i framtiden, eftersom det kan finnas personer som är kvalificerade för sändningen i varje tidszon över hela världen. Om vi påbörjar bearbetningen vid den här tidpunkten i den första tidszonen garanterar vi att vi kommer att leverera e-postmeddelandet vid det schemalagda datumet och den schemalagda tidpunkten för varje mottagare.

1. Gå till fliken **[!UICONTROL Streams]** i ditt engagemangsprogram och klicka på ett strömmens cadence-schema för att redigera det.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Ange dina cadence-inställningar](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) som vanligt, och markera sedan kryssrutan **[!UICONTROL Recipient Time Zone]**. Kom ihåg att din första sändning måste vara minst 25 timmar i framtiden. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Observera att när mottagartidszon är aktiv visas ingen specifik tidszon i schemat för stängning, eftersom det kan finnas flera. Den visar bara timmen.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Förstå mottagarens tidszon](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Ange strömavslut](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
