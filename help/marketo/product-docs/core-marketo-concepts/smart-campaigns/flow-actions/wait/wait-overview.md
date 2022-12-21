---
unique-page-id: 1146950
description: Vänta - Marketo Docs - produktdokumentation
title: Vänta
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Vänta {#wait}

## Översikt {#overview}

Pausa en person i ett smart kampanjflöde med användaren **väntesteg**.

![](assets/wait-overview.png)

Lägg märke till hur du kan skriva på ett naturligt språk som&quot;4 timmar&quot;. Gör **not** Förkortar dock orden (dvs. 4 timmar). Den smarta kampanjen körs fortfarande, men väntesteget ignoreras.

>[!CAUTION]
>
>Om du ändrar varaktigheten för ett väntesteg påverkas inte personer som redan har angivit det. Till exempel: Om du har ett väntesteg på 5 dagar, anger en person det, ändrar du väntesteget till 7 dagar - personen väntar fortfarande bara 5 dagar innan han/hon går vidare till nästa flödessteg.

>[!TIP]
>
>Om du har någon som redan är i ett vänteläge och du inte vill att de ska fortsätta efter vänteperiodens slut infogar du [ta bort från flöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) direkt efter väntesteget. Ange vem du vill ta bort genom att använda [lägg till alternativ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) alternativ.

## Användning {#usage}

Det finns tre sätt att använda ett vänteflödessteg:

1. [Använd en varaktighet i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Använd en datumtoken i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
