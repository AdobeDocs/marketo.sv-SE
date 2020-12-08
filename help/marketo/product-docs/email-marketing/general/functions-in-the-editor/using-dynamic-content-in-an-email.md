---
unique-page-id: 2950617
description: Använda dynamiskt innehåll i ett e-postmeddelande - Marketo Docs - Produktdokumentation
title: Använda dynamiskt innehåll i ett e-postmeddelande
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# Använda dynamiskt innehåll i ett e-postmeddelande {#using-dynamic-content-in-an-email}

>[!NOTE]
>
>**Förutsättningar**
>
>* [Skapa en segmentering](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

>



Använd dynamiskt innehåll i e-postmeddelanden för att skicka riktade leads-uppgifter.

## Lägg till segmentering {#add-segmentation}

1. Gå till Marknadsföringsaktiviteter.

   ![](assets/login-marketing-activities.png)

1. Markera din e-postadress och klicka sedan på Redigera utkast.

   ![](assets/1.2.png)

1. I det här exemplet gör vi ämnesraden dynamisk. Klicka i ämnesfältet och klicka sedan på knappen **Gör dynamisk** .

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Du kan också göra ett element inuti e-postmeddelandet dynamiskt. Det gör du genom att markera området, klicka på kugghjulsikonen och välja **Gör dynamisk** (eller [Ersätt med fragment](../../../../product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), beroende på vad du gör).

   Ange namnet på segmenteringen, markera det och klicka på Spara.

   ![](assets/1.4.png)

   Segmenteringen och segmenten visas under fliken Dynamisk till höger.

   ![](assets/1.5.png)

## Använd dynamiskt innehåll {#apply-dynamic-content}

>[!CAUTION]
>
>Antalet tillåtna element med dynamiskt innehåll är inte obegränsat. Även om det inte finns någon specifik nummergräns (den kan variera beroende på innehållskombinationen) kan överanvändning av dynamiskt innehåll påverka e-postens prestanda negativt. Vi rekommenderar att du behåller mängden dynamiska innehållselement som används till under 20 per e-post.

1. Klicka på segmenten och lägg till ämnesraden.

![](assets/2.1.png)

1. Upprepa för varje segment.

   ![](assets/2.2.png)

>[!TIP]
>
>Skapa ett standardmeddelande innan du lägger till innehåll i de olika segmenten.

>[!CAUTION]
>
>Ändringar i standardsegmentets innehållsblock tillämpas på alla segment.

Söt! Nu kan ni skicka flexibla e-postmeddelanden till er målgrupp.

>[!NOTE]
>
>**Relaterade artiklar**
>
>* [Förhandsgranska ett e-postmeddelande med dynamiskt innehåll](preview-an-email-with-dynamic-content.md)
>* [Använd dynamiskt innehåll på en landningssida](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)

>



