---
unique-page-id: 10094188
description: Godkänn ett anpassat objekt - Marketo Docs - produktdokumentation
title: Godkänn ett anpassat objekt
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Godkänn ett anpassat objekt {#approve-a-custom-object}

Du måste godkänna ett anpassat objekt innan du kan använda det. Processen skiljer sig något mellan nya anpassade objekt och objekt som du har redigerat.

## Godkänn ett nytt anpassat objekt {#approve-a-new-custom-object}

Du har skapat ett helt nytt anpassat objekt. Så här godkänner du det.

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/approve-a-custom-object-1.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/approve-a-custom-object-2.png)

1. Markera ett objekt som är i utkastläge.

   ![](assets/approve-a-custom-object-3.png)

1. Klicka på listrutan **[!UICONTROL Custom Object Actions]** och välj **[!UICONTROL Approve Object]**.

   ![](assets/approve-a-custom-object-4.png)

1. Läget ändras till [!UICONTROL Approved].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Ett anpassat objekt som används i en _en-till-många-struktur_ måste ha minst ett dedupliceringsfält, ett länkfält, ett länkat objektnamn och ett länkat fältnamn som ska godkännas.
   >
   >Ett anpassat objekt som används i en _många-till-många-struktur_ **behöver inte** ett länkfält, ett länkat objektnamn eller ett länkat fältnamn när du godkänner det (eftersom de finns i mellanliggande objekt).
   >
   >Ett anpassat objekt som används som _mellanliggande objekt_ kräver ett länkfält, ett länkat objektnamn och ett länkat fältnamn, men **kräver inte** ett borttagningsfält.
   >
   >Mer information finns i [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md).

Så ja! Nu kan du välja det anpassade objektet i begränsningarna för filter och utlösare som ska användas i dina kampanjer.

## Godkänn ett redigerat anpassat objekt {#approve-an-edited-custom-object}

När du har redigerat ett godkänt anpassat objekt måste du godkänna utkastet för att kunna återställa det anpassade objektet till läget Godkänd.

1. När du redigerar ett redan godkänt anpassat objekt får det ett [!UICONTROL Approved with Draft]-läge.

   ![](assets/approve-a-custom-object-6.png)

1. När du är klar att godkänna utkastet klickar du på listrutan **[!UICONTROL Custom Object Actions]** och väljer **[!UICONTROL Approve Object]**.

   ![](assets/approve-a-custom-object-7.png)

1. I en förhandsgranskning visas de objekt som har ändrats i utkastet. Klicka på **[!UICONTROL Approve]**.

   ![](assets/approve-a-custom-object-8.png)
