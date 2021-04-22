---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - fältsynkronisering
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Fältsynkronisering {#microsoft-dynamics-sync-field-sync}

Synkroniseringen mellan Marketo och Dynamics är superkraftfull. Här är detaljerna.

## Hur synkroniseras fältinformation mellan de två systemen? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad för lead- och kontaktentiteter. Om du ändrar ett lead eller en kontakt i Dynamics eller en person i Marketo återspeglas uppdateringarna i båda systemen.

Synkroniseringen är envägs för konton, användare, affärstillfällen, team och anpassade entiteter: Dynamics till Marketo. Om du ändrar något i de här enheterna i Dynamics återspeglas dina uppdateringar i Marketo.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Även om detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM). För enkelriktade synkroniseringsenheter vinner Dynamics alltid.

## Kan jag skapa ett fält i Dynamics med Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Nej, det stöds inte för närvarande.

## Jag skapade ett fält i Dynamics. Kan jag synkronisera den till Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, du kan [synkronisera fältet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) så länge din synkroniseringsanvändare har åtkomst till det i Dynamics.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [välja fält att synkronisera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) under installationen.

## Vad händer om jag behöver lägga till ett anpassat fält efter att Marketo och Dynamics har synkroniserats? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Du kan lägga till fält när som helst och förvänta dig att data uppdateras från Dynamics till Marketo. Mer information finns i [Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).

## Vad händer om jag vill ta bort ett fält i Dynamics efter att fältet har lagts till för synkronisering? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo lagrar en referens till de fält som ska synkroniseras. Om du tar bort ett fält i Dynamics rekommenderar vi att du gör det med [synkroniseringen inaktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Uppdatera sedan schemat i Marketo genom att redigera och spara [Välj fält att synkronisera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
