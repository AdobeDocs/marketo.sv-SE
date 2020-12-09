---
unique-page-id: 4719283
description: Förstå Salesforce-synkronisering - Marketo-dokument - produktdokumentation
title: Förstå Salesforce-synkronisering
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Förstå Salesforce-synkronisering {#understanding-the-salesforce-sync}

Marketo och Salesforce går ihop som ärter och morötter. Vi synkroniserar era sälj- och marknadsföringsdata.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar med Salesforce hela dagen, varje dag. Varje synkronisering tar en stund och pausar sedan i 5 minuter och startar sedan igen.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen kan ta timmar eller till och med dagar eftersom Marketo kopierar hela databasen från Salesforce. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

![](assets/sync-illustration.png)

Synkroniseringen mellan Salesforce och Marketo är endast dubbelriktad för leads, kontakter och Salesforce-kampanjer. När du gör ändringar i antingen Salesforce eller Marketo återspeglas dina uppdateringar i båda systemen. Alla andra synkroniseringar är endast från Salesforce till Marketo. Klicka på länkarna nedan om du vill ha information om var och en av länkarna.

## Vad är Synkroniserat mellan Marketo och Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Kontakter](sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Konton](sfdc-sync-details/sfdc-sync-account-sync.md)
* [Användare](sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Möjligheter](sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce-kampanjer](sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Egna objekt](sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Aktivitet](sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>De [autentiseringsuppgifter du anger i Marketo för Salesforce](setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

Det finns många nyanser och funktioner om Salesforce-synkronisering. Läs mer i avsnittet [om](http://docs.marketo.com/display/docs/sfdc+sync+details)SFDC-synkronisering.

>[!MORELIKETHIS]
>
>* [Inställningar för Salesforce-synkronisering](http://docs.marketo.com/display/docs/setup)
>* [Information om SFDC-synkronisering](http://docs.marketo.com/display/docs/sfdc+sync+details)

>



Marketos synkronisering med Salesforce är den mest kraftfulla i sitt slag i världen. Det känns som magi - en förändring görs och det andra systemet är snart uppdaterat.