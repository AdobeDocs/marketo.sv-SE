---
unique-page-id: 2953459
description: SFDC Sync -Account Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - kontosynkronisering
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# SFDC-synkronisering: Kontosynkronisering {#sfdc-sync-account-sync}

Marketo synkroniserar även din kontoinformation med Salesforce. Här är några specifika saker du bör känna till!

## På vilket sätt synkroniseras informationen? {#which-way-does-the-information-sync}

Bara ett sätt: från SFDC till Marketo.

## Hur fungerar uppdateringarna? {#how-do-the-updates-work}

Om du uppdaterar ett kontofält för en kontakt i Marketo, ändras värdena för alla kontakter som tillhör det kontot i Marketo. Den synkroniseras inte till SFDC. Nästa gång som kontot uppdateras i SFDC kommer dock ändringarna att åsidosätta all kontoinformation i Marketo.

## Kan en kontakt tillhöra flera konton?  {#can-a-contact-belong-to-multiple-accounts}

Nej. Ett konto kan ha många kontakter, en kontakt kan bara ha ett konto.

## Kan jag skapa konton från Marketo? {#can-i-create-accounts-from-marketo}

För det mesta, nej. Om du däremot använder flödessteget [Konvertera person](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) för en person skapas en ny kontakt, ett nytt konto och ett nytt säljprojekt.

>[!CAUTION]
>
>Det här flödessteget har mycket begränsad användning. Om du inte är säker bör du antagligen inte använda den.

## Blir en ändring av ett kontofält i Salesforce en aktivitetslogg för att ändra datavärde för varje kontakt?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

För det mesta, ja. Om ett konto har fler än 5 000 kontakter och ett fält på det kontot ändras i SFDC, synkroniseras ändringen men aktiviteten loggas inte för de mer än 5 000 kontakterna.
