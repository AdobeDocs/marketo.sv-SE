---
unique-page-id: 1147082
description: Ta bort person - Marketo Docs - produktdokumentation
title: Ta bort person
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '123'
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

Du kan ta bort från Marketo Engage och inte från CRM, som:

![](assets/three-3.png)

>[!NOTE]
>
>Ta bort personen från CRM _fungerar bara med[!DNL Salesforce]_. Om du tar bort en person från Marketo och väljer att behålla den [!DNL Salesforce]kommer de att återskapas i Marketo om deras [!DNL Salesforce] posten uppdateras.
