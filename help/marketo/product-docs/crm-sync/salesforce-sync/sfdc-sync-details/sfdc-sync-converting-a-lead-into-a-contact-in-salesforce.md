---
unique-page-id: 2953465
description: SFDC-synkronisering - Konvertera en lead till en kontakt i Salesforce - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Konvertera en lead till en kontakt i Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC-synkronisering: Konvertera en lead till en kontakt i Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Tänk dig tre olika scenarier i Salesforce: (används inte i [steget Konvertera person i flödet](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) i Marketo)

1. Konverterar en lead till en **ny kontakt och ett nytt konto**
1. Konverterar en lead till en **ny kontakt** i ett **befintligt konto**

1. Konverterar en lead till en **befintlig kontakt** i ett **befintligt konto** (fungerar identiskt med [sammanslagning](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

I alla tre fallen får du **1 kontakt och inga leads i Salesforce och 1 kontakt och inga personer i Marketo.**

I Marketo har posten nu SFDC-typ = kontakt.

>[!TIP]
>
>När du konverterar i Salesforce måste du se till att dina anpassade [lead-fält mappas bra](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Du vill inte förlora några data.

Du kan aktivera och filtrera med: &quot;Lead konverteras&quot; och &quot;Lead konverterades.&quot;
