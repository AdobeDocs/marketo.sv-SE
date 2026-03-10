---
unique-page-id: 10098625
description: Läs om hur Microsoft Dynamics-synkroniseringen håller Marketo- och Dynamics-data synkroniserade. Se vad som synkroniseras och hur dubbelriktad synkronisering fungerar för leads och kontakter.
title: Förstå Microsoft Dynamics Sync
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Förstå synkroniseringen av [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo och [!DNL Microsoft Dynamics] går ihop. Vi synkroniserar era sälj- och marknadsföringsdata.

>[!CAUTION]
>
>Vi stöder för närvarande inte uppdatering av sandlådan för synkronisering av [!DNL Marketo Dynamics]. Om du behöver uppdatera din [!DNL Dynamics] CRM-sandlåda krävs en ny Marketo-sandlåda. Kontakta din Customer Success Manager om du vill ha mer information.

## Så här fungerar Synkronisera {#how-sync-works}

Marketo synkroniserar kontinuerligt data med [!DNL Microsoft Dynamics] hela dagen, varje dag. Det görs med bakgrundssynkronisering, gruppvis, inte i realtid.

>[!NOTE]
>
>Den allra första synkroniseringen i prenumerationen tar minuter till timmar, beroende på databasens storlek. Marketo kopierar hela databasen från [!DNL Dynamics]. Efter det tar varje synkronisering vanligtvis några sekunder eller minuter och synkroniserar bara data som har ändrats.

Synkroniseringen mellan Marketo och [!DNL Dynamics] är dubbelriktad för leads och kontakter. Om du gör ändringar i antingen Marketo eller [!DNL Dynamics] återspeglas dina uppdateringar i båda systemen. Alla andra fält, som konton och affärsmöjligheter, synkroniseras endast på ett sätt, från [!DNL Dynamics] till Marketo.

## Vad är synkroniserat mellan Marketo och [!DNL Microsoft Dynamics]? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konton](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Användare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Team (grupper med SystemUsers)
* [Möjligheter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Anpassade entiteter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

De [autentiseringsuppgifter du anger i Marketo för [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) används för att synkronisera data.

>[!NOTE]
>
>Instanskopiering stöds inte om källinstansen är integrerad med [!DNL Microsoft Dynamics].
