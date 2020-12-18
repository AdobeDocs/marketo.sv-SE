---
unique-page-id: 10617431
description: Ange er målgrupp för meddelanden i appen - Marketo Docs - Produktdokumentation
title: Ange målgrupp för meddelanden i appen
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Ange målgrupp för meddelanden i appen {#set-your-in-app-message-audience}

Det första steget är att bestämma vem som ska få ditt meddelande i appen. Du måste konfigurera din smarta lista.

1. Klicka på **Redigera smart lista**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. I den smarta listan fylls utlösaren med aktivitet i mobilappar i automatiskt. Klicka på listrutan och välj programmet som du vill placera meddelandet i.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >Flera värden för fältet Mobilapp stöds för närvarande inte för meddelandeprogram i appen.

1. **Programöppning är** standardinställningen för Åtgärd, men du kan välja alla anpassade händelser som du redan har konfigurerat.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >Standardutlösaren (App Open) och alla anpassade utlösare som läggs till i koden av din utvecklare visas automatiskt i åtgärdsväljaren. Om en anpassad händelse saknas bör du kontrollera med utvecklaren att de har lagt till anpassade händelser i appen. Tänk på att det kan ta lite tid att slutföra den anpassade händelsekodningen och godkännandeprocessen. Mer information finns i [den här artikeln](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md).

1. Begränsningar är tillgängliga för utlösaren **Har aktivitet för mobilapp** om du behöver dem.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Du kan lägga till filter i din smarta lista för att begränsa vem som får ett meddelande i appen. I det här exemplet kommer endast personer som skaffats den 9 juni 2016 att skickas med meddelandet i appen med hjälp av filtret **Anskaffningsdatum**.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Återgå till Kontrollpanelen för meddelanden i programmet. Ange visningsgränsen i listrutan.

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >Standardvisningsgränsen är **En gång per session**. Om du vill att meddelandet ska sluta visas när mottagaren har svarat väljer du **Varje gång tills användaren knackar på**. Om den ska visas varje gång, oavsett vad mottagaren gör, väljer du **Varje gång**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

Snyggt jobbat! Ni har er målgrupp. Du har fått den blå och gröna bockmarkeringen.

Det är dags att [välja meddelandet i appen](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)!
