---
description: Salesforce Sync Errors - Marketo Docs - Produktdokumentation
title: Salesforce-synkroniseringsfel
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Salesforce-synkroniseringsfel {#salesforce-sync-errors}

Visa en sammanfattning av de fel som uppstod under synkroniseringsprocessen. Detta inkluderar fel som orsakas av fel vid synkronisering av inkompatibla data.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Visa synkroniseringsfel {#view-sync-errors}

1. Klicka på **Admin**.

   ![](assets/salesforce-sync-errors-1.png)

1. Under Integrering klickar du på **Salesforce** och sedan på fliken **Synkroniseringsfel**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>De listade felen sträcker sig från den aktuella tiden till fem dagar före den aktuella synkroniseringen.

| Fält | Beskrivning |
|---|---|
| Misslyckades | Postnivå _eller_ jobbnivå |
| Datum/tid för felet | Felinformation |
| Feltyp | SFDC-returmeddelande |

>[!TIP]
>
>Om du klickar på posten på postnivå visas det relaterade objektets Marketo- och Salesforce-ID. I vissa fall är meddelandet på post- och jobbnivåfelen direkt från Salesforce. Om du söker efter dem online kan du få mer information.

## Filtersynkroniseringsfel {#filter-sync-errors}

1. Om du vill filtrera data klickar du på filterikonen längst till höger på sidan.

   ![](assets/salesforce-sync-errors-3.png)

1. Välj datum- och tidsintervall och filtrera sedan efter feltyp (jobbnivå eller postnivå). Klicka på **Använd** när du är klar.

   ![](assets/salesforce-sync-errors-4.png)

**Valfritt steg**: Om du vill exportera synkroniseringsfel klickar du på  **Exportera**. Data exporteras som en CSV-fil.

![](assets/salesforce-sync-errors-5.png)
