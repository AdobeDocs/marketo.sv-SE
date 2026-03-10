---
unique-page-id: 7516241
description: Läs om hur du tilldelar personer till Salesforce ledköer från Marketo. Använd Synkronisera person till SFDC eller Ändra ägarflödesåtgärder för lead-distribution.
title: SFDC Sync - lead-kö
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# SFDC Sync: Leadkö {#sfdc-sync-lead-queue}

Med Marketo kan du lägga till personer i [[!DNL Salesforce] lead-köer](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) för att hjälpa till med leaddistributionen. Här är detaljerna.

## Hur tilldelar man en person till en kö i Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Du kan tilldela en person till en [!DNL Salesforce]-lead-kö med någon av följande flödesåtgärder:

* [Synkronisera person till SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Ändra ägare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Du kan inte skapa eller ändra köer i Marketo.

## Hur lagras information om lead-ägare om personen tillhör en kö? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Om ett lead ägs av en kö i [!DNL Salesforce], behålls dessa säljägarfält tomma tills leadet tilldelas en ägare.

* Förnamn för försäljningsägare
* Förs.ägare efternamn
* Ägartitel för försäljning
* Försäljningsägarens telefonnummer
* E-postadress för säljare
