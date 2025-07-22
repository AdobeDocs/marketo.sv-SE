---
unique-page-id: 5472402
description: Redigera din godkända modell - Marketo Docs - Produktdokumentation
title: Redigera din godkända modell
exl-id: 5f31b9bd-b008-4b97-ba5d-930488dd3da9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Redigera din godkända modell {#editing-your-approved-model}

## Redigera din modell {#editing-your-model}

1. Markera den modell som du vill ändra i avsnittet [!UICONTROL Analytics] och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/one.png)

1. Du kan inte ta bort faser när du redigerar en utkastmodell (efter att modellen har godkänts). I stället kan du sammanfoga scenen med en annan i modellen. Högerklicka på den scen som du vill sammanfoga och klicka på **[!UICONTROL Merge]**.

   ![](assets/two.png)

1. Välj den nya fasen för leads som finns i den markerade, eller välj **[!UICONTROL None]** om du vill ta bort leads från modellen. När du är klar klickar du på **[!UICONTROL Merge]**.

   ![](assets/three.png)

1. När du är klar med ändringarna av modellen godkänner du den igen genom att välja **[!UICONTROL Approve Model Draft]** på menyn **[!UICONTROL Model Actions]**.

   ![](assets/four.png)

   >[!TIP]
   >
   >Om du gör några ändringar i dina scener, till exempel lägger till eller sammanfogar dem, måste du ändra [!UICONTROL Assignment Rules] och faser så att de återspeglar dina redigeringar.

## Modellen godkänns inte {#unapproving-your-model}

>[!CAUTION]
>
>Om du inte godkänner modellen tas alla leads bort och deras historik i modellen tas bort. Överväg att redigera din modell i stället för att inte godkänna den.

1. Markera den modell som du vill avgodkänna. Välj **[!UICONTROL Model Actions]** på menyn **[!UICONTROL Unapprove Model]**.

   ![](assets/five.png)

1. Klicka på **[!UICONTROL Unapprove]**.

   ![](assets/six.png)

>[!NOTE]
>
>Om du vill omgodkänna den här modellen måste du först omtilldela leads till faserna.

## Skapa fler modeller {#creating-more-models}

Du kan bara ha en godkänd modell åt gången. Om du vill godkänna en modell men redan har en godkänd, måste du först avgodkänna den aktuella modellen. Om det är möjligt kan du prova att redigera modellen i stället för att skapa en ny.

>[!MORELIKETHIS]
>
>[Skapa en ny intäktsmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-new-revenue-model.md)
