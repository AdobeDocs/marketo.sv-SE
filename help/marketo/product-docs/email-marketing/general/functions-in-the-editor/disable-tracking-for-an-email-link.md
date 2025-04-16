---
unique-page-id: 1900579
description: Inaktivera spårning för en e-postlänk - Marketo Docs - produktdokumentation
title: Inaktivera spårning för en e-postlänk
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: ac2f8bf38b32344dd9414cf3611b69747e3587d4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Inaktivera spårning för en e-postlänk {#disable-tracking-for-an-email-link}

Ibland vill du inte aktivera **Marketo Tracking URL** för en länk i ett e-postmeddelande. Detta är användbart när målsidan inte stöder URL-parametrar och kan resultera i en bruten länk.

Om ett e-postmeddelande skickades för över 365 dagar sedan **och** ingen har klickat på någon av länkarna de senaste 180 dagarna, rensar Marketo Engage vägen till URL:en från vår databas, vilket gör att länken bryts. Så om du vill att länken ska vara permanent bör du inaktivera spårning.

1. Markera e-postmeddelandet och klicka på **Redigera utkast**.

   ![](assets/one-7.png)

1. Dubbelklicka på det redigerbara avsnitt som innehåller länken.

   ![](assets/two-6.png)

1. Klicka på länken i fråga och klicka sedan på knappen **Infoga/redigera länk** .

   ![](assets/three-6.png)

1. Avmarkera kryssrutan **Spåra länk** i popup-fönstret Redigera länk.

   ![](assets/four-4.png)

1. Du kommer att märka att rutan **Inkludera mkt_tok** försvinner. Klicka på **Använd**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Om du bara avmarkerar **Include mkt_tok** kan länken fortfarande spåras, men efter omdirigeringen kommer mål-URL:en inte att innehålla frågesträngsparametern mkt_tok. Den här parametern används av Marketo landningssidor och Munchkin för att säkerställa korrekt spårning av personaktiviteter (som när en person säger upp prenumerationen på ett e-postmeddelande). Du bör undvika att använda den här funktionen om du inte ser något konstigt beteende på webbplatsen på grund av att parametern finns.

1. Klicka på **Spara**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >Om du vill inaktivera klickspårning för en länk i en e-postmall, eller [textversion](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"} i ett e-postmeddelande, lägger du till `mktNoTrack` i *början* av strängen, inte i slutet, som i det här exemplet: `<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`. Annars kan länken försvinna. Om du behöver hjälp med att implementera ovanstående kod, konsultera din webbutvecklare.
