---
description: Översikt över e-postspårning - Marketo Docs - produktdokumentation
title: Översikt över e-postspårning
hide: true
hidefromtoc: true
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '510'
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

Sales Connect har funktioner för att spåra dina bilagor (.doc, .ppt, .pdf) så att du kan se när de har öppnats/laddats ned och vilka sidor mottagaren tittar igenom. Vi låter dig använda funktionen för spårbara bilagor från båda [webbprogram](https://toutapp.com/login) och Gmail (eller Google Apps).

>[!NOTE]
>
>Spårning av bilagor är bara tillgängligt för våra teamplaner (med början från vårt g3startup-plan).

**Skicka din första spårbara bilaga**

1. Skapa ett e-postmeddelande eller redigera en mall och klicka sedan på **Innehåll** -knappen.

1. Ladda upp den bifogade filen och skicka den. Vi stöder PDF, Word-dokument och PowerPoint-presentationer.

1. Välj **Lägg till i e-post**.

1. Klicka **Skicka** och tända din livefeed. Mottagarna visas när de öppnar och bläddrar igenom de bifogade filerna.

>[!TIP]
>
>Om du inte vill spåra en bifogad fil klickar du bara på Bifoga filer så spåras inte den bifogade filen.

## Hur spårning fungerar {#how-view-tracking-works}

Vi håller reda på e-postöppningar genom att placera en osynlig bild inuti de e-postmeddelanden du skickar.

Om någon svarar på ditt e-postmeddelande men Sales Connect säger att det inte visades, är det troligt att mottagaren inte aktiverade bilder i sin e-postklient (d.v.s. klicka på meddelandet&quot;klicka här för att hämta bilder&quot; i e-postmeddelandet).

Några tips för att få bättre spårningsstatistik i e-postmeddelanden:

* Inkludera en bild i dina e-postmeddelanden (som en logotyp) så att mottagaren uppmuntras att aktivera bilder för att se ditt meddelande.
* Inkludera en länk som ett meddelande om åtgärd i e-postmeddelandet.

## Testa e-postmeddelandet visas inte som det visats {#test-email-not-showed-as-viewed}

Även om du har skickat ditt meddelande till en annan e-postadress loggar vi inte om du visar e-postmeddelanden som du har skickat till dig själv i Live Feed. Vår spårning är enhetsbaserad; Så länge du använder en dator som du har loggat in på Sales Connect med, filtrerar vi bort aktiviteten.

Orsaken? Sales Connect är smart och våra aktiva användare förlåter oss aldrig om deras egen information visas i Live Feed Activity varje gång de tittar på ett e-postmeddelande de skickar.
