---
unique-page-id: 2953463
description: SFDC Sync -Lead/Account Owner Sync - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Synkronisering av lead-/kontoägare
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# SFDC-synkronisering: Lead-/kontoägarsynkronisering {#sfdc-sync-lead-account-owner-sync}

Dessa synkroniserar tekniskt tabellen &quot;användare&quot; i Salesforce, men vi kommer att hänvisa till den som lead-/kontoägarfält.

## Vilka fält synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

För varje person som synkroniseras till Marketo synkroniserar vi även följande ägarfält:

* Förnamn för försäljningsägare
* Förs.ägare efternamn
* Ägartitel för försäljning
* Försäljningsägarens telefonnummer
* E-postadress för säljare

För varje kontakt synkroniserar vi de fem ovanstående fälten för lead-ägare samt de här fälten för kontoägare:

* Förnamn för kontoägare
* Kontoägarens efternamn
* E-postadress för kontoägare

## Kan jag ändra huvudägaren i Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolut, använd bara flödesåtgärden [Ändra ägare](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Du kan inte ändra ägarinformationen med hjälp av [Personinformationssidan](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Vad kan jag göra med dessa data? {#what-can-i-do-with-this-data}

Det finns många skäl att använda dessa data, till exempel

* Skicka ett personligt e-postmeddelande med signatur från säljaren
* Filtrera på specifika säljare för marknadsföring eller till och med för att analysera effektiviteten
* Tilldelningsregler (och omtilldelningsregler) i Marketo
* Använd dem i flödesuppgifterna [Ändra ägare](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Synkronisera person till SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) och [Skapa aktivitet](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo har en fantastisk Salesforce-synkronisering. Ingen annan gör det så bra!
