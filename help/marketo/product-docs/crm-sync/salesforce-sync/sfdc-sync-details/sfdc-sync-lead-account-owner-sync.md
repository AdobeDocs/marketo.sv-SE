---
unique-page-id: 2953463
description: SFDC-synkronisering - synkronisering av lead-/kontoägare - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - synkronisering av lead-/kontoägare
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC-synkronisering: Synkronisering av lead-/kontoägare {#sfdc-sync-lead-account-owner-sync}

Dessa synkroniserar tekniskt tabellen &quot;användare&quot; i Salesforce, men vi kommer att hänvisa till den som lead-/kontoägarfält.

## Vilka fält synkroniseras med Marketo? {#which-fields-will-sync-to-marketo}

För varje person som synkroniseras till Marketo synkroniseras även följande ägarfält:

* Förnamn för försäljningsägare
* Förs.ägare efternamn
* Ägartitel för försäljning
* Försäljningsägarens telefonnummer
* E-postadress för säljare

För varje kontakt synkroniseras de fem ovanstående fälten för lead-ägare samt de här fälten för kontoägare:

* Förnamn för kontoägare
* Kontoägarens efternamn
* E-postadress för kontoägare

## Kan jag byta huvudägare i Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolut, använd bara [Ändra ägare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) flödesåtgärd.

>[!NOTE]
>
>Du kan inte ändra ägarinformationen med [Använda personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Vad kan jag göra med dessa data? {#what-can-i-do-with-this-data}

Det finns många skäl att använda dessa data, till exempel

* Skicka ett personligt e-postmeddelande med signatur från säljaren
* Filtrera på specifika säljare för marknadsföring eller till och med för att analysera effektiviteten
* Uppdragsregler (och omtilldelning) i Marketo
* Använd dem i [Ändra ägare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)och [Skapa uppgift](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) flödesåtgärder

Marketo har verkligen en fantastisk Salesforce-synkronisering. Ingen annan gör det så bra!
