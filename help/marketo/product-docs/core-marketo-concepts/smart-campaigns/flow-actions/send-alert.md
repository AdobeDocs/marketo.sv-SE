---
unique-page-id: 1146958
description: Skicka avisering - Marketo Docs - produktdokumentation
title: Skicka avisering
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Skicka avisering {#send-alert}

Marketo Engage kan skicka ett e-postmeddelande med personinformation till vem som helst - säljaren, en partner eller någon annan. Använd flödessteget [!UICONTROL Send Alert].

![](assets/send-alert-1.png)

1. Sök efter och välj det e-postmeddelande som du vill skicka.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Din e-postavisering måste innehålla all rubrikinformation och vara i läget **[!UICONTROL Approved]**.

1. Du kan klicka på förhandsgranskningsikonen för att kontrollera att du har valt rätt e-postadress.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Använd token [!UICONTROL Send Alert Info] i ditt e-postmeddelande.

1. Välj varningsmottagare. Du kan välja [!UICONTROL Sales Owner] eller [!UICONTROL Account Owner].

   ![](assets/send-alert-4.png)

1. Du kan också lägga till andra e-postadresser som du vill ha (avgränsade med kommatecken eller semikolon).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >I utlösarkampanjer kan du använda variabler i **[!UICONTROL To Other Emails]**, till exempel `{{lead.Territory Owner}}` eller `{{my.Alert Recipient}}`, förutsatt att värdena är giltiga e-postadresser. Tokens i **[!UICONTROL To Other Emails]** fungerar inte i en gruppkampanj.

>[!MORELIKETHIS]
>
>[Skapa ett e-postmeddelande](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
