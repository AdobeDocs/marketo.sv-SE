---
unique-page-id: 3571836
description: Microsoft Dynamics Sync -Account Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync -Account Sync
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics] Synkronisering: Kontosynkronisering {#microsoft-dynamics-sync-account-sync}

Visste du att Marketo synkroniserar hela databasen med [!DNL Dynamics]? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar [!DNL Dynamics]-konton.

## På vilket sätt synkroniseras informationen? {#which-way-does-the-information-sync}

Endast ett sätt: från [!DNL Dynamics] till Marketo.

## Hur fungerar uppdateringarna? {#how-do-the-updates-work}

Om du uppdaterar ett kontofält för en kontakt i Marketo ändras värdena för alla kontakter som hör till det kontot i Marketo. Den synkroniseras inte till [!DNL Dynamics]. Nästa gång som kontot uppdateras i [!DNL Dynamics] åsidosätter dock ändringarna all kontoinformation i Marketo.

## Kan jag skapa ett konto med Marketo? {#can-i-create-an-account-using-marketo}

Nej. Marketo kan inte skapa konton i [!DNL Dynamics].

## Vilka fält ska synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

Du kan [välja fält som ska synkroniseras](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) under installationen. Men Marketo synkroniserar bara de fält som din [!DNL Dynamics]-synkroniseringsanvändare har åtkomst till.

## Kommer en ändring i ett kontofält i [!DNL Dynamics] att resultera i en aktivitetslogg för att ändra datavärde för varje kontakt?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

För det mesta, ja. Om ett konto har fler än 5 000 kontakter och ett fält på det kontot ändras i [!DNL Dynamics] synkroniseras ändringen men aktiviteten för de 5 000+ kontakterna loggas inte.
