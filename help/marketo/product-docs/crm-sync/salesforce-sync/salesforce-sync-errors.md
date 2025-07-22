---
description: Salesforce Sync Errors - Marketo Docs - Produktdokumentation
title: Salesforce Sync-fel
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 1%

---

# [!DNL Salesforce] Synkroniseringsfel {#salesforce-sync-errors}

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
| Feltyp | SFDC Return message |

>[!TIP]
>
>Om du klickar på posten på postnivå visas det relaterade objektets Marketo- och [!DNL Salesforce]-ID. I vissa fall är meddelandet på post- och jobbnivåfelen direkt från [!DNL Salesforce]. Om du söker efter dem online kan du få mer information.

## Synkroniseringsfel för filter {#filter-sync-errors}

1. Om du vill filtrera data klickar du på filterikonen längst till höger på sidan.

   ![](assets/salesforce-sync-errors-3.png)

1. Välj datum- och tidsintervall och filtrera sedan efter feltyp (jobbnivå eller postnivå). Klicka på **[!UICONTROL Apply]** när du är klar.

   ![](assets/salesforce-sync-errors-4.png)

**VALFRITT STEG**: Om du vill exportera synkroniseringsfel klickar du på **[!UICONTROL Export]**. Data exporteras som en CSV-fil.

![](assets/salesforce-sync-errors-5.png)
