---
description: Felsökningsguide för migrering av Adobe IMS-användare - Marketo Docs - Produktdokumentation
title: Felsökningsguide för Adobe IMS User Migration
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Felsökningsguide för Adobe IMS User Migration {#adobe-ims-user-migration-troubleshooting-guide}

Under IMS-användarmigreringen skapas en Adobe-användare för varje Marketo Engage-användare som migreras (om det inte redan finns med samma e-postadress). Ibland skapas den inte, vilket kan bero på användarens post i Active Directory eller problem med e-postadressen. När detta inträffar ser Marketo Engage-administratören orsaken i användarens migreringsstatusfält i självmigreringskonsolen.

## Felmeddelanden {#error-messages}

Börja med att bestämma om användaren behöver migreras eller inte, eftersom det påverkar vilka upplösningssteg som ska följas.

Använd delen &quot;På den här sidan&quot; till höger för att gå direkt till ett visst fel.

### Finns inte i katalogen {#not-in-directory}

**Rotorsak**: Användaren finns inte i Active Directory (AD). För alla organ med enkel inloggning som har AD-synkronisering aktiverad, är det endast tillåtet att skapa användare via identitetsleverantören (IdP). Användaren kunde därför inte läggas till via Admin Console under användarmigreringen.

**Lösning**:

_Om användaren inte behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

_Om användaren måste migreras_ - Användaren måste läggas till i Active Directory med rätt behörigheter av en systemadministratör. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

### Ogiltigt Gmail-tecken {#gmail-invalid-character}

**Rotorsak**: Enligt Adobe säkerhetsprincip tillåts inte tecknen `.` och `+` i en Gmail-e-postadress. Båda tecknen tillåts i e-postadresser som inte är Gmail.

**Lösning**:

_Om användaren inte behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

_Om användaren måste migreras_ - E-postadressen måste uppdateras i Marketo Engage för att uppfylla Adobe säkerhetsprincip och verifieras på nytt. Marketo-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

### Inaktiv användare {#inactive-user}

**Rotorsak**: AD Sync är aktiverat och användarens federerade konto finns men har inaktiv/inaktiverad status.

**Lösning**:

_Om användaren inte behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

_Om användaren måste migreras_ måste användarens status och korrekta behörigheter återställas. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

### Inte i domänen {#not-in-domain}

**Rotorsak**: Domänkontroll har aktiverats i Admin Console, men domänen för användarens e-postadress är inte en av de tillåtna domänerna.

**Lösning**:

_Om användaren inte behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

_Om användaren måste migreras_ - E-postadressen måste uppdateras i Marketo Engage för att den ska uppfylla principen för domäntvingande (DE). Alternativt kan systemadministratören antingen [flytta domänen](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} till en annan inaktiverad katalog för Domain Enforcement (DE) eller [skapa en ny katalog](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"} som inte omfattas av DE-principen. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

### Skapa fel {#create-failure}

**Rotorsak**: Det här felet kan orsakas av olika orsaker i serverdelen.

**Lösning**:

Skicka ett supportärende med relevant information om [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Type2e-användarfel {#type2e-user-failure}

**Rotorsak**: Det här felet kan orsakas av olika orsaker i serverdelen.

**Lösning**:

Skicka ett supportärende med relevant information om [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
