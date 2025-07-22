---
unique-page-id: 18317340
description: Marketo Unsubscribe Check - Marketo Docs - produktdokumentation
title: Avbeställ Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Avbeställ Marketo {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check] använder teamets anslutning till Marketo för att förhindra att e-postmeddelanden skickas till personer som har avbrutit prenumerationen i Marketo Lead Management-system. När en säljanvändare skickar ett e-postmeddelande med [!DNL Sales Connect], görs ett API-anrop till Marketo för att kontrollera om e-post-ID:t har avbrutits. I så fall blockerar vi e-postmeddelandet från att skickas.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Aktiverar {#turning-it-on}

1. Klicka på kugghjulsikonen i webbprogrammet och välj **[!UICONTROL Settings]**.

   ![](assets/one-2.png)

1. Klicka på [!UICONTROL Admin Settings] under **[!UICONTROL Unsubscribes]**.

   ![](assets/two-3.png)

1. Klicka på **[!UICONTROL Integrations]**.

   ![](assets/three-3.png)

1. Klicka på skjutreglaget i avsnittet [!UICONTROL Marketo Unsubscribe Check] för att aktivera kontrollen.

   ![](assets/four-2.png)

## Saker att veta {#things-to-know}

The Marketo Unsubscribe check..

* Räknas inte med dina API-gränser
* Kräver en Marketo-anslutning
* Är en global inställning
* Blockerar e-postmeddelanden som skickas från webbprogrammet, e-postklienter och Salesforce
* Loggar ett misslyckat e-postmeddelande eller hindrar en användare från att skicka när han/hon försöker skicka för alla arbetsflöden (e-post-plugin-sändning, enskild sändning, säljkampanj, flera val och skicka) förutom [gruppmeddelanden](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md) där vi förhindrar att e-postmeddelanden skickas tyst
