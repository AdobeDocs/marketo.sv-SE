---
unique-page-id: 2952678
description: Använd Skicka aviseringsinformationstoken {{SP_Send_Alert_Info}} - Marketo Docs - Produktdokumentation
title: Använda Skicka aviseringsinformationstoken
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Använda Skicka aviseringsinformationstoken {#use-the-send-alert-info-token-sp-send-alert-info}

Denna `{{SP_Send_Alert_Info}}` token är en särskild token som ska användas när du skapar varningsmeddelanden för ditt säljteam.

>[!TIP]
>
>Denna token fungerar bara som avsett när du skickar e-postmeddelandet som innehåller det med flödessteget [Skicka avisering](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) . Det fungerar inte när det används i ett skicka-e-postflödessteg.

Exempelvarning:   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Skärp dig! URL:er i varningar har förfallodatum så kontrollera att de har en stängsel som stöder den här typen av meddelanden. Förfallodatum [konfigureras av en administratör](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Följande information ingår i `{{SP_Send_Alert_Info}}`:

* Förnamn och efternamn som en länk till personinformationen i Marketo
* En länk till personen i CRM
* Kampanjnamnet i Marketo som skickade aviseringen
* Tiden då varningen skickades

>[!NOTE]
>
>Länken till CRM visas bara om personen finns i CRM-systemet (som för närvarande inte är tillgänglig i Dynamics CRM). Länken är tillgänglig för både Marketo- och icke-Marketo-användare.

## Lägg till token SP_Send_Alert_Info i ett e-postmeddelande {#add-the-sp-send-alert-info-token-to-an-email}

1. Markera e-postmeddelandet och klicka på **Redigera utkast**.

   ![](assets/one-3.png)

1. Dubbelklicka på det redigerbara området där du vill lägga till variabeln.

   ![](assets/two-3.png)

1. Placera markören där du vill att token ska vara och klicka sedan på knappen **Infoga token** .

   ![](assets/three-3.png)

1. Leta reda på och välj **`{{SP_Send_Alert_Info}}`** variabeln och klicka på **Infoga**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicka på **Spara**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Påminnelse**
>
>Glöm inte att godkänna e-postmeddelandet.

Bra grejer! Denna token är mycket användbar och du bör använda den i alla aviseringar som du skapar för ditt säljteam.