---
description: Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce? - Marketo Docs - produktdokumentation
title: Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce?
source-git-commit: c50f0f08914076a440026fb368bf38763b282bbf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Varför synkroniseras inte mina försäljningsaktiviteter och aktivitetsfält till Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Jag ser inte e-post- eller samtalsaktiviteter som synkroniserats med Salesforce.**

* Kontrollera att du är ansluten till Salesforce. Varje användare måste ha en anslutning för att kunna logga sin e-post och sina samtal till Salesforce.
* Kontrollera att du har konfigurerat [Synkroniseringsinställningar för Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* E-postmeddelanden gör en postsökning baserad på Salesforce ID som primär sökning och e-postadress som sekundär. Du kan bekräfta att en personpost har ett Salesforce ID och en e-postadress länkad till dem i [Webbprogrammet Åtgärder](https://toutapp.com/next#command_center){target="_blank"}.
* Anrop gör en postsökning baserad enbart på Salesforce ID. Om det inte finns något Salesforce-ID för personposten i Åtgärder loggas inte anropet. Du kan bekräfta att en personpost har ett Salesforce-ID kopplat till sig i [Webbprogrammet Åtgärder](https://toutapp.com/next#command_center){target="_blank"}.

**Jag ser inte aktivitetsfält i Salesforce-uppdatering.**

Om du inte ser e-post [aktivitetsattributfält](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} i Salesforce kan det bero på begränsningar i teamets fälttillgänglighet. Salesforce-fältnivåsäkerhet ger Salesforce-administratörer möjlighet att placera begränsningar runt vilken information som kan visas och redigeras av användare. Om åtgärdsanvändare inte har tillgång till dessa fält för att visa och redigera dem kan åtgärdssynkroniseringen inte uppdatera dessa fält.

* Arbeta med din Salesforce-administratör för att se till att de här skyddsinställningarna inte stör [Åtgärder för Salesforce-aktivitetsfält](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Om du är Salesforce-administratör kan du se fälttillgängligheten på fliken Säkerhetskontroller. De huvudobjekt som funktionsmakron ska interagera med är: Leads, kontakter, konton, säljprojekt och aktivitet/aktiviteter.

>[!NOTE]
>
>Fält som är kopplade till lead-, kontakt-, konto- och säljprojektsobjekten installeras med Salesforce-paketet Sales Insight. Fält som är kopplade till [Posttypen Aktivitet/Aktivitet måste skapas](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} av en Salesforce-administratör.
