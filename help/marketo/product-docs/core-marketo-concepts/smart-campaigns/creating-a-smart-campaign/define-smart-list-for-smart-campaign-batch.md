---
unique-page-id: 1146940
description: Definiera smart lista för smart kampanj | Batch - Marketo Docs - produktdokumentation
title: Definiera smart lista för smart kampanj | Grupp
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: a9d902bf40e6193838a931ecb96a080bae098d68
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Definiera smart lista för smart kampanj | Grupp {#define-smart-list-for-smart-campaign-batch}

Smarta listor är en mekanism i hela Marketo Engage som definierar vem (vilka personer) som ska inkluderas, oavsett om det är en rapport, en lista eller en Smart Campaign. Så här definierar du en smart lista för en batchkampanj.

>[!CAUTION]
>
>Om du redigerar Smart List eller Flow Step i en aktiv kampanj kan det eventuellt bryta dess funktion. Om du väljer att göra det ska du vara försiktig.

1. Välj en smart kampanj och klicka sedan på **[!UICONTROL Smart List]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Skriv om du vill söka efter ett filter och dra det till arbetsytan. Upprepa för flera filter.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >En smart kampanj med bara filter körs i _Grupp_ läge. Den hittar personer i databasen som är kvalificerade baserat på filtren och kör alla via flödet samtidigt.

   >[!NOTE]
   >
   >Du kan få en smart kampanj att köras på en person i taget baserat på live-händelser genom att lägga till utlösare, vilket gör att den smarta kampanjen _Utlösare_ läge.

1. Klicka på listrutan och välj en filteroperator för det filter du valt.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Rödaktiga linjer indikerar fel eller att information saknas. Om den inte korrigeras blir kampanjen ogiltig och körs inte.

1. Ange filtervärdet.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Som standard är personer som uppfyller alla smarta listregler kvalificerade. Detta kan ändras för att passa era kampanjbehov. Checka ut  [Smart List-regler för komplex logik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} om du vill veta mer.

   Lär dig hur du aktiverar live-händelser för en person i taget [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
