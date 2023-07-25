---
unique-page-id: 10097873
description: Definiera en smart lista för aktiviteter med prediktivt innehåll - Marketo Docs - produktdokumentation
title: Definiera en smart lista för aktiviteter med prediktivt innehåll
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Definiera en smart lista för aktiviteter med prediktivt innehåll {#define-a-smart-list-for-predictive-content-activities}

Du kan använda prediktiva innehållsaktiviteter i utlösare och filter när du definierar en smart lista i en smart kampanj. Du kan aktivera en åtgärd för alla som klickar på prediktivt innehåll via [Multimediamall](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), [Innehållsrekommendationsfält](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)eller i en [e-post](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Navigera till **Smart List** -fliken.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Smarta listor kan göra fantastiska saker. Läs mer i [smart listdjup](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Sök efter utlösaren och dra och släpp den på arbetsytan.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >En smart kampanj med utlösare körs i utlösarläge. Den körs på en person i taget baserat på händelser som utlösts och filter som lagts till.

1. Klicka på **Namn** och välj en operator.

   ![](assets/smart-list-dropdown-hands.png)

1. Definiera utlösaren.

   ![](assets/smart-lislt-select-content-hands.png)

1. Lägg till **Typ** -begränsning.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Välj den källa du behöver för den smarta listan.

   ![](assets/pc-add-constraint.png)

1. Om du använder e-postkällan för ditt prediktiva innehåll lägger du till **Klicka på Länk i e-post** utlösare. Välj din e-postadress och lägg till **Är prediktiv** begränsning, definition som **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Lägg till eventuella andra filter efter behov.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >I en smart kampanj med både utlösare och filter ligger utlösarna överst. När det aktiveras går bara personer som uppfyller filtervillkoren igenom flödet.

   >[!NOTE]
   >
   >Med flera utlösare går en person igenom flödet om någon av utlösarna aktiveras.

   Lär dig hur man kör kampanjen på en uppsättning personer samtidigt [definiera en smart lista för en batchsmart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definiera smart lista för smart kampanj | Grupp](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Lägg till ett flödessteg i en smart kampanj](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definiera en smart lista för webbpersonaliseringsaktiviteter](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Aktivera prediktivt innehåll för multimedia för webben](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Aktivera innehållsrekommendationsfältet](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
