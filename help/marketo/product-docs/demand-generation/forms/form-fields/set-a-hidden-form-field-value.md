---
unique-page-id: 2359663
description: Ange ett dolt formulärfältsvärde - Marketo Docs - Produktdokumentation
title: Ange ett dolt formulärfältsvärde
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Ange ett dolt formulärfältsvärde {#set-a-hidden-form-field-value}

Dolda fält fylls vanligtvis i dynamiskt. De visas inte för den som fyller i formuläret. Så här anger du värdet.

>[!PREREQUISITES]
>
>[Ange ett formulärfält som dolt](set-a-form-field-as-hidden.md)

## Markera fältet {#select-the-field}

1. Markera det dolda fältet i formuläret och klicka på **Redigera** för **Fyll i automatiskt**.

   ![](assets/autofill.png)

## Använd standardvärde {#use-default-value}

Genom att välja Använd standardvärde kan du hårdkoda ett specifikt värde som alltid ska användas när formuläret skickas. Ange standardvärdet och klicka på Spara.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL-parameter {#url-parameter}

Om du vill hämta URL-parametrar (frågesträngar) från sidan som personen är på när du fyller i formuläret kan du använda **URL** **Parametrar** för att fylla i det dolda fältet.

>[!NOTE]
>
>Parametrar är ganska tekniska, eller hur? När man väl fått dem, är de kraftfulla. Den här [Wikipedia-sidan om frågesträngar](http://en.wikipedia.org/wiki/Query_string) är något användbar.

1. Välj **URL-parameter** för **Hämta värdetyp**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Ange **parameternamn** och klicka på **Spara**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Du kan ange ett standardvärde om URL-parametern inte hittas.

## Cookie-värde {#cookie-value}

Om du lagrar data i cookies kan du använda **cookie** **Value** för att hämta data när formuläret skickas.

1. Välj **Cookie** **Värde** för **Hämta** **Värde** **Från**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Ange det cookie-parameternamn du vill använda och klicka på **Spara**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Du kan ange ett standardvärde om parametern/cookien inte hittas.

## Referensparameter {#referrer-parameter}

Om du vill hämta data från den sida som besökaren kom från innan du fyller i formuläret kan du använda **Referent** **Parameter**.

1. Ange **Hämta** **Värde** **Från** till **Referent** **Parameter**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Ange **parameternamnet** som du vill fästa från hänvisarens URL och klicka på **Spara**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Du kan ange ett **Default** **värde** om referentparametern inte hittas.

1. Klicka på **Slutför**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Klicka på **Godkänn och stäng**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)

Söt! Du klarar dig ganska bra. Det finns mer att lära sig om [formulär](http://docs.marketo.com/display/docs/forms).
