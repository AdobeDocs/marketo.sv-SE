---
unique-page-id: 2359951
description: Ta bort en medlem från ett engagemangsprogram - Marketo Docs - produktdokumentation
title: Ta bort en medlem från ett engagemangsprogram
exl-id: c97f15cc-b01a-4148-a150-84901ee2567e
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Ta bort en medlem från ett engagemangsprogram {#remove-a-member-from-an-engagement-program}

Oj då! Hur kom de in dit? Du kan ta bort medlemmar från ett engagemangsprogram med flödessteget **[!UICONTROL Change Program Status]**.

>[!TIP]
>
>Använd inte detta för att pausa innehåll för en person. På så sätt elimineras all attribuering i analysen. Läs mer om hur du [pausar personer i ett engagemangsprogram](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).

## Flödessteg {#flow-step}

1. Dra i flödessteget **[!UICONTROL Change Program Status]**.

   ![](assets/image2014-9-15-18-3a15-3a57.png)

   Välj status, **[!UICONTROL Not in Program]**.

   ![](assets/image2014-9-15-18-3a16-3a2.png)

   Groovy. Alla medlemmar som du har definierat i den [smarta listan](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) kommer inte längre att ingå i det här engagemangsprogrammet.

## Pausa personer  {#pause-people}

Ibland vill man bara pausa personer i ett engagemangsprogram och inte ta bort dem. Detta görs med **[!UICONTROL Change Engagement Program Cadence]**.

>[!MORELIKETHIS]
>
>[Pausa personer i ett engagemangsprogram](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md)
