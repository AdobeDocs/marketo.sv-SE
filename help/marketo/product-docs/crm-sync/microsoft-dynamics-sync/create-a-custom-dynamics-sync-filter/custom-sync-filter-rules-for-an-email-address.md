---
unique-page-id: 10095307
description: Lär dig hur du ställer in anpassade synkroniseringsfilterregler för e-postadresser i Dynamics. Använd arbetsflöden för att ställa in Synkronisera med MKto baserat på om lead eller kontakt har ett e-postmeddelande.
title: Anpassade synkroniseringsfilterregler för en e-postadress
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Anpassade synkroniseringsfilterregler för en e-postadress {#custom-sync-filter-rules-for-an-email-address}

Följ de här reglerna för att förhindra synkronisering av poster som inte har någon e-postadress.

* När ett lead skapas ELLER när leadets e-postadressfält uppdateras, kontrollerar du om leadet har en e-postadress och, om så är fallet, ändrar du Synkronisera till Mkto till **[!UICONTROL True]**. Ändra annars till **[!UICONTROL False]**

* När en kontakt skapas ELLER när kontaktens e-postadressfält uppdateras, kontrollerar du om kontakten har en e-postadress och om den har det, ändrar Synkronisera till MKto till **[!UICONTROL True]** och ändrar Synkronisera till MKto till **[!UICONTROL True]** i kontoposten. Annars ändrar du till **[!UICONTROL False]**

* När kontaktens företagsnamnfält (parentcustomerid) uppdateras kontrollerar du om kontaktens fält Synkronisera med KTO är sant. Om det är det ändrar du även Synkronisera till MKTO för kontot till **[!UICONTROL True]**
* När fältet Potentiell kund (anpassad) eller Kontakt (parentkontaktaktid) för affärsmöjligheten uppdateras, kontrollerar du om kontots Synkronisera med MKto-fält är sant eller om kontaktens Synkronisera med MKto-fält är sant. Om det är det ändrar du även Synkronisera till MKTO för affärsmöjligheten till **[!UICONTROL True]**
