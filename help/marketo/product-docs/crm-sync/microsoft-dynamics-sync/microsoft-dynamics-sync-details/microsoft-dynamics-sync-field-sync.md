---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - fältsynkronisering
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Fältsynkronisering {#microsoft-dynamics-sync-field-sync}

Marketo to Dynamics sync är superkraftfull. Här är detaljerna.

## Hur synkroniseras fältinformation mellan de två systemen? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad för lead- och kontaktentiteter. Om du ändrar ett lead eller en kontakt i Dynamics eller en person i Marketo återspeglas dina uppdateringar i båda systemen.

Synkroniseringen är envägs för konton, användare, affärstillfällen, team och anpassade entiteter: Dynamics till Marketo. Om du gör ändringar i de här enheterna i Dynamics återspeglas dina uppdateringar i Marketo.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Trots att detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM). För enkelriktade synkroniseringsenheter vinner Dynamics alltid.

## Kan jag skapa ett fält i Dynamics med Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Nej, det stöds inte för närvarande.

## Jag skapade ett fält i Dynamics. Kan jag synkronisera den till Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, du kan [synkronisera fältet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) så länge din synkroniseringsanvändare har åtkomst till det i Dynamics.

Vilka fält synkroniseras med Marketo?

Du kan [välja fält att synkronisera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) under installationen.

## Vad händer om jag behöver lägga till ett anpassat fält efter att Marketo och Dynamics har synkroniserats? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Du kan lägga till fält när som helst och förvänta dig att data uppdateras från Dynamics till Marketo. Mer information finns i [Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).
