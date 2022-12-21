---
unique-page-id: 2359520
description: Använd A/B-testning av datum/tid - Marketo Docs - produktdokumentation
title: Använd A/B-testning av datum/tid
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Använd A/B-testning av datum/tid {#use-date-time-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett test är **Datum/tid** test. Detta testar vilken tid på dygnet eller veckodagen som är bäst för att skicka e-postmeddelanden. Så här ställer du in det.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Under **E-post** platta, klicka **Lägg till A/B-test**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Ett nytt fönster öppnas. Välj **Datum/tid** for **Testtyp**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Om du har tidigare testinformation (t.ex. ett ämnestest) kan du klicka **Återställ test**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Välj datum för ditt första datum/tid.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Välj tid för ditt första datum/tid.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Gör samma sak med ditt andra datum/tid.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Använd reglaget för att välja hur stor procentandel av publiken du vill ha i A/B-testet och klicka på **Nästa**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >De olika variationerna gäller för lika delar av den valda provstorleken.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 % som provstorlek**. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du ställer in samplingsstorleken på 100 % och vinnaren går inte till någon. Om du använder en **smart** lista: om du anger samplingsstorleken till 100 % skickas e-postmeddelandet till alla i målgruppen _vid den tidpunkten_. När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är ett steg närmare. Nu behöver vi [definiera kriterier för A/B-testvinnare](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
