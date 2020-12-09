---
unique-page-id: 2359502
description: Använd A/B-testning i hele-post - Marketo Docs - produktdokumentation
title: Använd A/B-testning i"hele-post"
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Använd A/B-testning i&quot;hele-post&quot; {#use-whole-email-a-b-testing}

Du kan enkelt A/B-testa dina e-postmeddelanden. Ett bra test är **Hela e-posttestet** . Så här ställer du in det.

>[!PREREQUISITES]
>
>* [Lägg till ett A/B-test](add-an-a-b-test.md)

>



1. Klicka på Lägg till A/B-test under rutan E-post med ditt e-postmeddelande markerat.

` ![](assets/image2014-9-12-15-3a22-3a12.png)

`

1. Ett nytt fönster öppnas. Klicka på listrutan **Testtyp** och välj **Hela e-postmeddelanden**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Om du har tidigare testinformation (till exempel ett ämnestest) kan du klicka på **Återställ test**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Välj ditt första e-postmeddelande.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Klicka på **Lägg till** för att använda e-postmeddelandet.

   ` ![](assets/image2014-9-12-15-3a23-3a20.png)

   `

   >[!TIP]
   >
   >Du kan lägga till flera e-postmeddelanden. Om du lägger till för många kan det dock göra testprocessen långsammare.

1. Välj ditt andra e-postmeddelande.

   ` ![](assets/image2014-9-12-15-3a23-3a49.png)

   `

1. Klicka på **Lägg till** för att använda det andra e-postmeddelandet. Dra skjutreglaget för att välja hur stor procentandel av publiken du vill ska få A/B-testet och klicka på **Nästa**.

   ` ![](assets/image2014-9-12-15-3a24-3a1.png)

   `

   >[!NOTE]
   >
   >De olika variationerna skickas till samma delar av den valda **provstorleken**.

   >[!CAUTION]
   >
   >**Vi rekommenderar att du inte anger 100 %** som provstorlek. Om du använder en statisk lista skickas e-postmeddelandet till alla i målgruppen om du anger att exempelstorleken ska vara 100 %, och vinnaren går inte till någon. Om du använder en **smart** lista skickas e-postmeddelandet till alla i målgruppen *vid den tidpunkten om du anger 100 % för exempelstorleken. *När e-postprogrammet körs igen vid ett senare tillfälle kommer alla nya personer som är kvalificerade för den smarta listan också att få e-postmeddelandet eftersom de nu ingår i målgruppen.

   Vi är nästan framme. Nu måste vi [definiera kriterierna](define-the-a-b-test-winner-criteria.md)för A/B-testvinnare.

   >[!NOTE]
   >
   >**Relaterade artiklar**
   >
   >    
   >    
   >    * [Definiera villkor för A/B-testvinnare](define-the-a-b-test-winner-criteria.md)


