---
unique-page-id: 2952636
description: Hitta duplicerade personer med anpassad logik - Marketo Docs - produktdokumentation
title: Sök efter duplicerade personer med anpassad logik
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 5%

---

# Sök efter duplicerade personer med anpassad logik {#find-duplicate-people-with-custom-logic}

Marketo Engage har en smart systemlista som söker efter duplicerade personer genom att matcha deras e-postadresser. Så här använder du ett annat fält för att hitta dubbletter.

>[!PREREQUISITES]
>
>[Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Gå till **[!UICONTROL Marketing Activities]** område.

![](assets/ma-2.png)

1. Välj din smarta lista och klicka på **[!UICONTROL Smart List]** -fliken.

   ![](assets/two-4.png)

1. Sök och dra **[!UICONTROL Duplicate Fields]** filter på arbetsytan.

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
