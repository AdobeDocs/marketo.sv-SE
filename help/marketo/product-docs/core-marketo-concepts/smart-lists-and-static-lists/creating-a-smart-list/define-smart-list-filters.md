---
unique-page-id: 557316
description: Definiera smarta listfilter - Marketo Docs - produktdokumentation
title: Definiera smarta listfilter
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Definiera smarta listfilter {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Skapa en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Söka efter och lägga till filter i smarta listor](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Nu när du har [skapade en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} så definierar vi filtren. Så här gör du.

Låt oss definiera de här filtren för att hitta alla i Kalifornien med en poäng över 50.

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-1.png)

1. Markera den smarta listan och klicka på **[!UICONTROL Smart List]** -fliken.

   ![](assets/smarlist-choosefilters.png)

1. Sök efter och välj &quot;CA&quot; för **[!UICONTROL State]** filter.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Du kanske lagrar både &quot;Kalifornien&quot; och &quot;CA&quot;. För att filtrera efter både värden och inkludera _alla_ från Kalifornien, lär dig hur  [lägga till flera värden i ett Smart List-filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Välj **[!UICONTROL greater than]** och ange &quot;50&quot;.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Om du tror att du har poster i databasen som innehåller ofullständiga e-postadresser (t.ex. bara &quot;@adobe.com&quot;) använder du två e-postadressfilter när du använder operatorn &quot;contains&quot;. Ett filter med &quot;innehåller @adobe.com&quot; och ett separat filter med &quot;innehåller adobe.com&quot; (utelämnar symbolen @).

Nu vet du hur du skapar en smart lista och lägger till/definierar filter.
