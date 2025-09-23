---
description: Marketo Unsubscribe Check - Marketo Docs - produktdokumentation
title: Avbeställ Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# [!UICONTROL Marketo Unsubscribe Check] {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check] använder teamets anslutning till Marketo för att förhindra att e-postmeddelanden skickas till personer som har avbrutit prenumerationen i Marketo Lead Management-system. När en säljanvändare skickar ett e-postmeddelande med [!DNL Marketo Sales], görs ett API-anrop till Marketo för att kontrollera om e-post-ID:t har avbrutits. I så fall blockerar vi e-postmeddelandet från att skickas.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Aktiverar {#turning-it-on}

1. Klicka på kugghjulsikonen och välj **[!UICONTROL Settings]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL Unsubscribes]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicka på fliken **[!UICONTROL Integrations]**. Klicka på skjutreglaget i avsnittet [!UICONTROL Marketo Unsubscribe Check] för att aktivera kontrollen.

   ![](assets/marketo-unsubscribe-check-3.png)

## Saker att veta {#things-to-know}

The Marketo Unsubscribe check..

* Räknas inte med dina API-gränser
* Kräver en Marketo-anslutning
* Är en global inställning
* Blockerar e-postmeddelanden som skickas från webbprogrammet, e-postklienter och [!DNL Salesforce]
