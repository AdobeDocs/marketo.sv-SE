---
unique-page-id: 14352600
description: Konfigurera din SMTP-server för Outlook 365 med Sales Connect - Marketo Docs - produktdokumentation
title: Konfigurera din SMTP-server för Outlook 365 med Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Konfigurera din SMTP-server för Outlook 365 med Sales Connect {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Om din organisation använder Outlook och du försöker konfigurera en e-postleveranskanal med Marketo Sales Connect rekommenderar vi att du ansluter till Exchange-servern [med vår e-postanslutningsfunktion](http://docs.marketo.com/x/Z4AOAQ).

Om du vill konfigurera en anpassad [SMTP](http://docs.marketo.com/x/zYTS)-server som en alternativ leveranskanal, kräver ToutApp att du använder någon form av autentisering av säkerhetsskäl. Du kan konfigurera en SMTP-server på din [SMTP-konfigurationssida](http://toutapp.com/next#settings/email-servers/smtp/configure). Microsoft rekommenderar följande konfiguration för att konfigurera en Office365 SMTP-server:\
**SMTP-server**: smtp.office365.com\
**Serverport**: Port 587 - säkrad\
**Autentiseringsmetod**: Inloggning (SSL/TLS)\
**Användarnamn eller inloggning**: din e-postadress för Office365\
**Lösenord**: ditt e-postlösenord för Office365\
**Din domän**: företagets domän

Om du fortfarande har problem med att konfigurera SMTP-servern måste du samarbeta med Exchange-administratören för att säkerställa att rätt autentiseringsuppgifter används.

>[!NOTE]
>
>När Microsoft skickar via Office 365 SMTP lägger Microsoft in en `limit of 30 messages sent per minute` och en gräns på 10 000 mottagare per dag. Dessutom måste `each member` av teamet som vill skicka e-post via Office365 SMTP-servern konfigurera detta med sin egen e-postadress och lösenord i sina inställningar för Sales Connect. Markera rutan för inställningen `Make this deliverability channel to all my team members` `" will not work` för den här konfigurationen, i enlighet med Microsofts Office365-kontoprinciper.

