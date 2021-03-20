---
unique-page-id: 14352482
description: Hur Spåra svar fungerar - Marketo Docs - Produktdokumentation
title: Hur Svara Tracking fungerar
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Spåra svar fungerar {#how-reply-tracking-works}

Spåra svar görs genom att titta på ett meddelande-ID som finns i varje e-postmeddelande som du skickar. Alla e-postmeddelanden innehåller ett unikt meddelande-ID som gör att vi kan använda någon av de bästa svarsuppföljningarna.

>[!PREREQUISITES]
>
>**Anslutning till e-postserver:** Sales Connect måste vara anslutet till din inkorg så att vi vet när ett nytt svar har kommit. Du måste ha ditt Sales Connect-konto [anslutet till Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Om du använder Outlook måste vi integrera med din [Exchange-server](https://toutapp.com/next#settings/exchange_settings).

Om Sales Connect inte kan spåra den potentiella kundens svar på ditt e-postmeddelande kan den inte stoppa en kampanj baserat på svarsidentifiering eller loggning som svarar till Salesforce.  Vad menar vi med e-postadresser som kan svara?

Det innebär att om du skickar e-post till flynn@flynnsarcade.com och han svarar med kevinf@flynnsarcade.com, kan vi spåra svaret. Om du dessutom skickar e-post till flynn@flynnsarcade.com och CC alan@encom.com, och Alan skriver tillbaka dig, kommer den också att upptäcka svaret och avsluta kampanjen.
