---
unique-page-id: 2953373
description: Konfigurera sidfot för avanmälan i Marketo Sales Insight - Marketo Docs - produktdokumentation
title: Konfigurera sidfot för avanmälan i Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Konfigurera sidfot för att avbryta prenumerationen i [!DNL Marketo Sales Insight] {#configure-unsubscribe-footers-in-marketo-sales-insight}

Säljmejl placerar automatiskt sidfoten längst ned. Du kan dock justera inställningarna efter dina behov.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

>[!NOTE]
>
>**Definition**
>
>**Försäljningsmeddelanden** är de som skickas från [!DNL Sales Insight] (de som inte skickas från Marketo Outlook-plugin-programmet).

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Klicka på **[!UICONTROL Sales Insight]** och sedan på **[!UICONTROL Edit Settings]**.

   ![](assets/two-1.png)

   Det finns flera alternativ. Först tittar vi på de typer av e-post som du kan ändra inställningarna för.

   ![](assets/three-1.png)

   * **[!UICONTROL No Template]** - Manuellt sammansatt av säljanvändare.
   * **[!UICONTROL Standard Email]** - E-postmeddelanden baserade på en mall.
   * **[!UICONTROL Operational Email]** - E-postmeddelanden som ignorerar Avsluta prenumeration, Markering pausad och Kommunikationsbegränsningar (de skickas oavsett vad).

   Du kan ange olika beteenden för varje typ.

   >[!CAUTION]
   >
   >**[!UICONTROL Respect Unsubscribe Settings]**: leads för avbeställning får INTE e-postmeddelandet även om det publicerade e-postmeddelandet fungerar
   >
   >**[!UICONTROL Ignore Unsubscribe Settings]**: leads för avanmälan får e-postmeddelandet

1. Gör önskade ändringar och klicka sedan på **[!UICONTROL Save]**.

   >[!TIP]
   >
   >De två sista alternativen gör att du dynamiskt kan inkludera/exkludera sidfoten för avanmälan beroende på antalet mottagare (större än 1 eller större än 5).

   ![](assets/four-1.png)

Vis! Lite komplicerat, men ganska flexibelt, eller hur?
