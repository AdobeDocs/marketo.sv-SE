---
unique-page-id: 2359504
description: Använd A/B-testning från adress - Marketo Docs - Produktdokumentation
title: Använd A/B-testning från adress
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# Använd A/B-testning från adressen {#use-from-address-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett intressant test är **From Address**-testet. Så här ställer du in det.

>[!PREREQUISITES]
>
>* [Lägg till ett A/B-test](add-an-a-b-test.md)

>



1. Klicka på **Lägg till A/B-test** under rutan **E-post** med ditt e-postmeddelande markerat.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Ett nytt fönster öppnas. Välj **Från adress** för **Testtyp**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Om du har tidigare testinformation (till exempel ett ämnestest) kan du klicka på **Återställ test**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Ange den andra **Från-adressen**-informationen som du vill testa.

   >[!NOTE]
   >
   >Alternativ A fylls i automatiskt med informationen i det valda e-postmeddelandet.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Du kan klicka på **plustecknet** för att lägga till så många från adresser du vill.

1. Använd reglaget för att välja hur stor procentandel av publiken du vill ha i A/B-testet och klicka på **Nästa**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >De olika variationerna skickas till lika delar av den valda provstorleken.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 %** som provstorlek. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du anger att exempelstorleken ska vara 100 %, och vinnaren går inte till någon. Om du använder en **smart**-lista skickas e-postmeddelandet till alla i målgruppen *vid den tidpunkten när du anger samplingsstorleken till 100 %. *När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är nästan framme. Nu måste vi [definiera kriterierna för A/B-testvinnare](define-the-a-b-test-winner-criteria.md).

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Definiera villkor för A/B-testvinnare](define-the-a-b-test-winner-criteria.md)


