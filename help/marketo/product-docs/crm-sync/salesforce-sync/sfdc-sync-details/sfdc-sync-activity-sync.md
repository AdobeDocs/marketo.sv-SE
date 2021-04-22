---
unique-page-id: 2953473
description: SFDC Sync -Activity Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Aktivitetssynkronisering
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# SFDC-synkronisering: Aktivitetssynkronisering {#sfdc-sync-activity-sync}

Marketo synkroniserar också över Salesforce-aktivitetsdata. Här är några frågor och svar.

## Vilka typer av aktivitetsdata synkroniseras Marketo över? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synkroniserar över både händelser och uppgifter som är kopplade till ett lead eller en kontakt.

## Hur synkroniseras aktivitetsinformationen mellan de två systemen? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är ett sätt, från Salesforce till Marketo. Men du kan skapa en uppgift i Salesforce med flödessteget [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) eller [Anpassa aktiviteter Synkronisera](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) till Salesforce.

## Kan jag skapa en uppgift med Marketo? {#can-i-create-a-task-using-marketo}

Ja, du kan använda åtgärden [Skapa uppgiftsflöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Vilka utlösare/filter är relaterade till aktiviteten? {#what-are-the-triggers-filters-related-to-activity}

Utlösare

* Aktiviteten är loggad
* Aktiviteten har uppdaterats

Filter

* Aktiviteten loggades/aktiviteten var inte loggad
* Aktiviteten har uppdaterats/aktiviteten har inte uppdaterats

>[!TIP]
>
>Är du inte säker på den ordalydelsen &quot;Inte aktivitet&quot;? &quot;not&quot; refererar till ett inaktivitetsfilter. Läs mer om dem här: [Använd inaktivitetsfilter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
