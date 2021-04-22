---
unique-page-id: 10093688
description: Lägg till anpassade Marketo-objektfält - Marketo Docs - produktdokumentation
title: Lägg till anpassade Marketo-objektfält
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Lägg till anpassade Marketo-objektfält {#add-marketo-custom-object-fields}

När du har skapat ett anpassat objekt måste du lägga till fält för att uppfylla dina affärsbehov.

Fält definierar den specifika information som används av ett anpassat objekt. Länkfält har ett särskilt jobb för att ansluta anpassade objekt och beskrivs i en [separat artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Klicka på **Admin** och välj **Marketo anpassade objekt** i **Databashantering**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Markera det objekt som du vill lägga till fältet i till höger.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Klicka på **Nytt fält** på fliken **Fält**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >De tre fälten ovan skapas automatiskt av Marketo när du skapar ett anpassat objekt. Marketo hanterar dessa fält automatiskt och du kan inte redigera eller ta bort dem.

1. Ange ett visningsnamn och en beskrivning.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >API-namnet kan bara redigeras tills det har godkänts.

1. Välj en lämplig datatyp i listan.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Dra skjutreglaget för borttagning om du vill använda det nya fältet som en unik identifierare. Klicka på **Spara** för att slutföra.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Dedupliceringsfält kan användas för att hämta, uppdatera eller ta bort anpassade objekt. Varje anpassad objektdefinition måste innehålla minst ett (och inte mer än tre) dedupliceringsfält.

1. Lägg till andra fält som du behöver.

   >[!NOTE]
   >
   >Om du skapar en en en-till-många-struktur måste du lägga till ett länkfält i det anpassade objektet. För en många-till-många-struktur behöver du inte ha något länkfält i det anpassade objektet, men du måste lägga till två länkfält i det mellanliggande objektet. Se [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) för att skapa länkfälten och [Förstå Marketo anpassade objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) för mer information om typer av anpassade objekt.

>[!MORELIKETHIS]
>
>* [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Redigera och ta bort ett anpassat Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Redigera och ta bort anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

