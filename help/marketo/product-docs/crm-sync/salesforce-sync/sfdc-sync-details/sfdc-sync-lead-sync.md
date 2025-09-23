---
unique-page-id: 2953455
description: SFDC Sync - Lead Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - Lead Sync
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# SFDC Sync: Leadsynkronisering {#sfdc-sync-lead-sync}

Visste du att Marketo synkroniserar från din [!DNL Salesforce]-databas? Den synkas, väntar 5 minuter och synkroniseras sedan igen. Hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar [!DNL Salesforce] leads.

## Synkroniseringsriktning {#sync-direction}

Synkroniseringen av lead (person) och kontakt är dubbelriktad. Om du ändrar en post i antingen [!DNL Salesforce] eller Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om ändringar görs i båda systemen samtidigt? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo vinner. Det är sällsynt att en sådan kollision mellan data inträffar.

## Kan jag skapa ett lead i [!DNL Salesforce] med Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, använd flödesåtgärden [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Detta skapar ett lead i [!DNL Salesforce] om leadet inte finns.

## Kan jag manuellt tvinga en synkronisering av en person i Marketo till ett lead i [!DNL Salesforce]? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, använd flödesåtgärden [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} så synkroniseras den i realtid.

## Synkroniserar alla standardfält med Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nej, alla standardfält är inte användbara. Alla anpassade fält kan ingå i synkroniseringen.

>[!NOTE]
>
>Marketo synkroniserar bara de fält som din [!DNL Salesforce]-synkroniseringsanvändare har åtkomst till.

## Kommer Marketo att respektera verifieringsreglerna för [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Synkroniseringen misslyckas om dataformatet är fel eller om nödvändig fältinformation saknas. Marketo loggar resultatet i den inledande aktivitetsloggen om detta händer.
