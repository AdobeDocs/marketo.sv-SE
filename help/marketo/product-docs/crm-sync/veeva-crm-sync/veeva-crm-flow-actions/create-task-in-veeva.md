---
description: Lär dig hur du skapar uppgifter i Veeva från Marketo för att informera säljarna om vad de ska göra och när. Använd steget Skapa uppgiftsflöde och anpassa ämne, beskrivning och förfallodatum.
title: Skapa aktivitet i  [!DNL Veeva]
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---

# Skapa aktivitet i [!DNL Veeva] {#create-task-in-veeva}

Som marknadsförare har ni information som kan hjälpa försäljningen att sluta avtal. Du kan skapa uppgifter för att tala om för dem vad de ska göra och när de ska göra det.

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>När Marketo Sync User skapar uppgifter är **[!UICONTROL Due In]** ett obligatoriskt fält för uppgiften som ska skapas i [!DNL Veeva]. Marketo anger fem dagar som standard om det inte finns något värde.

Som standard ser flödessteget ut så här:

![](assets/create-task-in-veeva-2.png)

Anpassa alla fält för att skapa uppgiften som du vill.

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>Du kan använda `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` och `{{system.tokens}}` i [!UICONTROL Subject] och [!UICONTROL Description]. Mer information finns i [Token för flödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}.
