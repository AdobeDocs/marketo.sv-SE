---
description: Begränsning av e-postanslutning - Marketo Docs - Produktdokumentation
title: Begränsning för e-postanslutning
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# Begränsning för e-postanslutning {#email-connection-throttling}

Genom att integrera ditt Sales Connect-konto för att skicka via Exchange- eller Gmail-e-postleverantörer får du en smidig konfiguration och optimerar e-postleveransen för 1:1-säljkommunikation. Men för att skydda systemen och kontona tillämpar Gmail och Exchange e-postgränser. Dessa gränser kan ökas eller minskas efter leverantörens gottfinnande.

## Begränsning för e-postanslutning (beta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>Den här funktionen är för närvarande i betaversion. Kontakta din Customer Success Manager om du vill gå med i betaversionen.

Begränsning av e-postanslutning gör att Sales Connect-administratörer kan konfigurera sändningsfrekvensen för e-postmeddelanden när Gmail eller Exchange används som leveranskanal, så att den hastighet med vilken e-postmeddelanden skickas till leveranskanalleverantören inte överskrider de tvingande gränserna.

När gränserna genomgående överskrids kan detta ibland ses som misstänkt beteende från leverantören av leveranskanalen, vilket får e-postmeddelanden att misslyckas och ibland även ett konto att inaktiveras.

**Anteckningar/högdagrar**

* Aktiveras automatiskt när en användare ansluter till Gmail eller Exchange
* Kan anpassas om du vill öka eller minska inställningarna från rekommendationer efter dina behov
* Det är bara e-postmeddelanden som skickas via Gmail eller Exchange som stryper för en anpassad leveranskanal
* Begränsningen för e-postanslutning placerar varje enskild användare i e-postmeddelanden separat eftersom varje användare har sin egen anslutning till sin e-postleverantör

**Konfigurera inställningarna för begränsning av e-postanslutning**

1. Klicka på kugghjulsikonen och välj **Inställningar**.

   ![](assets/email-connection-throttling-1.png)

1. Klicka på **Allmänt**.

   ![](assets/email-connection-throttling-2.png)

1. Ange önskad batchstorlek för e-postmeddelanden som ska skickas till e-postkanalleverantören på kortet för e-postanslutningsbegränsning.

   ![](assets/email-connection-throttling-3.png)

1. Ange väntetiden innan varje batch skickas. I det här exemplet väljer vi 25 e-postmeddelanden var 45:e sekund.

   ![](assets/email-connection-throttling-4.png)

1. Klicka på **Spara**.

   ![](assets/email-connection-throttling-5.png)

När ändringarna har sparats får alla användare sina e-postmeddelanden skickade gruppvis till det anslutna Gmail- eller Exchange-kontot för leverans.

## Begränsningar för e-postleverantör {#email-provider-limits}

**Outlook 365**

Företag

* 10 000 per dag
* 30 per minut
* 500 mottagare per e-post

Mer information [finns här](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 per dag (500 för testversioner och flaggade konton)
* 2 e-postmeddelanden per sekund (API-gräns)
* 2 000 mottagare per meddelande (max 500 för externa mottagare)

Mer information [finns här](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

Begränsningar anges av organisationens IT-avdelning när servern hanteras av organisationen. Kontakta nätverks- eller systemadministratören om du vill ha mer information.

>[!MORELIKETHIS]
>
>* [Översikt över leveranskanalen](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [E-postanslutning för Gmail-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-postanslutning för Outlook-användare](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
