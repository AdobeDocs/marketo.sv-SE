---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Lead Sync
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Leadsynkronisering {#microsoft-dynamics-sync-lead-sync}

Synkroniseringen mellan Marketo och Dynamics är superkraftfull. Här är detaljerna:

## Hur synkroniseras informationen mellan de två systemen? {#how-are-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad. Om du ändrar något i ett lead i Dynamics eller en person i Marketo återspeglas uppdateringen i båda systemen.

>[!NOTE]
>
>Borttagningar synkroniseras inte alltid automatiskt i båda riktningarna. Se [Ta bort en lead eller kontakt](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Även om detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM).

## Kan jag skapa en lead i Dynamics med Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, använd [Synkronisera person till Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) flödesåtgärd. Detta skapar ett lead i Dynamics om leadet inte finns. Om leadet finns utför flödessteget ingen åtgärd.

>[!NOTE]
>
>När du använder flödesåtgärden &quot;Synkronisera person till Microsoft&quot; (endast i en utlösarkampanj) skapas lead/kontakt i realtid i Dynamics.

## Kan jag manuellt tvinga en synkronisering av en person från Marketo till ett lead i Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nej, den automatiska bakgrundssynkroniseringen är det enda sättet att synkronisera uppdateringar mellan Marketo och Dynamics. The [Synkronisera person till Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) Flödesåtgärden tvingar inte fram en synkronisering av leadet.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) under installationen.

## Kommer Marketo att respektera Dynamics-valideringsreglerna? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Synkroniseringen misslyckas om dataformatet är fel eller om nödvändig fältinformation saknas. Marketo loggar resultatet i personens aktivitetslogg om detta händer.
