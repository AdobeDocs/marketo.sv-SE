---
unique-page-id: 2952678
description: Använd informationstoken för skicka-varning {{SP_Send_Alert_Info}} - Marketo Docs - produktdokumentation
title: Använda Skicka aviseringsinformationstoken
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Använda Skicka aviseringsinformationstoken {#use-the-send-alert-info-token-sp-send-alert-info}

Token `{{SP_Send_Alert_Info}}` är en särskild token som ska användas när du skapar varningsmeddelanden för ditt säljteam.

>[!TIP]
>
>Denna token fungerar bara som avsett när du skickar e-postmeddelandet som innehåller det med flödessteget [Skicka avisering](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). Det fungerar inte när det används i ett skicka-e-postflödessteg.

Exempelvarning:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Skärp dig! URL:er i varningar har förfallodatum så kontrollera att de har en stängsel som stöder den här typen av meddelanden. Förfallodatum är [konfigurerade av en administratör](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Följande information ingår i `{{SP_Send_Alert_Info}}`:

* Förnamn och efternamn som länk till personinformationen i Marketo
* En länk till personen i CRM
* Kampanjnamnet i Marketo som skickade aviseringen
* Den tidpunkt då varningen skickades

>[!NOTE]
>
>Länken till CRM visas bara om personen finns i CRM-systemet (som för närvarande inte är tillgänglig i Dynamics CRM). Länken är tillgänglig för både Marketo- och icke-Marketo-användare.

## Lägg till token SP_Send_Alert_Info i ett e-postmeddelande {#add-the-sp-send-alert-info-token-to-an-email}

1. Markera e-postmeddelandet och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/one-3.png)

1. Dubbelklicka på det redigerbara området där du vill lägga till variabeln.

   ![](assets/two-3.png)

1. Placera markören där du vill att token ska vara och klicka sedan på knappen **[!UICONTROL Insert Token]**.

   ![](assets/three-3.png)

1. Sök efter och välj token **[!UICONTROL {{SP_Send_Alert_Info}}]** och klicka på **[!UICONTROL Insert]**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Klicka på **[!UICONTROL Save]**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Glöm inte att godkänna e-postmeddelandet.

Bra grejer! Denna token är mycket användbar och du bör använda den i alla aviseringar som du skapar för ditt säljteam.
