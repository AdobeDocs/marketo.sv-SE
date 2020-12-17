---
unique-page-id: 1147324
description: Rensa fältvärden - Marketo Docs - Produktdokumentation
title: Rensa fältvärden
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Rensa fältvärden {#clear-field-values}

** [Ändra datavärde](../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** är bra, men hur tar du *bort* värdet fullständigt? Bra fråga!

1. I flödessteget väljer du det fält som du vill rensa och skriver in **NULL **(all caps) som **Nytt värde**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Det visste du säkert inte! När flödessteget är klart rensas värdet för det fält du valde.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Om du lämnar det nya värdet tomt eller bara anger ett blanksteg töms fältet inte. Du måste skriva in NULL. Kom ihåg att flödessteg inte kan ångras efter körning.

   ![(leende)](assets/smile.svg)

Förresten, den här lilla tekniken finns på Marketo-certifieringsprovet. Säg inte till dem att vi sa så!