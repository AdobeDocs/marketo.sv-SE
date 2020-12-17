---
unique-page-id: 2359947
description: Överför personer mellan engagemangsströmmar - Marketo Docs - Produktdokumentation
title: Överför personer mellan engagemangsströmmar
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Överför personer mellan engagemangsströmmar {#transition-people-between-engagement-streams}

Engagement-program kan ha fler än en ström. Om du [lägger till en ström](../../../../product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md) måste du definiera ett sätt för personer att flytta från en ström till en annan. Dessa kallas **övergångsregler.**

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Välj ditt multistreaming-engagemangsprogram och gå till **Streams**.

   ![](assets/multistream.jpg)

1. Klicka på **Övergångsregler** för den ström du vill hämta från andra strömmar och klicka sedan på **Redigera övergångsregler. **

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Övergångsregler dras in i en ström. definierar alltid reglerna för den ström som du vill hämta till.

   När fönstret med övergångsregeln öppnas kan du söka efter och dra i valfri utlösare. I det här fallet vill vi flytta personer till Mid Stage när det läggs till i en affärsmöjlighet.
` ![](assets/image2014-9-15-18-3a10-3a46.png)

   `

1. Låt oss ställa in operatorn på** är vilket** som helst, så att personerna kan gå över för nya möjligheter.

   ` ![](assets/image2014-9-15-18-3a11-3a14.png)

   `

   >[!TIP]
   >
   >Du kan lägga till flera utlösare och filter i en övergångsregel, men övergångsregeln använder alla filter (det enda alternativet är att använda ALLA filter). Om du behöver använda ELLER i en övergångsregel rekommenderar vi att du i stället skapar en extern smart kampanj.

1. Klicka på **Stäng**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Bra! Nu kommer alla personer i ditt engagemangsprogram som läggs till i en affärsmöjlighet att flyttas till Mid Stage-strömmen.

   ` ![](assets/image2014-9-15-18-3a11-3a29.png)

   `

   >[!NOTE]
   >
   >Stegen ovan *do* gäller även personer som är [på paus](http://docs.marketo.com/display/DOCS/Pause+People+in+an+Engagement+Program).

