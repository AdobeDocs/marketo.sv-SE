---
description: Översikt över e-postspårning - Marketo Docs - produktdokumentation
title: E-postspårning - översikt
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# E-postspårning - översikt {#email-tracking-overview}

## Hur Svara Tracking fungerar {#how-reply-tracking-works}

Spåra svar görs genom att titta på ett meddelande-ID som finns i alla e-postmeddelanden som du skickar. Alla e-postmeddelanden innehåller ett unikt meddelande-ID som gör att vi kan använda någon av de bästa svarsuppföljningarna.

>[!PREREQUISITES]
>
>Anslutning till e-postserver: [!DNL Sales Connect] måste vara ansluten till din inkorg så att vi vet när ett nytt svar har kommit. Du måste ha ditt [!DNL Sales Connect]-konto anslutet till Gmail. Om du använder Outlook måste vi integrera med din Exchange-server.

Om [!DNL Sales Connect] inte kan spåra den potentiella kundens svar på ditt e-postmeddelande kan den inte stoppa en kampanj baserat på svarsidentifiering eller logga svaret på Salesforce. Vad menar vi med e-postadresser som kan svara?

Det innebär att om du skickar e-post till <flynn@flynnsarcade.com> och han svarar med <kevinf@flynnsarcade.com> kan vi spåra svaret. Om du dessutom skickar e-post till <flynn@flynnsarcade.com> och CC <alan@encom.com> och Alan skriver tillbaka dig, upptäcks även svaret och kampanjen avslutas.

## Spåra e-postbilagor {#how-to-track-your-email-attachments}

[!DNL Sales Connect] erbjuder spårning för dina bifogade filer (.doc, .ppt, .pdf) så att du kan se när de har öppnats/hämtats och vilka sidor mottagaren tittar igenom. Du kan använda funktionen för spårbara bilagor från både [webbprogrammet](https://toutapp.com/login) och Gmail (eller Google-appar).

>[!NOTE]
>
>Spårning av bilagor är bara tillgängligt för våra teamplaner (med början från vårt g3startup-plan).

**Så här skickar du din första spårbara bilaga**

1. Skapa ett e-postmeddelande eller redigera en mall och klicka sedan på knappen **[!UICONTROL Content]**.

1. Ladda upp den bifogade filen och skicka den. Vi stöder PDF-filer, [!DNL Word] dokument och [!DNL Powerpoint] presentationer.

1. Välj **[!UICONTROL Add to Email]**.

1. Klicka på **[!UICONTROL Send]** och starta din Live-feed. Mottagarna visas när de öppnar och bläddrar igenom de bifogade filerna.

>[!TIP]
>
>Om du inte vill spåra en bifogad fil klickar du bara på Bifoga filer så spåras inte den bifogade filen.

## Hur spårning fungerar {#how-view-tracking-works}

Vi spårar öppnandet av e-postmeddelanden genom att placera en osynlig bild inuti de e-postmeddelanden du skickar.

Om någon svarar på ditt e-postmeddelande men [!DNL Sales Connect] säger att det inte visades, är det troligt att mottagaren inte aktiverade bilder i sin e-postklient (d.v.s. klicka på meddelandet&quot;klicka här för att hämta bilder&quot; i e-postmeddelandet).

Några tips för att få bättre spårningsstatistik i e-postmeddelanden:

* Inkludera en bild i dina e-postmeddelanden (som en logotyp) så att mottagaren uppmuntras att aktivera bilder för att se ditt meddelande.
* Ta med en länk som call to action i e-postmeddelandet.

## Testa e-postmeddelandet visas inte som det visats {#test-email-not-showed-as-viewed}

Även om du har skickat ditt meddelande till en annan e-postadress loggar vi inte om du visar e-postmeddelanden som du har skickat till dig själv i Live Feed. Vår spårning är enhetsbaserad. Så länge du använder en dator som du har loggat in på [!DNL Sales Connect] med filtrerar vi bort aktiviteten.

Orsaken? [!DNL Sales Connect] är smart, och våra aktiva användare förlåter oss aldrig om deras egen information visas i Live Feed Activity varje gång de tittar på ett e-postmeddelande de skickar.
