---
unique-page-id: 1146942
description: Definiera smart lista för smart kampanj | Utlösare - Marketo Docs - produktdokumentation
title: Definiera smart lista för smart kampanj | Utlösare
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: a9d902bf40e6193838a931ecb96a080bae098d68
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Definiera smart lista för smart kampanj | Utlösare {#define-smart-list-for-smart-campaign-trigger}

Låt en Smart Campaign köras på en person i taget baserat på live-händelser genom att lägga till utlösare.

>[!CAUTION]
>
>Om du redigerar Smart List eller Flow Step i en aktiv kampanj kan det eventuellt bryta dess funktion. Om du väljer att göra det ska du vara försiktig.

1. I din smarta kampanj klickar du på **[!UICONTROL Smart List]** -fliken.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Sök efter önskad utlösare och dra och släpp den på arbetsytan.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >En smart kampanj med utlösare körs i _Utlösare_ läge. Den körs på en person i taget baserat på händelser som utlösts och eventuella ytterligare filter.

   >[!IMPORTANT]
   >
   >När du använder ett booleskt fält i en utlösarkampanj med Smart List måste du explicit ange det till &quot;false&quot; för att fältet ska kunna utvärderas korrekt under kampanjens körning.

1. Klicka på listrutan och välj en operator.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Rödaktiga linjer indikerar fel eller att information saknas. Om den inte korrigeras blir kampanjen ogiltig och körs inte.

   >[!TIP]
   >
   >I en Smart Campaign med både utlösare och filter ligger utlösarna överst och när de aktiveras går bara personer som uppfyller filtervillkoren igenom flödet.

1. Definiera utlösaren.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Med flera utlösare går en person igenom flödet om _VALFRITT_ en av utlösarna aktiveras.

Lär dig hur man kör kampanjen på en uppsättning personer samtidigt [Definiera smart lista för smart kampanj | Grupp](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
