---
unique-page-id: 4719332
description: Distribuera RTP JavaScript - Marketo Docs - produktdokumentation
title: Distribuera RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Distribuera RTP JavaScript {#deploy-the-rtp-javascript}

Följ installationsanvisningarna nedan för att skapa och konfigurera RTP-taggen

## Generera tagg {#generate-tag}

1. Logga in på ditt RTP-konto. Gå till **Kontoinställningar**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. I **Domän** och **Domänkonfiguration**, letar upp den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Kopiera och klistra in taggen för webbpersonalisering (RTP) på webbplatsen.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera RTP JavaScript-taggen och klistra in den som det första skriptet i sidhuvudet - mellan `<head> </head>` -taggar.

   Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till Visa sidkälla i en webbläsare. Sök: &quot;RTP&quot;.

1. Växla tagg till **PÅ**.

   Bekräfta att växlingsknappen Tagg är inställd på ON. Du bör börja se dataflödet på fliken Organisationen.

   Du är nu konfigurerad med RTP-taggen och klar att börja [skapa segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) och realtidskampanjer!

1. Kontrollera att taggen finns på alla sidor.
