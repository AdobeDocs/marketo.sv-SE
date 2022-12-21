---
unique-page-id: 2359494
description: Använd"Subject line" A/B-testning - Marketo Docs - produktdokumentation
title: Använd A/B-testning på ämnesraden
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Använd A/B-testning på ämnesraden {#use-subject-line-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett av de vanligaste testerna är **Subject line** test.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicka på Lägg till A/B-test under rutan E-post med ditt e-postmeddelande markerat.

![](assets/image2014-9-12-15-3a6-3a2.png)

1. Testredigeringsfönstret öppnas. Ange en eller flera nya ämnesrader.

   >[!NOTE]
   >
   >Val **A** fylls i automatiskt med informationen i det valda e-postmeddelandet.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Du kan klicka på **+** om du vill lägga till fler ämnesrader.

1. Använd skjutreglaget för att välja hur stor procentandel av publiken du vill ska få ditt A/B-test och klicka på **Nästa**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 % som provstorlek**. Om du använder en statisk lista och anger 100 % som exempelstorlek skickas e-postmeddelandet till alla i målgruppen och vinnaren går inte till någon. Om du använder en smart lista skickar du e-postmeddelandet till alla i målgruppen genom att ange samplingsstorleken till 100 % _vid den tidpunkten_. Och när e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   >[!NOTE]
   >
   >De olika variationerna av motivet tar jämna delar av den valda provstorleken.

   Vi är nästan framme. Nu behöver vi [definiera kriterier för A/B-testvinnare](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
