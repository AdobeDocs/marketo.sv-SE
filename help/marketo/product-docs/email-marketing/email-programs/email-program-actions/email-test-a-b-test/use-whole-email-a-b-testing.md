---
unique-page-id: 2359502
description: Använd A/B-testning i hele-post - Marketo Docs - produktdokumentation
title: Använd A/B-testning i"hele-post"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Använd A/B-testning i&quot;hele-post&quot; {#use-whole-email-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett bra test är **Hela e-postmeddelandet** test. Så här ställer du in det.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Under rutan E-post, med ditt e-postmeddelande markerat, klickar du på **Lägg till A/B-test**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Ett nytt fönster öppnas. Klicka på **Testtyp** nedrullningsbar meny och välj **Hela e-postmeddelanden**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Om du har tidigare testinformation (t.ex. ett ämnestest) kan du klicka **Återställ test**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Välj ditt första e-postmeddelande.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Klicka **Lägg till** för att använda e-postmeddelandet.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Du kan lägga till flera e-postmeddelanden. Om du lägger till för många kan det dock göra testprocessen långsammare.

1. Välj ditt andra e-postmeddelande.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Klicka **Lägg till** för att använda det andra e-postmeddelandet. Dra skjutreglaget för att välja vilken procentandel av publiken du vill ska få A/B-testet och klicka på **Nästa**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >De olika variationerna skickas till lika delar av den valda **Provstorlek**.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 % som provstorlek**. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du ställer in samplingsstorleken på 100 % och vinnaren går inte till någon. Om du använder en **smart** lista: om du anger samplingsstorleken till 100 % skickas e-postmeddelandet till alla i målgruppen _vid den tidpunkten_. När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är nästan framme. Nu behöver vi [definiera kriterier för A/B-testvinnare](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
