---
unique-page-id: 2949413
description: Lägg till en begränsning i ett smart listfilter - Marketo Docs - Produktdokumentation
title: Lägga till en begränsning i ett smart listfilter
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Lägga till en begränsning i ett smart listfilter {#add-a-constraint-to-a-smart-list-filter}

När du skapar smarta listor har vissa filter avancerade alternativ som kallas *begränsningar. *Det här är extra villkor som du kan lägga till i filter och utlösare för att begränsa sökningen ytterligare.

I det här exemplet lägger vi till några begränsningar i ett ** [Data Value Changed](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**-filter för att hitta personer som har en statusändring från MQL till SQL.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>* [Skapa en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Använd filtret&quot;Datavärdet har ändrats&quot; i en smart lista](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Gå till **marknadsföringsaktiviteter**.

   ![](assets/ma-1.png)

1. Markera den smarta listan med ett filter som du vill lägga till en begränsning i och klicka på fliken **Smart lista** .

   ![](assets/two-3.png)

1. Under **Lägg till begränsning** väljer du **Föregående värde**.

   ![](assets/three-3.png)

1. Ange **föregående värde**. I det här exemplet använder vi MQL.

   ![](assets/four-2.png)

1. Under **Lägg till begränsning** väljer du **Nytt värde**.

   ![](assets/five.png)

1. Ange det **nya värdet**. I det här exemplet använder vi SQL.

   ![](assets/six.png)

1. Snyggt gjort! Klicka på fliken **Personer** för att se alla personer som haft en **status** som har ändrats från **MQL** till **SQL** under de senaste 30 dagarna.

