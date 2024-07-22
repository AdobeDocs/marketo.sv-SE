---
unique-page-id: 2953373
description: Konfigurera sidfot för avanmälan i Marketo Sales Insight - Marketo Docs - produktdokumentation
title: Konfigurera sidfot för avanmälan i Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
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
>**Försäljningsmeddelanden** är de som skickas från Sales Insight (de som inte skickas från Marketo Outlook-plugin).

1. Gå till området **Admin**.

   ![](assets/one-1.png)

1. Klicka på **Försäljningsinsikter** och sedan på **Redigera inställningar**.

   ![](assets/two-1.png)

   Det finns flera alternativ. Först tittar vi på de typer av e-post som du kan ändra inställningarna för.

   ![](assets/three-1.png)

   * **Ingen mall** - Manuellt sammansatt av säljanvändare.
   * **Standard-e-post** - E-postmeddelanden baserade på en mall.
   * **Driftlig e-post** - E-postmeddelanden som ignorerar Avsluta prenumeration, Markering pausad och Kommunikationsbegränsningar (de skickar oavsett vad).

   Du kan ange olika beteenden för varje typ.

   >[!CAUTION]
   >
   >**Respektera inställningarna för att avbryta prenumerationen**: leads som inte längre prenumererar får INTE e-postmeddelandet även om det publicerade e-postmeddelandet fungerar
   >
   >**Ignorera inställningar för att avbryta prenumerationen**: leads kommer att få e-postmeddelandet

1. Gör önskade ändringar och klicka sedan på **Spara**.

   >[!TIP]
   >
   >De två sista alternativen gör att du dynamiskt kan inkludera/exkludera sidfoten för avanmälan beroende på antalet mottagare (större än 1 eller större än 5).

   ![](assets/four-1.png)

Vis! Lite komplicerat, men ganska flexibelt, eller hur?
