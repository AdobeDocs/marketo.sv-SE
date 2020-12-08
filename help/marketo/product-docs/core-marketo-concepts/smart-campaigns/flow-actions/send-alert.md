---
unique-page-id: 1146958
description: Skicka varning - Marketo Docs - Produktdokumentation
title: Skicka avisering
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Skicka avisering {#send-alert}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Översikt {#overview}

Marketo kan skicka ett e-postmeddelande med personinformation till vem som helst - säljaren, en partner eller någon annan. Använd flödessteget **Skicka avisering** .

![](assets/one-1.png)

## Användning {#usage}

1. Sök efter och välj det e-postmeddelande som du vill skicka.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Din e-postavisering måste innehålla all rubrikinformation och vara i läget **Godkänd** .

1. Du kan klicka på förhandsgranskningsikonen för att kontrollera att du har valt rätt e-postadress.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**Påminnelse**
   >
   >Var noga med att använda **skicka varningsinformation** i ditt e-postmeddelande.

1. Välj varningsmottagare. Du kan välja Säljare eller Kontoägare.

   ![](assets/four-2.png)

1. Du kan också lägga till andra e-postadresser som du vill ha (avgränsade med kommatecken eller semikolon).

   ![](assets/five.png)

   >[!TIP]
   >
   >I utlösande kampanjer kan du använda variabler i **till andra e-postmeddelanden** , till exempel `{{lead.Territory Owner}}` eller `{{my.Alert Recipient}}` , så länge som värdena är giltiga e-postadresser. Tokens in **To Other Emails** fungerar inte i en gruppkampanj.

Så ja! Nu vet du hur du använder flödessteget **Skicka avisering** .

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Skapa ett e-postmeddelande](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

