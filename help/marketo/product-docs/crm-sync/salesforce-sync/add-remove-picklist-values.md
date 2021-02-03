---
unique-page-id: 4719312
description: Lägg till/ta bort plocklistevärden - Marketo-dokument - Produktdokumentation
title: Lägg till/ta bort värden för plocklistor
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Lägg till/ta bort värden för plocklistor {#add-remove-picklist-values}

Här är några saker du bör känna till när det gäller att lägga till och ta bort plocklistevärden i Salesforce.

## Lägger till värden för plocklista {#adding-picklist-values}

1. Om ett extra värde läggs till i Salesforce för en typ av listfält får du ett [meddelande](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) som identifierar vilka formulär som detta påverkar.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Gå till formulärredigeraren och [lägg till det extra värdet](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) i listan med förslag.

## Ta bort värden för plocklista {#remove-picklist-values}

När ett listvärde tas bort från ett fält i Salesforce måste du ta bort det här värdet manuellt från alla formulär som är värdar för det här fältet.

>[!NOTE]
>
>Om ett lead-fält och ett kontaktfält i Salesforce har olika värden är de gemensamma värdena tillgängliga för användning i Marketo.

Om ett lead-fält och ett kontaktfält i Salesforce har olika värden:

1. Om du lägger till ytterligare ett värde i SFDC i en plocklista visas ett meddelande.
1. Meddelandet talar om var det används. Du kan nu lägga till det nya värdet som ett alternativ i formuläret om du vill.

Om en lista med SFDC-leads har andra värden än en lista för en SFDC-kontakt, används de gemensamma värdena som standardvärdesalternativ i formuläret.

Om du tar bort ett värde från en lista måste du ta bort det manuellt som ett alternativ från formulären.
