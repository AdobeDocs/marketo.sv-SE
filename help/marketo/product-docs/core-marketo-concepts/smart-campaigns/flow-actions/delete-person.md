---
unique-page-id: 1147082
description: Ta bort person - Marketo Docs - Produktdokumentation
title: Ta bort person
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Ta bort person {#delete-person}

Fel personer kommer ibland in i databasen. Flödessteget Ta bort person kan ta bort dem.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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
>Att ta bort personen från CRM fungerar **bara med Salesforce**. Om du tar bort en person från Marketo och väljer att behålla dem i Salesforce, återskapas de i Marketo om deras Salesforce-post någonsin uppdateras.

