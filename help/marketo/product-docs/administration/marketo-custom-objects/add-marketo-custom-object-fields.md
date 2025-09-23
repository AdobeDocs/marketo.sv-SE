---
unique-page-id: 10093688
description: Lägg till anpassade Marketo-objektfält - Marketo Docs - produktdokumentation
title: Lägg till anpassade Marketo-objektfält
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Lägg till anpassade Marketo-objektfält {#add-marketo-custom-object-fields}

När du har skapat ett anpassat objekt måste du lägga till fält för att uppfylla dina affärsbehov.

Fält definierar den specifika information som används av ett anpassat objekt. Länkfält har ett särskilt jobb för att ansluta anpassade objekt och täcks av en [separat artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Gå till området **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Klicka på **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Markera det objekt som du vill lägga till fältet i till höger.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Klicka på fliken **[!UICONTROL Fields]** och sedan på **[!UICONTROL New Field]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >De tre fälten ovan skapas automatiskt av Marketo när du skapar ett anpassat objekt. Marketo hanterar dessa fält automatiskt och du kan inte redigera eller ta bort dem.

1. Ange [!UICONTROL Display Name] och (valfritt) [!UICONTROL Description].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >[!UICONTROL API Name] kan bara redigeras tills den har godkänts.

1. Välj en lämplig [!UICONTROL Data Type] i listan.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Dra reglaget [!UICONTROL Dedupe] över om du vill använda det nya fältet som en unik identifierare. Klicka på **[!UICONTROL Save]** för att slutföra.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Dedupliceringsfält kan användas för att hämta, uppdatera eller ta bort anpassade objekt. Varje anpassad objektdefinition måste innehålla minst ett (och högst tre) dedupliceringsfält.

1. Lägg till andra fält som du behöver.

   >[!NOTE]
   >
   >Om du skapar en en en-till-många-struktur måste du lägga till ett länkfält i det anpassade objektet. För en många-till-många-struktur behöver du inte ha något länkfält i det anpassade objektet, men du måste lägga till två länkfält i det mellanliggande objektet. Se [Lägg till anpassade Marketo-objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) för att skapa länkfälten och [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) för mer information om typer av anpassade objekt.

>[!MORELIKETHIS]
>
>* [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Redigera och ta bort ett anpassat Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Redigera och ta bort anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
