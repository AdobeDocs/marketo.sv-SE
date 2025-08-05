---
unique-page-id: 14352482
description: Hur Spåra svar fungerar - Marketo Docs - Produktdokumentation
title: Hur Svara Tracking fungerar
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---

# Hur Svara Tracking fungerar {#how-reply-tracking-works}

Spåra svar görs genom att titta på ett meddelande-ID som finns i varje e-postmeddelande som du skickar. Alla e-postmeddelanden innehåller ett unikt meddelande-ID som gör att vi kan använda någon av de bästa svarsuppföljningarna.

>[!PREREQUISITES]
>
>**Anslutning till e-postserver:** [!DNL Sales Connect] måste vara ansluten till din inkorg så att vi vet när ett nytt svar har kommit. Du måste ha ditt [!DNL Sales Connect]-konto [anslutet till Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Om du använder [!DNL Outlook] måste vi integrera med din [Exchange-server](https://toutapp.com/next#settings/exchange_settings).

Om [!DNL Sales Connect] inte kan spåra den potentiella kundens svar på ditt e-postmeddelande kan den inte stoppa en kampanj baserat på svarsidentifiering eller logg som svarar på [!DNL Salesforce].  Vad menar vi med e-postadresser som kan svara?

Det innebär att om du skickar e-post till <flynn@flynnsarcade.com> och han svarar med <kevinf@flynnsarcade.com> kan vi spåra svaret. Om du dessutom skickar e-post till <flynn@flynnsarcade.com> och CC <alan@encom.com> och Alan skriver tillbaka dig, upptäcks även svaret och kampanjen avslutas.
