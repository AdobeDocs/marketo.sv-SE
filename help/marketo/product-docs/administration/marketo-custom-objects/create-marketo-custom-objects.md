---
unique-page-id: 10093192
description: Skapa anpassade Marketo-objekt - Marketo Docs - produktdokumentation
title: Skapa anpassade Marketo-objekt
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Skapa anpassade Marketo-objekt {#create-marketo-custom-objects}

Använd anpassade objekt i Marketo för att spåra mätvärden som är specifika för ditt företag. Det kan vara allt från bilar till kurser - allt du vill göra i Marketo för att genomföra kampanjer.

>[!NOTE]
>
>Du kan ställa in anpassade objekt så att de fungerar på en-till-många- eller många-till-många-basis. Du skapar det ursprungliga objektet på samma sätt, men stegen är olika när du börjar lägga till fält till objektet. Se  [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) för mer information.

>[!NOTE]
>
>Du kan inte skapa, redigera eller ta bort ett länk- eller borttagningsfält när det anpassade objektet har godkänts.

## Skapa ett anpassat objekt för en 1:N-struktur {#create-a-custom-object-for-a-one-to-many-structure}

I det här exemplet visas ett anpassat bildobjekt som kan användas i en en-till-många-struktur. Senare skapar du ett kursanpassat objekt och ett mellanliggande objekt som du kan använda i en många-till-många-struktur.

1. Gå till **Administratör** område.

   ![](assets/create-marketo-custom-objects-1.png)

1. Klicka **Anpassade Marketo-objekt**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Klicka **Nytt anpassat objekt**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >På fliken Anpassade objekt i Marketo visas alla anpassade objekt till höger och information om godkända objekt, inklusive antalet poster och fält vid den senaste uppdateringen.

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och **Visa i Lead-detalj** skjutreglage.

1. Dra **Visa i Lead-detalj** skjutreglage som ska visas **Visa** om du vill visa anpassade objektdata på databassidan. Klicka **Spara**.

   ![](assets/create-marketo-custom-objects-5.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   ![](assets/create-marketo-custom-objects-6.png)

   Nästa steg är att lägga till fält i [bygga ut ditt anpassade objekt](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Du kan bara fylla i anpassade Marketo-objekt via en listimport eller [API](https://developers.marketo.com/documentation/rest/).

## Skapa ett anpassat objekt för en många-till-många-struktur {#create-a-custom-object-for-a-many-to-many-structure}

I det här exemplet visas ett anpassat kursobjekt som du använder för att skapa en många-till-många-relation mellan människor/företag och kurser. När du är klar skapar du ett mellanliggande objekt som kopplar det till personer eller företag i din databas.

>[!NOTE]
>
>För många-till-många-relationer behöver du inte skapa någon länk i det anpassade objektet. I stället lägger du till två länkar till mellanliggande objekt (se nedan).

1. Gå till **Administratör** område.

   ![](assets/create-marketo-custom-objects-7.png)

1. Klicka **Anpassade Marketo-objekt**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Klicka **Nytt anpassat objekt**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och **Visa i Lead-detalj** skjutreglage.

1. Dra **Visa i Lead-detalj** skjutreglage som ska visas **Visa** om du vill visa anpassade objektdata på databassidan. Klicka **Spara**.

   ![](assets/create-marketo-custom-objects-11.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Du kan bara fylla i anpassade Marketo-objekt via en listimport eller [API](https://developers.marketo.com/documentation/rest/).

Nästa steg är att skapa ett mellanliggande objekt (se nedan). Innan dess måste du skapa ett fält som du kan länka till.

## Skapa ett mellanliggande objekt {#create-an-intermediary-object}

Använd ett mellanliggande objekt för att koppla ett anpassat objekt till personer eller företag. I det här exemplet används den för att koppla ihop kurser i ditt anpassade kursobjekt med personer eller företag i din databas.

>[!NOTE]
>
>Du behöver inte skapa ett mellanliggande objekt för en anpassad objektstruktur med en-till-många.

1. Gå till **Administratör** område.

   ![](assets/create-marketo-custom-objects-13.png)

1. Klicka **Anpassade Marketo-objekt**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Klicka **Nytt anpassat objekt**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och reglaget Visa i Leaddetalj.

1. Dra **Visa i Lead-detalj** skjutreglage som ska visas **Visa** om du vill visa anpassade objektdata på databassidan. Klicka **Spara**.

   ![](assets/create-marketo-custom-objects-17.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   Nästa steg är att du ska [lägg till länkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) för att ansluta ditt mellanliggande objekt till en person/ett företag och ett anpassat objekt.

>[!MORELIKETHIS]
>
>* [Lägg till anpassade Marketo-objektfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Lägg till Marketo anpassade objektlänkfält](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

