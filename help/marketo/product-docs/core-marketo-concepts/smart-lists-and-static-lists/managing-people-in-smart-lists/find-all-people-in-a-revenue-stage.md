---
unique-page-id: 557331
description: Hitta alla personer på en intäktsscen - Marketo Docs - produktdokumentation
title: Söka efter alla personer i en intäktsfas
exl-id: aa5b30bf-96f1-4c1f-8170-86ba808e9705
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Söka efter alla personer i en intäktsfas {#find-all-people-in-a-revenue-stage}

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

## Sök efter alla medlemmar i en viss intäktsfas {#find-all-members-of-a-specific-revenue-stage}

1. I en smart lista klickar du på fliken **[!UICONTROL Smart List]**, letar upp filtret **[!UICONTROL Revenue Stage]** och drar det till arbetsytan.

   ![](assets/draginrevenuefilter.png)

1. Välj en **[!UICONTROL Revenue Stage]**.

   ![](assets/two.jpg)

1. Gå till fliken **[!UICONTROL People]** för att visa resultaten.

   ![](assets/peopleresults.jpg)

## Köra ett flödessteg på medlemmarna i en intäktsfas {#run-a-flow-step-on-the-members-of-a-revenue-stage}

Nu när ni vet vilka människor som befinner sig i vilka intäktsfaser kan ni marknadsföra direkt till dem. Förutom att välja **[!UICONTROL Revenue Stage]** som ett smart listfilter kan du även välja det som ett if-filter i flödet.

1. Klicka på **[!UICONTROL Add Choice]** i det önskade flödessteget och välj **[!UICONTROL Revenue Stage]** i listrutan.

   ![](assets/six.png)

   Därifrån kan du välja vilka medlemmar som ska påverkas av vilken aspekt av flödessteget.
