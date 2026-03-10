---
unique-page-id: 2953459
description: Läs om hur kontoinformation synkroniseras från Salesforce till Marketo. Förstå envägssynkronisering, kontaktkontorelation och skapande av konton via Konvertera person.
title: SFDC Sync - kontosynkronisering
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# SFDC Sync: Kontosynkronisering {#sfdc-sync-account-sync}

Marketo synkroniserar även din kontoinformation med [!DNL Salesforce]. Här är några specifika saker du bör känna till!

## På vilket sätt synkroniseras informationen? {#which-way-does-the-information-sync}

Bara ett sätt: från SFDC till Marketo.

## Hur fungerar uppdateringarna? {#how-do-the-updates-work}

Om du uppdaterar ett kontofält för en kontakt i Marketo ändras värdena för alla kontakter som hör till det kontot i Marketo. Den synkroniseras inte med SFDC. Nästa gång kontot uppdateras i SFDC kommer dock ändringarna att åsidosätta all kontoinformation i Marketo.

## Kan en kontakt tillhöra flera konton?  {#can-a-contact-belong-to-multiple-accounts}

Nej. Ett konto kan ha många kontakter, en kontakt kan bara ha ett konto.

## Kan jag skapa konton från Marketo? {#can-i-create-accounts-from-marketo}

För det mesta, nej. Om du däremot använder flödessteget [Konvertera person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} för en person skapas en ny kontakt, ett nytt konto och ett nytt säljprojekt.

>[!CAUTION]
>
>Det här flödessteget har mycket begränsad användning. Om du inte är säker bör du antagligen inte använda den.

## Gör en ändring i ett kontofält i [!DNL Salesforce] en aktivitetslogg för att ändra datavärde för varje kontakt?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

För det mesta, ja. Om ett konto har fler än 5 000 kontakter och ett fält på det kontot ändras i SFDC, synkroniseras ändringen men aktiviteten för de 5 000+ kontakterna loggas inte.
