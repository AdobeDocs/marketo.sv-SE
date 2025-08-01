---
unique-page-id: 4719312
description: Lägg till/ta bort värden för plocklistor - Marketo Docs - Produktdokumentation
title: Lägg till/ta bort värden för plocklistor
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Lägg till/ta bort värden för plocklistor {#add-remove-picklist-values}

Här är några saker du bör känna till när det gäller att lägga till och ta bort plocklistevärden i [!DNL Salesforce].

## Lägga till värden för plocklista {#adding-picklist-values}

1. Om ett extra värde läggs till i Salesforce för en ifyllningsfältstyp får du ett [meddelande](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} som identifierar vilka formulär som detta påverkar.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Gå till formulärredigeraren och [lägg till det extra värdet](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} i listan med förslag.

## Ta bort värden för plocklistor {#remove-picklist-values}

När ett listvärde tas bort från ett fält i [!DNL Salesforce] måste du ta bort det här värdet manuellt från alla formulär som är värdar för det här fältet.

>[!NOTE]
>
>Om ett lead-fält och ett kontaktfält i Salesforce har olika värden är de gemensamma värdena tillgängliga i Marketo Engage.

Om ett lead-fält och ett kontaktfält i [!DNL Salesforce] har olika värden:

1. Om du lägger till ytterligare ett värde i SFDC i en lista visas ett meddelande.
1. Meddelandet talar om var det används. Du kan nu lägga till det nya värdet som ett alternativ i formuläret om du vill.

Om en lista med ett SFDC-lead har andra värden än en plocklista för en SFDC-kontakt, används de gemensamma värdena som standardvärdesalternativ i formuläret.

Om du tar bort ett värde från en lista måste du ta bort det manuellt som ett alternativ från formulären.
