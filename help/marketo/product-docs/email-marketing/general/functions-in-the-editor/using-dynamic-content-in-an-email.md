---
unique-page-id: 2950617
description: Använda dynamiskt innehåll i ett e-postmeddelande - Marketo Docs - produktdokumentation
title: Använda dynamiskt innehåll i ett e-postmeddelande
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Använda dynamiskt innehåll i ett e-postmeddelande {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Skapa en segmentering](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Använd dynamiskt innehåll i e-postmeddelanden för att skicka riktade leads-uppgifter.

>[!NOTE]
>
>Användning av variabler i dynamiskt innehåll i ett e-postmeddelande stöds bara när du använder Utlösarkampanjer. Det stöds **inte** när gruppkampanjer används.

## Lägg till segmentering {#add-segmentation}

1. Gå till **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities.png)

1. Välj din e-postadress och klicka på **[!UICONTROL Edit Draft]**.

   ![](assets/1.2.png)

1. I det här exemplet gör vi ämnesraden dynamisk. Klicka i fältet [!UICONTROL Subject] och sedan på knappen **Gör dynamisk** .

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Du kan också göra ett element inuti e-postmeddelandet dynamiskt. Det gör du genom att markera området, klicka på kugghjulsikonen och välja **Gör dynamisk** (eller [Ersätt med fragment](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), beroende på vad du gör).

1. Ange segmenteringsnamnet, markera det och klicka på **[!UICONTROL Save]**.

   ![](assets/1.4.png)

   Segmenteringen och segmenten visas på fliken [!UICONTROL Dynamic] till höger.

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
