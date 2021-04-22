---
unique-page-id: 7515131
description: SFDC-synkronisering -Tar bort en lead/kontakt - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Ta bort en lead/kontakt
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC-synkronisering: Ta bort en lead/kontakt {#sfdc-sync-deleting-a-lead-contact}

Här är några av detaljerna:

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i Salesforce. I stället anges flaggan &quot;SFDC is Deleted&quot; till true. Om du vill kan du aktivera det här fältet och ta bort det i Marketo.
* [Ta bort ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) anpassningsåtgärd. Detta tar bort en person i MKTO men du kan även ta bort den i `Salesforce`.

* [Åtgärden Ta bort från ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: Detta tar bort ett lead i SFDC, men du kan även välja att ta bort en person i Marketo.
* Om ett lead tas bort i Salesforce (men en person inte tas bort i Marketo) och sedan körs genom flödesåtgärden [Synkronisera med Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), skapas ett nytt lead i Salesforce.
