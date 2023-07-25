---
unique-page-id: 7515131
description: SFDC-synkronisering - Tar bort en lead/kontakt - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Tar bort en lead/kontakt
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC-synkronisering: Ta bort en lead/kontakt {#sfdc-sync-deleting-a-lead-contact}

Här är några av detaljerna:

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i Salesforce. I stället anges flaggan &quot;SFDC is Deleted&quot; till true. Om du vill kan du aktivera det här fältet och ta bort det i Marketo.
* [Ta bort person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) flödesåtgärd. Detta tar bort en person i MKTO men du kan välja att ta bort i `Salesforce` också.

* [Ta bort från SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) flödesåtgärd: Detta tar bort ett lead i SFDC, men du kan även välja att ta bort en person i Marketo.
* Om ett lead tas bort i Salesforce (men en person inte tas bort i Marketo) och sedan körs det i [Synkronisera med Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flödesåtgärd, då skulle en ny lead skapas i Salesforce.
