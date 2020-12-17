---
unique-page-id: 10095307
description: Anpassade synkroniseringsfilterregler för en e-postadress - Marketo Docs - Produktdokumentation
title: Anpassade synkroniseringsfilterregler för en e-postadress
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Anpassade synkroniseringsfilterregler för en e-postadress {#custom-sync-filter-rules-for-an-email-address}

Följ de här reglerna för att förhindra synkronisering av poster som inte har någon e-postadress.

* När ett lead skapas ELLER när leadets e-postadressfält uppdateras, kontrollerar du om leadet har en e-postadress och, om det har det, ändrar du Synkronisera till **Sant**. Ändra annars till **Falskt**

* När en kontakt skapas ELLER när kontaktens e-postadressfält uppdateras kontrollerar du om kontakten har en e-postadress och om den har det ändrar du Synkronisera till **True** och ändrar Synkronisera till **True** för kontoposten. I annat fall ändrar du till **Falskt**

* När kontaktens företagsnamn (parentcustomerid) uppdateras kontrollerar du om kontaktens fält Synkronisera med KTO är true. Om det är det ändrar du även Synkronisera till MKTO för kontot till **True**
* När fältet Potentiell kund (anpassad) eller Kontakt (parentkontaktaktid) för affärsmöjligheten uppdateras, kontrollerar du om kontots Synkronisera med MKto-fält är sant eller om kontaktens Synkronisera med MKto-fält är sant. I så fall ändrar du Synkronisera till MKTO för affärsmöjligheten till **Sant** även

