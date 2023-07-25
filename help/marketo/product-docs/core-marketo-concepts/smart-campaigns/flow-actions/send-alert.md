---
unique-page-id: 1146958
description: Skicka avisering - Marketo Docs - produktdokumentation
title: Skicka avisering
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Skicka avisering {#send-alert}

## Översikt {#overview}

Marketo kan skicka ett e-postmeddelande med personinformation till vem som helst - säljaren, en partner eller någon annan. Använd **Skicka avisering** flödessteg.

![](assets/one-1.png)

## Användning {#usage}

1. Sök efter och välj det e-postmeddelande som du vill skicka.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Din e-postavisering måste innehålla all rubrikinformation och finnas i **Godkänd** tillstånd.

1. Du kan klicka på förhandsgranskningsikonen för att kontrollera att du har valt rätt e-postadress.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Var noga med att använda **Skicka aviseringsinformation** din e-postadress.

1. Välj varningsmottagare. Du kan välja Säljare eller Kontoägare.

   ![](assets/four-2.png)

1. Du kan också lägga till andra e-postadresser som du vill ha (avgränsade med kommatecken eller semikolon).

   ![](assets/five.png)

   >[!TIP]
   >
   >I utlösande kampanjer kan du använda variabler i **Till andra e-postmeddelanden** som `{{lead.Territory Owner}}` eller `{{my.Alert Recipient}}` så länge som värdena är giltiga e-postadresser. Tokens in **Till andra e-postmeddelanden** kommer inte att fungera i en batchkampanj.

Så ja! Nu vet du hur man använder **Skicka avisering** flödessteg.

>[!MORELIKETHIS]
>
>[Skapa ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
