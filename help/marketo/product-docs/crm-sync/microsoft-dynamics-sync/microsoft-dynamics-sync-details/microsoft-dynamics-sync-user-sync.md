---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Användarsynkronisering - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync -Användarsynkronisering
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Användarsynkronisering {#microsoft-dynamics-sync-user-sync}

Visste du att Marketo synkroniserar hela databasen med Dynamics? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Dynamics-konton.

Du behöver en dedikerad Microsoft Dynamics CRM-användare för integreringen. Vi kallar den här användaren för Synkronisera användare.

## Hur synkroniseras användarinformationen mellan de två systemen? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Användarsynkroniseringen är ett sätt - Dynamics till Marketo. Om du ändrar en användare i Dynamics återspeglas ändringarna i Marketo.

## Kan jag skapa en användare med Marketo? {#can-i-create-an-user-using-marketo}

Nej. Marketo kan inte skapa användare i Dynamics.

## Vilka fält synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

Du kan [välja fält att synkronisera](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) under installationen. Marketo synkroniserar bara de fält som din Dynamics-synkroniseringsanvändare har åtkomst till.
