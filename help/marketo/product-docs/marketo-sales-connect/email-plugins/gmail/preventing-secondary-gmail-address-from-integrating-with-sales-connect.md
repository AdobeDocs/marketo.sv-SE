---
unique-page-id: 14352546
description: Förhindra att en sekundär Gmail-adress integreras med Sales Connect - Marketo Docs - produktdokumentation
title: Förhindrar att den sekundära Gmail-adressen integreras med Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Förhindrar att den sekundära Gmail-adressen integreras med Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Bruten Gmail-integrering (varför är min egen Gmail-e-post?) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Den vanligaste orsaken till en trasig Gmail-anslutning är en oavsiktlig integrering med en användares personliga konto. Det här kan hända när en användare klickar på &quot;Anslut&quot; eller försöker skicka ett e-postmeddelande från sitt personliga konto. Det här kan vara mycket frestande eftersom alternativet kommer att finnas när du öppnar ditt Gmail-konto i samma instans av Chrome som ditt e-postmeddelande.

## Varför försöker Sales Connect ens integrera med min egen Gmail? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect integreras med Gmail via ett tillägg som installeras i Chrome webbläsare. När tillägget känner av en instans av Gmail som är öppen finns det ett alternativ för att integrera med den. För att förhindra integrering med ditt personliga Gmail-konto rekommenderar vi en av tre saker...

Logga in som en annan Chrome-användare (rekommenderas)

Klicka på [den här länken](https://support.google.com/chrome/answer/2364824?hl=en) om du vill läsa om hur du skapar en annan Chrome-profil.

**Pros**: Om du loggar in som en annan användare öppnas en ny instans av Chrome. Den här instansen är ett helt nytt fönster för Chrome, och inga av dina gamla tillägg kommer att finnas i den här. Den sparar också cookies så att du inte behöver logga in på din Gmail varje gång.

**Kon**: Två fönster måste vara öppna i Chrome.

Använd en annan webbläsare

**Pros:** Om du använder en annan webbläsare (IE eller Firefox) som inte har tillägget installerat kommer detta inte att fungera.

**Kon**: Det kan vara irriterande att använda flera webbläsare.

Använda ett inkognito-fönster

**Pros:** Ett inkognito-fönster är som att öppna en naken version av Chrome. Det innebär att inga av dina tillägg kommer att vara installerade, och Sales Connect kommer inte att finnas där för att ansluta.

**Kon**: Du måste logga in på Gmail varje gång du startar din dag och sedan igen om du stänger fönstret av misstag.
