---
unique-page-id: 2949413
description: Lägg till en begränsning i ett smart listfilter - Marketo Docs - Produktdokumentation
title: Lägga till en begränsning i ett smart listfilter
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Lägga till en begränsning i ett smart listfilter {#add-a-constraint-to-a-smart-list-filter}

När du skapar smarta listor har vissa filter avancerade alternativ som kallas &quot;begränsningar&quot;. Det här är extra villkor som du kan lägga till i filter och utlösare för att begränsa sökningen ytterligare.

I det här exemplet lägger vi till några begränsningar i en **[Datavärdet har ändrats](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** filtrera för att hitta personer som har en statusändring från MQL till SQL.

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Använd filtret&quot;Datavärdet har ändrats&quot; i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera den smarta listan med ett filter som du vill lägga till en begränsning i och klicka på **Smart List** -fliken.

   ![](assets/two-3.png)

1. Under **Lägg till begränsning**, markera **Föregående värde**.

   ![](assets/three-3.png)

1. Ange **Föregående värde**. I det här exemplet använder vi MQL.

   ![](assets/four-2.png)

1. Under **Lägg till begränsning**, markera **Nytt värde**.

   ![](assets/five.png)

1. Ange **Nytt värde**. I det här exemplet använder vi SQL.

   ![](assets/six.png)

1. Snyggt gjort! Klicka på **Folk** för att se alla personer som har en **Status** ändra från **MQL** till **SQL** de senaste 30 dagarna.
