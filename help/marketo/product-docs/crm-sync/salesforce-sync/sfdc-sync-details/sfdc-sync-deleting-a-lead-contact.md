---
unique-page-id: 7515131
description: SFDC-synkronisering -Tar bort en lead/kontakt - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Ta bort en lead/kontakt
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# SFDC-synkronisering: Ta bort en lead/kontakt {#sfdc-sync-deleting-a-lead-contact}

Här är några av detaljerna:

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i Salesforce. I stället anges flaggan &quot;SFDC is Deleted&quot; till true. Om du vill kan du aktivera det här fältet och ta bort det i Marketo.
* [Ta bort ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) anpassningsåtgärd. Detta tar bort en person i MKTO men du kan även ta bort den i `Salesforce`.

* [Åtgärden Ta bort från ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: Detta tar bort ett lead i SFDC, men du kan även välja att ta bort en person i Marketo.
* Om ett lead tas bort i Salesforce (men en person inte tas bort i Marketo) och sedan körs genom flödesåtgärden [Synkronisera med Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), skapas ett nytt lead i Salesforce.

Med andra ord fungerar det som magi!

![—](assets/image2015-5-20-15-3a3-3a27.png)

