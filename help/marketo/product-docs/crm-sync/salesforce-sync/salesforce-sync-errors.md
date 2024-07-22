---
description: Salesforce-synkroniseringsfel - Marketo Docs - produktdokumentation
title: Salesforce-synkroniseringsfel
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Salesforce-synkroniseringsfel {#salesforce-sync-errors}

Visa en sammanfattning av de fel som uppstod under synkroniseringsprocessen. Detta inkluderar fel som orsakas av fel vid synkronisering av inkompatibla data.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Visa synkroniseringsfel {#view-sync-errors}

1. Klicka på **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-errors-1.png)

1. Under Integrering klickar du på **Salesforce** och sedan på fliken **[!UICONTROL Sync Errors]**.

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

## Synkroniseringsfel för filter {#filter-sync-errors}

1. Om du vill filtrera data klickar du på filterikonen längst till höger på sidan.

   ![](assets/salesforce-sync-errors-3.png)

1. Välj datum- och tidsintervall och filtrera sedan efter feltyp (jobbnivå eller postnivå). Klicka på **[!UICONTROL Apply]** när du är klar.

   ![](assets/salesforce-sync-errors-4.png)

**VALFRITT STEG**: Om du vill exportera synkroniseringsfel klickar du på **[!UICONTROL Export]**. Data exporteras som en CSV-fil.

![](assets/salesforce-sync-errors-5.png)
