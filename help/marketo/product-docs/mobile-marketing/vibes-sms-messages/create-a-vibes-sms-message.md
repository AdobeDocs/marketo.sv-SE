---
unique-page-id: 11378869
description: Skapa ett Vibes SMS-meddelande - Marketo Docs - Produktdokumentation
title: Skapa ett Vibes SMS-meddelande
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Skapa ett Vibes SMS-meddelande {#create-a-vibes-sms-message}

Så här skapar du ett Vibes SMS-meddelande.

>[!AVAILABILITY]
>
>Den här funktionen är tillgänglig som tillägg för ditt Adobe Marketo Engage-konto. För att den ska kunna tillhandahållas på rätt sätt måste den köpas via Adobe. Kontakta kontoteamet (din kontoansvarige) för mer information.

>[!NOTE]
>
>SMS-textmeddelanden är inte HIPAA-kompatibla.

1. Gå till **Marknadsföringsaktiviteter** och högerklicka.

   ![](assets/mobile-right-click-hand.jpg)

1. Klicka **Ny lokal resurs**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >Du kan även klicka på **Nytt** nedrullningsbar meny.

1. Klicka **SMS-meddelande**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. Ange ett namn och en valfri beskrivning för det nya SMS-meddelandet och klicka på **Skapa**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. Klicka **Redigera utkast**.

   ![](assets/edit-draft-hand.jpg)

1. Klicka i den blå bubblan i meddelanderedigeraren och börja skriva text.

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >USA och Kanada har olika gränser, med 160 respektive 130 tecken. Om du överskrider teckengränserna kan meddelandet delas upp. Vi visar när du överskrider gränsen för Kanada, men redigeraren är optimerad för USA och delar upp meddelandet baserat på USA:s gräns.

1. Klicka **Token** på Infoga-menyn för att lägga till en token i meddelandet.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >Om du lägger till en variabel kan meddelandet överskrida teckengränsen. Meddelandet delas sedan upp, vilket medför ytterligare kostnader.

1. Klicka **Länk** på Infoga-menyn för att lägga till en länk till meddelandet.

   ![](assets/full-message-link-hand.jpg)

1. Välj en länktyp. Marketo landningssida är standard. Om du går med på det måste du välja landningssidan i listrutan och klicka på **Infoga**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >De två spårningslänkarna är markerade som standard.

1. Om du vill använda en extern URL i stället klickar du på **Extern URL** och ange URL-adressen i URL-fältet. Klicka **Infoga**.

   ![](assets/insert-link-url-hands.jpg)

1. Länken visas i meddelandet.

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo visar en länkförhandsgranskning av domänen för varumärkesspårning. Om du avmarkerar kryssrutan för länken mkt_tok ändras länken. Avmarkera kryssrutan Spåra länk också så förkortas URL-adressen till dess grundläggande längd (till exempel www.mygooglepage.com).

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >Teckenantalet återspeglar endast tecknen i det lägsta meddelandet.

Om du infogar mer än USA:s gräns bryts meddelandet ned i avsnitt. Det finns en absolut gräns på 900 tecken. När gränsen har nåtts trunkeras meddelandet automatiskt när det skickas till målgruppen.
