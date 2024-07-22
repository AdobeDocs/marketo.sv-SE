---
unique-page-id: 11382593
description: Ställa in Web Personalization till Do Not Track - Marketo Docs - produktdokumentation
title: Ange att webb-Personalization inte ska spåras
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Ange att webb-Personalization inte ska spåras {#setting-web-personalization-to-do-not-track}

Webbbesökarna kan ställa in sin webbläsare så att de inte kan spåras av någon webbplats genom att välja&quot;Do Not Track&quot; (DNT). Detta förhindrar spårning för just den webbläsaren och enheten.

I Web Personalization och Predictive Content kan en marknadsförare ställa in en växlingsknapp som anger om webbläsarens DNT-inställning (Do Not Track) ska stödjas eller ignoreras. Växlingsknappen för konton är inaktiverad som standard, vilket innebär att DNT inte stöds av programmet.

## Aktivera eller inaktivera växlingen {#enable-or-disable-the-toggle}

1. Gå till **Kontoinställningar**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. I Domän- och domänkonfiguration väljer du **På** för att aktivera växeln för Honor-DNT.

   ![](assets/two-1.png)

   När växlingsknappen är inställd på På respekterar och stöder Web Personalization webbläsarens DNT-inställning (Do Not Track) och spårar inte någon webbaktivitet eller kör några kampanjer eller innehållsrekommendationer på webbplatsen.

   >[!NOTE]
   >
   >Om du väljer På kan det påverka Marketo värde och funktioner i specifika områden.

1. Om du vill inaktivera inställningen för Honor-DNT och ignorera webbläsarens DNT-inställning (Do No Track) väljer du **Av** under Honor-DNT.
