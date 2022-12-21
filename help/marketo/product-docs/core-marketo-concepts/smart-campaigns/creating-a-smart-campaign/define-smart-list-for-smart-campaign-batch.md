---
unique-page-id: 1146940
description: Definiera smart lista för smart kampanj | Batch - Marketo Docs - produktdokumentation
title: Definiera smart lista för smart kampanj | Grupp
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Definiera smart lista för smart kampanj | Grupp {#define-smart-list-for-smart-campaign-batch}

Smarta listor är en mekanism i hela Marketo som definierar vem (vilka personer) som ska inkluderas, oavsett om det är en rapport, en lista eller en smart kampanj. Så här definierar du en smart lista för en batchkampanj.

1. Välj en smart kampanj och klicka sedan på **Smart List**.

   ![](assets/campaignchoose-hand.png)

1. Skriv om du vill söka efter ett filter och sedan dra och släppa det på arbetsytan. Upprepa för flera filter.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >En smart kampanj med bara filter körs i **Grupp** läge. Den hittar personer i databasen som är kvalificerade baserat på filtren och kör alla via flödet samtidigt.

   >[!NOTE]
   >
   >Du kan få en smart kampanj att köras på en person i taget baserat på live-händelser genom att lägga till utlösare, vilket placerar den smarta kampanjen i **Utlösare** läge.

1. Klicka på listrutan och välj en filteroperator för det filter du valt.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Rödaktiga linjer indikerar fel eller att information saknas. Om den inte korrigeras blir kampanjen ogiltig och körs inte.

1. Ange filtervärdet.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >Som standard är personer som uppfyller ALLA regler för smarta listor kvalificerade. Detta kan ändras för att passa era kampanjbehov. Checka ut  [Smart List-regler för komplex logik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) om du vill veta mer.

   Lär dig hur du aktiverar live-händelser för en person i taget [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definiera smart lista för smart kampanj | Utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

