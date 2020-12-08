---
unique-page-id: 18317340
description: Marketo Unsubscribe Check - Marketo Docs - Produktdokumentation
title: Marketo Avbeställ kontroll
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Marketo Avbeställ kontroll {#marketo-unsubscribe-check}

Marketo Unsubscribe Check använder teamets anslutning till Marketför att förhindra att e-postmeddelanden skickas till personer som har avbrutit prenumerationen i Marketos Lead Management-system. När en säljanvändare skickar ett e-postmeddelande med Sales Connect, görs ett API-anrop till Marketo för att kontrollera om e-post-ID:t har avbrutits. I så fall blockerar vi e-postmeddelandet från att skickas.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Aktiverar {#turning-it-on}

1. Klicka på kugghjulsikonen i webbprogrammet och välj **Inställningar**.

   ![](assets/one-2.png)

1. Klicka på **Avbeställ** under Administratörsinställningar.

   ![](assets/two-3.png)

1. Klicka på **Integrationer**.

   ![](assets/three-3.png)

1. Klicka på skjutreglaget i avsnittet Marketo Unsubscribe Check (Avsluta prenumeration) för att aktivera kontrollen.

   ![](assets/four-2.png)

## Saker att veta {#things-to-know}

Marketo Unsubscribe check..

* Räknas inte med dina API-gränser
* Kräver en Marketo-anslutning
* Är en global inställning
* Blockerar e-postmeddelanden som skickas från webbprogrammet, e-postklienter och Salesforce

