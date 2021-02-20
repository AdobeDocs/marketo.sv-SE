---
unique-page-id: 11385053
description: Distribuera JavaScript för Content-AI - Marketo Docs - produktdokumentation
title: Distribuera JavaScript för Content-AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Distribuera JavaScript för Content-AI {#deploy-the-javascript-for-content-ai}

Om du vill använda Predictive Content måste du skapa och konfigurera RTP-taggen (Web Personalization).

## Generera tagg {#generate-tag}

1. Logga in på ditt Predictive Content-konto. Gå till **Kontoinställningar**.

   ![](assets/settings-dropdown-account-hands.png)

1. I **Domänkonfiguration** letar du reda på den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/generate-tag.png)

1. Kopiera och klistra in taggen Web Personalization i webbplatsens HTML-kod.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera JavaScript-taggen för webbanpassning och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>`-taggarna. Mer detaljerade [implementeringsinstruktioner finns här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till **Visa sidkälla** i en webbläsare. Sök: &quot;RTP&quot;.

1. Bekräfta att växlingsknappen Tagg är inställd på **ON**.
