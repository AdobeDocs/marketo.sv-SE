---
unique-page-id: 2359447
description: Lär dig hur du skapar en segmentering för att gruppera människor för rapportering och dynamiskt innehåll. Lägg till segment i databasen, ange ordning och definiera segmentregler.
title: Skapa en segmentering
exl-id: a7907f1d-bc78-4b63-9875-044e96609755
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 1%

---

# Skapa en segmentering {#create-a-segmentation}

Med segmentering kan ni gruppera människor i olika profiler för rapportering och dynamiskt innehåll. Så här skapar du dem.

1. Gå till din **[!UICONTROL Database]**.

   ![](assets/create-a-segmentation-1.png)

1. Klicka på **[!UICONTROL New]** och sedan på **[!UICONTROL New Segmentation]**.

   ![](assets/create-a-segmentation-2.png)

   >[!TIP]
   >
   >Du kan skapa upp till 20 segment.

1. Ange en **[!UICONTROL Name]**, klicka på **[!UICONTROL Add Segment]** och ge den ett namn.

   ![](assets/create-a-segmentation-3.png)

   >[!NOTE]
   >
   >Det går inte att flytta, redigera eller ta bort standard.

1. Lägg till så många segment du vill (upp till 100).

   ![](assets/create-a-segmentation-4.png)

   >[!CAUTION]
   >
   >Det totala antalet segment som du kan skapa i en segmentering beror på antalet och typen av filter som används och även på hur komplex logiken i segmenten är. Du kan skapa upp till 100 segment med hjälp av standardfält, men med andra typer av filter kan det bli mer komplicerat och segmenteringen kanske inte kan godkännas. Några exempel är: anpassade fält, listmedlem, leadägarfält och intäktsfaser.
   >
   >Om du får ett felmeddelande under godkännandet och behöver hjälp med att minska komplexiteten i din segmentering kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Dra och släpp segmenten runt om för att ändra deras ordning. Klicka på **[!UICONTROL Create]** när du är klar.

   ![](assets/create-a-segmentation-5.png)

   >[!NOTE]
   >
   >En person kvalificerar sig för det första matchande segmentet i [order](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md) som definierats.

   >[!NOTE]
   >
   >Du måste definiera segmentregler innan du kan använda segmenteringen.

   Grattis! Du är ett steg närmare att använda dynamiskt innehåll.

   >[!MORELIKETHIS]
   >
   >[Definiera segmentregler](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
