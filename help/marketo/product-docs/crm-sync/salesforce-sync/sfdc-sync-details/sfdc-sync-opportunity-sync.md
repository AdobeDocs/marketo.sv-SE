---
unique-page-id: 2953467
description: SFDC Sync -Opportunity Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Affärsmöjlighet - synkronisering
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# SFDC-synkronisering: Synkronisering av affärsmöjlighet {#sfdc-sync-opportunity-sync}

## Hur synkroniseras informationen om affärsmöjligheterna mellan de två systemen? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är ett sätt: från Salesforce till Marketo. Uppdateringar av affärsmöjligheter i Salesforce synkroniseras med Marketo.

>[!NOTE]
>
>De [autentiseringsuppgifter du anger i Marketo för Salesforce](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

## Kan jag starta en säljprojektssynkronisering? {#can-i-initiate-an-opportunity-sync}

Nej, det kan du inte. Ändringarna i alla affärsmöjligheter i Salesforce synkroniseras automatiskt till Marketo.

## Stöder Marketo mer än en valuta i säljprojektsbeloppet? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Nej, Marketo stöder bara en valuta. Affärsmöjlighetsbeloppet synkroniseras från Salesforce, men valutan blir [standardvalutan](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription) i din Marketo-prenumeration.

## Hur kopplar Marketo möjligheter och kontakter? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associerar affärsmöjligheter och kontakter med hjälp av [säljprojektskontaktroller](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Affärsmöjligheter utan tilldelade kontaktroller synkroniseras med Marketo, men tillhör inte någon. Personen kvalificerar till exempel inte filtret Har affärsmöjlighet.

## Hur kan jag se alla möjligheter för en person? {#how-can-i-see-all-the-opportunities-of-a-person}

Du kan visa en lista med affärsmöjligheter på fliken **Affärsinformation** på sidan [Personinformation](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) .

## Vilka utlösare/filter hör till affärsmöjligheten? {#what-are-the-triggers-filters-related-to-opportunity}

Utlösare:

* Tillagd i affärsmöjlighet
* Borttagen från affärsmöjligheten
* Affärsmöjligheten har uppdaterats

Filter:

* Har möjlighet
* Affärsmöjligheten har uppdaterats/affärsmöjligheten har inte uppdaterats
* lades till i affärsmöjligheten/lades inte till i affärsmöjligheten
* Borttagen från affärsmöjligheten/inte togs bort från affärsmöjligheten
* Totalt tomt belopp
* Antal optyer
* Förväntad intäkt för total optisk summa

>[!TIP]
>
>Ta en titt på begränsningarna för filter och utlösare. Massor av coola detaljer där inne.
>
>Gör bara ett nytt fält i affärsmöjlighetsobjektet i Salesforce så blir det automatiskt en begränsning!

Marketo har den bästa Salesforce-synkroniseringen i världen!