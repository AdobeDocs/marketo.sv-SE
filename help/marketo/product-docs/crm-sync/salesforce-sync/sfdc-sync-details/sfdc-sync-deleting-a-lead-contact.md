---
unique-page-id: 7515131
description: SFDC Sync - Tar bort en lead/kontakt - Marketo Docs - produktdokumentation
title: SFDC Sync - Ta bort en lead/kontakt
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# SFDC Sync: Ta bort en lead/kontakt {#sfdc-sync-deleting-a-lead-contact}

Här är några av detaljerna:

* Marketo tar inte automatiskt bort personer bara för att leads har tagits bort i [!DNL Salesforce]. I stället är fältet&quot;SFDC is Deleted&quot; satt till true. Om du vill kan du aktivera det här fältet och ta bort det i Marketo.
* [Flödesåtgärden Ta bort person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md). Detta tar bort en person i MKTO, men du kan också ta bort den i `Salesforce`.

* Flödesåtgärden [Ta bort från SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md): Detta tar bort ett lead i SFDC, men du kan även välja att ta bort en person i Marketo.
* Om ett lead tas bort i [!DNL Salesforce] (men en person inte tas bort i Marketo) och sedan körs genom flödesåtgärden [Synkronisera med  [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) skapas ett nytt lead i [!DNL Salesforce].
