---
unique-page-id: 37356429
description: Skapa uppgift i Microsoft - Marketo Docs - produktdokumentation
title: Skapa uppgift i Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Skapa uppgift i Microsoft {#create-task-in-microsoft}

Som marknadsförare har ni information som kan hjälpa försäljningen att sluta avtal. Du kan skapa uppgifter för att tala om för dem vad de ska göra och när de ska göra det.

Skapa uppgift i Microsoft skapar en uppgift under Aktiviteter som är relaterade till personen (lead eller kontakt) i Microsoft.

>[!NOTE]
>
>Det här flödessteget **fungerar bara när de används med utlösare**, inte filter, i er smarta kampanj.

Som standard ser flödessteget ut så här:

![](assets/msd1.png)

>[!NOTE]
>
>När Marketo Sync User skapar uppgifter **Förfaller** är ett obligatoriskt fält för uppgiften som ska skapas i Microsoft. Marketo anger fem dagar som standard om inget värde anges.

Anpassa alla fält för att skapa uppgiften som du vill.

![](assets/msd2.png)

>[!NOTE]
>
>Fältet &quot;Status&quot; som anges för aktiviteten i Flow Action uppdaterar fältet: &quot;Statusorsak&quot; i Microsoft.

>[!TIP]
>
>Du kan använda `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` och `{{system.tokens}}` i **Ämne** och **Beskrivning**. Se [Token för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) för mer information.
