---
unique-page-id: 11385053
description: Lär dig hur du skapar och placerar RTP Web Personalization-taggen för prediktivt innehåll. Kopiera den till sidhuvudet, verifiera täckning och bekräfta att växlingen är aktiverad.
title: Installera JavaScript för Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: cd7a000c415bedd561aa509e375ba0dee8e81d9f
workflow-type: tm+mt
source-wordcount: '148'
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
