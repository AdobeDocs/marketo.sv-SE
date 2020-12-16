---
unique-page-id: 2953465
description: SFDC-synkronisering - Konvertera en lead till en kontakt i Salesforce - Marketo Docs - Produktdokumentation
title: SFDC-synkronisering - Konvertera en lead till en kontakt i Salesforce
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC-synkronisering: Konvertera en lead till en kontakt i Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Tänk dig tre olika scenarier i Salesforce: (som inte använder flödessteget [](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) Konvertera person i Marketo)

1. Konvertera en lead till en **ny kontakt och ett nytt konto**
1. Konvertera en lead till en **ny kontakt** i ett **befintligt konto**

1. Konvertera en lead till en **befintlig kontakt** i ett **befintligt konto** (fungerar på samma sätt som [sammanslagning](sfdc-sync-merging-a-lead-contact-person.md))

I alla tre fallen får du **1 kontakt och inga leads i Salesforce och 1 kontakt och inga personer i Marketo.**

I Marketo har posten nu SFDC-typ = kontakt.

>[!TIP]
>
>När du konverterar i Salesforce måste du se till att dina anpassade [lead-fält mappas bra](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Du vill inte förlora några data.

Du kan aktivera och filtrera med: &quot;Lead konverteras&quot; och &quot;Lead konverterades.&quot;