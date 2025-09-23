---
unique-page-id: 11385053
description: Distribuera JavaScript för Content-AI - Marketo Docs - produktdokumentation
title: Installera JavaScript för Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Installera JavaScript för Content-AI {#deploy-the-javascript-for-content-ai}

Om du vill använda Predictive Content måste du generera och konfigurera RTP-taggen (Web Personalization).

## Generera tagg {#generate-tag}

1. Logga in på ditt Predictive Content-konto. Gå till **[!UICONTROL Account Settings]**.

   ![](assets/settings-dropdown-account-hands.png)

1. Leta reda på den relevanta domänen i **[!UICONTROL Domain Configuration]** och klicka på **[!UICONTROL Generate Tag]**.

   ![](assets/generate-tag.png)

1. Kopiera och klistra in taggen Web Personalization i HTML på din webbplats.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera taggen Web Personalization JavaScript och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>` -taggarna. Mer detaljerade [implementeringsinstruktioner finns här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till **[!UICONTROL View Page Source]** i en webbläsare. Sök: RTP.

1. Bekräfta att växlingsknappen Tagg har värdet **[!UICONTROL ON]**.
