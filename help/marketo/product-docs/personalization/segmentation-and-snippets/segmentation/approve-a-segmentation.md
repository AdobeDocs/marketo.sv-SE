---
unique-page-id: 2359457
description: Godkänn en segmentering - Marketo Docs - produktdokumentation
title: Godkänn en segmentering
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: b29186ba84ec88be42432e56d1ad0e77c5b43900
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Godkänn en segmentering {#approve-a-segmentation}

En segmentering måste godkännas innan den kan användas.

>[!PREREQUISITES]
>
>* [Skapa en segmentering](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definiera segmentregler](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Högst 20 segment kan godkännas åt gången.

1. Gå till **[!UICONTROL Database]**.

   ![](assets/approve-a-segmentation-1.png)

1. Klicka på **[!UICONTROL Segmentation Actions]** i segmenteringen och sedan på **[!UICONTROL Approve]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >Statusen ändras till _Godkänner_ medan godkännandet pågår.

   >[!CAUTION]
   >
   >Godkännandet kan ta från några minuter till en dag eller två för att slutföra, beroende på databasens storlek.

1. När det har godkänts ändras [!UICONTROL Status] från [!UICONTROL Approving] till [!UICONTROL Approved].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >Antalet personer i varje segment visas inom hakparenteser bredvid segmentnamnet.

1. Fliken **[!UICONTROL People]** i **[!UICONTROL Segment]** visar nu den slutliga listan över personer för segmentet.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>Det totala antalet segment som du kan skapa i en segmentering beror på antalet och typen av filter som används och även på hur komplex logiken i segmenten är. Du kan skapa upp till 100 segment med hjälp av standardfält, men med andra typer av filter kan det bli mer komplicerat och segmenteringen kanske inte kan godkännas. Några exempel är: anpassade fält, listmedlem, leadägarfält och intäktsfaser.
>
>Om du får ett felmeddelande under godkännandet och behöver hjälp med att minska komplexiteten i din segmentering kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Använd segmentfilter i en smart lista](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
