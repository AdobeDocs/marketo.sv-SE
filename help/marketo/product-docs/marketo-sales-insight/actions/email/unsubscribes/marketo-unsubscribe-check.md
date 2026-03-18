---
description: Läs mer om Marketo Unsubscribe Check så att säljarna inte kan mejla personer som avbeställt prenumerationer i Marketo.
title: Avbeställ Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '135'
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
