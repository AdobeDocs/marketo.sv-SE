---
unique-page-id: 14352482
description: Hur Spåra svar fungerar - Marketo Docs - Produktdokumentation
title: Hur Svara Tracking fungerar
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Spåra svar fungerar {#how-reply-tracking-works}

Spåra svar görs genom att titta på ett meddelande-ID som finns i varje e-postmeddelande som du skickar. Alla e-postmeddelanden innehåller ett unikt meddelande-ID som gör att vi kan använda någon av de bästa svarsuppföljningarna.

>[!PREREQUISITES]
>
>**Anslutning till e-postserver:** Sales Connect måste vara anslutet till din inkorg så att vi vet när ett nytt svar har kommit. Du måste ha ditt Sales Connect-konto [anslutet till Gmail](http://docs.marketo.com/x/kYMOAQ). Om du använder Outlook måste vi integrera med din [Exchange-server](http://toutapp.com/next#settings/exchange_settings).

Om Sales Connect inte kan spåra den potentiella kundens svar på ditt e-postmeddelande kan den inte stoppa en kampanj baserat på svarsidentifiering eller loggning som svarar till Salesforce.  Vad menar vi med e-postadresser som kan svara?

Det innebär att om du skickar [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) och han/hon svarar med [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), kan vi spåra svaret. Om du dessutom skickar ett e-postmeddelande till [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) och CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153) och Alan skriver tillbaka dig, identifierar det svaret och avslutar kampanjen.
