---
unique-page-id: 557322
description: Köra ett enda flödessteg från en smart lista - Marketo Docs - produktdokumentation
title: Köra ett enda flödessteg från en smart lista
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Köra ett enda flödessteg från en smart lista {#run-a-single-flow-step-from-a-smart-list}

Om du vill köra ett enda steg för ett enda flöde kan du använda ett enda flödessteg i en smart lista i stället för att skapa en hel smart kampanj.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Välj en lista eller smart lista med personer i den och gå sedan till **Folk** -fliken.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Både statiska listor och smarta listor har den här funktionen.

1. Klicka **Markera alla**. Du kan också använda **Ctrl/Cmd** och klicka för att markera några poster manuellt.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Om resultatet sträcker sig över flera sidor klickar du på **Markera alla** markerar alla personer på alla sidor.

1. Under **Person** **Åtgärder** väljer du ett flödessteg. I det här exemplet kommer vi att använda [Ändra datavärde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Söka efter och markera en **Attribut**. I det här exemplet tar vi alla som har delstat&quot;Kalifornien&quot; och ändrar det till&quot;Kalifornien&quot;.

   ![](assets/runaction-hands.png)

1. Ange ett nytt värde. Klicka **Kör nu**.

   ![](assets/runactionnewvalue-hands.png)

1. Om du ändrar datavärden för ett stort antal personer kan du behöva bekräfta ändringen genom att skriva in talet. Klicka **Gå för den**.

   ![](assets/changedatavalue.jpg)

Fantastiskt arbete! Status för det enskilda flödessteget visas i det övre högra hörnet.

![](assets/completesingleflowaction.jpg)

Uppdatera listan när den är klar så ser du den uppdaterade informationen.
