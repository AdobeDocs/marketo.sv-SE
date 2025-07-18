---
unique-page-id: 4720758
description: Versionsinformation -januari 2015 - Marketo Docs - produktdokumentation
title: Versionsinformation - januari 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Versionsinformation: januari 2015 {#release-notes-january}

Följande funktioner ingår i januari 2015-versionen. Kontrollera om det finns funktioner i Marketo Edition. Efter releasen måste du komma tillbaka för att hitta länkar till detaljerade artiklar för varje funktion!

## Automatiseringsuppdateringar {#marketing-automation-updates}

**Mobilanpassade landningssidor**

Du kan nu [skapa mobilvyer för landningssidor](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) inifrån landningssidans redigerare. Leverera ert budskap effektivt oavsett enhet och öka engagemanget genom att skräddarsy ert innehåll för enkel användning oavsett var ni är. Den här funktionen kommer gradvis att lanseras under veckan efter releasen.

[-landande sidgenomgång - ](https://youtu.be/aPQHlG2X6c0)

**Nya REST API-anrop**

Tre nya anrop till lead- och aktivitetsREST API:

* Ta bort lead
* Hämta leads per program-ID
* Hämta borttagna leads

Det finns också ett nytt alternativ för Synkronisera lead, som gör att leadet ändras asynkront för ett snabbare API-anrop. Fullständig information finns tillgänglig efter lanseringen på [https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/home)

**Stöd för anpassade objekt för e-postskript**

Nu kan du komma åt anpassade objekt som är kopplade till kontoobjektet inifrån e-postskript!

## Personalization i realtid {#real-time-personalization}

**Anpassad marknadsföring för Google och[!DNL Facebook]**

Marknadsföring visar annonser för personer som har besökt din webbplats. Nu kan du personalisera dina återmarknadsföringskampanjer på [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) och [[!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) med data från Personalization i realtid. Marknadsför till målgrupper från olika branscher, namngivna kontolistor, företagsstorlekar eller data från kända leads.

[Modulen Namngiven kontolista](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Förbättringar av modulen Namngivna konton förbättrar matchningsfrekvenserna och valideringarna för användarna. Bland tilläggen finns:

* Matchande organisationer från din lista över namngivna konton med leadens e-postadress (även för kunder som bara använder RTP)
* Stöd för upp till 100 000 poster per konto
* CSV-filmall för visning och hämtning

![](assets/image2015-1-14-11-3a12-3a16.png)

**Uppdaterade alternativ för RTP-tagg**

Alternativen för RTP-tagg under Kontoinställningar har uppdaterats till att omfatta:

1. CDN och asynkron (rekommenderas)
1. CDN och synkron (hög hastighet)
1. Asynkron tagg utan CDN
1. Synkron tagg utan CDN

För bästa prestanda bör du placera taggen högst upp i sidhuvudet på webbsidan efter `<head>`. Alla taggar tillåter användning av [RTP API](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Mer information om hur du distribuerar RTP-taggen finns [här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
