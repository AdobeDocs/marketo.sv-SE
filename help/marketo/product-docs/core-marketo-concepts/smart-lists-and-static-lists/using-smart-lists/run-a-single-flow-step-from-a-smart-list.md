---
unique-page-id: 557322
description: Köra ett enda flödessteg från en smart lista - Marketo Docs - Produktdokumentation
title: Köra ett enda flödessteg från en smart lista
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Kör ett enskilt flödessteg från en smart lista {#run-a-single-flow-step-from-a-smart-list}

Om du vill köra ett enda steg för ett enda flöde kan du använda ett enda flödessteg i en smart lista i stället för att skapa en hel smart kampanj.

>[!PREREQUISITES]
>
>* [Skapa en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

>



1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Välj en lista eller smart lista med personer i den och gå sedan till fliken **Personer**.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Både statiska listor och smarta listor har den här funktionen.

1. Klicka på **Markera alla**. Du kan också använda** Ctrl/Cmd** och klicka för att markera några poster manuellt.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Om resultatet sträcker sig över flera sidor och du klickar på **Markera alla** markeras alla personer på alla sidor.

1. Välj önskat flödessteg under **Person** **Åtgärder**. I det här exemplet använder vi [Ändra datavärde](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Sök efter och välj ett **attribut**. I det här exemplet tar vi alla som har delstat&quot;Kalifornien&quot; och ändrar det till&quot;Kalifornien&quot;.

   ![](assets/runaction-hands.png)

1. Ange ett nytt värde. Klicka på **Kör nu**.

   ![](assets/runactionnewvalue-hands.png)

1. Om du ändrar datavärden för ett stort antal personer kan du behöva bekräfta ändringen genom att skriva in talet. Klicka på **Gå till**.

   ![](assets/changedatavalue.jpg)

Fantastiskt arbete! Status för det enskilda flödessteget visas i det övre högra hörnet.

![](assets/completesingleflowaction.jpg)

Uppdatera listan när den är klar så ser du den uppdaterade informationen.
