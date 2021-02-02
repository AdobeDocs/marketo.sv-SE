---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Contact Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - kontaktsynkronisering
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Kontaktsynkronisering {#microsoft-dynamics-sync-contact-sync}

Visste du att Marketo synkroniserar hela databasen med Dynamics? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Dynamics Contacts.

## Hur synkroniseras informationen mellan de två systemen? {#how-are-details-kept-in-sync-between-the-two-systems}

Kontaktsynkroniseringen är dubbelriktad. Om du ändrar en kontakt i Dynamics eller en person i Marketo återspeglas dina uppdateringar i båda systemen.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Trots att detta är sällsynt kommer Marketo att vinna för människor och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM).

## Kan jag skapa en kontakt med Marketo? {#can-i-create-a-contact-using-marketo}

Ja. [Så här](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>När du använder flödesåtgärden &quot;Synkronisera person till Microsoft&quot; (endast i en utlösarkampanj) skapas lead/kontakt i realtid i Dynamics.

## Kan jag framtvinga en manuell synkronisering av en person eller en kontakt? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Nej, den automatiska bakgrundssynkroniseringen är det enda sättet att synkronisera uppdateringar mellan Marketo och Dynamics. [Synkronisering av person till Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) tvingar inte till en synkronisering av leadet.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [välja fält att synkronisera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) under installationen. Marketo synkroniserar bara de fält som din Dynamics-synkroniseringsanvändare har åtkomst till.

## Kommer Marketo att respektera Dynamics-valideringsreglerna? {#will-marketo-respect-the-dynamics-validation-rules}

Ja, om det finns en konflikt loggas resultatet i lead-aktivitetsloggen.
