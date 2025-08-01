---
description: Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce? - Marketo Docs - produktdokumentation
title: Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Jag ser inte e-post- eller samtalsaktiviteter som synkroniserats med Salesforce.**

* Kontrollera att du är ansluten till Salesforce. Varje användare måste ha en anslutning för att kunna logga sin e-post och sina samtal till Salesforce.
* Kontrollera att du har konfigurerat [Salesforce Sync Settings](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* E-postmeddelanden gör en postsökning baserad på Salesforce ID som primär sökning och e-postadress som sekundär. Du kan bekräfta att en personpost har ett Salesforce ID och en e-postadress länkad till dem i [webbappen Åtgärder](https://toutapp.com/next#command_center){target="_blank"}.
* Anrop gör en postsökning baserad enbart på Salesforce ID. Om det inte finns något Salesforce-ID för personposten i Åtgärder loggas inte samtalet. Du kan bekräfta att en personpost har ett Salesforce-id kopplat till sig i webbappen [Åtgärder](https://toutapp.com/next#command_center){target="_blank"}.

**Jag ser inte aktivitetsfält i Salesforce-uppdatering.**

Om du inte ser någon uppdatering av [aktivitetsattributfält](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} i Salesforce kan det bero på begränsningar i teamets fälttillgänglighet. Salesforce fältnivåsäkerhet ger Salesforce-administratörer möjlighet att lägga in begränsningar kring vilken information som kan visas och redigeras av användare. Om åtgärdsanvändare inte har tillgång till dessa fält för att visa och redigera dem kan åtgärdssynkroniseringen inte uppdatera dessa fält.

* Arbeta med din Salesforce-administratör för att se till att de här säkerhetsinställningarna inte stör [Åtgärder i Salesforce aktivitetsfält](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Om du är Salesforce-administratör kan du visa hjälpmedel för fält på fliken Säkerhetskontroller. De huvudobjekt som funktionsmakron ska interagera med är: Leads, Kontakter, Konton, Affärsmöjligheter och Aktivitet/Aktiviteter.

>[!NOTE]
>
>Fält som är kopplade till lead-, kontakt-, konto- och säljprojektsobjekten installeras med Salesforce-paketet Sales Insight. Fält som är associerade med posttypen [Aktivitet/Aktivitet måste skapas](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} av en Salesforce-administratör.
