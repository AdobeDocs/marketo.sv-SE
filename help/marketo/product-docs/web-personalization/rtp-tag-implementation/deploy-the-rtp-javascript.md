---
unique-page-id: 4719332
description: Distribuera RTP JavaScript - Marketo Docs - produktdokumentation
title: Distribuera RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Distribuera RTP JavaScript {#deploy-the-rtp-javascript}

Följ installationsanvisningarna nedan för att skapa och konfigurera RTP-taggen

## [!UICONTROL Generate Tag] {#generate-tag}

1. Logga in på ditt RTP-konto. Gå till **[!UICONTROL Account Settings]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. Leta reda på den relevanta domänen i **[!UICONTROL Domain]** och **[!UICONTROL Domain Configuration]** och klicka på **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Kopiera och klistra in taggen Web Personalization (RTP) på webbplatsen.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera RTP JavaScript-taggen och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>`-taggarna.

   Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till View Page Source i en webbläsare. Sök: RTP.

1. [!UICONTROL Tag] växlingsuppsättning: **[!UICONTROL ON]**.

   Bekräfta att växlingsknappen [!UICONTROL Tag] är inställd på [!UICONTROL ON]. Du bör börja se dataflödet på fliken Organisationen.

   Du är nu konfigurerad med RTP-taggen och redo att börja [skapa segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) och realtidskampanjer!

1. Kontrollera att taggen finns på alla sidor.
