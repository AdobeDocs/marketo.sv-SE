---
description: Översikt över e-postspårning - Marketo Docs - produktdokumentation
title: Översikt över e-postspårning
hide: true
hidefromtoc: true
source-git-commit: d8f7d7ddf804847e20bf978bf2fc74694b719009
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Översikt över e-postspårning {#email-tracking-overview}

## Hur Svara Tracking fungerar {#how-reply-tracking-works}

Spåra svar görs genom att titta på ett meddelande-ID som finns i alla e-postmeddelanden som du skickar. Alla e-postmeddelanden innehåller ett unikt meddelande-ID som gör att vi kan använda någon av de bästa svarsuppföljningarna.

>[!PREREQUISITES]
>
>Anslutning till e-postserver: Sales Connect måste vara ansluten till din inkorg så att vi vet när ett nytt svar har kommit. Du måste ha ditt Sales Connect-konto kopplat till Gmail. Om du använder Outlook måste vi integrera med din Exchange-server.

Om Sales Connect inte kan spåra den potentiella kundens svar på ditt e-postmeddelande kan den inte stoppa en kampanj baserat på svarsidentifiering eller logg som svarar till Salesforce. Vad menar vi med e-postadresser som kan svara?

Det innebär att om du skickar e-post till flynn@flynnsarcade.com och han/hon svarar med kevinf@flynnsarcade.com kan vi spåra svaret. Om du dessutom skickar e-post till flynn@flynnsarcade.com och CC alan@encom.com, och Alan skriver tillbaka dig, kommer den också att upptäcka svaret och avsluta kampanjen.

## Spåra e-postbilagor {#how-to-track-your-email-attachments}

text

## Hur spårning fungerar {#how-view-tracking-works}

text

## Testa e-postmeddelandet visas inte som det visats {#test-email-not-showed-as-viewed}

text
