---
unique-page-id: 2359951
description: Ta bort en medlem från ett engagemangsprogram - Marketo Docs - Produktdokumentation
title: Ta bort en medlem från ett engagemangsprogram
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Ta bort en medlem från ett engagemangsprogram {#remove-a-member-from-an-engagement-program}

Oj då! Hur kom de in dit? Du kan ta bort medlemmar från ett engagemangsprogram med **flödessteget Ändra** programstatus.

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!TIP]
>
>Använd inte detta för att pausa innehåll för en person. På så sätt elimineras all attribuering i analysen.  Läs mer om hur man [pausar personer i ett engagemangsprogram](pause-people-in-an-engagement-program.md).

## Flödessteg {#flow-step}

1. Dra i **flödessteget Ändra** programstatus.

   ![](assets/image2014-9-15-18-3a15-3a57.png)

   Välj status, **Inte i programmet**.

   ![](assets/image2014-9-15-18-3a16-3a2.png)

   Groovy. Alla medlemmar som du har definierat i den [smarta listan](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) kommer inte längre att ingå i det här engagemangsprogrammet.

## Pausa personer  {#pause-people}

Ibland vill man bara pausa personer i ett engagemangsprogram och inte ta bort dem. Detta görs med **Change Engagement Program Cadence**.

>[!MORELIKETHIS]
>
>* [Pausa personer i ett engagemangsprogram](pause-people-in-an-engagement-program.md)

