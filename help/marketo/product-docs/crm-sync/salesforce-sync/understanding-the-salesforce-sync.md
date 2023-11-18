---
unique-page-id: 4719283
description: Förstå Salesforce-synkronisering - Marketo Docs - produktdokumentation
title: Förstå Salesforce-synkronisering
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Förstå Salesforce-synkronisering {#understanding-the-salesforce-sync}

Marketo Engage och Salesforce går samman som ärter och morötter. Vi synkroniserar era sälj- och marknadsföringsdata.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar med Salesforce hela dagen, varje dag. Varje synkronisering tar en stund och pausar sedan i 5 minuter och startar sedan igen.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen kan ta timmar eller till och med dagar eftersom Marketo kopierar hela databasen från Salesforce. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

![](assets/sync-illustration.png)

Synkroniseringen mellan Salesforce och Marketo är endast dubbelriktad för leads, kontakter och Salesforce-kampanjer. När du gör ändringar i antingen Salesforce eller Marketo återspeglas dina uppdateringar i båda systemen. Alla andra synkroniseringar är endast från Salesforce till Marketo. Klicka på länkarna nedan om du vill ha information om var och en av länkarna.

## Vad synkroniseras mellan Marketo och Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Kontakter](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Konton](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Användare](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Möjligheter](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce-kampanjer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Egna objekt](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Aktivitet](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>The [inloggningsuppgifter som du anger i Marketo för Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

Marketo synkronisering med Salesforce är den mest kraftfulla av sitt slag i världen. Det känns som magi; en förändring görs och det andra systemet är snart uppdaterat.
