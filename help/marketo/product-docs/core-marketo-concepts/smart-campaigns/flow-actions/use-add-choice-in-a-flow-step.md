---
unique-page-id: 1146980
description: Använd Lägg till val i ett flödessteg - Marketo Docs - produktdokumentation
title: Använd Lägg till alternativ i ett flödessteg
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Använd Lägg till alternativ i ett flödessteg {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Med Lägg till alternativ kan du använda ett flödessteg och säga att det är beroende när du väljer detaljerna.

1. Lägg till ett flödessteg på fliken **[!UICONTROL Flow]** i den smarta kampanjen och klicka sedan på **[!UICONTROL Add Choice]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Välj önskat villkor.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Välj önskad operator och ange ett valvärde. Detta ställer in kriterier eller val.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Ange ett flödesstegvärde för valet.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Token _fungerar inte_ i villkorsdelen av ett urvalsflödessteg.

1. Upprepa stegen ovan för att lägga till flera alternativ och lägg sedan till/justera standardvärdet.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Du kan ange att något av dina flödessteg ska vara —Do None—. I så fall kommer ingen åtgärd att utföras.

   >[!CAUTION]
   >
   >Endast det första matchande alternativet används för flödessteget. Lär dig hur du [ändrar ordning på&quot;Lägg till val&quot; i en flödesåtgärd](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Bra! Nu kan ni skapa en enda smart kampanj med flödesstegalternativ i stället för att skapa flera smarta kampanjer för varje val.

   >[!MORELIKETHIS]
   >
   >[Ändra ordning på Lägg till alternativ i ett flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
