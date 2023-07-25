---
unique-page-id: 1147324
description: Rensa fältvärden - Marketo Docs - produktdokumentation
title: Rensa fältvärden
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Rensa fältvärden {#clear-field-values}

[Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) är bra, men hur mår du? _ta bort_ värdet fullständigt? Bra fråga!

1. I flödessteget väljer du det fält som du vill ta bort och skriver in **NULL** (all caps) som **Nytt värde**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Det visste du säkert inte! När flödessteget är klart rensas värdet för det fält du valde.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Om du lämnar det nya värdet tomt eller bara anger ett blanksteg töms fältet inte. Du måste skriva in NULL. Kom ihåg att flödessteg inte kan ångras efter körning.
