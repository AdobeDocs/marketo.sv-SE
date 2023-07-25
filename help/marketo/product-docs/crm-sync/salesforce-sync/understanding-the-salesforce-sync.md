---
unique-page-id: 4719283
description: Förstå Salesforce-synkronisering - Marketo Docs - produktdokumentation
title: Förstå Salesforce-synkronisering
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Förstå Salesforce-synkronisering {#understanding-the-salesforce-sync}

Marketo och Salesforce går ihop som ärtor och morötter. Vi synkroniserar era sälj- och marknadsföringsdata.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar med Salesforce hela dagen, varje dag. Varje synkronisering tar en stund och pausar sedan i 5 minuter och startar sedan igen.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen kan ta timmar eller till och med dagar eftersom Marketo kopierar hela databasen från Salesforce. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

![](assets/sync-illustration.png)

Synkroniseringen mellan Salesforce och Marketo är endast dubbelriktad för leads, kontakter och Salesforce-kampanjer. När du gör ändringar i antingen Salesforce eller Marketo återspeglas dina uppdateringar i båda systemen. Alla andra synkroniseringar är endast från Salesforce till Marketo. Klicka på länkarna nedan om du vill ha information om var och en av länkarna.

## Vad synkroniseras mellan Marketo och Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Kontakter](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Konton](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Användare](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Möjligheter](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce-kampanjer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Egna objekt](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Aktivitet](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>The [inloggningsuppgifter som du anger i Marketo för Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

Marketo synkronisering med Salesforce är den mest kraftfulla av sitt slag i världen. Det känns som magi. en ändring görs och det andra systemet är snart uppdaterat.
