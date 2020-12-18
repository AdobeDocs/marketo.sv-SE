---
unique-page-id: 14352581
description: Begränsningsfel - Marketo Docs - Produktdokumentation
title: Begränsningsfel
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Begränsningsfel {#throttling-errors}

## Filgränsen har nåtts {#file-limit-reached}

Om du skickar via din egen server har den begränsningar för hur många e-postmeddelanden du kan skicka samtidigt. När du skickar via Sales Connect kan du skicka många e-postmeddelanden, men vi försöker skicka alla samtidigt. Om du är medveten om att servern kommer att skära av dig med 100 e-postmeddelanden per minut, behöver du bara skicka upp till 100 e-postmeddelanden via [webbprogrammet](http://toutapp.com/login). Annars kan e-postmeddelandena landa här på grund av att e-postmeddelandena stryps på servern.

## Autentiseringsfel {#authentication-error}

Det innebär att det inte gick att autentisera anslutningen till SMTP-servern. Ditt lösenord har antagligen ändrats nyligen och du behöver bara autentisera dina nya inloggningsuppgifter.

Det gör du genom att gå till [SMTP-inställningarna](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

Gå till Misslyckade leveranser och försök skicka om dessa e-postmeddelanden.
