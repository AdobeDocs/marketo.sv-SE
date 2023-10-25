---
unique-page-id: 3571840
description: Microsoft Dynamics Sync -User Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - användarsynkronisering
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Användarsynkronisering {#microsoft-dynamics-sync-user-sync}

Visste du att Marketo Engage synkroniserar hela databasen med Dynamics? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Dynamics-konton.

Du behöver en dedikerad Microsoft Dynamics CRM-användare för integreringen. Vi kallar den här användaren för Synkronisera användare.

## Hur synkroniseras användarinformationen mellan de två systemen? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Användarsynkroniseringen är ett sätt: Dynamics till Marketo. Om du gör ändringar för en användare i Dynamics återspeglas ändringarna i Marketo.

## Kan jag skapa en användare med Marketo? {#can-i-create-an-user-using-marketo}

Nej. Marketo kan inte skapa användare i Dynamics.

## Vilka fält ska synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

Du kan [markera fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} under installationen. Men Marketo synkroniserar bara de fält som din Dynamics-synkroniseringsanvändare har åtkomst till.
