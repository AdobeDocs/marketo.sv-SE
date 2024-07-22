---
unique-page-id: 11385053
description: Distribuera JavaScript för Content-AI - Marketo Docs - produktdokumentation
title: Installera JavaScript för Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Installera JavaScript för Content-AI {#deploy-the-javascript-for-content-ai}

Om du vill använda Predictive Content måste du generera och konfigurera RTP-taggen (Web Personalization).

## Generera tagg {#generate-tag}

1. Logga in på ditt Predictive Content-konto. Gå till **Kontoinställningar**.

   ![](assets/settings-dropdown-account-hands.png)

1. I **Domänkonfiguration** letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/generate-tag.png)

1. Kopiera och klistra in Web Personalization-taggen HTML på webbplatsen.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera taggen Web Personalization JavaScript och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>` -taggarna. Mer detaljerade [implementeringsinstruktioner finns här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till **Visa sidan Source** i en webbläsare. Sök: RTP.

1. Bekräfta att växlingsknappen Tagg har värdet **ON**.
