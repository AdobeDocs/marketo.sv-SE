---
unique-page-id: 1146950
description: Vänta - Marketo Docs - Produktdokumentation
title: Vänta
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Vänta {#wait}

## Översikt {#overview}

Pausa en person i ett smart kampanjflöde med handboken **wait step**.

![](assets/wait-overview.png)

Lägg märke till hur du kan skriva på ett naturligt språk som&quot;4 timmar&quot;. Gör **inte**, men förkorta orden (d.v.s. 4 tim). Den smarta kampanjen körs fortfarande, men väntesteget ignoreras.

>[!CAUTION]
>
>Om du ändrar varaktigheten för ett väntesteg påverkas inte personer som redan har angivit det. Till exempel: Om du har ett väntesteg på 5 dagar, anger en person det, ändrar du väntesteget till 7 dagar - personen väntar fortfarande bara 5 dagar innan han/hon går vidare till nästa flödessteg.

>[!TIP]
>
>Om du har någon som redan är i ett väntesteg och du inte vill att de ska gå vidare efter vänteperioden, infogar du [ta bort från flöde](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) direkt efter väntesteget. Ange vem du vill ta bort med alternativet [lägg till alternativ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md).

## Användning {#usage}

Det finns tre sätt att använda ett vänteflödessteg:

1. [Använd en varaktighet i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Använd en datumtoken i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
