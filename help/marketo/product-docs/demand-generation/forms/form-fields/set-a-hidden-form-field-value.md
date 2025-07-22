---
unique-page-id: 2359663
description: Ange ett dolt formulärfältsvärde - Marketo Docs - produktdokumentation
title: Ange ett dolt formulärfältsvärde
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Ange ett dolt formulärfältsvärde {#set-a-hidden-form-field-value}

Dolda fält fylls vanligtvis i dynamiskt. De visas inte för den som fyller i formuläret. Så här anger du värdet.

>[!PREREQUISITES]
>
>[Ange ett formulärfält som dolt](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Markera fältet {#select-the-field}

1. Markera det dolda fältet i formuläret och klicka på **[!UICONTROL Edit]** för **[!UICONTROL Autofill]**.

   ![](assets/autofill.png)

## Använd standardvärde {#use-default-value}

Genom att välja Använd **[!UICONTROL Default Value]** kan du hårdkoda ett specifikt värde som alltid ska användas när formuläret skickas. Ange **[!UICONTROL Default Value]** och klicka på **[!UICONTROL Save]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL-parameter {#url-parameter}

Om du vill hämta URL-parametrar (frågesträngar) från sidan som personen är på när du fyller i formuläret kan du använda **[!UICONTROL URL Parameters]** för att fylla i det dolda fältet.

>[!NOTE]
>
>Parametrar är ganska tekniska, eller hur? När man väl fått dem, är de kraftfulla. Den här [Wikipedia-sidan om frågesträngar](https://en.wikipedia.org/wiki/Query_string) är något användbar.

1. Välj **[!UICONTROL URL Parameter]** för **[!UICONTROL Get Value Type]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Ange **[!UICONTROL Parameter Name]** och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Du kan ange en **[!UICONTROL Default Value]** om URL-parametern inte hittas.

## Cookie-värde {#cookie-value}

Om du lagrar data i cookies kan du använda **[!UICONTROL Cookie Value]** för att hämta data när formuläret skickas.

1. Välj **[!UICONTROL Cookie Value]** för **[!UICONTROL Get Value From]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Ange den cookie **[!UICONTROL Parameter Name]** som du vill använda och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Du kan ange en **[!UICONTROL Default Value]** om parametern/cookien inte hittas.

## Referensparameter {#referrer-parameter}

Om du vill hämta data från sidan som besökaren kom från innan du fyllde i formuläret kan du använda **[!UICONTROL Referrer Parameter]**.

1. Ange **[!UICONTROL Get Value From]** till **[!UICONTROL Referrer Parameter]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Ange **[!UICONTROL Parameter Name]** som du vill fästa från hänvisarens URL och klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Du kan ange **[!UICONTROL Default Value]** om refererarparametern inte hittas.

1. Klicka på **[!UICONTROL Finish]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Klicka på **[!UICONTROL Approve and Close]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
