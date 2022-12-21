---
unique-page-id: 2359947
description: Överför personer mellan engagemangsströmmar - Marketo Docs - produktdokumentation
title: Överför personer mellan engagemangsströmmar
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Överför personer mellan engagemangsströmmar {#transition-people-between-engagement-streams}

Engagement-program kan ha fler än en ström. Om du [lägga till en ström](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)ska du definiera ett sätt för människor att gå från en ström till en annan. Dessa kallas **övergångsregler.**

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/ma.png)

1. Välj ditt multistreaming-engagemangsprogram och gå till **Strömmar**.

   ![](assets/multistream.jpg)

1. Klicka **Övergångsregler** för den ström du vill hämta in från andra strömmar, och klicka sedan på **Redigera övergångsregler**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Övergångsregler dras in i en ström. definierar alltid reglerna för den ström som du vill hämta till.

   När fönstret med övergångsregeln öppnas kan du söka efter och dra i valfri utlösare. I det här fallet vill vi flytta personer till Mid Stage när det läggs till i en affärsmöjlighet.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Låt oss ställa in operatorn på **är** så att alla kan gå över för nya möjligheter.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Du kan lägga till flera utlösare och filter i en övergångsregel, men övergångsregeln använder alla filter (det enda alternativet är att använda ALLA filter). Om du behöver använda ELLER i en övergångsregel rekommenderar vi att du i stället skapar en extern smart kampanj.

1. Klicka **Stäng**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Bra! Nu kommer alla personer i ditt engagemangsprogram som läggs till i en affärsmöjlighet att flyttas till Mid Stage-strömmen.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Stegen som beskrivs ovan *do* gäller för personer som [vid paus](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) också.
