---
unique-page-id: 14352581
description: Begränsningsfel - Marketo Docs - Produktdokumentation
title: Begränsningsfel
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Begränsningsfel {#throttling-errors}

## Filgränsen har nåtts {#file-limit-reached}

Om du skickar via din egen server har den begränsningar för hur många e-postmeddelanden du kan skicka samtidigt. När du skickar via Sales Connect kan du skicka många e-postmeddelanden, men vi försöker skicka alla samtidigt. Om du är medveten om att servern kommer att skära av dig med 100 e-postmeddelanden per minut, behöver du bara skicka upp till 100 e-postmeddelanden via [webbprogrammet](https://toutapp.com/login). Annars kan e-postmeddelandena landa här på grund av att e-postmeddelandena stryps på servern.

## Autentiseringsfel {#authentication-error}

Det innebär att det inte gick att autentisera anslutningen till SMTP-servern. Ditt lösenord har antagligen ändrats nyligen och du behöver bara autentisera dina nya inloggningsuppgifter.

Det gör du genom att gå till SMTP-inställningarna, där du bör få samma felmeddelande. Uppdatera dina inloggningsuppgifter och tryck på **Verifiera och spara** för att se ett bekräftelsemeddelande.

Gå till Misslyckade leveranser och försök skicka om dessa e-postmeddelanden.
