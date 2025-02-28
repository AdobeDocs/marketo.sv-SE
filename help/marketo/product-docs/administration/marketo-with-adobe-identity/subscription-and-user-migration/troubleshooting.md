---
description: Felsökningsguide för Adobe IMS - Marketo Docs - Produktdokumentation
title: Felsökningsguide för Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Felsökningsguide för Adobe IMS {#adobe-ims-troubleshooting-guide}

Under IMS-användarmigreringen skapas en Adobe-användare för varje Marketo Engage-användare som migreras. Ibland skapas den inte (av olika anledningar relateras till användarens post i Active Directory eller problem med e-postadressen). När detta inträffar ser Marketo Engage-administratören orsaken i användarens migreringsstatusfält på självmigreringskonsolen.

## Felmeddelanden {#error-messages}

Använd delen &quot;På den här sidan&quot; till höger för att gå direkt till ett specifikt fel och lära dig hur du löser det.

### Finns inte i katalogen {#not-in-directory}

_Rotorsak_: Användaren finns inte i Active Directory (AD). För alla organ med enkel inloggning som har AD-synkronisering aktiverad, är det endast tillåtet att skapa användare via identitetsleverantören (IdP). Användaren kunde därför inte läggas till via Admin Console under användarmigreringen.

_Lösning_:

Före migrering - Marketo Enage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

Efter migrering - Användaren måste läggas till i Active Directory med rätt behörigheter. Marketo Engage-administratör kör sedan om användarmigreringen för den här användaren från migreringskonsolen.

### Ogiltigt Gmail-tecken {#gmail-invalid-character}

_Rotorsak_: Enligt Adobe säkerhetsprincip tillåts inte tecknen `.` och `+` i en Gmail-e-postadress. Båda tecknen tillåts i e-postadresser som inte är Gmail.

_Lösning_:

Före migrering - Marketo Enage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

Efter migrering - E-postadressen måste uppdateras i Marketo Engage för att uppfylla Adobe säkerhetspolicy. Marketo-administratör för att köra användarmigreringen för den här användaren igen från migreringskonsolen.

### Inaktiv användare {#inactive-user}

_Rotorsak_: AD Sync är aktiverat och användarens federerade konto finns men har inaktiv/inaktiverad status.

_Lösning_:

Före migrering - Marketo Enage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

Eftermigrering - Användarens status och korrekta behörigheter måste återställas. Marketo Engage-administratör kör sedan om användarmigreringen för den här användaren från migreringskonsolen.

### Inte i domänen {#not-in-domain}

_Rotorsak_: Domänkontroll har aktiverats i Admin Console, men domänen för användarens e-postadress är inte en av de tillåtna domänerna.

_Lösning_:

Före migrering - Marketo Enage-administratör för att hoppa över användaren i migreringskonsolen. Knappen&quot;Slutförd migrering&quot; visas när alla användare räknas med genom att migrera eller hoppa över. Klicka på knappen för att slutföra användarmigreringsprocessen.

Efter migrering - E-postadressen måste uppdateras i Marketo Engage för att följa de domänbaserade reglerna (DE). Alternativt kan systemadministratören antingen [flytta domänen](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} till en annan inaktiverad katalog för Domain Enforcement (DE) eller [skapa en ny katalog](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"} som inte omfattas av DE-principen. Marketo Engage-administratör kör sedan om användarmigreringen för den här användaren från migreringskonsolen.

### Skapa fel {#create-failure}

_Rotorsak_: Det här felet kan orsakas av olika orsaker i serverdelen.

_Lösning_:

Före migrering - Skicka ett supportärende för de [som inte har migrerats än](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Efter migrering - skicka ett supportärende för de [som redan har migrerats](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Type2e-användarfel {#type2e-user-failure}

_Rotorsak_: Det här felet kan orsakas av olika orsaker i serverdelen.

_Lösning_:

Före migrering - Skicka ett supportärende för de [som inte har migrerats än](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Efter migrering - skicka ett supportärende för de [som redan har migrerats](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
