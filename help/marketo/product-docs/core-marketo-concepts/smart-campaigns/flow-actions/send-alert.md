---
unique-page-id: 1146958
description: Skicka varning - Marketo Docs - Produktdokumentation
title: Skicka avisering
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Skicka avisering {#send-alert}

## Översikt {#overview}

Marketo kan skicka ett e-postmeddelande med personinformation till vem som helst - säljaren, en partner eller någon annan. Använd flödessteget **Skicka varning**.

![](assets/one-1.png)

## Användning {#usage}

1. Sök efter och välj det e-postmeddelande som du vill skicka.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Din e-postavisering måste innehålla all rubrikinformation och vara i läget **Godkänd**.

1. Du kan klicka på förhandsgranskningsikonen för att kontrollera att du har valt rätt e-postadress.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Var noga med att använda token **Skicka varningsinformation** i ditt e-postmeddelande.

1. Välj varningsmottagare. Du kan välja Säljare eller Kontoägare.

   ![](assets/four-2.png)

1. Du kan också lägga till andra e-postadresser som du vill ha (avgränsade med kommatecken eller semikolon).

   ![](assets/five.png)

   >[!TIP]
   >
   >I utlösarkampanjer kan du använda variabler i **till andra e-postmeddelanden**, till exempel `{{lead.Territory Owner}}` eller `{{my.Alert Recipient}}`, förutsatt att värdena är giltiga e-postadresser. Token i **To Other Emails** fungerar inte i en gruppkampanj.

Så ja! Nu vet du hur du använder flödessteget **Skicka varning**.

>[!MORELIKETHIS]
>
>[Skapa ett e-postmeddelande](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

