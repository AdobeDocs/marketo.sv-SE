---
unique-page-id: 2953473
description: SFDC Sync -Activity Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Aktivitetssynkronisering
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# SFDC-synkronisering: Aktivitetssynkronisering {#sfdc-sync-activity-sync}

Marketo synkroniserar även över Salesforce-aktivitetsdata. Här är några frågor och svar.

## Vilka typer av aktivitetsdata synkroniserar Markto över? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synkroniserar över både händelser och uppgifter som är kopplade till en lead eller kontakt.

## Hur synkroniseras aktivitetsinformationen mellan de två systemen? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är ett sätt, från Salesforce till Marketo. Men du kan skapa en uppgift i Salesforce med flödessteget [Skapa uppgift](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) eller [Anpassa aktiviteter Synkronisera](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) till Salesforce.

## Kan jag skapa en uppgift med Marketo? {#can-i-create-a-task-using-marketo}

Ja, du kan använda åtgärden [Skapa uppgiftsflöde](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Vilka utlösare/filter är relaterade till aktiviteten? {#what-are-the-triggers-filters-related-to-activity}

Utlösare

* Aktiviteten är loggad
* Aktiviteten har uppdaterats

Filter

* Aktiviteten loggades/aktiviteten var inte loggad
* Aktiviteten har uppdaterats/aktiviteten har inte uppdaterats

>[!TIP]
>
>Är du inte säker på den ordalydelsen &quot;Inte aktivitet&quot;? &quot;not&quot; refererar till ett inaktivitetsfilter. Läs mer om dem här: [Använd inaktivitetsfilter i en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

