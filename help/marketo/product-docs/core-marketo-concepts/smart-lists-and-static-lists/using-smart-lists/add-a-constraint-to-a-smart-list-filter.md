---
unique-page-id: 2949413
description: Lägg till en begränsning i ett smart listfilter - Marketo Docs - Produktdokumentation
title: Lägga till en begränsning i ett smart listfilter
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: aeefe7a5c265e3a7ddd50920820742a463ab178a
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 2%

---

# Lägga till en begränsning i ett smart listfilter {#add-a-constraint-to-a-smart-list-filter}

När du skapar en smart lista har vissa filter avancerade alternativ som kallas &quot;begränsningar&quot;. Det här är extra villkor som du kan lägga till i filter och utlösare för att begränsa sökningen ytterligare.

I det här exemplet lägger vi till några begränsningar i en **[Datavärdet har ändrats](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** filtrera för att hitta personer som har en statusändring från MQL till SQL.

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Använd filtret&quot;Datavärdet har ändrats&quot; i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/ma-1.png)

1. Markera den smarta listan med ett filter som du lägger till en begränsning till och klicka på **[!UICONTROL Smart List]** -fliken.

   ![](assets/two-3.png)

1. Under **[!UICONTROL Add Constraint]** väljer du **[!UICONTROL Previous Value]**.

   ![](assets/three-3.png)

1. Ange **[!UICONTROL Previous Value]**. I det här exemplet använder vi MQL.

   ![](assets/four-2.png)

1. Under **[!UICONTROL Add Constraint]** väljer du **[!UICONTROL New Value]**.

   ![](assets/five.png)

1. Ange det nya värdet. I det här exemplet använder vi SQL.

   ![](assets/six.png)

1. Snyggt gjort! Klicka på **[!UICONTROL People]** för att se alla personer som haft en statusändring från &quot;MQL&quot; till &quot;SQL&quot; under de senaste 30 dagarna.
