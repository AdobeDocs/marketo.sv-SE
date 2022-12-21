---
unique-page-id: 10098625
description: Förstå Microsoft Dynamics Sync - Marketo Docs - produktdokumentation
title: Förstå Microsoft Dynamics Sync
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Förstå Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo och Microsoft Dynamics går ihop. Vi synkroniserar era sälj- och marknadsföringsdata.

>[!NOTE]
>
>Marketo stöder endast SSL-certifikat som för närvarande är kompatibla med Java 7.

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar kontinuerligt data med Microsoft Dynamics hela dagen, varje dag. Det görs med bakgrundssynkronisering, gruppvis, inte i realtid.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen tar minuter till timmar, beroende på databasens storlek. Marketo kopierar hela databasen från Dynamics. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

Synkroniseringen mellan Marketo och Dynamics är dubbelriktad för leads och kontakter. Om du gör ändringar i antingen Marketo eller Dynamics återspeglas dina uppdateringar i båda systemen. Alla andra fält, som konton och affärsmöjligheter, synkroniseras på ett sätt, från Dynamics till Marketo.

## Vad synkroniseras mellan Marketo och Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konton](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Användare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (grupper med SystemUsers)
* [Möjligheter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Anpassade entiteter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

The [inloggningsuppgifter som du anger i Marketo för Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) används för att synkronisera data.

>[!NOTE]
>
>Instanskopiering stöds inte om källinstansen är integrerad med Microsoft Dynamics.
