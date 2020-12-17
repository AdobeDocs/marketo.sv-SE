---
unique-page-id: 10098625
description: Förstå Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Förstå Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Förstå Microsoft Dynamics-synkronisering {#understanding-the-microsoft-dynamics-sync}

Marketo och Microsoft Dynamics går ihop. Vi synkroniserar era sälj- och marknadsföringsdata.

>[!NOTE]
>
>Marketo stöder endast SSL-certifikat som är kompatibla med Java 7 just nu.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar kontinuerligt data med Microsoft Dynamics hela dagen, varje dag. Det görs med bakgrundssynkronisering, gruppvis, inte i realtid.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen tar minuter till timmar, beroende på databasens storlek. Marketo kopierar hela databasen från Dynamics. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

Synkroniseringen mellan Marketo och Dynamics är dubbelriktad för leads och kontakter. Om du ändrar något i Marketo eller Dynamics återspeglas dina uppdateringar i båda systemen. Alla andra fält, som konton och affärsmöjligheter, synkroniseras på ett sätt, från Dynamics till Marketo.

## Vad synkroniseras mellan Marketo och Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakter](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konton](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Användare](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (grupper med SystemUsers)
* [Möjligheter](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Anpassade entiteter](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>De [autentiseringsuppgifter du anger i Marketo för Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) används för att synkronisera data.

Det finns många nyanser och funktioner om Dynamics-synkronisering. Läs mer i avsnittet [Synkroniseringsinformation för Microsoft Dynamics](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details).

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för Marketo Dynamics Sync. Om du behöver uppdatera din Dynamics CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

>[!MORELIKETHIS]
>
>* [Synkronisera inställningar](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Synkroniseringsinformation för Microsoft Dynamics](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

