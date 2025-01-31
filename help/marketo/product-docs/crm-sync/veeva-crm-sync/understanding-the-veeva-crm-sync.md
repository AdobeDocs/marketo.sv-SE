---
description: Så här fungerar Veeva CRM Sync - Marketo Docs - produktdokumentation
title: Så här fungerar Veeva CRM Sync
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Så här fungerar Veeva CRM Sync {#understanding-the-veeva-crm-sync}

Med några enkla steg är det enkelt att synkronisera mellan Adobe Marketo Engage och Veeva CRM.

## Så här fungerar synkroniseringen {#how-the-sync-works}

Marketo Engage synkroniserar med Veeva CRM hela dagen, varje dag. Varje synkronisering tar en stund, pausar i 5 minuter och startar sedan igen.

>[!NOTE]
>
>Den allra första synkroniseringen kan ta timmar eller till och med dagar eftersom Marketo Engage kopierar hela databasen från Veeva. Efter det tar varje synkronisering vanligtvis minuter (ibland sekunder) och synkroniserar bara data som har ändrats.

![](assets/understanding-the-veeva-sync-1.png)

Synkroniseringen mellan Veeva och Marketo Engage är endast dubbelriktad för kontaktfält i Person-kontoobjektet. När du gör ändringar i antingen Veeva eller Marketo Engage återspeglas dina uppdateringar i båda systemen. Alla andra synkningar är endast från Veeva till Marketo Engage. Klicka på länkarna nedan om du vill ha information om var och en av länkarna.

## Vad synkroniseras mellan Marketo Engage och Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Personkonton](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Användare
* [Anropa och anropa nyckelobjekt](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Egna objekt](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Saker att veta {#things-to-know}

* De [autentiseringsuppgifter som du anger i Marketo Engage för Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

* Veeva CRM baseras på force.com och den omfattande upplevelse som Marketo Engage har med plattformen ärvs i den här synkroniseringen.

* Veeva CRM visar: Lead, Contact, Accounts, Business Accounts, Opportunity, Campaign och Activity. De stöds dock inte i synkroniseringen med Marketo Engage.
