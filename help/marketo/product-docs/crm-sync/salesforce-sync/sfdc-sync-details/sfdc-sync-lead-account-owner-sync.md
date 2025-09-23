---
unique-page-id: 2953463
description: SFDC Sync - synkronisering av lead-/kontoägare - Marketo Docs - produktdokumentation
title: SFDC Sync - synkronisering av lead-/kontoägare
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# SFDC Sync: Synkronisering av lead-/kontoägare {#sfdc-sync-lead-account-owner-sync}

De här synkroniserar tekniskt tabellen &quot;användare&quot; i [!DNL Salesforce], men vi kommer att hänvisa till den som fält för lead-/kontoägare.

## Vilka fält ska synkroniseras med Marketo Engage? {#which-fields-will-sync-to-marketo-engage}

För varje person som synkroniseras till Marketo synkroniseras även följande ägarfält:

* Förnamn för försäljningsägare
* Förs.ägare efternamn
* Ägartitel för försäljning
* Försäljningsägarens telefonnummer
* E-postadress för säljare

För varje kontakt synkroniserar vi de fem ovanstående fälten för lead-ägare samt de här fälten för kontoägare:

* Förnamn för kontoägare
* Kontoägarens efternamn
* E-postadress för kontoägare

## Kan jag byta huvudägare i Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolut, använd bara flödesåtgärden [Ändra ägare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Du kan inte ändra ägarinformationen med hjälp av [Personinformationssidan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Vad kan jag göra med dessa data? {#what-can-i-do-with-this-data}

Det finns många skäl att använda dessa data, till exempel

* Skicka ett personligt e-postmeddelande med signatur från säljaren
* Filtrera på specifika säljare för marknadsföring eller till och med för att analysera effektiviteten
* Uppdragsregler (och omtilldelning) i Marketo
* Använd dem i flödesåtgärderna [Ändra ägare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} och [Skapa aktivitet](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

Marketo har en toppensynkronisering av [!DNL Salesforce]. Ingen annan gör det så bra!
