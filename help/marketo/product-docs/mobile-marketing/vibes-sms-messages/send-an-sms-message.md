---
description: Skicka ett SMS-meddelande - Marketo Docs - produktdokumentation
title: Skicka ett SMS
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Skicka ett SMS {#send-a-vibes-sms-message}

Du har [skapade SMS-meddelandet](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, nu är det dags att skicka det. Du kan skicka det via Gruppera eller Utlös kampanj.

>[!NOTE]
>
>När SMS-meddelanden skickas:
>
>* Marketo Engage dedupes per telefonnummer. Om flera personer har samma telefonnummer får bara en person meddelandet om de bara är medlemmar i en prenumerationslista för Adobe. Deduping görs på prenumerationslistenivån för Vibes, inte på programnivån för Marketo.
>* Marketo skickar inte till personer som är blocklist eller har avbrutit sin marknadsföring.
>* Ett SMS-meddelande kommer inte att skickas till någon som avbeställt prenumerationen om de inte finns med i listan Vibes Mobile Database.

## Skicka ett batch-SMS {#send-a-batch-sms}

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/send-an-sms-message-1.png)

1. Hitta och välj önskad smart kampanj.

   ![](assets/send-an-sms-message-2.png)

1. Klicka på **Smart List** och definiera målgruppen för SMS:et. I det här exemplet skickar vi till alla i vår databas som har &quot;Adobe&quot; som företag.

   ![](assets/send-an-sms-message-3.png)

1. I **Flöde** tabb, dra över **Skicka SMS-meddelande**. Välj önskad SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Väljaren Vibes List fungerar som ett ytterligare filter för den målgrupp som redan identifierats i Smart List så att den endast riktar sig till personer som tillhör den listan.

1. Klicka på **Schema** och schemalägga ditt SMS.

   ![](assets/send-an-sms-message-5.png)

## Skicka utlösar-SMS {#send-a-trigger-sms}

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/send-an-sms-message-6.png)

1. Hitta och välj önskad smart kampanj.

   ![](assets/send-an-sms-message-7.png)

1. Klicka på **Smart List** väljer du önskad utlösare och definierar dess värde. I detta exempel använder vi **Fyller i formulär**.

   ![](assets/send-an-sms-message-8.png)

1. I **Flöde** tabb, dra över **Skicka SMS-meddelande**. Välj önskad SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Väljaren Vibes List fungerar som ett ytterligare filter för den målgrupp som redan identifierats i Smart List så att den endast riktar sig till personer som tillhör den listan.

1. Klicka på **Schema** tabbtangenten, sedan **Aktivera**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Skapa ett Vibes-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}
>* [Använda SMS-alternativ i en smart kampanj](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
