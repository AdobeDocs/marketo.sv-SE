---
unique-page-id: 18317340
description: Marketo Unsubscribe Check - Marketo Docs - produktdokumentation
title: Avbeställ Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Avbeställ Marketo {#marketo-unsubscribe-check}

Marketo Unsubscribe Check (Avbeställ kontroll) använder teamets anslutning till Marketo för att förhindra att e-postmeddelanden skickas till personer som har avbeställt tjänsten i Marketo Lead Management System. När en säljanvändare skickar ett e-postmeddelande med Sales Connect, görs ett API-anrop till Marketo för att kontrollera om e-post-ID:t har avbrutits. I så fall blockerar vi e-postmeddelandet från att skickas.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Aktiverar {#turning-it-on}

1. Klicka på kugghjulsikonen i webbprogrammet och välj **Inställningar**.

   ![](assets/one-2.png)

1. Klicka på **Avsluta prenumeration** under Administratörsinställningar.

   ![](assets/two-3.png)

1. Klicka på **Integrationer**.

   ![](assets/three-3.png)

1. Aktivera kontrollen genom att klicka på skjutreglaget i avsnittet Avsluta prenumeration på Marketo.

   ![](assets/four-2.png)

## Saker att veta {#things-to-know}

The Marketo Unsubscribe check..

* Räknas inte med dina API-gränser
* Kräver en Marketo-anslutning
* Är en global inställning
* Blockerar e-postmeddelanden som skickas från webbprogrammet, e-postklienter och Salesforce
* Loggar ett misslyckat e-postmeddelande eller hindrar en användare från att skicka när han/hon försöker skicka för alla arbetsflöden (e-post-plugin-sändning, enskild sändning, säljkampanj, flera val och skicka) förutom [gruppmeddelanden](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md) där vi förhindrar att e-postmeddelanden skickas tyst
