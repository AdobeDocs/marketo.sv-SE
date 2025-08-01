---
unique-page-id: 10100642
description: Skapa meddelandetext i appen - Marketo Docs - produktdokumentation
title: Skapa meddelandetext i appen
exl-id: 8fe5f004-dafb-4e03-9628-bd92fcb3fd44
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Skapa meddelandetext i appen {#create-in-app-message-text}

Klicka på textområdet om du vill arbeta med textformatet och innehållet.

>[!CAUTION]
>
>Vi rekommenderar att du inte använder känslolägesikoner i texten eftersom de inte stöds fullt ut just nu.

1. Klicka på huvudtexten om du vill redigera den infogade texten.

   ![](assets/image2016-5-6-9-3a56-3a56.png)

1. Välj textfärgen genom att klicka på den eller genom att ange de hexadecimala eller RGB-numeriska värdena i färgväljaren.

   ![](assets/image2016-5-6-9-3a59-3a1.png)

1. Klicka på pilarna för att välja en textstorlek.

   ![](assets/image2016-5-6-10-3a6-3a51.png)

   >[!CAUTION]
   >
   >För stor textstorlek kan medföra att innehållet flyttas förbi de maximala tre synliga textraderna.

1. Välj en valfri typstil för betoning: **Fet**, _Kursiv_ eller Understruken.

   ![](assets/image2016-5-6-10-3a15-3a32.png)

1. Välj textjustering: Vänster, Centrerad, Höger. Centrerad är standard.

   ![](assets/image2016-5-6-10-3a18-3a45.png)

   >[!NOTE]
   >
   >Det teckensnitt som återges i annonsen är standardteckensnittet för varje plattform: Helvetica för Apple och Roboto för Android

1. Markera rutan för att välja **[!UICONTROL Text Tap action]**.

   ![](assets/image2016-5-6-10-3a20-3a41.png)

1. Välj en tryckåtgärd för varje plattform: Apple eller Android.

   ![](assets/image2016-5-6-10-3a22-3a12.png)

   >[!NOTE]
   >
   >För tryckningsåtgärder kan du ange olika åtgärder för Apple- och Android-plattformar. Djuplänkar hanteras till exempel på olika sätt för Apple och Android. Om ditt meddelande bara ska visas på en plattform eller på en annan, kan du lämna den andra i standardinställningen eller välja [!UICONTROL None].

1. Klicka på stödtexten för att redigera den. Det fungerar på samma sätt som att redigera huvudtexten, men standardtextstorleken är mindre.

   ![](assets/image2016-5-6-10-3a26-3a27.png)

1. Klicka på ikonen Token för att lägga till en token för antingen huvudtexten eller stödtexten.

   ![](assets/image2016-5-6-10-3a29-3a2.png)

1. Välj en Min token i listrutan, lägg till ett standardvärde och klicka på **[!UICONTROL Insert]**.

   ![](assets/mytoken.png)

   >[!NOTE]
   >
   >Endast Mina token är tillgängliga som alternativ. Om inga Mina token har konfigurerats i programmet kommer listrutan [!UICONTROL Token] att vara tom.

   >[!TIP]
   >
   >Se till att du tar hänsyn till hur lång teckenlängd en variabel kan resultera i när den visas av din målgrupp. Lämna tillräckligt med utrymme för att ta hänsyn till potentiellt längre värden för att förhindra att de skärs av.

   Ändringar som du gör i token som används i ett godkänt meddelandeprogram i appen börjar inte gälla i meddelandet i appen förrän programmet pausas och sedan återupptas.

Du är guld. Därefter måste du [konfigurera meddelandeknappen i appen](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/set-up-the-in-app-message-button.md).

>[!MORELIKETHIS]
>
>* [Förstå meddelanden i appen](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md)
>* [Välj en layout för ditt meddelande i appen](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/choose-a-layout-for-your-in-app-message.md)
