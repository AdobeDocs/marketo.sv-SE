---
unique-page-id: 7515131
description: SFDC-synkronisering -Tar bort en lead/kontakt - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Ta bort en lead/kontakt
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# SFDC-synkronisering: Ta bort en lead/kontakt {#sfdc-sync-deleting-a-lead-contact}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Här är några av detaljerna:

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i Salesforce. I stället anges flaggan &quot;SFDC is Deleted&quot; till true. Om du vill kan du aktivera det här fältet och ta bort det i Marketo.
* [Åtgärden Ta bort](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) personflöde. Detta tar bort en person i MKTO, men du kan även välja att ta bort den i `Salesforce` .

* [Åtgärd för att ta bort från SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) -flöde: Detta tar bort ett lead i SFDC, men du kan även välja att ta bort en person i Marketo.
* Om ett lead tas bort i Salesforce (men en person inte tas bort i Marketo) och sedan körs genom [synkroniseringen med Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) -flödesåtgärden, skapas ett nytt lead i Salesforce.

Med andra ord fungerar det som magi!

![--](assets/image2015-5-20-15-3a3-3a27.png)

