---
unique-page-id: 10099680
description: Importera anpassade objektdata - Marketo Docs - produktdokumentation
title: Importera anpassade objektdata
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Importera anpassade objektdata {#import-custom-object-data}

Det är enkelt att importera anpassade objektdata till databasen. Om du använder anpassade objekt med företag finns mer information i [Använda anpassade objekt med företag](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) för mer information.

1. I My Marketo går du till **Databas**.

   ![](assets/import-custom-object-data-1.png)

1. Klicka **Nytt** och markera **Importera anpassade objektdata**.

   ![](assets/import-custom-object-data-2.png)

1. Klicka **Bläddra** för att hitta datafilen. Markera filformatet (kommaseparerade värden i det här exemplet).

   ![](assets/import-custom-object-data-3.png)

1. Markera det anpassade objektet.

   ![](assets/import-custom-object-data-4.png)

1. Välj borttagningsläget i listrutan. Klicka **Nästa**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Använd Dedupe-fält som unika identifierare när du skapar eller uppdaterar anpassade objektposter. I det här exemplet används fältet för borttagning av dubbletter i **bil** anpassat objekt - vin (fordons-ID-nummer). Om du bara uppdaterar anpassade objektposter kan du välja Marketo Guid som borttagningsläge.

1. Mappa varje kolumn till ett Marketo-fält och välj den i listrutan.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Kontrollera att värdena i filen matchar den typ av fält som du matchar dem till (t.ex. text, heltal osv.), annars kommer filen att refuseras.

1. Klicka **Nästa**.

   ![](assets/import-custom-object-data-7.png)

1. Klicka **Importera**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Storleksgränsen för anpassade objekt är 100 MB.

   >[!TIP]
   >
   >Ange din e-postadress i dialogrutan **Skicka avisering till:** och Marketo skickar ett e-postmeddelande till dig när importen är klar!

1. I skärmens övre högra hörn visas ett meddelande när importen körs och det slutliga resultatet när den är klar.

   ![](assets/import-custom-object-data-9.png)

   Ja!

>[!MORELIKETHIS]
>
>[Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
