---
unique-page-id: 2359457
description: Godkänn en segmentering - Marketo Docs - produktdokumentation
title: Godkänn en segmentering
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '232'
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

1. Gå till **databasen**.

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. I segmenteringen klickar du på **Segmenteringsåtgärder** och sedan på **Godkänn**.

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >Status ändras till Godkännande med ett snurrhjul ( ![](assets/image2014-9-15-15-3a31-3a43.png)) medan godkännandet pågår.

   >[!CAUTION]
   >
   >Godkännandet kan ta några minuter till mer än en dag, beroende på databasens storlek.

   När det är godkänt ändras statusen från Godkännande till Godkänt.
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >Antalet personer i varje segment visas inom hakparenteser bredvid segmentnamnet.

1. Fliken **Personer** i **segmentet** visar nu den slutliga listan över personer för segmentet.

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>Det totala antalet segment som du kan skapa i en segmentering beror på antalet och typen av filter som används och även på hur komplex logiken i segmenten är. Du kan skapa upp till 100 segment med hjälp av standardfält, men med andra typer av filter kan det bli mer komplicerat och segmenteringen kanske inte kan godkännas. Några exempel är: anpassade fält, listmedlem, leadägarfält och intäktsfaser.
>
>Om du får ett felmeddelande under godkännandet och behöver hjälp med att minska komplexiteten i din segmentering kontaktar du [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Använd segmentfilter i en smart lista](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
