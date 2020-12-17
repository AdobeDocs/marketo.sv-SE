---
unique-page-id: 1147082
description: Ta bort person - Marketo Docs - Produktdokumentation
title: Ta bort person
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# Ta bort person {#delete-person}

Fel personer kommer ibland in i databasen. Flödessteget Ta bort person kan ta bort dem.

## Översikt {#overview}

Använd flödessteget i en smart kampanj.

![](assets/one-4.png)

>[!CAUTION]
>
>När du tar bort en person tas även alla deras historiska RCE-data bort. Det kan inte ångras.

## Användning {#usage}

När du drar i flödessteget ställs den automatiskt in så att den även tas bort från CRM.

![](assets/two-4.png)

Du kan ta bort från Marketo och inte från CRM, som:

![](assets/three-3.png)

>[!NOTE]
>
>Att ta bort personen från CRM **fungerar bara med Salesforce**. Om du tar bort en person från Marketo och väljer att behålla dem i Salesforce, återskapas de i Marketo om deras Salesforce-post någonsin uppdateras.

