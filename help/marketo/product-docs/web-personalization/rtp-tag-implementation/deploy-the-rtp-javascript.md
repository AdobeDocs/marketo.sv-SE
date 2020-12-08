---
unique-page-id: 4719332
description: Distribuera RTP JavaScript - Marketo Docs - Produktdokumentation
title: Distribuera RTP JavaScript
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Distribuera RTP JavaScript {#deploy-the-rtp-javascript}

Följ installationsanvisningarna nedan för att skapa och konfigurera RTP-taggen

## Generera tagg {#generate-tag}

1. Logga in på ditt RTP-konto. Gå till **Kontoinställningar**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. I **Domän** och **Domänkonfiguration** letar du reda på den relevanta domänen och klickar på **Generera tagg.**

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Kopiera och klistra in taggen för webbpersonalisering (RTP) på webbplatsen.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera JavaScript-taggen RTP och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>` -taggarna.

   Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till Visa sidkälla i en webbläsare. Sök: &quot;RTP&quot;.

1. Taggväxlingen är inställd på **PÅ**.

   Bekräfta att växlingsknappen Tagg är inställd på ON. Du bör börja se dataflödet på fliken Organisationen.

   Du är nu klar med RTP-taggen och redo att börja [skapa segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) och realtidskampanjer!

1. Kontrollera att taggen finns på alla sidor.

>[!MORELIKETHIS]
>
>* [Implementering av RTP-tagg](http://docs.marketo.com/display/docs/rtp+tag+implementation)

