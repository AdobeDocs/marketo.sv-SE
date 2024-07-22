---
unique-page-id: 2953467
description: SFDC-synkronisering - Affärsmöjlighet, synkronisering - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Affärsmöjlighet synkroniserad
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# SFDC-synkronisering: Affärsmöjlighet synkroniserad {#sfdc-sync-opportunity-sync}

## Hur synkroniseras informationen om affärsmöjligheterna mellan de två systemen? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Synkroniseringen är ett sätt: från Salesforce till Marketo Engage. Uppdateringar av affärsmöjligheter i Salesforce synkroniseras med Marketo.

>[!NOTE]
>
>De [autentiseringsuppgifter du anger i Marketo för Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} används för att synkronisera data. Endast data som dessa autentiseringsuppgifter har åtkomst till inkluderas.

## Kan jag starta en säljprojektssynkronisering? {#can-i-initiate-an-opportunity-sync}

Nej, det kan du inte. Ändringarna i alla affärsmöjligheter i Salesforce synkroniseras automatiskt till Marketo.

## Har Marketo stöd för mer än en valuta i säljprojektsbeloppet? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Nej, Marketo har bara stöd för en valuta. Affärsmöjlighetsbeloppet synkroniseras från Salesforce, men valutan blir [standardvalutan](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"} i din Marketo-prenumeration.

## Hur kopplar Marketo möjligheter och kontakter? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associerar affärsmöjligheter och kontakter med [Roller för säljprojektskontakt](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Möjligheter utan tilldelade kontaktroller synkroniseras med Marketo, men tillhör inte någon. Personen kvalificerar till exempel inte filtret Har affärsmöjlighet.

## Hur kan jag se alla möjligheter för en person? {#how-can-i-see-all-the-opportunities-of-a-person}

Du kan visa en lista över affärsmöjligheter på fliken **Information om säljprojekt** på sidan [Personinformation](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} .

## Vilka utlösare/filter hör till affärsmöjligheten? {#what-are-the-triggers-filters-related-to-opportunity}

Utlösare:

* Tillagd i affärsmöjlighet
* Borttagen från affärsmöjligheten
* Möjligheten har uppdaterats

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
>Se begränsningarna för filter och utlösare. Massor av coola detaljer där inne.
>
>Gör bara ett nytt fält i affärsmöjlighetsobjektet i Salesforce så blir det automatiskt en begränsning!
