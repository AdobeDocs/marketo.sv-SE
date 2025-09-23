---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sync -User Sync - Marketo Docs - Produktdokumentation
title: Microsoft [!DNL Dynamics] Synkronisera -Användarsynkronisering
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Microsoft [!DNL Dynamics] Synkronisera: Användarsynkronisering {#microsoft-dynamics-sync-user-sync}

Visste du att Marketo synkroniserar hela databasen med [!DNL Dynamics]? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar [!DNL Dynamics]-konton.

Du behöver en dedikerad Microsoft [!DNL Dynamics] CRM-användare för integreringen. Vi kallar den här användaren för Synkronisera användare.

## Hur synkroniseras användarinformationen mellan de två systemen? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Användarsynkroniseringen är ett sätt - [!DNL Dynamics] till Marketo. Om du gör ändringar för en användare i [!DNL Dynamics] återspeglas ändringarna i Marketo.

## Kan jag skapa en användare med Marketo? {#can-i-create-an-user-using-marketo}

Nej. Marketo kan inte skapa användare i [!DNL Dynamics].

## Vilka fält ska synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

Du kan [välja fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) under installationen. Men Marketo synkroniserar bara de fält som din [!DNL Dynamics]-synkroniseringsanvändare har åtkomst till.
