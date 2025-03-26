---
unique-page-id: 11382535
description: Använda URL:er i Mina token - Marketo Docs - Produktdokumentation
title: Använda URL:er i Mina token
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 165dca2573f340ede147866c3a30707bbfb6857c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Använda URL:er i Mina token {#using-urls-in-my-tokens}

Följ stegen nedan för att använda Mina token för att infoga URL:er i dina e-postmeddelanden.

1. Välj ditt program och klicka på **Mina token**.

   ![](assets/one-4.png)

1. Välj **Text** Min token, dra och släpp den på arbetsytan.

   ![](assets/two-4.png)

1. Ge token ett unikt namn, ange en URL (utan mappen https://) och klicka på **Spara**.

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**Använder http/https..**
   >
   >* Om du vill vara säker på att klick spåras i ditt e-postmeddelande anger du **inte** https:// _inuti_ tokenvärdet. Använd den utanför token, vilket visas i steg 7.
   >
   >* Vi rekommenderar att du inte utelämnar http/https. Om du gör det kan det leda till att [webbversionen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} av ditt e-postmeddelande återges felaktigt.

1. Välj e-postadressen i programmet.

   ![](assets/four-3.png)

1. Klicka på **Redigera utkast**.

   ![](assets/five-3.png)

1. Dubbelklicka i textområdet som du vill redigera.

   ![](assets/six-1.png)

1. Skriv `https://` var som helst i e-postmeddelandet (utan att lämna ett blanksteg efter) och klicka på ikonen Infoga token.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Du kan naturligtvis också ange `http://` om din webbplats inte använder https.

1. Leta reda på din Min token, markera den och klicka på **Infoga**.

   ![](assets/eight.png)

1. Markera https:// och token och tryck sedan på Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac) för att klippa ut texten.

   ![](assets/nine.png)

1. Markera den text som du vill att länken ska visa och klicka på ikonen Infoga/redigera länk.

   ![](assets/ten.png)

1. Tryck på Ctrl/Cmd+V för att klistra in innehållet i rutan **URL** och klicka på **Infoga**.

   ![](assets/eleven.png)

1. Klicka på **Spara**.

   ![](assets/twelve.png)

   Och du är klar! URL:en fylls i efter att du har skickat och tack vare att du placerar https:// framför token skapas en spårbar länk.
