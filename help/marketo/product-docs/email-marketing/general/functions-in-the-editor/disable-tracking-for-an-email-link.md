---
unique-page-id: 1900579
description: Inaktivera spårning för en e-postlänk - Marketo-dokument - Produktdokumentation
title: Inaktivera spårning för en e-postlänk
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Inaktivera spårning för en e-postlänk {#disable-tracking-for-an-email-link}

Ibland vill du inte aktivera URL:en **Marketo Tracking** för en länk i ett e-postmeddelande. Detta är användbart när målsidan inte stöder URL-parametrar och kan resultera i en bruten länk.

1. Markera e-postmeddelandet och klicka på **Redigera** **Utkast**.

   ![](assets/one-7.png)

1. Dubbelklicka på det redigerbara avsnitt som innehåller länken.

   ![](assets/two-6.png)

1. Klicka på länken i fråga och klicka sedan på knappen **Infoga/redigera länk**.

   ![](assets/three-6.png)

1. Avmarkera kryssrutan **Spåra länk** i popup-fönstret Redigera länk.

   ![](assets/four-4.png)

1. Du kommer att märka att rutan **Inkludera mkt_tok** försvinner. Klicka på **Använd**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Om du bara avmarkerar **Include mkt_tok** kan länken fortfarande spåras, men efter omdirigeringen kommer mål-URL:en inte att innehålla frågesträngsparametern mkt_tok. Den här parametern används av Marketo Landing Pages och Munchkin för att säkerställa korrekt spårning av personaktiviteter (som när en person säger upp prenumerationen på ett e-postmeddelande). Du bör undvika att använda den här funktionen om du inte ser något konstigt beteende på webbplatsen på grund av att parametern finns.

1. Klicka på **Spara**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Vill du inaktivera klickspårning för en länk i ett e-postmeddelande **mall**? Använd det här formatet:
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Kontakta din webbutvecklare om du behöver hjälp med att implementera detta.

Snyggt! Du har nu inaktiverat spårning för en länk.
