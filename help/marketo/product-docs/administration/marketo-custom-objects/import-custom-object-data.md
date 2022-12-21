---
unique-page-id: 10099680
description: Importera anpassade objektdata - Marketo Docs - produktdokumentation
title: Importera anpassade objektdata
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importera anpassade objektdata {#import-custom-object-data}

Det är enkelt att importera anpassade objektdata till databasen. Om du använder anpassade objekt med företag finns mer information i [Använda anpassade objekt med företag](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) för mer information.

1. I My Marketo går du till **Databas**.

   ![](assets/db-1.png)

1. Klicka **Nytt** och markera **Importera anpassade objektdata**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Klicka **Bläddra** för att hitta datafilen. Markera filformatet (kommaseparerade värden i det här exemplet).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Markera det anpassade objektet.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Välj borttagningsläget i listrutan. Klicka **Nästa**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Använd Dedupe-fält som unika identifierare när du skapar eller uppdaterar anpassade objektposter. I det här exemplet används fältet för borttagning av dubbletter i **bil** anpassat objekt - vin (fordons-ID-nummer). Om du bara uppdaterar anpassade objektposter kan du välja Marketo Guid som borttagningsläge.

1. Mappa varje kolumn till ett Marketo-fält och välj den i listrutan.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Kontrollera att värdena i filen matchar den typ av fält som du matchar dem till (t.ex. text, heltal osv.), annars kommer filen att refuseras.

1. Klicka **Nästa**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Klicka **Importera**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Storleksgränsen för anpassade objekt är 100 MB.

   >[!TIP]
   >
   >Ange din e-postadress i dialogrutan **Skicka avisering till:** och Marketo skickar ett e-postmeddelande till dig när importen är klar!

1. I skärmens övre högra hörn visas ett meddelande när importen körs och det slutliga resultatet när den är klar.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Ja!

>[!MORELIKETHIS]
>
>[Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
