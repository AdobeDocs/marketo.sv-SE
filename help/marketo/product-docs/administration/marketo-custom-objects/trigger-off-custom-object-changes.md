---
unique-page-id: 11378713
description: Utlös anpassade objektändringar - Marketo Docs - produktdokumentation
title: Utlös ändringar av anpassade objekt
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Utlös ändringar av anpassade objekt {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Den här funktionen är endast tillgänglig:
>
>* För kunder med Orion-infrastrukturen
>* Kan endast användas med anpassade Marketo-objekt, inte anpassade objekt som synkroniseras via den inbyggda Salesforce- eller Microsoft Dynamics-integreringen
>* Som utlösare, inte ett filter
>
>Kontakta [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support) om du vill att utlösare för anpassade objektändringar ska vara aktiverade.

I den smarta kampanjens lista kan du utlösa en flödesåtgärd när ett anpassat objekt läggs till en person eller ett företag. Du kan också skapa en smart lista som använder en *change* i ett anpassat objekt som utlösare. Du kan till exempel använda den för att skicka ett e-postmeddelande när ett kursnamn uppdateras.

>[!NOTE]
>
>Ingen aktivitetsloggpost skapas när en anpassad objektpost ändras.

1. I Marketo går du till **Marknadsföringsaktiviteter.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Skapa eller öppna en befintlig smart kampanj och välj Smart lista.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Sök efter den utlösare du behöver och dra den till arbetsytan.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Markera utlösarattributet.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Du kan också ange en begränsning.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Och där är du. Ändringen sparas automatiskt.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Förstå anpassade Marketo-objekt](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

