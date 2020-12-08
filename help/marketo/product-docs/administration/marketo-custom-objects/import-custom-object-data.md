---
unique-page-id: 10099680
description: Importera anpassade objektdata - Marketo Docs - Produktdokumentation
title: Importera anpassade objektdata
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Importera anpassade objektdata {#import-custom-object-data}

Det är enkelt att importera anpassade objektdata till databasen. Om du använder anpassade objekt med företag kan du läsa [Använda anpassade objekt med företag](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies) för mer information.

1. På My Marketo går du till **Database**.

   ![](assets/db-1.png)

1. Klicka på **Nytt** och välj **Importera anpassade objektdata**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Klicka på **Bläddra** för att leta reda på datafilen. Markera filformatet (kommaseparerade värden i det här exemplet).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Markera det anpassade objektet.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Välj borttagningsläget i listrutan. Klicka på **Nästa**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Använd Dedupe-fält som unika identifierare när du skapar eller uppdaterar anpassade objektposter. I det här exemplet används fältet Dedupe för det anpassade objektet **car** - vin (fordons-ID-nummer). Om du bara uppdaterar anpassade objektposter kan du välja Marketo Guid som borttagningsläge.

1. Koppla varje kolumn till ett Marketo-fält och välj den i listrutan.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Kontrollera att värdena i filen matchar den typ av fält som du matchar dem till (t.ex. text, heltal osv.), annars kommer filen att refuseras.

1. Klicka på **Nästa**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Klicka på **Importera**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Storleksgränsen för anpassade objekt är 100 MB.

   >[!TIP]
   >
   >Ange din e-postadress i **Skicka avisering till:** och Marketo skickar e-post till dig när importen är klar!

1. I skärmens övre högra hörn visas ett meddelande när importen körs och det slutliga resultatet när den är klar.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Ja!

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Förstå anpassade objekt i Marketo](understanding-marketo-custom-objects.md)

>



