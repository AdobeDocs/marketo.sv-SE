---
description: Felsökningsguide för migrering av Adobe IMS-användare - Marketo Docs - Produktdokumentation
title: Felsökningsguide för Adobe IMS User Migration
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 5d6269ca9b229311ed4260d5340aad6cd1ea0067
workflow-type: tm+mt
source-wordcount: '1017'
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

_Om användaren **inte**&#x200B;behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Användaren finns inte i katalogen {#user-not-in-directory}

**Rotorsak**: Användaren finns inte i Active Directory (AD). För alla organ med enkel inloggning som har AD-synkronisering aktiverad, är det endast tillåtet att skapa användare via identitetsleverantören (IdP). Användaren kunde därför inte läggas till via Admin Console under användarmigreringen.

**Lösning**:

_Om användaren måste migreras_ - Användaren måste läggas till i Active Directory med rätt behörigheter av en systemadministratör. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**&#x200B;behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Inaktiv användare {#inactive-user}

**Rotorsak**: AD Sync är aktiverat och användarens federerade konto finns men har inaktiv/inaktiverad status.

**Lösning**:

_Om användaren måste migreras_ - Användarens status och korrekta behörigheter måste återställas av en systemadministratör. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**&#x200B;behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Ogiltig domän {#invalid-domain}

**Rotorsak**: Domänkontroll har aktiverats i Admin Console. Domänen för användarens e-postadress är dock inte en av de tillåtna domänerna eller så har domänen tagits i anspråk i en annan organisation/Admin Console.

**Lösning**:

_Om användaren måste migreras_ (och domänanvändningen är aktiverad i migreringsorganisationen) måste e-postadressen uppdateras i Marketo Engage för att uppfylla principen för domäntvingande (DE). Alternativt kan systemadministratören antingen [flytta domänen](https://helpx.adobe.com/se/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} till en annan katalog som inte är aktiverad för Domain Enforcement (DE), eller [skapa en ny katalog](https://helpx.adobe.com/se/enterprise/using/set-up-identity.html){target="_blank"} som inte finns under DE-principen. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren måste migreras_ (och domänanvändningen är aktiverad i en annan organisation) måste en systemadministratör för organisationen där domänen har tagits i anspråk lägga till användarens e-postadress i undantagslistan. Marketo Engage-administratör kör sedan användarmigreringen för den här användaren igen från migreringskonsolen.

_Om användaren **inte**&#x200B;behöver migreras_ - Marketo Engage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

### Type2E-fel {#type2e-failure}

**Rotorsak**: Det gick inte att skapa ett federerat användarkonto (för enkel inloggning) under användarmigreringen eftersom det redan finns en Adobe ID för samma e-postadress som en enskild användare.

**Lösning**:

1. Ta bort den enskilda användaren från Adobe-organisationen. Obs! Användaren förlorar åtkomsten till alla produkter och måste få ny behörighet senare.
1. Kör om användarmigreringen så att ett federerat användarkonto skapas för den här användaren.
1. Lägg till användaren i de produkter som han/hon tidigare hade tillgång till.

### Pendo-migrering misslyckades {#pendo-migration-failed}

**Rotorsak**: Användarens federerade konto är antingen inaktivt/inaktiverat eller saknas i Active Directory (AD).

**Lösning**:

_Om användaren måste migreras_

1. En systemadministratör måste återställa användarens kontostatus och behörigheter.

1. För SSO-organ med AD-synkronisering:

   * Skapa användaren via Identity Provider (IdP).
   * Synkronisera användardata med AD.

1. För organ utan SSO/AD-synkronisering:

   * Återskapa det hanterade kontot för att återställa status.
   * Organisationsadministratören måste omtilldela roller och behörigheter.

1. Marketo Engage Admin kör migreringen igen i migreringskonsolen.

1. Om konsolen inte är tillgänglig kontaktar du [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support) för att köra migreringen igen.

_Om användaren **inte**&#x200B;behöver migreras_

* Marketo Engage Admin bör hoppa över användaren i migreringskonsolen.
* När alla användare har migrerats eller hoppats över klickar du på **[!UICONTROL Migration Complete]** för att slutföra.
* Om felet kvarstår skickar du ett supportärende med relevant information till [Marketo Support](https://nation.marketo.com/t5/support/ct-p/Support).


### Det gick inte att skapa användare {#user-creation-failed}

[Se nedan](#failed)

### Marketo Entitlement Failed {#marketo-entitlement-failed}

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
