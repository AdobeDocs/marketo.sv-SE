---
description: Skicka ett Vibes SMS-meddelande - Marketo Docs - Produktdokumentation
title: Skicka ett Vibes SMS-meddelande
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Skicka ett Vibes SMS-meddelande {#send-a-vibes-sms-message}

Du har [skapade ditt Vibes SMS-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), nu är det dags att skicka det. Du kan skicka det via Gruppera eller Utlös kampanj.

>[!NOTE]
>
>När SMS-meddelanden skickas:
>
>* Marketo Engage dedupes per telefonnummer. Om flera personer har samma telefonnummer får bara en person meddelandet om de bara är medlemmar i en prenumerationslista för Adobe. Deduping görs på prenumerationslistenivån för Vibes, inte på programnivån för Marketo.
>* Marketo skickar inte till personer som är blocklist eller har avbrutit sin marknadsföring.

## Skicka ett batch-SMS {#send-a-batch-sms}

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. Hitta och välj önskad smart kampanj.

   ![](assets/send-a-vibes-sms-message-2.png)

1. Klicka på **Smart List** och definiera målgruppen för SMS:et. I det här exemplet skickar vi till alla i vår databas som har &quot;Adobe&quot; som företag.

   ![](assets/send-a-vibes-sms-message-3.png)

1. I **Flöde** tabb, dra över **Skicka SMS-meddelande**. Välj önskad SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >Väljaren Vibes List fungerar som ett ytterligare filter för den målgrupp som redan identifierats i Smart List så att den endast riktar sig till personer som tillhör den listan.

1. Klicka på **Schema** och schemalägga ditt SMS.

   ![](assets/send-a-vibes-sms-message-5.png)

## Skicka utlösar-SMS {#send-a-trigger-sms}

1. I Min Marketo klickar du på **Marknadsföringsaktiviteter**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. Hitta och välj önskad smart kampanj.

   ![](assets/send-a-vibes-sms-message-7.png)

1. Klicka på **Smart List** väljer du önskad utlösare och definierar dess värde. I detta exempel använder vi **Fyller i formulär**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. I **Flöde** tabb, dra över **Skicka SMS-meddelande**. Välj önskad SMS-meddelande och Vibes-lista i listrutorna.

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >Väljaren Vibes List fungerar som ett ytterligare filter för den målgrupp som redan identifierats i Smart List så att den endast riktar sig till personer som tillhör den listan.

1. Klicka på **Schema** tabbtangenten, sedan **Aktivera**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Skapa ett Vibes-meddelande](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Vibes Flow Steps

