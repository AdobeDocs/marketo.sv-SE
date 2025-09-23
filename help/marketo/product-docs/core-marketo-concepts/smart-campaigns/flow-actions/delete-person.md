---
unique-page-id: 1147082
description: Ta bort person - Marketo Docs - produktdokumentation
title: Ta bort person
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 0%

---

# Ta bort person {#delete-person}

Fel personer kommer ibland in i databasen. Flödessteget Ta bort person kan ta bort dem.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>När du tar bort en person tas även alla deras historiska RCE-data bort. Det kan inte ångras.

1. När du drar i flödessteget ställs det automatiskt in på att tas bort från CRM.

   ![](assets/delete-person-2.png)

1. Du kan ta bort från Marketo Engage och inte från CRM, till exempel:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Det går bara att ta bort personen från CRM _med[!DNL Salesforce]_. Om du tar bort en person från Marketo och väljer att behålla den i [!DNL Salesforce], återskapas personen i Marketo om hans/hennes [!DNL Salesforce]-post någonsin uppdateras.
