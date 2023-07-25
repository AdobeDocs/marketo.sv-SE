---
unique-page-id: 10093688
description: Lägg till anpassade Marketo-objektfält - Marketo Docs - produktdokumentation
title: Lägg till anpassade Marketo-objektfält
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Lägg till anpassade Marketo-objektfält {#add-marketo-custom-object-fields}

När du har skapat ett anpassat objekt måste du lägga till fält för att uppfylla dina affärsbehov.

Fält definierar den specifika information som används av ett anpassat objekt. Länkfält har ett särskilt jobb för att ansluta anpassade objekt och täcks av en [separat artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Gå till **[!UICONTROL Admin]** område.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Markera det objekt som du vill lägga till fältet i till höger.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Kicka **[!UICONTROL Fields]** tabben **[!UICONTROL New Field]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >De tre fälten ovan skapas automatiskt av Marketo när du skapar ett anpassat objekt. Marketo hanterar dessa fält automatiskt och du kan inte redigera eller ta bort dem.

1. Ange [!UICONTROL Display Name] och (valfritt) [!UICONTROL Description].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >API-namnet kan bara redigeras tills det har godkänts.

1. Välj en lämplig [!UICONTROL Data Type] från listan.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Dra [!UICONTROL Dedupe] om du vill använda det nya fältet som en unik identifierare. Klicka **[!UICONTROL Save]** till slut.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Dedupliceringsfält kan användas för att hämta, uppdatera eller ta bort anpassade objekt. Varje anpassad objektdefinition måste innehålla minst ett (och inte mer än tre) dedupliceringsfält.

1. Lägg till andra fält som du behöver.

   >[!NOTE]
   >
   >Om du skapar en en en-till-många-struktur måste du lägga till ett länkfält i det anpassade objektet. För en många-till-många-struktur behöver du inte ha något länkfält i det anpassade objektet, men du måste lägga till två länkfält i det mellanliggande objektet. Se [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) för att skapa länkfälten, och [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) om du vill ha mer information om olika typer av anpassade objekt.

>[!MORELIKETHIS]
>
>* [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Redigera och ta bort ett anpassat Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Redigera och ta bort anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
