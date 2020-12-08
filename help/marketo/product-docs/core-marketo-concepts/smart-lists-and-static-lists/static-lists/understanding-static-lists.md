---
unique-page-id: 2949891
description: Statiska listor - Marketo Docs - Produktdokumentation
title: Statiska listor
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# Statiska listor {#understanding-static-lists}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Statiska listor är en av de mest enkla och användbara funktionerna i Marketo. De är bara en lista med namn från din databas. Det finns många skäl att använda dem.

>[!NOTE]
>
>En person i databasen kan finnas i många olika statiska listor.

Skillnaden mellan en statisk och smart lista är avgörande för att förstå.

| Typ | Logic |
|---|---|
| Smart List | Baserat på **definierade regler** |
| Statisk lista | Baserat på **tillägg/borttagning av varje person** |

>[!CAUTION]
>
>Ett av de vanligaste felen är att man kan ta bort en person från en lista genom att helt enkelt ta bort personen. **Det här är fel.** Om du tar bort personen tas de bort från **hela databasen**, inte bara från listan.

## Olika sätt att lägga till/ta bort personer från en lista {#ways-to-add-remove-people-from-a-list}

1. Steg för smart kampanjflöde ([Lägg till i lista](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md), [Ta bort från lista](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md))

1. [Steg för ett åtgärdsflöde](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md)
1. Dra personer till en lista i trädet
1. [Listimport](../../../../getting-started/quick-wins/import-a-list-of-people.md)

## Vissa användningsområden för en statisk lista {#some-uses-of-a-static-list}

* En lista som har förvalts för att ta emot ett marknadsföringsmeddelande.
* En lista över &quot;konkurrenter&quot; som du använder för att skicka diskreta motintelligensmeddelanden.
* En tillfällig lista över personer i ett visst läge, som sedan tas bort av smarta kampanjer när de avslutar det läget.

Njut av kraften i LIST!

>[!NOTE]
>
>**Relaterade artiklar**
>
>[Skapa en statisk lista](https://docs.marketo.com/x/ecKt)

