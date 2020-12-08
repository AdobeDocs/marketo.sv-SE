---
unique-page-id: 1146950
description: Vänta - Marketo Docs - Produktdokumentation
title: Vänta
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Vänta {#wait}

>[!NOTE]
>
>**FYI**
>
>Marketo standardiserar nu språk för alla prenumerationer, så du kan se lead/leads i din prenumeration och person/personer på docs.marketo.com. Dessa termer betyder samma sak. det påverkar inte artikelinstruktionerna. Det finns andra förändringar också. [Läs mer](/help/marketo/getting-started/updates-to-marketo-terminology.md).

## Översikt {#overview}

Pausa en person i ett smart kampanjflöde med det praktiska **väntesteget**.

![](assets/wait-overview.png)

Lägg märke till hur du kan skriva på ett naturligt språk som&quot;4 timmar&quot;. Förkorta **dock inte** orden (dvs. 4 timmar). Den smarta kampanjen körs fortfarande, men väntesteget ignoreras.

>[!CAUTION]
>
>Om du ändrar varaktigheten för ett väntesteg påverkas inte personer som redan har angivit det. Till exempel: Om du har ett väntesteg på 5 dagar, anger en person det, ändrar du väntesteget till 7 dagar - personen väntar fortfarande bara 5 dagar innan han/hon går vidare till nästa flödessteg.

>[!TIP]
>
>Om du har någon som redan är i ett väntesteg och du inte vill att de ska gå vidare efter vänteperioden, infogar du [ta bort från flödet](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) direkt efter väntesteget. Ange vem du vill ta bort genom att använda alternativet [Lägg till](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) .

## Användning {#usage}

Det finns tre sätt att använda ett vänteflödessteg:

1. [Använd en varaktighet i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Använd ett specifikt datum i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Använd en datumtoken i ett vänteflödessteg](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
