---
unique-page-id: 2952678
description: Använda Skicka aviseringsinformationstoken {{SP_Send_Alert_Info}} - Marketo Docs - produktdokumentation
title: Använda Skicka aviseringsinformationstoken
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Använda Skicka aviseringsinformationstoken {#use-the-send-alert-info-token-sp-send-alert-info}

The `{{SP_Send_Alert_Info}}` -token är en särskild token som ska användas när du skapar varningsmeddelanden för ditt säljteam.

>[!TIP]
>
>Denna token fungerar bara som avsett när du skickar e-postmeddelandet som innehåller det med [Skicka avisering](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) flödessteg. Det fungerar inte när det används i ett skicka-e-postflödessteg.

Exempelvarning:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Skärp dig! URL:er i varningar har förfallodatum så kontrollera att de har en stängsel som stöder den här typen av meddelanden. Förfallodatum är [konfigurerad av en administratör](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Följande information ingår i `{{SP_Send_Alert_Info}}`:

* Förnamn och efternamn som länk till personinformationen i Marketo
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

1. Placera markören där du vill att variabeln ska vara och klicka sedan på **Infoga token** -knappen.

   ![](assets/three-3.png)

1. Sök och välj **`{{SP_Send_Alert_Info}}`** token och klicka **Infoga**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicka **Spara**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Glöm inte att godkänna e-postmeddelandet.

Bra grejer! Denna token är mycket användbar och du bör använda den i alla aviseringar som du skapar för ditt säljteam.
