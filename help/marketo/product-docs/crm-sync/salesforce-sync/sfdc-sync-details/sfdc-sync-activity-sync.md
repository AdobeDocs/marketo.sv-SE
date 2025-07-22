---
unique-page-id: 2953473
description: SFDC Sync - Activity Sync - Marketo Docs - produktdokumentation
title: SFDC Sync - aktivitetssynkronisering
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# SFDC Sync: Aktivitetssynkronisering {#sfdc-sync-activity-sync}

Marketo synkroniserar även över aktivitetsdata för [!DNL Salesforce]. Här är några frågor och svar.

## Vilka typer av aktivitetsdata synkroniseras Marketo över? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synkroniserar över både händelser och uppgifter som är kopplade till ett lead eller en kontakt.

## Hur synkroniseras aktivitetsinformationen mellan de två systemen? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är ett sätt, från [!DNL Salesforce] till Marketo. Men du kan skapa en uppgift i [!DNL Salesforce] med flödessteget [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) eller [Anpassa aktiviteter, synkronisera](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) till [!DNL Salesforce].

## Kan jag skapa en uppgift med Marketo? {#can-i-create-a-task-using-marketo}

Ja, du kan använda åtgärden [Skapa uppgiftsflöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Vilka utlösare/filter är relaterade till aktiviteten? {#what-are-the-triggers-filters-related-to-activity}

Utlösare

* Aktiviteten är loggad
* Aktiviteten har uppdaterats

Filter

* Aktiviteten loggades/aktiviteten var inte loggad
* Aktiviteten uppdaterades/aktiviteten uppdaterades inte

>[!TIP]
>
>Är du inte säker på den ordalydelsen &quot;Inte aktivitet&quot;? &quot;not&quot; avser ett inaktivitetsfilter. Läs mer om dem här: [Använd inaktivitetsfilter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
