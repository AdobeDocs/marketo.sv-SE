---
unique-page-id: 2950617
description: Använda dynamiskt innehåll i ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Använda dynamiskt innehåll i ett e-postmeddelande
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Använda dynamiskt innehåll i ett e-postmeddelande {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Skapa en segmentering](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Använd dynamiskt innehåll i e-postmeddelanden för att skicka riktade leads-uppgifter.

>[!NOTE]
>
>Användning av variabler i dynamiskt innehåll i ett e-postmeddelande stöds bara när du använder Utlösarkampanjer. Det är **not** stöds när gruppkampanjer används.

## Lägg till segmentering {#add-segmentation}

1. Gå till **Marknadsföringsaktiviteter**.

   ![](assets/login-marketing-activities.png)

1. Välj e-post och klicka **Redigera utkast**.

   ![](assets/1.2.png)

1. I det här exemplet gör vi ämnesraden dynamisk. Klicka i ämnesfältet och klicka sedan på **Gör dynamisk** -knappen.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Du kan också göra ett element inuti e-postmeddelandet dynamiskt. Markera området, klicka på kugghjulsikonen och välj **Gör dynamisk** (eller [Ersätt med fragment](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), beroende på vad du gör).

1. Ange namnet på segmenteringen, markera det och klicka på **Spara**.

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

>[!MORELIKETHIS]
>
>* [Förhandsgranska ett e-postmeddelande med dynamiskt innehåll](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Använd dynamiskt innehåll på en landningssida](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
