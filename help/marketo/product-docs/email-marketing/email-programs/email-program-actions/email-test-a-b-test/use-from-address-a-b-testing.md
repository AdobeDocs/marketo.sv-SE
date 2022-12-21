---
unique-page-id: 2359504
description: Använd A/B-testning från adress - Marketo Docs - produktdokumentation
title: Använd A/B-testning från adress
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Använd A/B-testning från adress {#use-from-address-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett intressant test är **Från adress** test. Så här ställer du in det.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Under **E-post** sida vid sida, med ditt e-postmeddelande markerat, klicka på **Lägg till A/B-test**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ett nytt fönster öppnas, välj **Från adress** for **Testtyp**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Om du har tidigare testinformation (t.ex. ett ämnestest) kan du klicka **Återställ test**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Ange den andra **Från adress** information som du vill testa.

   >[!NOTE]
   >
   >Alternativ A fylls i automatiskt med informationen i det valda e-postmeddelandet.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Du kan klicka på **+** om du vill lägga till så många från adresser du vill.

1. Använd reglaget för att välja hur stor procentandel av publiken du vill ha i A/B-testet och klicka på **Nästa**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >De olika variationerna skickas till lika delar av den valda provstorleken.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 % som provstorlek**. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du ställer in samplingsstorleken på 100 % och vinnaren går inte till någon. Om du använder en **smart** lista: om du anger samplingsstorleken till 100 % skickas e-postmeddelandet till alla i målgruppen _vid den tidpunkten_. När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är nästan framme. Nu behöver vi [definiera kriterier för A/B-testvinnare](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
