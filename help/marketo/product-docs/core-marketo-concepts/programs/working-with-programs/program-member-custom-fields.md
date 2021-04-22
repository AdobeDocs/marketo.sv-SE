---
unique-page-id: 37355569
description: Anpassade fält för programmedlemmar - Marketo Docs - produktdokumentation
title: Anpassade fält för programmedlem
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Anpassade fält för programmedlem {#program-member-custom-fields}

Med anpassade fält för programmedlemmar kan du samla in programspecifika data för varje medlem. De kan användas i: Marketo-formulär, Smart List-filter och -utlösare samt Flödesåtgärder för smarta kampanjer. Data kan visas på fliken Medlemmar i programmet.

>[!NOTE]
>
>Anpassade fält för programmedlem har för närvarande ingen integrering med Salesforce Campaign-medlemsfält.

## Skapa ett anpassat fält för programmedlem {#create-a-program-member-custom-field}

1. Klicka på **Admin** i Marketo.

   ![](assets/one.png)

1. Klicka på **Fälthantering**.

   ![](assets/two.png)

1. Klicka på **Nytt anpassat fält**.

   ![](assets/three.png)

1. Klicka på listrutan Objekt och markera önskat objekt.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Anpassade fält för person och programmedlem kan inte ha samma namn.

1. Fyll i de återstående fälten och klicka på **Skapa**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Typer som stöds för anpassade fält för programmedlemmar är: boolesk, date, datetime, float, integer, string, URL. [Läs mer om fälttyper](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

## Objektbeskrivningar {#object-descriptions}

| Objekt | Beskrivning |
|---|---|
| Företag | Namnet på det företag som är associerat med personen. |
| Möjligheter | En affärsmöjlighet kan kopplas till en person eller ett konto som en potentiell framtida försäljning. De går vanligtvis in i Marketo via en CRM eller via API. |
| Person | En individ i er Marketo-databas som ni interagerar med via marknadsföringskampanjer. |
| Programmedlem | Person som även är medlem i ett program |

## Utlösare och filter {#triggers-and-filters}

Du kan utnyttja dessa programspecifika data i smarta listor via [utlösare](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) och/eller [filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## Saker att känna till {#things-to-know}

* Anpassade fält för programmedlemmar är endast tillgängliga i lokala resurser. De stöds inte i Design Studio eftersom det inte finns något sätt att knyta dem till ett specifikt program.
* Du kan inte klona/flytta ett formulär (eller en landningssida med ett formulär) som innehåller anpassade fält för programmedlem till Design Studio.
* Objektet Program Member kan ha upp till 20 anpassade fält. Dessa fält är tillgängliga för alla program.
* När du tar bort en medlem i ett program och har data i det anpassade fältet Programmedlem, rensas data från det fältet.
* Om du vill visa data klickar du på fliken Medlemmar i programmet och skapar en anpassad vy som innehåller dessa fält.
* Import och export via [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) och [API](https://developers.marketo.com/) stöds.
* När du sammanfogar två personer används vinnarens anpassade fältdata för programmedlemmen. Men om vinnaren inte har något värde kommer förlorarens värde att användas.

>[!MORELIKETHIS]
>
>[Skapa ett anpassat fält i Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
