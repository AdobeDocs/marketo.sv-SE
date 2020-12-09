---
unique-page-id: 1146901
description: Använda logik för avancerad smart listregel - Marketo Docs - Produktdokumentation
title: Använda avancerad logik för smarta listregler
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Använda avancerad logik för smarta listregler {#using-advanced-smart-list-rule-logic}

Du kan hitta exakt de personer du behöver genom att tillämpa logik för smarta listregler på flera filter i en smart lista. Så här gör du.

>[!PREREQUISITES]
>
>* [Söka efter och lägga till filter i en smart lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definiera smarta listfilter](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>Avancerad filterlogik är bara tillgänglig om det finns tre eller fler filter i den smarta listan.

## Lägg till logik i en smart lista {#add-logic-to-a-smart-list}

Som standard hittar den smarta listan de personer som matchar **ALLA** filter (filtren 1 *och* 2 *och* 3). Du kan ändra regellogiken för att hitta personer som matchar **något** av de definierade filtren (filter 1 *eller* 2 *eller* 3) eller använda avancerade filter (filter 1 *och* 2 *eller *3).

I det här exemplet ska vi säga att du vill hitta personer i Kalifornien *och* ha minst 50 poäng *eller* statusen&quot;Försäljningskvalificerad&quot;.

1. Välj **Använd** **avancerade** **filter** i listrutan.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Om du använder **avancerade** filter behöver du inte skapa smarta listor med filtret Medlem i smart lista. Detta hjälper till att optimera prestanda.

1. I textrutan **Avancerade** **filter** visas&quot;och&quot; som standardvärde mellan alla filter.

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

