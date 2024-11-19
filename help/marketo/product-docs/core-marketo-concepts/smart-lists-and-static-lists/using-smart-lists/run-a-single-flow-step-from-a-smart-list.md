---
unique-page-id: 557322
description: Köra ett enda flödessteg från en smart lista - Marketo Docs - produktdokumentation
title: Köra ett enda flödessteg från en smart lista
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: e0106eddf3ed6ecd2d9d90147a56258f61958665
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# Köra ett enda flödessteg från en smart lista {#run-a-single-flow-step-from-a-smart-list}

Om du vill köra ett enda steg för ett enda flöde kan du använda ett enda flödessteg i en smart lista i stället för att skapa en hel smart kampanj.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. Välj en lista eller Smart List med personer i den och gå sedan till fliken **[!UICONTROL People]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >Både statiska listor och smarta listor har den här funktionen.

1. Klicka på **[!UICONTROL Select All]**. Du kan också använda **Ctrl/Cmd** och klicka för att markera några poster manuellt.

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >Om resultatet sträcker sig över flera sidor, kan du klicka på **[!UICONTROL Select All]** för att markera alla personer på alla sidor.

1. Välj önskat flödessteg under **[!UICONTROL Person Actions]**. I det här exemplet använder vi [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. Sök efter och välj en **[!UICONTROL Attribute]**. I det här exemplet ska vi ta alla som har delstat&quot;Kalifornien&quot; och ändra det till&quot;Kalifornien&quot;.

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. Ange ett nytt värde. Klicka på **[!UICONTROL Run Now]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. Om du ändrar datavärden för ett stort antal personer kan du behöva bekräfta ändringen genom att skriva in talet. Klicka på **[!UICONTROL Go For It]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

Fantastiskt arbete! Status för det enskilda flödessteget visas i det övre högra hörnet.

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

Uppdatera listan när den är klar så ser du den uppdaterade informationen.
