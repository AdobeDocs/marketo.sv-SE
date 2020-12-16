---
unique-page-id: 2953457
description: SFDC Sync -Contact Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - kontaktsynkronisering
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# SFDC-synkronisering: Kontaktsynkronisering {#sfdc-sync-contact-sync}

Visste du att Marketo synkroniserar hela databasen med Salesforce? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Salesforce-kontakter.

## Synkroniseringsriktning {#sync-direction}

Kontaktsynkroniseringen är dubbelriktad. Om du ändrar en kontakt i antingen Salesforce eller Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om ändringar görs i båda systemen samtidigt? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Vi är trevliga och låter Salesforce vinna. Det är sällsynt att en sådan kollision mellan data inträffar.

## Kan jag konvertera en person till en kontakt i Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, använd flödesåtgärden ** [Convert Person](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>Konvertering av en person i Marketo resulterar i ett nytt konto och en ny affärsmöjlighet i Salesforce. Om du inte vill ha dubblettkonton använder du Salesforce för att konvertera.

## Kan jag framtvinga en synkronisering av en kontakt manuellt? {#can-i-manually-force-a-sync-of-a-contact}

Ja, använd ** [Sync Person to SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **flow och synkronisera i realtid.

## Synkroniserar alla standardfält med Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som Marketo Sync-användaren har åtkomst till.

## Kommer Marketo att respektera Salesforce-valideringsreglerna? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, om det finns en konflikt loggas resultatet i lead-aktivitetsloggen.
