---
unique-page-id: 37356429
description: Skapa uppgift i Microsoft - Marketo Docs - produktdokumentation
title: Skapa uppgift i Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Skapa uppgift i Microsoft {#create-task-in-microsoft}

Som marknadsförare har ni information som kan hjälpa försäljningen att sluta avtal. Du kan skapa uppgifter för att tala om för dem vad de ska göra och när de ska göra det.

Skapa uppgift i Microsoft skapar en aktivitet under Aktiviteter som är relaterade till personen (lead eller kontakt) i [!DNL Microsoft].

>[!NOTE]
>
>Det här flödessteget _fungerar bara när de används med utlösare_, inte filter, i er smarta kampanj.

Som standard ser flödessteget ut så här:

![](assets/msd1.png)

>[!NOTE]
>
>När Marketo Sync User skapar uppgifter **[!UICONTROL Due In]** är ett obligatoriskt fält för uppgiften som ska skapas i [!DNL Microsoft]. Marketo anger fem dagar som standard om inget värde anges.

Anpassa alla fält för att skapa uppgiften som du vill.

![](assets/msd2.png)

>[!NOTE]
>
>Fältet &quot;Status&quot; som anges för aktiviteten i Flow Action uppdaterar fältet: &quot;Status Reason&quot; i [!DNL Microsoft].

>[!TIP]
>
>Du kan använda `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` och `{{system.tokens}}` i **[!UICONTROL Subject]** och **[!UICONTROL Description]**. Se [Token för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} för mer information.
