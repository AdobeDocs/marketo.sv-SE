---
unique-page-id: 2953373
description: Konfigurera sidfot för avanmälan i Marketo Sales Insight - Marketo Docs - Produktdokumentation
title: Konfigurera Unsubscribe Footers in Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Konfigurera sidfot för avanmälan i Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Säljmejl placerar automatiskt sidfoten längst ned. Du kan dock justera inställningarna efter dina behov.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Definition**
>
>**E-** postmeddelanden skickas från Sales Insight. (Detta inkluderar inte de som skickas från Marketo Outlook-plugin.)

1. Gå till området **Admin**.

   ![](assets/one-1.png)

1. Klicka på **Sales Insight, **och sedan **Redigera inställningar**.

   ![](assets/two-1.png)

   Det finns flera alternativ. Först tittar vi på de typer av e-post som du kan ändra inställningarna för.

   ![](assets/three-1.png)

   * **Ingen mall **- Skapas manuellt av säljare.
   * **Standardbaserad e-post**  - E-post baserad på en mall.
   * **E-post**  - E-postmeddelanden som ignorerar Avbeställning, Marknadsföring avbruten och Kommunikationsbegränsningar (de skickas oavsett vad).

   Du kan ange olika beteenden för varje typ.

   >[!CAUTION]
   >
   >**Inställningar för att avbryta prenumerationen: **leads för avbeställning får INTE e-postmeddelandet även om det publicerade e-postmeddelandet är i drift
   >
   >
   >**Ignorera inställningar för att avbryta prenumerationen:** leads för att avbryta prenumerationen får e-postmeddelandet

   Gör önskade ändringar och klicka sedan på Spara.

   >[!TIP]
   >
   >De två sista alternativen gör att du dynamiskt kan inkludera/exkludera sidfoten för att avbryta prenumerationen beroende på antalet mottagare (större än 1 eller större än 5).

   ![](assets/four-1.png)

Vis! Lite komplicerat, men ganska flexibelt, eller hur?

>[!NOTE]
>
>**Djupdykning**
>
>Läs mer om [Marketo Sales Insight](http://docs.marketo.com/display/docs/marketo+sales+insight).

