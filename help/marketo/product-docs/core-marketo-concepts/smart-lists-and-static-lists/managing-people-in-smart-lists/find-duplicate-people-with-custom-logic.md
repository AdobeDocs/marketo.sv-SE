---
unique-page-id: 2952636
description: Hitta duplicerade personer med anpassad logik - Marketo Docs - produktdokumentation
title: Sök efter duplicerade personer med anpassad logik
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Sök efter duplicerade personer med anpassad logik {#find-duplicate-people-with-custom-logic}

Marketo har en systemsmart lista som söker efter duplicerade personer genom att matcha deras e-postadresser. Så här använder du ett annat fält för att hitta dubbletter.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Gå till **Marknadsföringsaktiviteter**.

![](assets/ma-2.png)

1. Välj den smarta listan och klicka på fliken **Smart lista**.

   ![](assets/two-4.png)

1. Hitta och dra filtret **Duplicera fält** till arbetsytan.

   ![](assets/three-4.png)

1. Välj ett av fyra tillgängliga alternativ:

   * E-postadress
   * Fullständigt namn
   * Efternamn
   * Uppdaterat den

   >[!NOTE]
   >
   >Alla fält, med undantag för E-postadress, är skiftlägeskänsliga. Om du använder &quot;john do&quot; i fältet Fullständigt namn skulle _inte_ returnera resultatet för John Doe.

   ![](assets/four-2.png)

   Klart! Kör den smarta listan för att hitta personer med samma värde i det tidigare markerade fältet.
