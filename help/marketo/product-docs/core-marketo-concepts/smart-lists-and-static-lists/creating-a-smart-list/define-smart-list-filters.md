---
unique-page-id: 557316
description: Definiera smarta listfilter - Marketo Docs - produktdokumentation
title: Definiera smarta listfilter
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Definiera smarta listfilter {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Sök efter och lägg till filter i smarta listor](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Nu när du har [skapat en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} och [lagt till filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} i den definierar vi filtren. Så här gör du.

Låt oss definiera de här filtren för att hitta alla i Kalifornien med en poäng över 50.

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/define-smart-list-filters-1.png)

1. Markera önskad smart lista och klicka på fliken **[!UICONTROL Smart List]**.

   ![](assets/define-smart-list-filters-2.png)

1. Sök efter och välj CA för filtret **[!UICONTROL State]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Du kanske lagrar både &quot;Kalifornien&quot; och &quot;CA&quot;. Lär dig hur du [lägger till flera värden i ett Smart List-filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"} om du vill filtrera efter båda värdena och inkludera _alla_ personer från Kalifornien.

1. Välj operatorn **[!UICONTROL greater than]** och ange &quot;50&quot;.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Om du tror att du har poster i databasen som innehåller ofullständiga e-postadresser (t.ex. bara &quot;@adobe.com&quot;) använder du två e-postadressfilter när du använder operatorn &quot;contains&quot;. Ett filter med &quot;innehåller @adobe.com&quot; och ett separat filter med &quot;innehåller adobe.com&quot; (utelämnar symbolen @).

Nu vet du hur du skapar en smart lista och lägger till/definierar filter.
