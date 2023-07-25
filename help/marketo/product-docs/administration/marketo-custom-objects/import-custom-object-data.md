---
unique-page-id: 10099680
description: Importera anpassade objektdata - Marketo Docs - produktdokumentation
title: Importera anpassade objektdata
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Importera anpassade objektdata {#import-custom-object-data}

Det är enkelt att importera anpassade objektdata till databasen. Om du använder anpassade objekt med företag finns mer information i [Använda anpassade objekt med företag](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) för mer information.

1. I My Marketo går du till **[!UICONTROL Database]**.

   ![](assets/import-custom-object-data-1.png)

1. Klicka på **[!UICONTROL New]** och välj **[!UICONTROL Import Custom Object Data]**.

   ![](assets/import-custom-object-data-2.png)

1. Klicka **[!UICONTROL Browse]** för att hitta datafilen. Markera filformatet (kommaseparerade värden i det här exemplet).

   ![](assets/import-custom-object-data-3.png)

1. Välj [!UICONTROL custom object].

   ![](assets/import-custom-object-data-4.png)

1. Välj [!UICONTROL Dedupe Mode] i listrutan. Klicka på **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Använd Dedupe-fält som unika identifierare när du skapar eller uppdaterar anpassade objektposter. I det här exemplet används fältet för borttagning av dubbletter i **bil** anpassat objekt - vin (fordons-ID-nummer). Om du bara uppdaterar anpassade objektposter kan du välja [!UICONTROL Marketo Guid] som [!UICONTROL Dedupe Mode].

1. Mappa varje kolumn till ett Marketo-fält och välj den i listrutan.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Kontrollera att värdena i filen matchar den typ av fält som du matchar dem till (t.ex. text, heltal osv.), annars kommer filen att refuseras.

1. Klicka på **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-7.png)

1. Klicka på **[!UICONTROL Import]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Storleksgränsen för anpassade objekt är 100 MB.

   >[!TIP]
   >
   >Ange din e-postadress i dialogrutan **[!UICONTROL Send Alert To]** och Marketo skickar ett e-postmeddelande till dig när importen är klar!

1. I skärmens övre högra hörn visas ett meddelande när importen körs och det slutliga resultatet när den är klar.

   ![](assets/import-custom-object-data-9.png)

   Ja!

>[!MORELIKETHIS]
>
>[Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
