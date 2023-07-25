---
unique-page-id: 1147082
description: Ta bort person - Marketo Docs - produktdokumentation
title: Ta bort person
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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

Du kan ta bort från Marketo och inte från CRM, till exempel:

![](assets/three-3.png)

>[!NOTE]
>
>Ta bort personen från CRM **fungerar endast med Salesforce**. Om du tar bort en person från Marketo och väljer att behålla den i Salesforce, återskapas personen i Marketo om deras Salesforce-post någonsin uppdateras.
