---
unique-page-id: 4720758
description: Versionsinformation -januari 2015 - Marketo Docs - Produktdokumentation
title: Versionsinformation - januari 2015
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Versionsinformation: Januari 2015 {#release-notes-january}

Följande funktioner ingår i januari 2015-versionen. Kontrollera om din Marketo Edition innehåller funktioner. Efter releasen måste du komma tillbaka för att hitta länkar till detaljerade artiklar för varje funktion!

## Automatiseringsuppdateringar {#marketing-automation-updates}

**Nya foton av Rick DeCosta!**

Rick är Marketo-kund hos SmartBear och har [en fantastisk samling foton](https://www.flickr.com/photos/rickdecosta). Kolla in dem!

## Mobilanpassade landningssidor {#mobile-friendly-landing-pages}

Du kan nu [skapa mobilvyer för landningssidor](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) inifrån startsidans redigerare. Leverera ert budskap effektivt oavsett enhet och öka engagemanget genom att skräddarsy ert innehåll för enkel användning oavsett var ni är. Den här funktionen lanseras gradvis under veckan efter releasen.

`<iframe width="420" height="315" src="//www.youtube-nocookie.com/embed/aPQHlG2X6c0" frameborder="0" allowfullscreen></iframe>`

**Nya ReST API-anrop**

Tre nya anrop till API:t Lead &amp; Activity ReST:

* Ta bort lead
* Hämta leads per program-ID
* Hämta borttagna leads

Det finns också ett nytt alternativ för Synkronisera lead, som gör att leadet ändras asynkront för ett snabbare API-anrop. Fullständig information kommer att finnas tillgänglig efter releasen på [developers.marketo.com](http://developers.marketo.com)

**Stöd för anpassade objekt för e-postskript**

Nu kan du komma åt anpassade objekt som är kopplade till kontoobjektet inifrån e-postskript!

## Realtidspersonalisering {#real-time-personalization}

**Personaliserad Remarketing för Google och Facebook**

Marknadsföring visar annonser för personer som har besökt din webbplats. Nu kan du personalisera dina återmarknadsföringskampanjer på [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) och [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) med data från Real-Time Personalization. Marknadsför till målgrupper från olika branscher, namngivna kontolistor, företagsstorlekar eller data från kända leads.

[Modulen Namngiven kontolista](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Förbättringar av modulen Namngivna konton förbättrar matchningsfrekvenserna och valideringarna för användarna. Bland tilläggen finns:

* Matchande organisationer från din lista över namngivna konton med leadens e-postadress (även för RTP-kunder)
* Stöd för upp till 100 000 poster per konto
* CSV-filmall för visning och hämtning

![](assets/image2015-1-14-11-3a12-3a16.png)

Uppdaterade alternativ för RTP-tagg

[RTP-](http://docs.marketo.com/display/docs/rtp+tag+implementation) taggalternativen under Kontoinställningar har uppdaterats till att omfatta:

1. CDN och asynkron (rekommenderad tagg)
1. CDN och synkron (hög hastighet)
1. Asynkron tagg utan CDN
1. Synkron tagg utan CDN

För bästa prestanda bör du placera taggen högst upp i sidhuvudet på webbsidan efter `<head>`. Alla taggar tillåter användning av [RTP API](http://developers.marketo.com/documentation/websites/rtp-js-api/). Mer information om hur du distribuerar RTP-taggen finns i [här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
