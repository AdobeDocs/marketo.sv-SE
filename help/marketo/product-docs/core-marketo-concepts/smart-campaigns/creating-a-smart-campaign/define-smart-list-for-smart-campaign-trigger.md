---
unique-page-id: 1146942
description: Definiera smart lista för smart kampanj | Utlösare - Marketo Docs - produktdokumentation
title: Definiera smart lista för smart kampanj | Utlösare
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Definiera smart lista för smart kampanj | Utlösare {#define-smart-list-for-smart-campaign-trigger}

Få en smart kampanj att köras på en person i taget baserat på live-händelser genom att lägga till utlösare.

1. Klicka på **Smart List** -fliken.

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. Sök efter utlösaren och dra och släpp sedan utlösaren på arbetsytan.

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >En smart kampanj med utlösare körs i **Utlösare** läge. Den körs på en person i taget baserat på händelser som utlösts och eventuella ytterligare filter.

   >[!IMPORTANT]
   >
   >När du använder ett booleskt fält i en smart lista med utlösande kampanjer måste du explicit ställa in det på false för att fältet ska kunna utvärderas korrekt under kampanjens körning.

1. Klicka på listrutan och välj en operator.

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >Rödaktiga linjer indikerar fel eller att information saknas. Om den inte korrigeras blir kampanjen ogiltig och körs inte.

   >[!TIP]
   >
   >I en smart kampanj med både utlösare och filter ligger utlösarna överst och när de aktiveras går bara personer som uppfyller filtervillkoren igenom flödet.

1. Definiera utlösaren.

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >Med flera utlösare går en person igenom flödet om **VALFRITT** en av utlösarna aktiveras.

Lär dig hur man kör kampanjen på en uppsättning personer samtidigt [Definiera smart lista för smart kampanj | Grupp](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
