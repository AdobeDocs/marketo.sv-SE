---
unique-page-id: 1147324
description: Rensa fältvärden - Marketo Docs - produktdokumentation
title: Rensa fältvärden
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '92'
ht-degree: 0%

---

# Rensa fältvärden {#clear-field-values}

[Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) är bra, men hur _tar du bort_ värdet fullständigt? Bra fråga!

1. I flödessteget väljer du det fält som du vill ta bort och skriver **[!UICONTROL NULL]** (endast versaler) som **[!UICONTROL New Value]**.

   ![](assets/clear-field-values-1.png)

1. När flödessteget är klart rensas värdet för det fält du valde.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Om du lämnar det nya värdet tomt eller bara anger ett blanksteg töms fältet inte. Du måste skriva in NULL. Kom ihåg att flödessteg inte kan ångras efter körning.
