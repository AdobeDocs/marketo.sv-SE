---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - fältsynkronisering
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Fältsynkronisering {#microsoft-dynamics-sync-field-sync}

Synkroniseringen mellan Marketo Engage och Dynamics är superkraftfull. Här är detaljerna.

## Hur synkroniseras fältinformation mellan de två systemen? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är dubbelriktad för lead- och kontaktentiteter. Om du ändrar ett lead eller en kontakt i Dynamics eller en person i Marketo återspeglas uppdateringarna i båda systemen.

För konto, användare, affärsmöjlighet, team och anpassade entiteter är synkroniseringen en enkelriktad åtgärd: Dynamics till Marketo. Om du ändrar något i de här enheterna i Dynamics återspeglas dina uppdateringar i Marketo.

## Vad händer om samma fält ändras i båda systemen samtidigt? (datakollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Även om detta är sällsynt kommer Marketo att vinna för människor (leads) och Dynamics kommer att vinna för kontakter. Detta beror på att vi anser att marknadsföringsavdelningen är auktoritativ för människor, medan det officiella systemet för kontakter finns på försäljningsavdelningen (CRM). För enkelriktade synkroniseringsenheter vinner Dynamics alltid.

## Kan jag skapa ett fält i Dynamics med Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Nej, det stöds inte för närvarande.

## Jag skapade ett fält i Dynamics. Kan jag synkronisera den till Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, du kan [synkronisera fältet](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} så länge din synkroniseringsanvändare har åtkomst till det i Dynamics.

## Vilka fält synkroniseras med Marketo? {#what-fields-will-sync-to-marketo}

Du kan [välja fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} under installationen.

## Vad händer om jag behöver lägga till ett anpassat fält efter att Marketo och Dynamics har synkroniserats? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Du kan lägga till fält när som helst och förvänta dig att data uppdateras från Dynamics till Marketo. Mer information finns i [Använd snabbsynkronisering med Microsoft Dynamics för ett nytt anpassat fält](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md){target="_blank"}.

## Vad händer om jag vill ta bort ett fält i Dynamics efter att fältet har lagts till för synkronisering? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo lagrar en referens till de fält som ska synkroniseras. Om du tar bort ett fält i Dynamics rekommenderar vi att du gör det med [synkroniseringen inaktiverad](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Uppdatera sedan schemat i Marketo genom att redigera och spara [Markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.
