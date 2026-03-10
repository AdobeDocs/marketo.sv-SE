---
unique-page-id: 2953465
description: Läs mer om vad som händer när du konverterar ett lead till en kontakt i Salesforce. Se hur Marketo återspeglar förändringen och hur Lead används är Konverterade utlösare och filter.
title: SFDC Sync - Konvertera en lead till en kontakt i Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC Sync: Konverterar en lead till en kontakt i [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Tänk dig tre olika scenarier i [!DNL Salesforce]: (använder inte [&#x200B; Konvertera personflödessteg &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) i Marketo)

1. Konverterar en lead till en **ny kontakt och ett nytt konto**
1. Konverterar en lead till en **ny kontakt** i ett **befintligt konto**

1. Konverterar en lead till en **befintlig kontakt** i ett **befintligt konto** (fungerar på samma sätt som [sammanslagning](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

I alla tre fallen får du **1-kontakt och inga leads i [!DNL Salesforce] och 1-kontakt och inga personer i Marketo.**

I Marketo har posten nu SFDC Type = Contact.

>[!TIP]
>
>När du konverterar i [!DNL Salesforce] måste du se till att dina anpassade [lead-fält mappas korrekt](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Du vill inte förlora några data.

Du kan aktivera och filtrera med: [!UICONTROL Lead is Converted] och [!UICONTROL Lead was Converted].
