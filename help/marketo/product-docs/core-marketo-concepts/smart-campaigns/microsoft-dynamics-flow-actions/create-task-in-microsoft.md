---
unique-page-id: 37356429
description: Skapa aktivitet i Microsoft - Marketo Docs - Produktdokumentation
title: Skapa uppgift i Microsoft
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Skapa aktivitet i Microsoft {#create-task-in-microsoft}

Som marknadsförare har ni information som kan hjälpa försäljningen att sluta avtal. Du kan skapa uppgifter för att tala om för dem vad de ska göra och när de ska göra det.

Skapa uppgift i Microsoft skapar en uppgift under Aktiviteter som är relaterade till personen (lead eller kontakt) i Microsoft.

>[!NOTE]
>
>Det här flödessteget **fungerar bara när det används med utlösare**, inte filter, i den smarta kampanjen.

Som standard ser flödessteget ut så här:

![](assets/msd1.png)

>[!NOTE]
>
>När Marketo Sync User skapar uppgifter är **Förfallodatum** ett obligatoriskt fält för uppgiften som ska skapas i Microsoft. Marketo anger fem dagar som standard om inget värde anges.

Anpassa alla fält för att skapa uppgiften som du vill.

![](assets/msd2.png)

>[!NOTE]
>
>Fältet &quot;Status&quot; som anges för aktiviteten i Flow Action uppdaterar fältet: &quot;Statusorsak&quot; i Microsoft.

>[!TIP]
>
>Du kan använda `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` och `{{system.tokens}}` i **Subject** och **Beskrivning**. Mer information finns i [Tokens for Flow Steps](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).
