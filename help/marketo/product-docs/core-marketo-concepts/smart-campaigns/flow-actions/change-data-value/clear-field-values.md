---
unique-page-id: 1147324
description: Rensa fältvärden - Marketo Docs - produktdokumentation
title: Rensa fältvärden
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Rensa fältvärden {#clear-field-values}

[Ändra datavärden ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) är bra, men hur tar du  __ bort värdet helt? Bra fråga!

1. I flödessteget väljer du det fält som du vill rensa och skriver **NULL** (all caps) som **Nytt värde**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Det visste du säkert inte! När flödessteget är klart rensas värdet för det fält du valde.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Om du lämnar det nya värdet tomt eller bara anger ett blanksteg töms fältet inte. Du måste skriva in NULL. Kom ihåg att flödessteg inte kan ångras efter körning.
