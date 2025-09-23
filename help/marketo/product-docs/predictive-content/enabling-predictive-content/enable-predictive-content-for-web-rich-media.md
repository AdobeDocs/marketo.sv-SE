---
unique-page-id: 7514956
description: Aktivera prediktivt innehåll för multimedia för webben - Marketo Docs - produktdokumentation
title: Aktivera prediktivt innehåll för multimedia för webben
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Aktivera prediktivt innehåll för multimedia för webben {#enable-predictive-content-for-web-rich-media}

Prediktivt innehåll engagerar webbbesökarna med det mest relevanta innehållet, som bygger på maskininlärning och prediktiv analys. Med Web Rich Media kan du förbättra innehållet med textbeskrivningar och bilder och bädda in olika prediktiva innehållsrekommendationer på webbplatsen.

>[!NOTE]
>
>Vi rekommenderar att du aktiverar över fem innehållsdelar per kategori och källa (e-post, multimedia, fält) innan du testar och använder Predictive Content. Mer innehåll ger ett bättre prediktivt resultat.

>[!PREREQUISITES]
>
>Innan du aktiverar Predictive Content måste du:
>
>* **Förbered ditt prediktiva innehåll**
>
>   * [Redigera prediktivt innehåll för e-postmeddelanden](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} eller
>   * [Redigera förebyggande innehåll för multimedia](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} eller
>   * [Redigera prediktivt innehåll för rekommendationsfältet](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Godkänn en titel för förebyggande innehåll](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

När du har förberett innehållets titel, beskrivning och bild för multimedia kan du aktivera enskilda eller flera innehållskomponenter.

1. Om du vill aktivera en enskild titel klickar du på den för att öppna redigeraren. Klicka på **[!UICONTROL Rich Media]**, markera kryssrutan **[!UICONTROL Enabled for Predictive Content in Rich Media]** och klicka på **[!UICONTROL Save]**.

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. Om det finns flera innehållsdelar på sidan **[!UICONTROL Predictive Content]** markerar du kryssrutorna intill rubriken/rubrikerna.

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. Klicka på listrutan **[!UICONTROL Content Actions]** och välj **[!UICONTROL Enable for Web Rich Media]**.

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## Anpassa JavaScript-koden och bädda in den på din webbplats  {#customize-the-javascript-code-and-embed-it-into-your-website}

Mer information finns i dokumentationen för Rekommendationsmallen för multimedia [ på webbplatsen för Marketo-utvecklare](https://experienceleague.adobe.com/sv/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation){target="_blank"}. Detta förklarar hur du anpassar mallen för webbplatsen.

Klistra in JavaScript-koden på webbplatsen där du vill att mallen ska visas.

**Mallexempel**

* Mall1: Tre vågräta innehållsdelar med bilder, rubrik och beskrivning
* Mall2: Tre vertikala innehållskomponenter med bilder, rubrik och beskrivning

Här är ett exempel på rekommendationsmallen för multimedia1:

![](assets/image2015-6-1-17-3a8-3a33.png)

Här är ett exempel på rekommendationsmallen för multimedia2:

![](assets/image2015-12-20-10-3a35-3a12.png)
