---
unique-page-id: 1147017
description: Skapa aktivitet - Marketo Docs - produktdokumentation
title: Skapa uppgift
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---

# Skapa uppgift {#create-task}

Som marknadsförare har ni information som kan hjälpa försäljningen att sluta avtal. Du kan skapa uppgifter för att tala om för dem vad de ska göra och när de ska göra det.

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>När Marketo Sync User skapar uppgifter **[!UICONTROL Due In]** är ett obligatoriskt fält för uppgiften som ska skapas i Salesforce. Marketo anger fem dagar som standard om det inte finns något värde.

Som standard ser flödessteget ut så här:

![](assets/image2014-9-22-14-3a54-3a49.png)

Anpassa alla fält för att skapa uppgiften som du vill.

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>Du kan använda `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` och `{{system.tokens}}` i **[!UICONTROL Subject]** och **[!UICONTROL Description]**. Se [Token för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} för mer information.
