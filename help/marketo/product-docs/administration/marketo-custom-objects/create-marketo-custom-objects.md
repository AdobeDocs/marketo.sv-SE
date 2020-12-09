---
unique-page-id: 10093192
description: Skapa anpassade Marketo-objekt - Marketo Docs - Produktdokumentation
title: Skapa anpassade Marketo-objekt
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# Skapa anpassade Marketo-objekt {#create-marketo-custom-objects}

Använd anpassade objekt i Marketo för att spåra mätvärden som är specifika för din verksamhet. Det kan vara allt från bilar till kurser - allt du vill modellera i Marketo för att köra era kampanjer.

>[!NOTE]
>
>Du kan ställa in anpassade objekt så att de fungerar på en-till-många- eller många-till-många-basis. Du skapar det ursprungliga objektet på samma sätt, men stegen är olika när du börjar lägga till fält till objektet. Mer information finns i [Förstå anpassade objekt](understanding-marketo-custom-objects.md) i Marketto.

>[!NOTE]
>
>Du kan inte skapa, redigera eller ta bort ett länk- eller borttagningsfält när det anpassade objektet har godkänts.

## Skapa ett anpassat objekt för en 1:N-struktur {#create-a-custom-object-for-a-one-to-many-structure}

I det här exemplet visas ett anpassat bildobjekt som kan användas i en en-till-många-struktur. Senare skapar du ett kursanpassat objekt och ett mellanliggande objekt som du kan använda i en många-till-många-struktur.

1. Klicka på **Admin** och välj Anpassade objekt **i** Databashantering ****.

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. Klicka på **Nytt anpassat objekt**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >På fliken Anpassade objekt i Marketo visas alla anpassade objekt till höger och information om godkända objekt, inklusive antal poster och fält vid den senaste uppdateringen.

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och reglaget **Visa i Leaddetalj** .

1. Dra reglaget **Visa i Leaddetalj **för att visa **Visa** om du vill visa anpassade objektdata på sidan Leaddatabas. Klicka på **Spara**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   Nästa steg är att lägga till fält för att [skapa det anpassade objektet](add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Du kan bara fylla i Marketo-anpassade objekt via en listimport eller [API](http://developers.marketo.com/documentation/rest/).

## Skapa ett anpassat objekt för en många-till-många-struktur {#create-a-custom-object-for-a-many-to-many-structure}

I det här exemplet visas ett anpassat kursobjekt som du använder för att skapa en många-till-många-relation mellan människor/företag och kurser. När du är klar skapar du ett mellanliggande objekt som kopplar det till personer eller företag i din databas.

>[!NOTE]
>
>För många-till-många-relationer behöver du inte skapa någon länk i det anpassade objektet. I stället lägger du till två länkar till mellanliggande objekt (se nedan).

1. Klicka på **Admin** och välj Anpassade objekt **i** Databashantering ****.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Klicka på **Nytt anpassat objekt**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och reglaget **Visa i Leaddetalj** .

1. Dra reglaget **Visa i Leaddetalj **för att visa Visa om du vill visa anpassade objektdata på sidan Leaddatabas. Klicka på **Spara**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Du kan bara fylla i Marketo-anpassade objekt via en listimport eller [API](http://developers.marketo.com/documentation/rest/).

Nästa steg är att skapa ett mellanliggande objekt (se nedan). Innan dess måste du skapa ett fält som du kan länka till.

## Skapa ett mellanliggande objekt {#create-an-intermediary-object}

Använd ett mellanliggande objekt för att koppla ett anpassat objekt till personer eller företag. I det här exemplet används den för att koppla ihop kurser i ditt anpassade kursobjekt med personer eller företag i din databas.

>[!NOTE]
>
>Du behöver inte skapa ett mellanliggande objekt för en anpassad objektstruktur med en-till-många.

1. Klicka på **Admin** och välj Anpassade objekt **i** Databashantering ****.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Klicka på **Nytt anpassat objekt**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Ange ett visningsnamn. API-namnet och pluronamnet fylls i automatiskt. Ange en beskrivning (valfritt).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Du kan redigera de här fälten när du skapar dem, men när de har sparats kan du bara redigera fältet Pluralnamn och reglaget Visa i Leaddetalj.

1. Dra skjutreglaget **Visa i Lead-detalj** över för att visa Visa om du vill visa anpassade objektdata på Lead-databassidan. Klicka på **Spara**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Den anpassade objektinformationen visar det innehåll du har angett. Observera att det är i utkastläge.

   Nästa steg är att du ska [lägga till länkfält](add-marketo-custom-object-link-fields.md) för att koppla ditt mellanliggande objekt till en person/ett företag och ett anpassat objekt.

>[!MORELIKETHIS]
>
>* [Lägg till markering i anpassade objektfält](add-marketo-custom-object-fields.md)
>* [Lägg till markering i anpassade objektlänkfält](add-marketo-custom-object-link-fields.md)
>* [Förstå anpassade objekt i Marketo](understanding-marketo-custom-objects.md)

>



