---
unique-page-id: 2952636
description: Hitta duplicerade personer med anpassad logik - Marketo Docs - produktdokumentation
title: Sök efter duplicerade personer med anpassad logik
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 5%

---

# Sök efter duplicerade personer med anpassad logik {#find-duplicate-people-with-custom-logic}

Marketo har en systemsmart lista som söker efter duplicerade personer genom att matcha deras e-postadresser. Så här använder du ett annat fält för att hitta dubbletter.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Gå till **Marknadsföringsaktiviteter** område.

![](assets/ma-2.png)

1. Välj din smarta lista och klicka på **Smart List** -fliken.

   ![](assets/two-4.png)

1. Sök och dra **Duplicera fält** filter på arbetsytan.

   ![](assets/three-4.png)

1. Välj ett av fyra tillgängliga alternativ:

   * E-postadress
   * Fullständigt namn
   * Efternamn
   * Uppdaterat den

   >[!NOTE]
   >
   >Alla fält, med undantag för E-postadress, är skiftlägeskänsliga. Så om du använder&quot;john doe&quot; i fältet Fullständigt namn skulle det _not_ returnera resultaten för John Doe.

   ![](assets/four-2.png)

   Klar! Kör den smarta listan för att hitta personer med samma värde i det tidigare markerade fältet.
