---
unique-page-id: 2953455
description: SFDC Sync -Lead Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Lead-synkronisering
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC-synkronisering: Leadsynkronisering {#sfdc-sync-lead-sync}

Visste du att Marketo synkroniserar från din Salesforce-databas? Den synkas, väntar 5 minuter och synkroniseras sedan igen. Hela dagen, varje dag. Här är några detaljer om hur Marketo behandlar Salesforce specifikt.

## Synkroniseringsriktning {#sync-direction}

Synkroniseringen av lead (person) och kontakt är dubbelriktad. Om du ändrar en post i antingen Salesforce eller Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om ändringar görs i båda systemen samtidigt? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo vinner. Det är sällsynt att en sådan kollision mellan data inträffar.

## Kan jag skapa en lead i Salesforce med Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, använd flödesåtgärden [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Detta skapar en lead i Salesforce om leadet inte finns.

## Kan jag manuellt tvinga en synkronisering av en person i Marketo till ett lead i Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, använd flödesåtgärden [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) så synkroniseras den i realtid.

## Synkroniserar alla standardfält med Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din Salesforce-synkroniseringsanvändare har åtkomst till.

## Kommer Marketo att respektera Salesforce-valideringsreglerna? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Synkroniseringen misslyckas om dataformatet är fel eller om nödvändig fältinformation saknas. Marketo loggar resultatet i den inledande aktivitetsloggen om detta händer.
