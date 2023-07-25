---
unique-page-id: 2953457
description: SFDC-synkronisering - kontaktsynkronisering - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - kontaktsynkronisering
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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

Ja, använd **[Konvertera person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** flödesåtgärd.

>[!CAUTION]
>
>Om du konverterar en person i Marketo skapas ett nytt konto och en ny affärsmöjlighet i Salesforce. Om du inte vill ha dubblettkonton använder du Salesforce för att konvertera.

## Kan jag framtvinga en synkronisering av en kontakt manuellt? {#can-i-manually-force-a-sync-of-a-contact}

Ja, använd **[Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** och den kommer att synkas i realtid.

## Synkroniserar alla standardfält med Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din Marketo Sync-användare har åtkomst till.

## Kommer Marketo att respektera Salesforce-valideringsreglerna? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, om det finns en konflikt loggas resultatet i lead-aktivitetsloggen.
