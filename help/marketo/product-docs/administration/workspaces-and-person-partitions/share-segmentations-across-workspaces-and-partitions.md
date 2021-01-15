---
unique-page-id: 7515767
description: Dela segment mellan arbetsytor och partitioner - Marketo Docs - Produktdokumentation
title: Dela segment mellan arbetsytor och partitioner
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# Dela segment över arbetsytor och partitioner {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Den här artikeln är endast avsedd för kunder som har Workspaces och partitioner.

## Vad är en segmentering? {#whats-a-segmentation}

Marketo är bra på att välja ut rätt personer för ett program eller en smart kampanj. För mer permanenta personligheter bör du dock använda segmenteringar. De behövs för att använda avancerat dynamiskt innehåll i Marketo.

>[!NOTE]
>
>Lär dig [hur du skapar segmenteringar](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

När du har konfigurerat de här personerna (_och_ du använder arbetsytor) vill du dela dem mellan arbetsytorna. Här är några bra saker att veta:

## Regler och tips {#rules-tips}

* Varje Marketo-prenumeration kan innehålla upp till 20 segment (totalt) över flera arbetsytor (**inte 20 per arbetsyta**).
* Du kan bara dela en segmentering med arbetsytor som du har tillgång till.
* Se till att skapa och använda en **standardarbetsyta som har synlighet i alla partitioner**.

* Segmenteringsbearbetningen körs bara på personerna på arbetsytan där segmenteringen skapas.

   * Skapa segmenteringen som du vill dela i standardarbetsytan.
      * Godkänn segmenteringen
      * Den delade arbetsytan ser en låst mapp och segmenteringen är skrivskyddad.
      * Det går inte att redigera den delade versionen. Du kan bara redigera det ursprungliga segmentet där det skapades.
   * När du klickar på ett segment (t.ex. Sjukvård) inom ett delat segment, kommer de personer du ser endast att vara personer i den partition som är kopplad till den arbetsyta du visar.
      * Om du skapar en segmentering i Workspace 1 (WS1) och delar den med WS2 och WS1 inte har åtkomst till partitionen för WS2, kommer segmenteringen INTE att beräknas om.
      * Om du skapar en segmentering på en arbetsyta som har begränsade partitioner och sedan delar den med en annan arbetsyta, kommer den arbetsytan som fick den delade segmenteringen endast att se personer om de överlappar varandra.


>[!NOTE]
>
>Vissa av dessa regler är lite komplexa. Det enklaste sättet att komma igång är att testa med specifika personer. Du kan alltid skapa nya segmenteringar och bli av med de gamla.

## Exempelscenarier {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Dela en segmentering {#share-a-segmentation}

1. Gå till **databasen**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Högerklicka på **Segmenteringar** och välj **Nya mappar**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Namnge mappen som du vill dela mellan arbetsytor (exempel: Dela segment).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Flytta de segment som du vill dela till mappen.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Högerklicka på mappen och välj **Dela mapp**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Markera den eller de arbetsytor som du vill dela mappen med. Klicka på **Spara**.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >I dialogrutan visas de arbetsytor som du har behörighet att visa. Det är därför Marketo rekommenderar att du skapar och delar segment från standardarbetsytan som har synlighet i alla arbetsytor och partitioner.

Ursprungsmappen visas i databasträdet med en pil som anger att den delas med andra arbetsytor. I den delade arbetsytan visas mappen med ett lås som anger att innehållet i mappen har delats från en annan arbetsyta och är skrivskyddat.
