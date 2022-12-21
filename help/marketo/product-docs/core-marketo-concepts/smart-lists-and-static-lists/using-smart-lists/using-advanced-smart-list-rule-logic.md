---
unique-page-id: 1146901
description: Använda avancerad logik för smarta listregler - Marketo Docs - produktdokumentation
title: Använda avancerad logik för smarta listregler
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Använda avancerad logik för smarta listregler {#using-advanced-smart-list-rule-logic}

Du kan hitta exakt de personer du behöver genom att tillämpa logik för smarta listregler på flera filter i en smart lista. Så här gör du.

>[!PREREQUISITES]
>
>* [Söka efter och lägga till filter i en smart lista](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definiera smarta listfilter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>Avancerad filterlogik är bara tillgänglig om det finns tre eller fler filter i den smarta listan.

## Lägg till logik i en smart lista {#add-logic-to-a-smart-list}

Som standard hittar din smarta lista de personer som matchar **ALLA** filter (filter 1 _och_ 2 _och_ 3). Du kan ändra regellogiken för att hitta personer som matchar **VALFRITT** av definierade filter (filter 1 _eller_ 2 _eller_ 3) eller använda avancerade filter (filter 1) _och_ 2 _eller_ 3).

I det här exemplet vill vi säga att du vill hitta folk i Kalifornien _och_ med minst 50 poäng _eller_ med statusen&quot;Försäljning kvalificerad&quot;.

1. Välj **Använd avancerade filter** i listrutan.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Använda **Avancerat** filter minskar behovet av att skapa smarta listor med filtret Medlem i smart lista. Detta hjälper till att optimera prestanda.

1. The **Avancerade filter** &quot;och&quot; visas som standardvärde mellan alla filter.

   ![](assets/two-2.png)

1. Skriv parenteser runt &quot;2 och 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Du måste använda&quot;och&quot; före&quot;eller&quot; när du anger regellogik.

1. Ändra &quot;och&quot; mellan &quot;2 och 3&quot; till &quot;eller&quot;.

   ![](assets/four-1.png)

## Använd parenteser vid blandning av&quot;And&quot; och&quot;Or&quot; {#use-parentheses-when-mixing-and-and-or}

Om du blandar&quot;och&quot;- och&quot;eller&quot;-logik måste du använda parenteser för att tydliggöra din avsikt.

![](assets/advancedfilters-parent.png)

## Använd kapslade parenteser för fyra eller fler filter vid behov {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Beroende på din avsikt kan du behöva lägga till kapslade parenteser när du använder fyra eller fler filter.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Om du anger en ogiltig regel visas en röd linje under regeln. Bläddra över texten för att se det relaterade felmeddelandet.
