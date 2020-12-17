---
unique-page-id: 3571836
description: Microsoft Dynamics Sync -Account Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - kontosynkronisering
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Kontosynkronisering {#microsoft-dynamics-sync-account-sync}

Visste du att Marketo synkroniserar hela databasen med Dynamics? Den synkas, väntar sedan i 5 minuter och synkas igen, hela dagen, varje dag. Här är några detaljer om hur Marketo specifikt behandlar Dynamics-konton.

## På vilket sätt synkroniseras informationen? {#which-way-does-the-information-sync}

Bara ett sätt: från Dynamics till Marketo.

## Hur fungerar uppdateringarna? {#how-do-the-updates-work}

Om du uppdaterar ett kontofält för en kontakt i Marketo, ändras värdena för alla kontakter som tillhör det kontot i Marketo. Den synkroniseras inte med Dynamics. Nästa gång som kontot uppdateras i Dynamics kommer dock ändringarna att åsidosätta all kontoinformation i Marketo.

## Kan jag skapa ett konto med Marketo? {#can-i-create-an-account-using-marketo}

Nej. Marketo kan inte skapa konton i Dynamics.

## Vilka fält synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

Du kan [välja fält att synkronisera](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) under installationen. Marketo synkroniserar bara de fält som din Dynamics-synkroniseringsanvändare har åtkomst till.

## Blir en ändring i ett kontofält i Dynamics en aktivitetslogg för att ändra datavärde för varje kontakt?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

För det mesta, ja. Om ett konto har fler än 5 000 kontakter och ett fält på det kontot ändras i Dynamics, synkroniseras ändringen men aktiviteten för de 5 000+ kontakterna loggas inte.
