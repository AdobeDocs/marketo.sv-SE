---
unique-page-id: 7516241
description: SFDC Sync -Lead Queue - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Lead-kö
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# SFDC-synkronisering: Leadkö {#sfdc-sync-lead-queue}

Med Marketo kan du lägga till personer i [Salesforce lead-köer](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) för att hjälpa till med lead-distributionen. Här är detaljerna.

## Hur tilldelar du en person till en kö i Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Du kan tilldela en person till en Salesforce-lead-kö med någon av följande flödesåtgärder:

* [Synkronisera person till SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Ändra ägare](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Du kan inte skapa eller ändra köer i Marketo.

## Hur lagras information om lead-ägare om personen tillhör en kö? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Om ett lead ägs av en kö i Salesforce, behålls dessa säljarfält tomma tills leadet tilldelas en ägare.

* Förnamn för försäljningsägare
* Förs.ägare efternamn
* Ägartitel för försäljning
* Försäljningsägarens telefonnummer
* E-postadress för säljare

