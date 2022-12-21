---
unique-page-id: 557316
description: Definiera smarta listfilter - Marketo Docs - produktdokumentation
title: Definiera smarta listfilter
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definiera smarta listfilter {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Skapa en smart lista](create-a-smart-list.md)
>* [Söka efter och lägga till filter i smarta listor](find-and-add-filters-to-a-smart-list.md)


Nu när du har [skapade en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) och [tillagda filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) så definierar vi filtren. Så här gör du.

Låt oss definiera de här filtren för att hitta alla i Kalifornien med en poäng över 50.

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities-1.png)

1. Välj den smarta listan och klicka på **Smart List** -fliken.

   ![](assets/smarlist-choosefilters.png)

1. Sök och markera **CA** för **Läge** filter.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Du kanske lagrar båda **Kalifornien** och **CA**. För att filtrera efter både värden och inkludera _alla_ från Kalifornien, lär dig hur  [lägga till flera värden i ett smart listfilter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Välj **större än** operatorn och ange **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Om du tror att du kan ha poster i databasen som innehåller ofullständiga e-postadresser (t.ex. bara &quot;@adobe.com&quot;) använder du **två** E-postadressfilter när du använder operatorn &quot;contains&quot;. Ett filter med &quot;innehåller @adobe.com&quot; och ett separat filter med &quot;innehåller adobe.com&quot; (utelämnar @-symbolen).

Nu vet du hur du skapar en smart lista och lägger till/definierar filter.
