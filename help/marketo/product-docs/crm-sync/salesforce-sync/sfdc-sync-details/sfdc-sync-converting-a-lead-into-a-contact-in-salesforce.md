---
unique-page-id: 2953465
description: SFDC-synkronisering - Konvertera en lead till en kontakt i Salesforce - Marketo Docs - produktdokumentation
title: SFDC-synkronisering - Konverterar en lead till en kontakt i Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# SFDC-synkronisering: Konvertera en lead till en kontakt i Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Tänk dig tre olika scenarier i Salesforce: (använd inte [Konvertera personflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} i Marketo Engage)

1. Konvertera en lead till en **ny kontakt och nytt konto**
1. Konvertera en lead till en **ny kontakt** i en **befintligt konto**

1. Konvertera en lead till en **befintlig kontakt** i en **befintligt konto** (fungerar identiskt med [sammanfoga](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

I alla tre fallen får du **1 kontakt och inga leads i Salesforce och 1 kontakt och inga personer i Marketo.**

I Marketo har posten nu SFDC-typ = kontakt.

>[!TIP]
>
>När du konverterar i Salesforce bör du kontrollera att [anpassade huvudfält är väl mappade](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Du vill inte förlora några data.

Du kan aktivera och filtrera med hjälp av: &quot;Lead is Converted&quot; och &quot;Lead was Converted.&quot;
