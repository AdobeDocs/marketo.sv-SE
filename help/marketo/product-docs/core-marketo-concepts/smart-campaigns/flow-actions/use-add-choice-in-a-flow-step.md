---
unique-page-id: 1146980
description: Använd Lägg till val i ett flödessteg - Marketo Docs - Produktdokumentation
title: Använd Lägg till alternativ i ett flödessteg
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Använd Lägg till alternativ i ett flödessteg {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>* [Lägg till ett flödessteg i en smart kampanj](add-a-flow-step-to-a-smart-campaign.md)

>



**Med Lägg till alternativ** kan du använda ett flödessteg och säga&quot;Det beror&quot; när du väljer detaljer.

1. Lägg till ett flödessteg på fliken **Flöde** i den smarta kampanjen och klicka sedan på **Lägg till val**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Välj önskat villkor.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Välj önskad operator och ange ett valvärde. Detta ställer in kriterier eller val.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Ange ett flödesstegvärde för valet.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >Token fungerar **inte** i villkorsdelen av ett urvalsflödessteg.

1. Upprepa stegen ovan för att lägga till flera alternativ och lägg sedan till/justera standardvärdet.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Du kan ange att något av dina flödessteg ska vara —Do None—. I så fall kommer ingen åtgärd att utföras.

   >[!CAUTION]
   >
   >Endast det första matchande alternativet används för flödessteget. Lär dig hur du [ändrar ordning på&quot;Lägg till val&quot; i en flödesåtgärd](reorder-add-choice-in-a-flow-step.md).

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >    
   >    
   >    * [Ändra ordning på&quot;Lägg till val&quot; i ett flödessteg](reorder-add-choice-in-a-flow-step.md)


Bra! Nu kan ni skapa en enda smart kampanj med alternativ för flödessteg i stället för att skapa flera smarta kampanjer för varje val.