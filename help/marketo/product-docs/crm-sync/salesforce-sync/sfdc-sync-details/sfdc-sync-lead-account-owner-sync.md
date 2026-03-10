---
unique-page-id: 2953463
description: Läs om hur lead- och kontoägarfält synkroniseras från Salesforce till Marketo. Ändra huvudägare i Marketo och använd ägardata i flödesåtgärder och smarta listor.
title: SFDC Sync - synkronisering av lead-/kontoägare
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '230'
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
