---
unique-page-id: 11385053
description: Distribuera JavaScript för Content-AI - Marketo Docs - produktdokumentation
title: Distribuera JavaScript för Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Distribuera JavaScript för Content-AI {#deploy-the-javascript-for-content-ai}

Om du vill använda Predictive Content måste du skapa och konfigurera RTP-taggen (Web Personalization).

## Generera tagg {#generate-tag}

1. Logga in på ditt Predictive Content-konto. Gå till **Kontoinställningar**.

   ![](assets/settings-dropdown-account-hands.png)

1. I **Domänkonfiguration**, letar upp den relevanta domänen och klickar på **Generera tagg**.

   ![](assets/generate-tag.png)

1. Kopiera och klistra in taggen för webbanpassning HTML på webbplatsen.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopiera JavaScript-taggen för webbanpassning och klistra in den som det första skriptet i sidhuvudet mellan `<head> </head>` -taggar. Se mer detaljerad [implementeringsanvisningar här](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Kontrollera att taggen visas på alla sidor, inklusive landningssidor och underdomäner. Kontrollera detta genom att högerklicka på webbplatsens sida. Gå till **Visa sidkälla** i en webbläsare. Sök: &quot;RTP&quot;.

1. Bekräfta att taggväxeln är inställd på **PÅ**.
