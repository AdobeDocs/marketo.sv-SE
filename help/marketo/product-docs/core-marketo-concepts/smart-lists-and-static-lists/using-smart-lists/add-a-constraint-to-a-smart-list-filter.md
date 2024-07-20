---
unique-page-id: 2949413
description: Lägg till en begränsning i ett smart listfilter - Marketo Docs - Produktdokumentation
title: Lägga till en begränsning i ett smart listfilter
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Lägga till en begränsning i ett smart listfilter {#add-a-constraint-to-a-smart-list-filter}

När du skapar en smart lista har vissa filter avancerade alternativ som kallas &quot;begränsningar&quot;. Det här är extra villkor som du kan lägga till i filter och utlösare för att begränsa sökningen ytterligare.

I det här exemplet lägger vi till begränsningar i ett **[datavärde ändrat](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}**-filter för att hitta personer som har en statusändring från MQL till SQL.

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Använd filtret&quot;Datavärdet har ändrats&quot; i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Markera den smarta listan med ett filter som du lägger till en begränsning i och klicka på fliken **[!UICONTROL Smart List]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. Välj **[!UICONTROL Previous Value]** under **[!UICONTROL Add Constraint]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Ange **[!UICONTROL Previous Value]**. I det här exemplet använder vi MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. Välj **[!UICONTROL New Value]** under **[!UICONTROL Add Constraint]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Ange det nya värdet. I det här exemplet använder vi SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Snyggt gjort! Klicka på fliken **[!UICONTROL People]** för att visa alla personer som har haft en statusändring från MQL till SQL under de senaste 30 dagarna.
