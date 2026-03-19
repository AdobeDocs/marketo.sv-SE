---
unique-page-id: 2359500
description: Lär dig mer om prioritet för segmenteringsorder och hur det avgör vilket segment en person tillhör. Redigera segmentordningen i databasen för att styra utvärderingen av segment.
title: Prioritet för segmenteringsordning
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---

# Prioritet för segmenteringsordning {#segmentation-order-priority}

Det är viktigt att förstå hur **order** anger prioriteten för utvärdering av dina personer i en segmentering.

>[!PREREQUISITES]
>
>[Skapa en segmentering](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[Definiera segmentregler](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Du kan bara redigera en segmentering i utkastläge.

1. Gå till **databasen**.

   ![](assets/segmentation-order-priority-1.png)

1. Välj din **segmentering**. Klicka på **[!UICONTROL Segmentation Actions]** i **[!UICONTROL Edit Segments]**.

   ![](assets/segmentation-order-priority-2.png)

   Du kan kontrollera eller redigera segmentens ordning på den här skärmen.

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* Segmenten utesluter varandra. En person kan bara vara medlem i ett segment åt gången.
>* När en person kvalificerar sig för två segment tillhör de bara det första i listan.
>* Om en person inte är berättigad till något segment blir han eller hon medlem i standardsegmentet.
