---
unique-page-id: 2949413
description: Lägg till en begränsning i ett smart listfilter - Marketo Docs - Produktdokumentation
title: Lägga till en begränsning i ett smart listfilter
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Lägg till en begränsning i ett smart listfilter {#add-a-constraint-to-a-smart-list-filter}

När du skapar smarta listor har vissa filter avancerade alternativ som kallas &quot;begränsningar&quot;. Det här är extra villkor som du kan lägga till i filter och utlösare för att begränsa sökningen ytterligare.

I det här exemplet lägger vi till begränsningar i ett **[datavärde ändrat](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**-filter för att hitta personer som har en statusändring från MQL till SQL.

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Använd filtret&quot;Datavärdet har ändrats&quot; i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera den smarta listan med ett filter som du vill lägga till en begränsning i och klicka på fliken **Smart lista**.

   ![](assets/two-3.png)

1. Under **Lägg till begränsning** väljer du **Föregående värde**.

   ![](assets/three-3.png)

1. Ange **föregående värde**. I det här exemplet använder vi MQL.

   ![](assets/four-2.png)

1. Välj **Nytt värde** under **Lägg till begränsning**.

   ![](assets/five.png)

1. Ange **Nytt värde**. I det här exemplet använder vi SQL.

   ![](assets/six.png)

1. Snyggt gjort! Klicka på fliken **Personer** om du vill visa alla personer som har en **status** som har ändrats från **MQL** till **SQL** de senaste 30 dagarna.
