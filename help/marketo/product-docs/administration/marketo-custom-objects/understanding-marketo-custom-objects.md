---
unique-page-id: 10093188
description: Understanding Marketo Custom Objects - Marketo Docs - produktdokumentation
title: Förstå anpassade objekt i Marketo
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Om Marketo-anpassade objekt {#understanding-marketo-custom-objects}

Använd anpassade objekt för att spåra mätvärden som är specifika för din verksamhet.

>[!NOTE]
>
>**Tillgänglighet**
>
>Alla kunder har inte köpt den här funktionen. Kontakta din säljare för mer information.

Använd anpassade objekt som filter och triggers i era smarta kampanjer. Till exempel:

* **Filter**: Skicka e-postmeddelanden endast till ägare av ett visst fordonsmärke
* **Utlösare**: Skicka ett e-postmeddelande när ett anpassat objekt läggs till en person eller ett företag.

Du kan ställa in anpassade objekt i en 1:N- eller många-till-många-relation. Till exempel:

* **En-till-många**: En person äger flera bilar
* **Många-till-många**: Flera studenter är inskrivna i flera kurser från en kurskatalog

I en en-till-många-struktur används ett enda länkfält för att koppla det anpassade objektet till en person eller ett företag.

Många-till-många anpassade objekt använder två länkfält, som ingår i ett mellanliggande objekt. Ett länkfält är anslutet till personen eller företaget och ett annat är anslutet till det anpassade objektet, t.ex. kurskatalogen. Detta mellanliggande objekt kan innehålla ytterligare anpassade fält, t.ex. en kursklass eller ett närvarodatum, som ytterligare definierar anslutningstypen.

>[!TIP]
>
>Importera egna objekt med kommaavgränsade värden (CSV) i användargränssnittet för att testa och validera ett dataexempel. Ladda sedan upp alla filer med ett API.

>[!CAUTION]
>
>Du kan inte återställa anpassade objekt, så kontrollera att du inte behöver dem längre innan du tar bort dem.

## Åtkomst till anpassade Marketo-objekt {#accessing-marketo-custom-objects}

1. Om du vill skapa eller redigera markering för anpassade objekt klickar du på länken **Admin **och sedan på länken **Marketo Custom Object** s.

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. Marketo-anpassade objekt visar alla dina anpassade objekt till höger, men bara de godkända objekten i huvudstödrastret.

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. I rutnätet visas objektnamn, antal poster, antal fält och datum för den senaste uppdateringen.

   >[!TIP]
   >
   >Marketo uppdaterar dessa fält automatiskt, men du kan uppdatera visningen genom att klicka på ikonen i kolumnen Poster.

1. Klicka på objektnamnet till höger för att öppna informationssidan.

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## Visa anpassade objekt som är kopplade till en person {#view-custom-objects-associated-to-a-person}

När du har skapat den anpassade objektstrukturen kopplas de anpassade objekten automatiskt till personer i databasen med hjälp av länkfältet i det anpassade objektet när du överför specifika anpassade objektdata. Du kan visa information på fliken Egna objekt på sidan med personinformation.

1. Gå till **Database**.

   ![](assets/db.png)

1. Öppna databasen och klicka på fliken **Personer**. Dubbelklicka på posten för en person som är kopplad till ett anpassat objekt.

   ![](assets/five.png)

1. Klicka på fliken **Egna objekt** på personinformationssidan. Markera objektet i listrutan.

   ![](assets/six.png)

1. Nu kan du visa en lista över alla anpassade objekt av den typen som är kopplade till den personen.

   ![](assets/seven.png)

## Använda anpassade objekt med företag {#using-custom-objects-with-companies}

Ett anpassat objekt som är länkat till företaget fungerar bäst om du synkroniserar företag från CRM eller om du uttryckligen skapar företag med API:t. Vi rekommenderar även att du använder företags-ID som länkfält.

Om du har flera personer i Marketo som är poster i CRM- eller Marketo-posterna, kopplas inte ett anpassat objekt som är länkat till ett företag till mer än en enskild post. Detta beror på att ett företag som har flera personer under det bara stöds när företag synkroniseras från CRM eller om du använder ett API för att skapa företag.

Anpassade objekt kan bara länka direkt till en enskild post. Det innebär att när din anpassade objekttyp är länkad efter företagsfält bör du se till att dina personposter är kopplade till ett företag antingen med hjälp av kontaktkonvertering i CRM eller med hjälp av fältet externalCompanyId om du hanterar företag med hjälp av Marketos REST API:er. För personposter som inte är uttryckligen länkade till företagsposter, kommer anpassade objekt som är länkade med hjälp av företag att slumpmässigt länkas till en enda post, även om värdet i företagsfältet delas av många personer.

Mer information finns i [Importera anpassade objektdata](import-custom-object-data.md).

>[!MORELIKETHIS]
>
>* [Skapa anpassade Marketo-objekt](create-marketo-custom-objects.md)
>* [Godkänn ett anpassat objekt](approve-a-custom-object.md)
>* [Redigera och ta bort ett markeringsobjekt till anpassat objekt](edit-and-delete-a-marketo-custom-object.md)
>* [Lägg till markering i anpassade objektfält](add-marketo-custom-object-fields.md)
>* [Redigera och ta bort markering i anpassade objektfält](edit-and-delete-marketo-custom-object-fields.md)
>* [Importera anpassade objektdata](import-custom-object-data.md)

>



