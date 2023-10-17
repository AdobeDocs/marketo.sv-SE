---
unique-page-id: 1146980
description: Använd Lägg till val i ett flödessteg - Marketo Docs - produktdokumentation
title: Använd Lägg till alternativ i ett flödessteg
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Använd Lägg till alternativ i ett flödessteg {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Med Lägg till alternativ kan du använda ett flödessteg och säga att det är beroende när du väljer detaljerna.

1. Under **[!UICONTROL Flow]** Lägg till ett flödessteg och klicka sedan på **[!UICONTROL Add Choice]**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Välj önskat villkor.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Välj önskad operator och ange ett valvärde. Detta ställer in kriterier eller val.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Ange ett flödesstegvärde för valet.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >Tokens kommer att _not_ arbeta i villkorsdelen av ett urvalsflödessteg.

1. Upprepa stegen ovan för att lägga till flera alternativ och lägg sedan till/justera standardvärdet.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Du kan ange att något av dina flödessteg ska vara —Do None—. I så fall kommer ingen åtgärd att utföras.

   >[!CAUTION]
   >
   >Endast det första matchande alternativet används för flödessteget. Lär dig hur [ändra ordning på&quot;Lägg till val&quot; i en flödesåtgärd](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Bra! Nu kan ni skapa en enda smart kampanj med flödesstegalternativ i stället för att skapa flera smarta kampanjer för varje val.

   >[!MORELIKETHIS]
   >
   >[Ändra ordning på Lägg till alternativ i ett flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
