---
unique-page-id: 3571848
description: Microsoft Dynamics Sync -Lead Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Lead Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Leadsynkronisering {#microsoft-dynamics-sync-lead-sync}

Marketo to Dynamics sync är superkraftfull. Här är detaljerna:

## Hur synkroniseras informationen mellan de två systemen? {#how-are-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad. Om du ändrar något av lead i Dynamics eller en person i Marketo återspeglas uppdateringen i båda systemen.

>[!NOTE]
>
>Borttagningar synkroniseras inte alltid automatiskt i båda riktningarna. Se [Ta bort en lead eller kontakt](http://docs.marketo.com/x/agO1Ag).

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Trots att detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM).

## Kan jag skapa en lead i Dynamics med Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, använd åtgärden [Synkronisera person till Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) -flöde. Detta skapar ett lead i Dynamics om leadet inte finns. Om leadet finns utför flödessteget ingen åtgärd.

>[!NOTE]
>
>När du använder flödesåtgärden &quot;Synkronisera person till Microsoft&quot; (endast i en utlösarkampanj) skapas lead/kontakt i realtid i Dynamics.

## Kan jag manuellt tvinga en synkronisering av en person från Marketo till ett lead i Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nej, den automatiska bakgrundssynkroniseringen är det enda sättet att synkronisera uppdateringar mellan Marketo och Dynamics. Åtgärden [Synkronisera person till Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) -flöde tvingar inte till en synkronisering av leadet.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [välja fält som ska synkroniseras](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) under installationen.

## Kommer Marketo att respektera Dynamics-valideringsreglerna? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Synkroniseringen misslyckas om dataformatet är fel eller om nödvändig fältinformation saknas. Marketo loggar resultatet i personens aktivitetslogg om detta händer.

