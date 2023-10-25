---
unique-page-id: 10095307
description: Anpassade synkroniseringsfilterregler för en e-postadress - Marketo Docs - Produktdokumentation
title: Anpassade synkroniseringsfilterregler för en e-postadress
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Anpassade synkroniseringsfilterregler för en e-postadress {#custom-sync-filter-rules-for-an-email-address}

Följ de här reglerna för att förhindra synkronisering av poster som inte har någon e-postadress.

* När ett lead skapas ELLER när leadets e-postadressfält uppdateras, kontrollerar du om leadet har en e-postadress och, om så är fallet, ändrar du Synkronisera till Mkto till **[!UICONTROL True]**. Ändra annars till **[!UICONTROL False]**.

* När en kontakt skapas ELLER när kontaktens e-postadressfält uppdateras, kontrollerar du om kontakten har en e-postadress och om den har det, ändrar du Synkronisera till MKTO till **[!UICONTROL True]** och ändra Synkronisera till Mkto till **[!UICONTROL True]** på kontoposten. Annars ändrar du till **[!UICONTROL False]**.

* När kontaktens företagsnamn (parentcustomerid) uppdateras kontrollerar du om kontaktens fält Synkronisera med kto är sant. I så fall ändrar du Synkronisera till MKTO för kontot till **[!UICONTROL True]** också.

* När fältet Potentiell kund (anpassad) eller Kontakt (parentkontaktaktid) för affärsmöjligheten uppdateras, kontrollerar du om kontots Synkronisera med MKto-fält är sant eller om kontaktens Synkronisera med MKto-fält är sant. I så fall ändrar du Synkronisera till MKTO på affärsmöjligheten till **[!UICONTROL True]** också.
