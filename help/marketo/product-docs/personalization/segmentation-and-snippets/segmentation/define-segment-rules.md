---
unique-page-id: 2359449
description: Definiera segmentregler - Marketo Docs - Produktdokumentation
title: Definiera segmentregler
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---


# Definiera segmentregler {#define-segment-rules}

Genom att definiera segmentregler kan du kategorisera dina personer i olika grupper som inte kan kombineras.

>[!PREREQUISITES]
>
>[Skapa en segmentering](create-a-segmentation.md)

1. Gå till **databasen.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Klicka på **Segmentering **i trädet och klicka sedan på ett visst **segment**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Klicka på **Smart List** och lägg till filter.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Segment har för närvarande inte stöd för operatorerna *In Past* och *In Timeframe *för filter. Det beror på att segmenteringar bara söker efter uppdateringar när ett ändringsdatavärde loggas. Dessa värden loggas *inte* för saker som ändras automatiskt, till exempel formelfält och datum. Dessutom stöds inte datumoperatorer med relativa datumintervall eftersom de beräknas vid tidpunkten för segmenteringsgodkännande, inte vid tidpunkten för en Ändra datavärdesaktivitet.

   >[!NOTE]
   >
   >Filtren &quot;SFDC-typ&quot; och &quot;Microsoft-typ&quot; stöds för närvarande inte i smarta segmenteringslistor.

1. Fyll i lämpliga värden för filtren.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**Djupdykning**
   >
   >
   >Smarta listor är fantastiska. Lär dig allt du kan göra med [smarta listor och statiska listor](http://docs.marketo.com/display/docs/smart+lists+and+static+lists).

1. Klicka på fliken **Personer (utkast)** för att visa vilka personer som kan kvalificera sig som medlemmar i det här segmentet.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Gå till **Segmenteringsåtgärder**. Klicka på **Godkänn**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Det totala antalet segment som du kan skapa i en segmentering beror på antalet och typen av filter som används och även på hur komplex logiken i segmenten är. Du kan skapa upp till 100 segment med hjälp av standardfält, men med andra typer av filter kan det bli mer komplicerat och segmenteringen kanske inte kan godkännas. Några exempel är: anpassade fält, listmedlem, fält för huvudägare och intäktsfaser.
   >
   >
   >Om du får ett felmeddelande under godkännandet och behöver hjälp med att minska komplexiteten i din segmentering kontaktar du [Marketo Support](http://nation.marketo.com/t5/Support/ct-p/Support).

1. På kontrollpanelen hittar du en snabb översikt över segmenten i ett cirkeldiagram samt vilka regler som används.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Bra jobbat! Dessa segment kommer att bli bra på många ställen i Marketo.

>[!NOTE]
>
>En person kan kvalificera sig för olika segment, men tillhör så småningom bara ett segment som är beroende av segmentens [prioritetsordning](segmentation-order-priority.md).

>[!NOTE]
>
>**Påminnelse**
>
>På skärmen Personer (utkast) visas alla personer som är berättigade att vara medlem och inte alltid är den slutliga listan över personer. Godkänn segmentet för att se den slutliga listan.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Godkänn en segmentering](approve-a-segmentation.md)

>



