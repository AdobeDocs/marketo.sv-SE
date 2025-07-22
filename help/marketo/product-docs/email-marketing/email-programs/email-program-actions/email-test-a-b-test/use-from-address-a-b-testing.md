---
unique-page-id: 2359504
description: Använd A/B-testning från adress - Marketo Docs - produktdokumentation
title: Använd A/B-testning från adress
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Använd A/B-testning i [!UICONTROL From Address] {#use-from-address-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett intressant test är **[!UICONTROL From Address]**-testet. Så här ställer du in det.

>[!PREREQUISITES]
>
>[Lägg till ett A/B-test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Klicka på **[!UICONTROL Email]** under rutan **[!UICONTROL Add A/B Test]** med ditt e-postmeddelande markerat.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ett nytt fönster öppnas. Välj **[!UICONTROL From Address]** för **[!UICONTROL Test Type]**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Om du har tidigare testinformation (till exempel ett ämnestest) kan du klicka på **[!UICONTROL Reset Test]**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Ange den andra **[!UICONTROL From Address]**-informationen som du vill testa.

   >[!NOTE]
   >
   >Alternativ A fylls i automatiskt med informationen i det valda e-postmeddelandet.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Du kan klicka på **+** för att lägga till så många från adresser du vill.

1. Använd reglaget för att välja hur stor procentandel av målgruppen du vill ha i A/B-testet och klicka på **[!UICONTROL Next]**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >De olika variationerna skickas till lika delar av den valda provstorleken.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 %** som provstorlek. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du anger att exempelstorleken ska vara 100 %, och vinnaren går inte till någon. Om du använder en **smart**-lista skickas e-postmeddelandet till alla i målgruppen _vid den tidpunkten_ om du anger samplingsstorleken till 100 %. När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är nästan framme. Nu måste vi [definiera kriterierna för A/B-testvinnaren](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
