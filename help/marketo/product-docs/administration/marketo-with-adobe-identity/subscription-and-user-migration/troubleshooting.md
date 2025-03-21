---
description: Felsökningsguide för migrering av Adobe IMS-användare - Marketo Docs - Produktdokumentation
title: Felsökningsguide för Adobe IMS User Migration
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 251f84b2dff6b7c0706c0f08fe8b51d8d4d897f0
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Felsökningsguide för Adobe IMS User Migration {#adobe-ims-user-migration-troubleshooting-guide}

Under IMS-användarmigreringen skapas en Adobe-användare för varje Marketo Engage-användare som migreras (om det inte redan finns med samma e-postadress). Ibland skapas den inte, vilket kan bero på användarens post i Active Directory eller problem med e-postadressen.

I den här artikeln listas alla felmeddelanden som du kan se i statusfältet i självmigreringskonsolen för användare som utför självmigrering.

>[!NOTE]
>
>Katalog-/domänrelaterade fel kan utlösas av en annan organisation/Admin Console där ett katalogförtroende har konfigurerats eller där domänen har tagits i anspråk.

## Felmeddelanden {#error-messages}

Börja med att bestämma om användaren behöver migreras eller inte, eftersom det påverkar vilka upplösningssteg som ska följas.

Använd delen &quot;På den här sidan&quot; till höger för att gå direkt till ett visst fel.

### Ogiltigt Gmail-tecken {#gmail-invalid-character}

**Rotorsak**: Enligt Adobe säkerhetsprincip tillåts inte tecknen `.` och `+` i en Gmail-e-postadress. Båda tecknen tillåts i e-postadresser som inte är Gmail.

**Lösning**:

_Om användaren måste migreras_ - E-postadressen måste uppdateras i Marketo Engage för att uppfylla Adobe säkerhetsprincip och verifieras igen. Marketo-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Användaren finns inte i katalogen {#user-not-in-directory}

**Rotorsak**: Användaren finns inte i Active Directory (AD). För alla organ med enkel inloggning som har AD-synkronisering aktiverad, är det endast tillåtet att skapa användare via identitetsleverantören (IdP). Användaren kunde därför inte läggas till via Admin Console under användarmigreringen.

**Lösning**:

_Om användaren måste migreras_ - Användaren måste läggas till i Active Directory med rätt behörigheter av en systemadministratör. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Inaktiv användare {#inactive-user}

**Rotorsak**: AD Sync är aktiverat och användarens federerade konto finns men har inaktiv/inaktiverad status.

**Lösning**:

_Om användaren måste migreras_ - Användarens status och korrekta behörigheter måste återställas av en systemadministratör. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Ogiltig domän {#invalid-domain}

**Rotorsak**: Domänkontroll har aktiverats i Admin Console. Domänen för användarens e-postadress är dock inte en av de tillåtna domänerna eller så har domänen tagits i anspråk i en annan organisation/Admin Console.

**Lösning**:

_Om användaren måste migreras_ (och domänanvändningen är aktiverad i migreringsorganisationen) måste e-postadressen uppdateras i Marketo Engage för att uppfylla principen för domäntvingande (DE). Alternativt kan systemadministratören antingen [flytta domänen](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} till en annan inaktiverad katalog för Domain Enforcement (DE) eller [skapa en ny katalog](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"} som inte omfattas av DE-principen. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren måste migreras_ (och domänanvändningen är aktiverad i en annan organisation) måste en systemadministratör för organisationen där domänen har tagits i anspråk lägga till användarens e-postadress i undantagslistan. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Det gick inte att skapa användare {#user-creation-failed}

[Se nedan](#failed)

### Type2E-fel {#type2e-failure}

[Se nedan](#failed)

### Marketo Entitlement Failed {#marketo-entitlement-failed}

[Se nedan](#failed)

### Pendo-migrering misslyckades {#pendo-migration-failed}

[Se nedan](#failed)

### Migreringen av användardata misslyckades {#user-data-migration-failed}

[Se nedan](#failed)

### Produktdatasynkronisering misslyckades {#product-data-sync-failed}

[Se nedan](#failed)

### Adobe Entitlement Failed {#adobe-entitlement-failed}

[Se nedan](#failed)

### Utloggning av användare misslyckades {#user-sign-out-failed}

[Se nedan](#failed)

### Adobe ID kunde inte skapas {#adobe-id-creation-failed}

[Se nedan](#failed)

### Misslyckades {#failed}

**Rotorsak**: Dessa fel kan orsakas av olika orsaker i serverdelen.

**Lösning**:

Skicka ett supportärende med relevant information om [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
