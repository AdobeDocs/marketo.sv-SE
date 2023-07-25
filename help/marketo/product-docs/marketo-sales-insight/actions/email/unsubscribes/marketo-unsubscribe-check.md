---
description: Avbeställ Marketo - Marketo Docs - produktdokumentation
title: Avbeställ Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Avbeställ Marketo {#marketo-unsubscribe-check}

Marketo Unsubscribe Check (Avbeställ kontroll) använder teamets anslutning till Marketo för att förhindra att e-postmeddelanden skickas till personer som har avbeställt tjänsten i Marketo Lead Management System. När en säljare skickar ett e-postmeddelande till Marketo Sales, görs ett API-anrop till Marketo för att kontrollera om e-post-ID:t har avbrutits. I så fall blockerar vi e-postmeddelandet från att skickas.

>[!NOTE]
>
>**Administratörsbehörigheter krävs**

## Aktiverar {#turning-it-on}

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Under Administratörsinställningar klickar du på **Avbeställ**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Klicka på **Integreringar** -fliken. Aktivera kontrollen genom att klicka på skjutreglaget i avsnittet Avsluta prenumeration på Marketo.

   ![](assets/marketo-unsubscribe-check-3.png)

## Saker att veta {#things-to-know}

The Marketo Unsubscribe check..

* Räknas inte med dina API-gränser
* Kräver en Marketo-anslutning
* Är en global inställning
* Blockerar e-postmeddelanden som skickas från webbprogrammet, e-postklienter och Salesforce
