---
unique-page-id: 11382593
description: Läs om hur du ställer in webbpersonalisering så att den inte spåras i Marketo Engage, inklusive att ställa in webbpersonalisering på. Slutför nästa steg med den här guiden.
title: Ange att webb-Personalization inte ska spåras
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Anger [!UICONTROL Web Personalization] som Do Not Track (Spåra inte) {#setting-web-personalization-to-do-not-track}

Webbbesökarna kan ställa in sin webbläsare så att de inte kan spåras av någon webbplats genom att välja&quot;Do Not Track&quot; (DNT). Detta förhindrar spårning för just den webbläsaren och enheten.

I [!UICONTROL Web Personalization] och [!UICONTROL Predictive Content] kan en markör ställa in en växlingsknapp som anger om webbläsarens DNT-inställning (Do Not Track) ska stödjas eller ignoreras. Växlingsknappen för konton är inaktiverad som standard, vilket innebär att DNT inte stöds av programmet.

## Aktivera eller inaktivera växlingen {#enable-or-disable-the-toggle}

1. Gå till **[!UICONTROL Account Settings]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. I [!UICONTROL Domain] och [!UICONTROL Domain Configuration] väljer du **[!UICONTROL On]** för att aktivera växlingsknappen [!UICONTROL Honor DNT].

   ![](assets/two-1.png)

   När växlingsknappen är inställd på [!UICONTROL On] respekterar och stöder Web Personalization webbläsarens DNT-inställning (Do Not Track) och spårar inte någon webbaktivitet eller kör några kampanjer eller innehållsrekommendationer på webbplatsen.

   >[!NOTE]
   >
   >Om du ställer in växeln på [!UICONTROL On] kan det påverka Marketo värde och funktioner i vissa områden.

1. Om du vill inaktivera inställningen [!UICONTROL Honor DNT] och ignorera webbläsarens DNT-inställning (Do No Track) väljer du **[!UICONTROL Off]** under [!UICONTROL Honor DNT].
