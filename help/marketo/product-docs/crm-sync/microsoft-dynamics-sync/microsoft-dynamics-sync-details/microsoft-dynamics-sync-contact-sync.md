---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Contact Sync - Marketo Docs - produktdokumentation
title: Microsoft Dynamics Sync -Contact Sync
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Kontakta Sync {#microsoft-dynamics-sync-contact-sync}

Visste du att Marketo Engage synkroniserar hela databasen med Dynamics? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Dynamics Contacts.

## Hur synkroniseras informationen mellan de två systemen? {#how-are-details-kept-in-sync-between-the-two-systems}

Kontaktsynkroniseringen är dubbelriktad. Om du ändrar en kontakt i Dynamics eller en person i Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Även om detta är sällsynt kommer Marketo att vinna för människor och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM).

## Kan jag skapa en kontakt med Marketo? {#can-i-create-a-contact-using-marketo}

Ja. [Så här ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>När du använder flödesåtgärden &quot;Synkronisera person till Microsoft&quot; (endast i en utlösarkampanj) skapas lead/kontakt i realtid i Dynamics.

## Kan jag tvinga en person eller en kontakt att synkronisera manuellt? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Nej, den automatiska bakgrundssynkroniseringen är det enda sättet att synkronisera uppdateringar mellan Marketo och Dynamics. [Synkroniseringspersonen till Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} tvingar inte fram en synkronisering av leadet.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [välja fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} under installationen. Men Marketo synkroniserar bara de fält som din Dynamics-synkroniseringsanvändare har åtkomst till.

## Kommer Marketo att respektera Dynamics-valideringsreglerna? {#will-marketo-respect-the-dynamics-validation-rules}

Ja, om det finns en konflikt loggas resultatet i lead-aktivitetsloggen.
