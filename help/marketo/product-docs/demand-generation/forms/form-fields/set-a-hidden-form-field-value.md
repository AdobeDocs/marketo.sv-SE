---
unique-page-id: 2359663
description: Ange ett dolt formulärfältsvärde - Marketo Docs - produktdokumentation
title: Ange ett dolt formulärfältsvärde
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Ange ett dolt formulärfältsvärde {#set-a-hidden-form-field-value}

Dolda fält fylls vanligtvis i dynamiskt. De visas inte för den som fyller i formuläret. Så här anger du värdet.

>[!PREREQUISITES]
>
>[Ange ett formulärfält som dolt](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Markera fältet {#select-the-field}

1. Markera det dolda fältet i formuläret och klicka på **Redigera** for **Autofyll**.

   ![](assets/autofill.png)

## Använd standardvärde {#use-default-value}

Genom att välja Använd standardvärde kan du hårdkoda ett specifikt värde som alltid ska användas när formuläret skickas. Ange standardvärdet och klicka på Spara.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL-parameter {#url-parameter}

Om du vill hämta URL-parametrar (frågesträngar) från sidan som personen är på när formuläret fylls i kan du använda **URL-parametrar** för att fylla i det dolda fältet.

>[!NOTE]
>
>Parametrar är ganska tekniska, eller hur? När man väl fått dem, är de kraftfulla. Detta [Wikipedia-sida om frågesträngar](https://en.wikipedia.org/wiki/Query_string) är till viss hjälp.

1. Välj **URL-parameter** for **Hämta värdetyp**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Ange **Parameternamn** och klicka **Spara**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Du kan ange ett standardvärde om URL-parametern inte hittas.

## Cookie-värde {#cookie-value}

Om du lagrar data i cookies kan du använda **Cookie-värde** för att hämta in data när formuläret skickas.

1. Välj **Cookie-värde** for **Hämta värde från**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Ange det cookie-parameternamn du vill använda och klicka på **Spara**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Du kan ange ett standardvärde om parametern/cookien inte hittas.

## Referensparameter {#referrer-parameter}

Om du vill hämta in data från sidan som besökaren kom från innan du fyllde i formuläret kan du använda **Referensparameter**.

1. Ange **Hämta värde från** till **Referensparameter**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Ange **Parameternamn** som du vill fästa från hänvisarens URL och klicka på **Spara**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Du kan ange en **Standardvärde** om refererarparametern inte hittas.

1. Klicka **Slutför**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Klicka **Godkänn och stäng**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
