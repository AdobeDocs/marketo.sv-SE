---
unique-page-id: 1146958
description: Skicka avisering - Marketo Docs - produktdokumentation
title: Skicka avisering
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Skicka avisering {#send-alert}

## Översikt {#overview}

Marketo kan skicka ett e-postmeddelande med personinformation till vem som helst - säljaren, en partner eller någon annan. Använd &quot;[!UICONTROL Send Alert]&quot;.

![](assets/one-1.png)

## Användning {#usage}

1. Sök efter och välj det e-postmeddelande som du vill skicka.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Din e-postavisering måste innehålla all rubrikinformation och finnas i **[!UICONTROL Approved]** tillstånd.

1. Du kan klicka på förhandsgranskningsikonen för att kontrollera att du har valt rätt e-postadress.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Använd kommandot[!UICONTROL Send Alert Info]&quot; i din e-postadress.

1. Välj varningsmottagare. Du kan välja [!UICONTROL Sales Owner] eller [!UICONTROL Account Owner].

   ![](assets/four-2.png)

1. Du kan också lägga till andra e-postadresser som du vill ha (avgränsade med kommatecken eller semikolon).

   ![](assets/five.png)

   >[!TIP]
   >
   >I utlösande kampanjer kan du använda variabler i **[!UICONTROL To Other Emails]** som `{{lead.Territory Owner}}` eller `{{my.Alert Recipient}}` så länge som värdena är giltiga e-postadresser. Tokens in **[!UICONTROL To Other Emails]** fungerar inte i en gruppkampanj.

>[!MORELIKETHIS]
>
>[Skapa ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
